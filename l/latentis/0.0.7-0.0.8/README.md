# Comparing `tmp/latentis-0.0.7.tar.gz` & `tmp/latentis-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latentis-0.0.7.tar", last modified: Wed Nov  8 09:14:44 2023, max compression
+gzip compressed data, was "latentis-0.0.8.tar", last modified: Wed May 15 17:02:43 2024, max compression
```

## Comparing `latentis-0.0.7.tar` & `latentis-0.0.8.tar`

### file list

```diff
@@ -1,83 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.262678 latentis-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-08 09:11:49.000000 latentis-0.0.7/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-11-08 09:11:49.000000 latentis-0.0.7/.env.template
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-08 09:11:49.000000 latentis-0.0.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.250678 latentis-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.254678 latentis-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2023-11-08 09:11:49.000000 latentis-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2023-11-08 09:11:49.000000 latentis-0.0.7/.github/workflows/test_suite.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-11-08 09:11:49.000000 latentis-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2023-11-08 09:11:49.000000 latentis-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-11-08 09:11:49.000000 latentis-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-11-08 09:14:44.262678 latentis-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-11-08 09:11:49.000000 latentis-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.254678 latentis-0.0.7/data/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-08 09:11:49.000000 latentis-0.0.7/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.254678 latentis-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2023-11-08 09:11:49.000000 latentis-0.0.7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.254678 latentis-0.0.7/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-11-08 09:11:49.000000 latentis-0.0.7/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-08 09:14:37.000000 latentis-0.0.7/env.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-11-08 09:11:49.000000 latentis-0.0.7/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.254678 latentis-0.0.7/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-11-08 09:14:37.000000 latentis-0.0.7/notebooks/demo_relative.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-11-08 09:14:37.000000 latentis-0.0.7/notebooks/demo_translation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-11-08 09:11:49.000000 latentis-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-11-08 09:14:44.262678 latentis-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-11-08 09:11:49.000000 latentis-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.250678 latentis-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.254678 latentis-0.0.7/src/latentis/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-08 09:14:44.000000 latentis-0.0.7/src/latentis/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.254678 latentis-0.0.7/src/latentis/estimate/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/estimate/affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/estimate/dim_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/estimate/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/estimate/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/estimate/orthogonal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/src/latentis/measure/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/measure/_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/src/latentis/project/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/project/relative.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/src/latentis/sample/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/sample/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/src/latentis/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/transform/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/transform/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/src/latentis/translate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/translate/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/src/latentis/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 09:11:49.000000 latentis-0.0.7/src/latentis/visualize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.254678 latentis-0.0.7/src/latentis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-11-08 09:14:44.000000 latentis-0.0.7/src/latentis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-11-08 09:14:44.000000 latentis-0.0.7/src/latentis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 09:14:44.000000 latentis-0.0.7/src/latentis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 09:13:41.000000 latentis-0.0.7/src/latentis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-11-08 09:14:44.000000 latentis-0.0.7/src/latentis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-08 09:14:44.000000 latentis-0.0.7/src/latentis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/tests/measure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/measure/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/measure/test_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/tests/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/project/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/project/test_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/tests/sample/
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/sample/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/test_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/transform/test_functional_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:14:44.258678 latentis-0.0.7/tests/translate/
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/translate/test_manual_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-11-08 09:11:49.000000 latentis-0.0.7/tests/translate/test_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.110935 latentis-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-15 17:02:36.000000 latentis-0.0.8/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 17:02:36.000000 latentis-0.0.8/.env.template
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 17:02:36.000000 latentis-0.0.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.090935 latentis-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.094935 latentis-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-15 17:02:36.000000 latentis-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-15 17:02:36.000000 latentis-0.0.8/.github/workflows/test_suite.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-15 17:02:36.000000 latentis-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-15 17:02:36.000000 latentis-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-15 17:02:36.000000 latentis-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-15 17:02:43.110935 latentis-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-15 17:02:36.000000 latentis-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.090935 latentis-0.0.8/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.094935 latentis-0.0.8/benchmarks/eval_estimator/
+-rw-r--r--   0 runner    (1001) docker     (127)   221647 2024-05-15 17:02:36.000000 latentis-0.0.8/benchmarks/eval_estimator/benchmark.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-15 17:02:36.000000 latentis-0.0.8/benchmarks/eval_estimator/benchmark_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.094935 latentis-0.0.8/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 17:02:36.000000 latentis-0.0.8/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.094935 latentis-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-15 17:02:36.000000 latentis-0.0.8/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.094935 latentis-0.0.8/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 17:02:36.000000 latentis-0.0.8/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-15 17:02:36.000000 latentis-0.0.8/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-15 17:02:36.000000 latentis-0.0.8/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.098935 latentis-0.0.8/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-15 17:02:36.000000 latentis-0.0.8/notebooks/demo_relative.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-15 17:02:36.000000 latentis-0.0.8/notebooks/demo_search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-15 17:02:36.000000 latentis-0.0.8/notebooks/demo_translation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-15 17:02:36.000000 latentis-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 17:02:43.110935 latentis-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-15 17:02:36.000000 latentis-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.090935 latentis-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.098935 latentis-0.0.8/src/latentis/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 17:02:43.000000 latentis-0.0.8/src/latentis/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.098935 latentis-0.0.8/src/latentis/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/benchmark/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/benchmark/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.098935 latentis-0.0.8/src/latentis/correspondence/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/correspondence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/correspondence/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/correspondence/correspondence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/correspondence/gen_correspondences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.098935 latentis-0.0.8/src/latentis/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/data/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/data/text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/data/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.102935 latentis-0.0.8/src/latentis/measure/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/measure/_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/measure/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/measure/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/measure/cka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.102935 latentis-0.0.8/src/latentis/measure/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/measure/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/measure/functional/cka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/measure/functional/svcca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/measure/svcca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/nexus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.102935 latentis-0.0.8/src/latentis/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/nn/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/nn/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/nn/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.102935 latentis-0.0.8/src/latentis/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/project/relative.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.102935 latentis-0.0.8/src/latentis/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/sample/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.102935 latentis-0.0.8/src/latentis/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/serialize/disk_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/serialize/io_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.102935 latentis-0.0.8/src/latentis/space/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/space/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23647 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/space/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/space/vector_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.102935 latentis-0.0.8/src/latentis/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/transform/_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/transform/dim_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/transform/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/transform/projection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.106935 latentis-0.0.8/src/latentis/transform/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/transform/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/transform/translate/aligner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/transform/translate/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.106935 latentis-0.0.8/src/latentis/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:36.000000 latentis-0.0.8/src/latentis/visualize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.106935 latentis-0.0.8/src/latentis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-15 17:02:43.000000 latentis-0.0.8/src/latentis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-15 17:02:43.000000 latentis-0.0.8/src/latentis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:02:43.000000 latentis-0.0.8/src/latentis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:02:42.000000 latentis-0.0.8/src/latentis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-15 17:02:43.000000 latentis-0.0.8/src/latentis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 17:02:43.000000 latentis-0.0.8/src/latentis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.106935 latentis-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.106935 latentis-0.0.8/tests/measure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/measure/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/measure/test_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.106935 latentis-0.0.8/tests/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/project/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/project/test_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.106935 latentis-0.0.8/tests/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/sample/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/test_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.106935 latentis-0.0.8/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/transform/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:02:43.106935 latentis-0.0.8/tests/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-15 17:02:36.000000 latentis-0.0.8/tests/translate/test_manual_translate.py
```

### Comparing `latentis-0.0.7/.github/workflows/publish.yml` & `latentis-0.0.8/.github/workflows/test_suite.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,162 +1,141 @@
-name: Publish
+name: tests
 
 on:
-  release:
+  push:
+    branches:
+      - main
+      - develop
+
+  pull_request:
     types:
-      - created
+      - opened
+      - reopened
+      - synchronize
 
 env:
-  CACHE_NUMBER: 0  # increase to reset cache manually
-  CONDA_ENV_FILE: './env.yaml'
-  CONDA_ENV_NAME: 'latentis'
-
+  CONDA_ENV_FILE: "./env.yaml"
+  CONDA_ENV_NAME: "latentis"
 
 jobs:
   build:
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9']
+        python-version: ["3.8", "3.9", "3.10"]
         include:
           - os: ubuntu-20.04
             label: linux-64
             prefix: /usr/share/miniconda3/envs/
 
+    #           - os: macos-latest
+    #             label: osx-64
+    #             prefix: /Users/runner/miniconda3/envs/$CONDA_ENV_NAME
+
+    #           - os: windows-latest
+    #             label: win-64
+    #             prefix: C:\Miniconda3\envs\$CONDA_ENV_NAME
+
     name: ${{ matrix.label }}-py${{ matrix.python-version }}
     runs-on: ${{ matrix.os }}
 
-    environment: release
-    permissions:
-      # IMPORTANT: this permission is mandatory for trusted publishing
-      id-token: write
-
     steps:
+      - name: Free Disk Space (Ubuntu)
+        uses: jlumbroso/free-disk-space@main
+        with:
+          # this might remove tools that are actually needed,
+          # if set to "true" but frees about 6 GB
+          tool-cache: false
+
+          # all of these default to true, but feel free to set to
+          # "false" if necessary for your workflow
+          android: true
+          dotnet: true
+          haskell: true
+          large-packages: true
+          docker-images: true
+          swap-storage: true
       - name: Parametrize conda env name
         run: echo "PY_CONDA_ENV_NAME=${{ env.CONDA_ENV_NAME }}-${{ matrix.python-version }}" >> $GITHUB_ENV
       - name: echo conda env name
         run: echo ${{ env.PY_CONDA_ENV_NAME }}
 
       - name: Parametrize conda prefix
         run: echo "PY_PREFIX=${{ matrix.prefix }}${{ env.PY_CONDA_ENV_NAME }}" >> $GITHUB_ENV
       - name: echo conda prefix
         run: echo ${{ env.PY_PREFIX }}
 
