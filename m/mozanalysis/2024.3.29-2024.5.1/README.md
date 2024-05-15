# Comparing `tmp/mozanalysis-2024.3.29.tar.gz` & `tmp/mozanalysis-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozanalysis-2024.3.29.tar", last modified: Fri Mar 29 14:35:18 2024, max compression
+gzip compressed data, was "mozanalysis-2024.5.1.tar", last modified: Tue May 14 18:40:50 2024, max compression
```

## Comparing `mozanalysis-2024.3.29.tar` & `mozanalysis-2024.5.1.tar`

### file list

```diff
@@ -1,104 +1,106 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.202560 mozanalysis-2024.3.29/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.190560 mozanalysis-2024.3.29/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4142 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1238 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      985 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1021 2024-03-29 14:35:18.202560 mozanalysis-2024.3.29/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2627 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.190560 mozanalysis-2024.3.29/docs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.190560 mozanalysis-2024.3.29/docs/_ext/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/_ext/metrics_docstrings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/about.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.190560 mozanalysis-2024.3.29/docs/adrs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4532 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/adrs/adr-0001-dependency_management.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.190560 mozanalysis-2024.3.29/docs/api/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.194560 mozanalysis-2024.3.29/docs/api/bayesian_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/bayesian_stats/bayesian_bootstrap.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/bayesian_stats/binary.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/bayesian_stats/survival_func.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/bayesian_stats.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/bq.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/config.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/experiment.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/exposure.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.194560 mozanalysis-2024.3.29/docs/api/frequentist_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/frequentist_stats/bootstrap.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/frequentist_stats/sample_size.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.194560 mozanalysis-2024.3.29/docs/api/metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/metrics/desktop.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/metrics/fenix.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/metrics/firefox_ios.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/metrics.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.194560 mozanalysis-2024.3.29/docs/api/segments/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/segments/desktop.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/segments.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api/sizing.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/api.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5711 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15311 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/guide.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      231 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/ruff.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2024-03-29 14:35:18.202560 mozanalysis-2024.3.29/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1273 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.186560 mozanalysis-2024.3.29/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.194560 mozanalysis-2024.3.29/src/mozanalysis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.194560 mozanalysis-2024.3.29/src/mozanalysis/bayesian_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9493 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/bayesian_stats/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11573 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8539 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/bayesian_stats/binary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5892 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/bayesian_stats/survival_func.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3172 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/bq.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8771 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    57151 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/experiment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3557 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/exposure.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.198560 mozanalysis-2024.3.29/src/mozanalysis/frequentist_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/frequentist_stats/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10766 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/frequentist_stats/bootstrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34453 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/frequentist_stats/sample_size.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.198560 mozanalysis-2024.3.29/src/mozanalysis/metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14870 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/metrics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2776 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/metrics/desktop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1033 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/metrics/fenix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      829 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/metrics/firefox_ios.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/metrics/focus_android.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/metrics/focus_ios.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      836 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/metrics/klar_android.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/metrics/klar_ios.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.198560 mozanalysis-2024.3.29/src/mozanalysis/segments/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8362 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/segments/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/segments/desktop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25702 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/sizing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4039 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/src/mozanalysis/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.202560 mozanalysis-2024.3.29/src/mozanalysis.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1021 2024-03-29 14:35:18.000000 mozanalysis-2024.3.29/src/mozanalysis.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2440 2024-03-29 14:35:18.000000 mozanalysis-2024.3.29/src/mozanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-29 14:35:18.000000 mozanalysis-2024.3.29/src/mozanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      259 2024-03-29 14:35:18.000000 mozanalysis-2024.3.29/src/mozanalysis.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-03-29 14:35:18.000000 mozanalysis-2024.3.29/src/mozanalysis.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.198560 mozanalysis-2024.3.29/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.202560 mozanalysis-2024.3.29/tests/bayesian_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/bayesian_stats/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7054 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/bayesian_stats/test_bayesian_bootstrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2287 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/bayesian_stats/test_binary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5514 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/bayesian_stats/test_consistency.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3358 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/bayesian_stats/test_init.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3990 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/bayesian_stats/test_survival_func.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.202560 mozanalysis-2024.3.29/tests/frequentist_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/frequentist_stats/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9479 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/frequentist_stats/test_bootstrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9096 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/frequentist_stats/test_sample_size_calc.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-29 14:35:18.202560 mozanalysis-2024.3.29/tests/helpers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/helpers/cheap_lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5117 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26177 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/test_experiment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1523 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/test_metric_libraries.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1282 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/test_metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2584 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/test_segment_libraries.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7936 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/test_sizing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tests/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1106 2024-03-29 14:35:02.000000 mozanalysis-2024.3.29/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.044798 mozanalysis-2024.5.1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.032797 mozanalysis-2024.5.1/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4142 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1238 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      985 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1051 2024-05-14 18:40:50.044798 mozanalysis-2024.5.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2627 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.032797 mozanalysis-2024.5.1/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.032797 mozanalysis-2024.5.1/docs/_ext/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/_ext/metrics_docstrings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/about.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.032797 mozanalysis-2024.5.1/docs/adrs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4532 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/adrs/adr-0001-dependency_management.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.036797 mozanalysis-2024.5.1/docs/api/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.036797 mozanalysis-2024.5.1/docs/api/bayesian_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/bayesian_stats/bayesian_bootstrap.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/bayesian_stats/binary.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/bayesian_stats/survival_func.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/bayesian_stats.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/bq.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/config.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/experiment.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/exposure.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.036797 mozanalysis-2024.5.1/docs/api/frequentist_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/frequentist_stats/bootstrap.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/frequentist_stats/sample_size.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.036797 mozanalysis-2024.5.1/docs/api/metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/metrics/desktop.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/metrics/fenix.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/metrics/firefox_ios.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/metrics.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.036797 mozanalysis-2024.5.1/docs/api/segments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/segments/desktop.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/segments.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api/sizing.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5711 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15311 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/guide.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      231 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/ruff.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2024-05-14 18:40:50.068798 mozanalysis-2024.5.1/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1300 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.032797 mozanalysis-2024.5.1/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.036797 mozanalysis-2024.5.1/src/mozanalysis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.040798 mozanalysis-2024.5.1/src/mozanalysis/bayesian_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9493 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/bayesian_stats/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11573 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8539 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/bayesian_stats/binary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5892 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/bayesian_stats/survival_func.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3172 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/bq.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8771 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57151 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/experiment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3557 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/exposure.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.040798 mozanalysis-2024.5.1/src/mozanalysis/frequentist_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/frequentist_stats/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10768 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/frequentist_stats/bootstrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17262 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/frequentist_stats/linear_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34453 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/frequentist_stats/sample_size.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.040798 mozanalysis-2024.5.1/src/mozanalysis/metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14870 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/metrics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2776 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/metrics/desktop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1033 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/metrics/fenix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      829 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/metrics/firefox_ios.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/metrics/focus_android.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/metrics/focus_ios.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      836 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/metrics/klar_android.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/metrics/klar_ios.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.040798 mozanalysis-2024.5.1/src/mozanalysis/segments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8362 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/segments/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/segments/desktop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25702 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/sizing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4039 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/src/mozanalysis/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.044798 mozanalysis-2024.5.1/src/mozanalysis.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1051 2024-05-14 18:40:49.000000 mozanalysis-2024.5.1/src/mozanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2537 2024-05-14 18:40:49.000000 mozanalysis-2024.5.1/src/mozanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-14 18:40:49.000000 mozanalysis-2024.5.1/src/mozanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      275 2024-05-14 18:40:49.000000 mozanalysis-2024.5.1/src/mozanalysis.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-05-14 18:40:49.000000 mozanalysis-2024.5.1/src/mozanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.044798 mozanalysis-2024.5.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.044798 mozanalysis-2024.5.1/tests/bayesian_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/bayesian_stats/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7054 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/bayesian_stats/test_bayesian_bootstrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2287 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/bayesian_stats/test_binary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5514 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/bayesian_stats/test_consistency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3358 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/bayesian_stats/test_init.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3990 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/bayesian_stats/test_survival_func.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.044798 mozanalysis-2024.5.1/tests/frequentist_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/frequentist_stats/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9479 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/frequentist_stats/test_bootstrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20560 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/frequentist_stats/test_linear_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9096 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/frequentist_stats/test_sample_size_calc.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 18:40:50.044798 mozanalysis-2024.5.1/tests/helpers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/helpers/cheap_lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5117 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26177 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/test_experiment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1523 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/test_metric_libraries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1282 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/test_metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2584 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/test_segment_libraries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7936 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/test_sizing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1106 2024-05-14 18:40:37.000000 mozanalysis-2024.5.1/tox.ini
```

### Comparing `mozanalysis-2024.3.29/.circleci/config.yml` & `mozanalysis-2024.5.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/.gitignore` & `mozanalysis-2024.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/CHANGELOG.rst` & `mozanalysis-2024.5.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/CODE_OF_CONDUCT.md` & `mozanalysis-2024.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/LICENSE` & `mozanalysis-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/PKG-INFO` & `mozanalysis-2024.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozanalysis
-Version: 2024.3.29
+Version: 2024.5.1
 Summary: A library for Mozilla experiments analysis
 Home-page: https://github.com/mozilla/mozanalysis
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.10,<=3.11
 License-File: LICENSE
 Requires-Dist: attrs