-      # extract the first two digits from the release note
-      - name: Set release notes tag
-        run: |
-          export RELEASE_TAG_VERSION=${{ github.event.release.tag_name }}
-          echo "RELEASE_TAG_VERSION=${RELEASE_TAG_VERSION%.*}">> $GITHUB_ENV
-
-      - name: Echo release notes tag
-        run: |
-          echo "${RELEASE_TAG_VERSION}"
-
       - uses: actions/checkout@v2
-        with:
-          fetch-depth: 0
 
       # Remove the python version pin from the env.yml which could be inconsistent
       - name: Remove explicit python version from the environment
         shell: bash -l {0}
         run: |
           sed -Ei '/^\s*-?\s*python\s*([#=].*)?$/d' ${{ env.CONDA_ENV_FILE }}
           cat  ${{ env.CONDA_ENV_FILE }}
 
-      - name: Setup Mambaforge
-        uses: conda-incubator/setup-miniconda@v2
-        with:
-            miniforge-variant: Mambaforge
-            miniforge-version: latest
-            activate-environment: ${{ env.PY_CONDA_ENV_NAME }}
-            python-version: ${{ matrix.python-version }}
-            use-mamba: true
-
-      - uses: actions/cache@v2
-        name: Conda cache
-        with:
-          path: ${{ env.PY_PREFIX }}
-          key: ${{ matrix.label }}-conda-${{ matrix.python-version }}-${{ env.CACHE_NUMBER }}-${{ env.PY_CONDA_ENV_NAME }}-${{ hashFiles(env.CONDA_ENV_FILE) }}-${{hashFiles('./setup.cfg') }}
-        id: conda_cache
+      # Remove pytorch-cuda line from the env.yml
+      - name: Remove explicit pytorch-cuda version from the environment
+        shell: bash -l {0}
+        run: |
+          sed -Ei '/^\s*-?\s*pytorch-cuda\s*([#=].*)?$/d' ${{ env.CONDA_ENV_FILE }}
+          cat  ${{ env.CONDA_ENV_FILE }}
 
-      - uses: actions/cache@v2
-        name: Pip cache
-        with:
-          path: ~/.cache/pip
-          key: ${{ matrix.label }}-pip-${{ matrix.python-version }}-${{ env.CACHE_NUMBER }}-${{ env.PY_CONDA_ENV_NAME }}-${{ hashFiles(env.CONDA_ENV_FILE) }}-${{hashFiles('./setup.cfg') }}
+      # Install torch cpu-only
+      - name: Install torch cpu only
+        shell: bash -l {0}
+        run: |
+          sed -i '/nvidia\|cuda/d' ${{ env.CONDA_ENV_FILE }}
+          cat  ${{ env.CONDA_ENV_FILE }}
 
-      - uses: actions/cache@v2
-        name: Pre-commit cache
+      - name: Setup Mambaforge
+        uses: conda-incubator/setup-miniconda@v2
         with:
-          path: ~/.cache/pre-commit
-          key: ${{ matrix.label }}-pre-commit-${{ hashFiles('.pre-commit-config.yaml') }}-${{ matrix.python-version }}-${{ env.CACHE_NUMBER }}-${{ env.PY_CONDA_ENV_NAME }}-${{ hashFiles(env.CONDA_ENV_FILE) }}-${{hashFiles('./setup.cfg') }}
+          miniforge-variant: Mambaforge
+          miniforge-version: latest
+          environment-file: ${{ env.CONDA_ENV_FILE }}
+          activate-environment: ${{ env.PY_CONDA_ENV_NAME }}
+          python-version: ${{ matrix.python-version }}
+          use-mamba: true
 
       # Ensure the hack for the python version worked
       - name: Ensure we have the right Python
         shell: bash -l {0}
         run: |
           echo "Installed Python: $(python --version)"
           echo "Expected: ${{ matrix.python-version }}"
           python --version | grep "Python ${{ matrix.python-version }}"
 
-      # https://stackoverflow.com/questions/70520120/attributeerror-module-setuptools-distutils-has-no-attribute-version
-      # https://github.com/pytorch/pytorch/pull/69904
-      # - name: Downgrade setuptools due to a but in PyTorch 1.10.1
+      # # https://stackoverflow.com/questions/70520120/attributeerror-module-setuptools-distutils-has-no-attribute-version
+      # # https://github.com/pytorch/pytorch/pull/69904
+      # - name: Downgrade setuptools due to a bug in PyTorch 1.10.1
       #   shell: bash -l {0}
       #   run: |
       #     pip install setuptools==59.5.0 --upgrade
-
-      - name: Update conda environment
-        run: mamba env update -n ${{ env.PY_CONDA_ENV_NAME }} -f ${{ env.CONDA_ENV_FILE }}
-        if: steps.conda_cache.outputs.cache-hit != 'true'
-
-      # Update pip env whether or not there was a conda cache hit
-      - name: Update pip environment
-        shell: bash -l {0}
-        run: pip install -e ".[dev]"
-        if: steps.conda_cache.outputs.cache-hit == 'true'
-
       - run: pip3 list
         shell: bash -l {0}
       - run: mamba info
       - run: mamba list
 
-      # Ensure the hack for the python version worked
+        # Ensure the hack for the python version worked
       - name: Ensure we have the right Python
         shell: bash -l {0}
         run: |
           echo "Installed Python: $(python --version)"
           echo "Expected: ${{ matrix.python-version }}"
           python --version | grep "Python ${{ matrix.python-version }}"
 
       - name: Run pre-commits
         shell: bash -l {0}
         run: |
           pre-commit install
           pre-commit run -v --all-files --show-diff-on-failure
 