@@ -12,14 +12,15 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: scipy
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-bigquery-storage
 Requires-Dist: statsmodels
+Requires-Dist: marginaleffects
 Requires-Dist: matplotlib
 Provides-Extra: testing
 Requires-Dist: mock; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-ruff; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-timeout; extra == "testing"
```

### Comparing `mozanalysis-2024.3.29/README.md` & `mozanalysis-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/docs/_ext/metrics_docstrings.py` & `mozanalysis-2024.5.1/docs/_ext/metrics_docstrings.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/docs/adrs/adr-0001-dependency_management.md` & `mozanalysis-2024.5.1/docs/adrs/adr-0001-dependency_management.md`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/docs/conf.py` & `mozanalysis-2024.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/docs/guide.rst` & `mozanalysis-2024.5.1/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/setup.py` & `mozanalysis-2024.5.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         "numpy",
         "pandas",
         "pyarrow",
         "scipy",
         "google-cloud-bigquery",
         "google-cloud-bigquery-storage",
         "statsmodels",
+        "marginaleffects",
         "matplotlib",
     ],
     setup_requires=["pytest-runner", "setuptools_scm"],
     extras_require={
         "testing": tests_require,
         "docs": docs_require,
     },
```

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/__init__.py` & `mozanalysis-2024.5.1/src/mozanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/bayesian_stats/__init__.py` & `mozanalysis-2024.5.1/src/mozanalysis/bayesian_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py` & `mozanalysis-2024.5.1/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/bayesian_stats/binary.py` & `mozanalysis-2024.5.1/src/mozanalysis/bayesian_stats/binary.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/bayesian_stats/survival_func.py` & `mozanalysis-2024.5.1/src/mozanalysis/bayesian_stats/survival_func.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/bq.py` & `mozanalysis-2024.5.1/src/mozanalysis/bq.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/config.py` & `mozanalysis-2024.5.1/src/mozanalysis/config.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/experiment.py` & `mozanalysis-2024.5.1/src/mozanalysis/experiment.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/exposure.py` & `mozanalysis-2024.5.1/src/mozanalysis/exposure.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/frequentist_stats/bootstrap.py` & `mozanalysis-2024.5.1/src/mozanalysis/frequentist_stats/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
+
+
 import numpy as np
 import pandas as pd
 
 import mozanalysis.bayesian_stats as mabs
 from mozanalysis.utils import filter_outliers
```

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/frequentist_stats/sample_size.py` & `mozanalysis-2024.5.1/src/mozanalysis/frequentist_stats/sample_size.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/metrics/__init__.py` & `mozanalysis-2024.5.1/src/mozanalysis/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/metrics/desktop.py` & `mozanalysis-2024.5.1/src/mozanalysis/metrics/desktop.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/metrics/fenix.py` & `mozanalysis-2024.5.1/src/mozanalysis/metrics/fenix.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/metrics/firefox_ios.py` & `mozanalysis-2024.5.1/src/mozanalysis/metrics/firefox_ios.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/metrics/focus_android.py` & `mozanalysis-2024.5.1/src/mozanalysis/metrics/focus_android.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/metrics/focus_ios.py` & `mozanalysis-2024.5.1/src/mozanalysis/metrics/focus_ios.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/metrics/klar_android.py` & `mozanalysis-2024.5.1/src/mozanalysis/metrics/klar_android.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/metrics/klar_ios.py` & `mozanalysis-2024.5.1/src/mozanalysis/metrics/klar_ios.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/segments/__init__.py` & `mozanalysis-2024.5.1/src/mozanalysis/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/segments/desktop.py` & `mozanalysis-2024.5.1/src/mozanalysis/segments/desktop.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/sizing.py` & `mozanalysis-2024.5.1/src/mozanalysis/sizing.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis/utils.py` & `mozanalysis-2024.5.1/src/mozanalysis/utils.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/src/mozanalysis.egg-info/PKG-INFO` & `mozanalysis-2024.5.1/src/mozanalysis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozanalysis
-Version: 2024.3.29
+Version: 2024.5.1
 Summary: A library for Mozilla experiments analysis
 Home-page: https://github.com/mozilla/mozanalysis
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.10,<=3.11
 License-File: LICENSE
 Requires-Dist: attrs
@@ -12,14 +12,15 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: scipy
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-bigquery-storage
 Requires-Dist: statsmodels
+Requires-Dist: marginaleffects
 Requires-Dist: matplotlib
 Provides-Extra: testing
 Requires-Dist: mock; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-ruff; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-timeout; extra == "testing"
```