-      # - name: Test with pytest
-      #   shell: bash -l {0}
-      #   run: |
-      #     pytest -v
-
-      # - name: Build docs website
-      #   shell: bash -l {0}
-      #   run: |
-      #     git config user.name ci-bot
-      #     git config user.email ci-bot@ci.com
-      #     mike deploy --rebase --push --update-aliases ${RELEASE_TAG_VERSION} latest
-
-      - name: Check working directory status
-        run: git status
-
-      - name: Restore working directory (env.yaml Python version)
-        run: git checkout .
-
-      - name: Build SDist and wheel
-        run: pipx run build
-
-      - name: Check metadata
-        run: pipx run twine check dist/*
+      - name: Run tests and collect coverage
+        shell: bash -l {0}
+        run: |
+          pytest --cov --cov-report xml:coverage.xml
 
-      - name: Publish distribution 📦 to PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
+      - name: Upload coverage reports to Codecov
+        uses: codecov/codecov-action@v3
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `latentis-0.0.7/.gitignore` & `latentis-0.0.8/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 wandb
 multirun.yaml
 storage
+# ignore only top level benchmark folder
+/benchmarks
+/nexus
 
 # ignore the _version.py file
 _version.py
 
 # .gitignore defaults for python and pycharm
 .idea
```

### Comparing `latentis-0.0.7/.pre-commit-config.yaml` & `latentis-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `latentis-0.0.7/docs/index.md` & `latentis-0.0.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `latentis-0.0.7/mkdocs.yml` & `latentis-0.0.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `latentis-0.0.7/notebooks/demo_relative.ipynb` & `latentis-0.0.8/notebooks/demo_relative.ipynb`

 * *Files identical despite different names*

### Comparing `latentis-0.0.7/notebooks/demo_translation.ipynb` & `latentis-0.0.8/notebooks/demo_translation.ipynb`

 * *Files identical despite different names*

### Comparing `latentis-0.0.7/pyproject.toml` & `latentis-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 
 [tool.coverage.report]
 exclude_lines = [
     "raise NotImplementedError",
     "raise NotImplementedError()",
     "pragma: nocover",
     "if __name__ == .__main__.:",
-    "if TYPE_CHECKING:"
+    "if TYPE_CHECKING:",
+]
+omit = [
+    # ignore all test cases in tests/
+    "tests/*",
 ]
 
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
 
 [tool.mypy]
-files= ["src/**/*.py", "test/*.py"]
+files = ["src/**/*.py", "test/*.py"]
 ignore_missing_imports = true
 
 [tool.isort]
 profile = 'black'
 line_length = 120
 known_third_party = ["numpy", "pytest", "wandb", "torch"]
 known_local_folder = "latentis"
```

### Comparing `latentis-0.0.7/setup.cfg` & `latentis-0.0.8/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -29,15 +29,20 @@
 packages = find:
 install_requires = 
 	torchmetrics
 	scikit-learn
 	backports.strenum
 	
 	python-dotenv
+	GitPython
 	matplotlib
+	faiss-cpu
+	pandas
+	fire
+	lightning
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.txt, *.md
 
@@ -45,20 +50,25 @@
 docs = 
 	mkdocs
 	mkdocs-material
 	mike
 test = 
 	pytest
 	pytest-cov
+data = 
+	transformers
+	datasets
+	torchvision
 dev = 
 	black
 	flake8
 	isort
 	pre-commit
 	bandit
-	%(test)s
 	%(docs)s
+	%(test)s
+	%(data)s
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `latentis-0.0.7/src/latentis/measure/_metrics.py` & `latentis-0.0.8/src/latentis/measure/_abstract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import TYPE_CHECKING, Any, Callable, Mapping, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Mapping, Tuple
 
 import torch
 from torch import nn
 
-import latentis
+from latentis.serialize.io_utils import IndexableMixin
+from latentis.space import LatentSpace
 
 if TYPE_CHECKING:
     from latentis.types import Space
 
 
-class Metric(nn.Module):
+class Metric(nn.Module, IndexableMixin):
     def __init__(self, name: str) -> None:
         super().__init__()
         self._name: str = name
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(name={self.name})"
 
     @property
     def name(self) -> str:
         return self._name
 
     @abstractmethod
-    def _forward(self, space1: Space, space2: Space) -> Mapping[str, Any]:
+    def forward(self, *spaces: Space) -> Mapping[Tuple[str], Mapping[str, Any]]:
         raise NotImplementedError
 
-    def forward(self, space1: Space, *others: Space) -> Sequence[Mapping[str, Any]]:
-        result = [self._forward(space1, other) for other in others]
 
-        return result[0] if len(result) == 1 else result
+class PairwiseMetric(Metric):
+    def __init__(self, name: str) -> None:
+        super().__init__(name=name)
+
+    @abstractmethod
+    def forward(self, x: Space, y: Space) -> Mapping[str, Any]:
+        raise NotImplementedError
 
 
-# TODO
-class MetricFn(Metric):
+class MetricFn(PairwiseMetric):
     def __init__(self, key: str, fn: Callable([Space, Space], torch.Tensor)) -> None:
         super().__init__(fn.__name__ if hasattr(fn, "__name__") else key)
         self.key = key
         self.fn = fn
 
-    def _forward(self, space1: Space, space2: Space) -> Mapping[str, Any]:
-        if isinstance(space1, latentis.LatentSpace):
-            space1 = space1.vectors
+    def forward(self, x: Space, y: Space) -> Mapping[str, Any]:
+        if isinstance(x, LatentSpace):
+            x = x.vectors
 
-        if isinstance(space2, latentis.LatentSpace):
-            space2 = space2.vectors
+        if isinstance(y, LatentSpace):
+            y = y.vectors
 
-        return {self.key: self.fn(space1, space2)}
+        return {self.key: self.fn(x, y)}
```

### Comparing `latentis-0.0.7/src/latentis/project/relative.py` & `latentis-0.0.8/src/latentis/project/relative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 from typing import Callable, Optional, Sequence
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
-from latentis import LatentSpace
+from latentis.space import LatentSpace
 from latentis.transform import Transform
 from latentis.types import ProjectionFunc, Space
 
 
 def change_of_basis_proj(x: torch.Tensor, anchors: torch.Tensor) -> torch.Tensor:
     return torch.linalg.lstsq(anchors.T, x.T)[0].T
```

### Comparing `latentis-0.0.7/src/latentis/sample/sampling.py` & `latentis-0.0.8/src/latentis/sample/sampling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from typing import Optional, Sequence, Union
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Optional, Sequence, Union
 
 import torch
 from torch import nn
 
-from latentis.space import LatentSpace, SpaceProperty
-from latentis.types import Space
+from latentis.space import LatentSpace
+
+if TYPE_CHECKING:
+    from latentis.types import Space
 
 
 class Sampler(nn.Module):
     pass
 
 
 class Uniform(Sampler):
@@ -44,20 +48,19 @@
         assert len(set(type(space) for space in spaces)) == 1, "All spaces must be of the same class"
 
         ids = torch.randperm(len(spaces[0]), generator=self.generator)[:n]
 
         if isinstance(spaces[0], LatentSpace):
             out = tuple(
                 LatentSpace(
-                    vectors=space.vectors[ids],
-                    name=f"{space.name}{self.suffix}",
-                    features={
-                        SpaceProperty.SAMPLING_IDS: ids,
-                        **{key: values[ids] for key, values in space.features.items()},
-                    },
+                    vector_source=space.vectors[ids],
+                    # features={
+                    #     SpaceProperty.SAMPLING_IDS: ids,
+                    #     **{key: values[ids] for key, values in space.features.items()},
+                    # },
                 )
                 for space in spaces
             )
         else:
             out = tuple(space[ids] for space in spaces)
 
         return out[0] if len(out) == 1 else out
```

### Comparing `latentis-0.0.7/tests/conftest.py` & `latentis-0.0.8/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,60 @@
-from typing import Tuple
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Tuple
 
 import pytest
 import torch
 from torch import Tensor
 
-from latentis import LatentSpace
-from latentis.types import Space
+from latentis.space import LatentSpace
 from latentis.utils import seed_everything
 
+if TYPE_CHECKING:
+    from latentis.types import Space
+
 
 class Space1Params(object):
     seed_everything(42)
     instances = [
         LatentSpace(
-            vectors=torch.randn(1000, 128, dtype=torch.double),
-            name="space1",
-            features={
-                "label": torch.rand(1000) > 0.5,
-            },
+            vector_source=torch.randn(1000, 128, dtype=torch.double),
         ),
         torch.randn(1000, 128, dtype=torch.double),
     ]
 
 
 @pytest.fixture(params=Space1Params().instances, scope="session")
 def space1(request) -> Space:
     return request.param
 
 
 class Space2Params(object):
     seed_everything(42)
     instances = [
         LatentSpace(
-            vectors=torch.randn(53, 250, dtype=torch.double),
-            name="space2",
-            features={
-                "label": torch.rand(53) > 0.5,
-            },
+            vector_source=torch.randn(53, 250, dtype=torch.double),
         ),
         torch.randn(53, 250, dtype=torch.double),
     ]
 
 
 @pytest.fixture(params=Space2Params().instances, scope="session")
 def space2(request) -> Space:
     return request.param
 
 
 class ParallelSpaces(object):
     instances = [
         (
             LatentSpace(
-                vectors=torch.randn(space1_n, space_1_dim, dtype=torch.double),
-                name="space1",
+                vector_source=torch.randn(space1_n, space_1_dim, dtype=torch.double),
             ),
             LatentSpace(
-                vectors=torch.randn(space2_n, space2_dim, dtype=torch.double),
-                name="space2",
+                vector_source=torch.randn(space2_n, space2_dim, dtype=torch.double),
             ),
         )
         for (space1_n, space_1_dim), (space2_n, space2_dim) in [
             ((50, 250), (50, 250)),
             ((50, 250), (50, 300)),
             ((50, 300), (50, 250)),
             ((1000, 100), (1000, 500)),
@@ -86,18 +80,18 @@
     return request.param
 
 
 class TensorSpaceWithRef(object):
     seed_everything(42)
     instances = [
         (
-            torch.randn(space1_n, space_1_dim, dtype=torch.double),
+            torch.randn(space1_n, space1_dim, dtype=torch.double),
             torch.randn(space2_n, space2_dim, dtype=torch.double),
         )
-        for (space1_n, space_1_dim), (space2_n, space2_dim) in [
+        for (space1_n, space1_dim), (space2_n, space2_dim) in [
             ((10, 250), (100, 250)),
             ((300, 300), (20, 300)),
             ((100, 700), (42, 700)),
         ]
     ]
```

### Comparing `latentis-0.0.7/tests/project/conftest.py` & `latentis-0.0.8/tests/project/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,37 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import pytest
 import torch
 
-from latentis import LatentSpace
-from latentis.types import Space
+from latentis.space import LatentSpace
 from latentis.utils import seed_everything
 
+if TYPE_CHECKING:
+    from latentis.types import Space
 BATCH_DIM = 4
 LATENT_DIM = 8
 N_CLASSES = 10
 NUM_ANCHORS = 20
 
 
 class Anchor1Params(object):
     seed_everything(42)
     instances = [
         LatentSpace(
-            vectors=torch.randn(NUM_ANCHORS, LATENT_DIM, dtype=torch.double),
-            name="space1",
-            features={
-                "label": torch.rand(NUM_ANCHORS) > 0.5,
-            },
+            vector_source=torch.randn(NUM_ANCHORS, LATENT_DIM, dtype=torch.double),
         ),
         torch.randn(NUM_ANCHORS, LATENT_DIM, dtype=torch.double),
     ]
 
 
 @pytest.fixture(params=Anchor1Params().instances, scope="session")
-def anchor_latents(request) -> Space:
+def x_anchors(request) -> Space:
     return request.param
 
 
 # @pytest.fixture
 # def anchor_targets() -> torch.Tensor:
 #     return torch.cat(
 #         (
@@ -40,20 +41,16 @@
 #     )
 
 
 class X1Params(object):
     seed_everything(42)
     instances = [
         LatentSpace(
-            vectors=torch.randn(BATCH_DIM, LATENT_DIM, dtype=torch.double),
-            name="space1",
-            features={
-                "label": torch.rand(BATCH_DIM) > 0.5,
-            },
+            vector_source=torch.randn(BATCH_DIM, LATENT_DIM, dtype=torch.double),
         ),
         torch.randn(BATCH_DIM, LATENT_DIM, dtype=torch.double),
     ]
 
 
 @pytest.fixture(params=X1Params().instances, scope="session")
-def x_latents() -> torch.Tensor:
+def x() -> torch.Tensor:
     return torch.randn(BATCH_DIM, LATENT_DIM, dtype=torch.double)
```

### Comparing `latentis-0.0.7/tests/sample/test_sampling.py` & `latentis-0.0.8/tests/sample/test_sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import pytest
-import torch
 
 from latentis.sample import Uniform
-from latentis.space import LatentSpace, SpaceProperty
-from latentis.types import Space
+
+if TYPE_CHECKING:
+    from latentis.types import Space
 
 
 def test_uniform_sampler(space1: Space, space2: Space):
     # Test invalid inputs
     uniform = Uniform()
     with pytest.raises(AssertionError):
         _ = uniform(space1, n=-1)
@@ -17,53 +21,55 @@
 
     with pytest.raises(AssertionError):
         _, _ = uniform(space1, space2, n=10)
 
     # Test suffix
     uniform = Uniform(random_seed=0, suffix="_custom")
     subspace1 = uniform(space1, n=10)
-    if isinstance(space1, LatentSpace):
-        assert subspace1.name.startswith(space1.name)
-        assert subspace1.name.endswith("_custom")
-        assert subspace1.name == space1.name + "_custom"
+    # if isinstance(space1, LatentSpace):
+    # assert subspace1.name.startswith(space1._name)
+    # assert subspace1.name.endswith("_custom")
+    # assert subspace1.name == space1._name + "_custom"
+
+    # TODO: restore id comparisons
 
     # Test sampling size
     uniform = Uniform(random_seed=0)
     subspace2 = uniform(space2, n=10)
     assert len(subspace1) == 10 == len(subspace2)
 
     # Test sampling ids are present but different
-    if isinstance(space1, LatentSpace) and isinstance(space2, LatentSpace):
-        assert not torch.all(
-            subspace1.features[SpaceProperty.SAMPLING_IDS] == subspace2.features[SpaceProperty.SAMPLING_IDS]
-        )
+    # if isinstance(space1, LatentSpace) and isinstance(space2, LatentSpace):
+    #     assert not torch.all(
+    #         subspace1.features[SpaceProperty.SAMPLING_IDS] == subspace2.features[SpaceProperty.SAMPLING_IDS]
+    #     )
 
     # Parallel sampling given same seed
     uniform = Uniform(random_seed=0)
     subspace1 = uniform(space1, n=5)
     uniform = Uniform(random_seed=0)
     space1_2 = uniform(space1, n=5)
     assert len(subspace1) == 5 == len(space1_2)
 
     # Test sampling ids are present and the same
-    if isinstance(space1, LatentSpace) and isinstance(space2, LatentSpace):
-        assert torch.all(
-            subspace1.features[SpaceProperty.SAMPLING_IDS] == space1_2.features[SpaceProperty.SAMPLING_IDS]
-        ).item()
+    # if isinstance(space1, LatentSpace) and isinstance(space2, LatentSpace):
+    #     assert torch.all(
+    #         subspace1.features[SpaceProperty.SAMPLING_IDS] == space1_2.features[SpaceProperty.SAMPLING_IDS]
+    #     ).item()
 
     # Parallel sampling in the same call
     uniform = Uniform()
     subspace1, space1_2 = uniform(space1, space1, n=10)
     assert len(subspace1) == 10 == len(space1_2)
 
     # Test sampling ids are present and the same
-    if isinstance(space1, LatentSpace) and isinstance(space2, LatentSpace):
-        assert torch.all(
-            subspace1.features[SpaceProperty.SAMPLING_IDS] == space1_2.features[SpaceProperty.SAMPLING_IDS]
-        )
+    # if isinstance(space1, LatentSpace) and isinstance(space2, LatentSpace):
+    #     assert torch.all(
+    #         subspace1.features[SpaceProperty.SAMPLING_IDS] == space1_2.features[SpaceProperty.SAMPLING_IDS]
+    #     )
 
 
 # @pytest.mark.parametrize(
 #     "targets, num_classes",
 #     (
 #         (
 #             (
```

### Comparing `latentis-0.0.7/tests/test_space.py` & `latentis-0.0.8/tests/test_space.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from latentis.sample import Uniform
 from latentis.space import LatentSpace
-from latentis.types import Space
+
+if TYPE_CHECKING:
+    from latentis.types import Space
 
 
 def test_space_len(space1: Space):
     if isinstance(space1, LatentSpace):
         assert len(space1) == space1.vectors.shape[0]
 
 
 def test_space_repr(space1: Space):
     assert repr(space1)
 
 
 def test_space_get(space1: Space):
     item = space1[0]
     if isinstance(space1, LatentSpace):
-        assert item["x"].shape[0] == space1.vectors.shape[-1]
-        assert item["label"] == space1.features["label"][0]
+        assert item.shape[0] == space1.vectors.shape[-1]
 
 
 def test_space_sample_hook(space1: Space):
     if isinstance(space1, LatentSpace):
         subspace = space1.sample(Uniform(), n=50)
-        assert subspace.name == space1.name + "_sampled"
-        assert subspace.features["sampling_ids"].shape == (50,)
+        # assert subspace._name == space1._name + "_sampled"
         assert len(subspace) == 50
```