### Comparing `mozanalysis-2024.3.29/src/mozanalysis.egg-info/SOURCES.txt` & `mozanalysis-2024.5.1/src/mozanalysis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 src/mozanalysis.egg-info/top_level.txt
 src/mozanalysis/bayesian_stats/__init__.py
 src/mozanalysis/bayesian_stats/bayesian_bootstrap.py
 src/mozanalysis/bayesian_stats/binary.py
 src/mozanalysis/bayesian_stats/survival_func.py
 src/mozanalysis/frequentist_stats/__init__.py
 src/mozanalysis/frequentist_stats/bootstrap.py
+src/mozanalysis/frequentist_stats/linear_models.py
 src/mozanalysis/frequentist_stats/sample_size.py
 src/mozanalysis/metrics/__init__.py
 src/mozanalysis/metrics/desktop.py
 src/mozanalysis/metrics/fenix.py
 src/mozanalysis/metrics/firefox_ios.py
 src/mozanalysis/metrics/focus_android.py
 src/mozanalysis/metrics/focus_ios.py
@@ -74,9 +75,10 @@
 tests/bayesian_stats/test_bayesian_bootstrap.py
 tests/bayesian_stats/test_binary.py
 tests/bayesian_stats/test_consistency.py
 tests/bayesian_stats/test_init.py
 tests/bayesian_stats/test_survival_func.py
 tests/frequentist_stats/__init__.py
 tests/frequentist_stats/test_bootstrap.py
+tests/frequentist_stats/test_linear_models.py
 tests/frequentist_stats/test_sample_size_calc.py
 tests/helpers/cheap_lint.py
```

### Comparing `mozanalysis-2024.3.29/tests/bayesian_stats/test_bayesian_bootstrap.py` & `mozanalysis-2024.5.1/tests/bayesian_stats/test_bayesian_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/bayesian_stats/test_binary.py` & `mozanalysis-2024.5.1/tests/bayesian_stats/test_binary.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/bayesian_stats/test_consistency.py` & `mozanalysis-2024.5.1/tests/bayesian_stats/test_consistency.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/bayesian_stats/test_init.py` & `mozanalysis-2024.5.1/tests/bayesian_stats/test_init.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/bayesian_stats/test_survival_func.py` & `mozanalysis-2024.5.1/tests/bayesian_stats/test_survival_func.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/frequentist_stats/test_bootstrap.py` & `mozanalysis-2024.5.1/tests/frequentist_stats/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/frequentist_stats/test_sample_size_calc.py` & `mozanalysis-2024.5.1/tests/frequentist_stats/test_sample_size_calc.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/test_config.py` & `mozanalysis-2024.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/test_experiment.py` & `mozanalysis-2024.5.1/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/test_metric_libraries.py` & `mozanalysis-2024.5.1/tests/test_metric_libraries.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/test_metrics.py` & `mozanalysis-2024.5.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/test_segment_libraries.py` & `mozanalysis-2024.5.1/tests/test_segment_libraries.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/test_sizing.py` & `mozanalysis-2024.5.1/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tests/test_utils.py` & `mozanalysis-2024.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.3.29/tox.ini` & `mozanalysis-2024.5.1/tox.ini`

 * *Files identical despite different names*

