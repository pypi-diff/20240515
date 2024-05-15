# Comparing `tmp/hipscat_import-0.3.1.tar.gz` & `tmp/hipscat_import-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat_import-0.3.1.tar", last modified: Wed Apr 24 16:22:19 2024, max compression
+gzip compressed data, was "hipscat_import-0.3.2.tar", last modified: Wed May 15 19:40:07 2024, max compression
```

## Comparing `hipscat_import-0.3.1.tar` & `hipscat_import-0.3.2.tar`

### file list

```diff
@@ -1,283 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.922298 hipscat_import-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.922298 hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/docs/catalogs/
--rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/arguments.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.926298 hipscat_import-0.3.1/docs/catalogs/public/
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/allwise.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/neowise.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/panstarrs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/sdss.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/tic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/public/zubercal.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/catalogs/temp_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.930298 hipscat_import-0.3.1/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/dask_on_ray.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/index_table.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/guide/margin_cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.930298 hipscat_import-0.3.1/docs/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7615 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/notebooks/estimate_pixel_threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/notebooks/unequal_schema.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.930298 hipscat_import-0.3.1/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)   136863 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/allwise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/allwise_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)    66486 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/neowise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/neowise_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/ps1_detections_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/ps1_otmo_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)   412559 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/sdss_wget.bash
--rw-r--r--   0 runner    (1001) docker     (127)    57050 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/tic_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/docs/static/tic_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.930298 hipscat_import-0.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.934298 hipscat_import-0.3.1/src/hipscat_import/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.934298 hipscat_import-0.3.1/src/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     9758 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/file_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/catalog/run_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.934298 hipscat_import-0.3.1/src/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/index/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/index/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/index/run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.934298 hipscat_import-0.3.1/src/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/pipeline_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/src/hipscat_import/soap/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/soap/run_soap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/src/hipscat_import/verification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/verification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/verification/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/src/hipscat_import/verification/run_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/src/hipscat_import.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 16:22:19.000000 hipscat_import-0.3.1/src/hipscat_import.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/hipscat_import/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_file_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_run_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/catalog/test_run_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.922298 hipscat_import-0.3.1/tests/hipscat_import/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/hipscat_import/data/blank/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/blank/blank.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.938298 hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/input_01.csv
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/input_02.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/schema.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.942298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.942298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.942298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.942298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/resume/intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.946298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.950298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.950298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.950298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.950298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source/
--rw-r--r--   0 runner    (1001) docker     (127)  1688789 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.954298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.954298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.954298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.954298 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.958298 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/0_4.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/1_47.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_176.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_177.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_178.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_179.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_180.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_181.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_182.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_183.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_184.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_185.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_186.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/2_187.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.918298 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.962298 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    33062 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    19958 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.962298 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/catalog.starr
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/gaia_minimum.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/hipscat_index.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/hipscat_index.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/macauff_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/pandasindex.parquet
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/pipe_delimited.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/small_sky.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.962298 hipscat_import-0.3.1/tests/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/index/test_index_argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/index/test_index_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/index/test_run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.962298 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_round_trip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/tests/hipscat_import/soap/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/test_run_soap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/test_pipeline_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/test_runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:22:19.966298 hipscat_import-0.3.1/tests/hipscat_import/verification/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/verification/test_run_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-24 16:22:07.000000 hipscat_import-0.3.1/tests/hipscat_import/verification/test_verification_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.346019 hipscat_import-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.346019 hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.346019 hipscat_import-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/arguments.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/catalogs/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/allwise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/neowise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/panstarrs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/sdss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/tic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/zubercal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/temp_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/dask_on_ray.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/index_table.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/margin_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.354019 hipscat_import-0.3.2/docs/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7615 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/notebooks/estimate_pixel_threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/notebooks/unequal_schema.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.354019 hipscat_import-0.3.2/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   136863 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/allwise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/allwise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    66486 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/neowise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/neowise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/ps1_detections_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/ps1_otmo_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   412559 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/sdss_wget.bash
+-rw-r--r--   0 runner    (1001) docker     (127)    57050 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/tic_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/tic_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.354019 hipscat_import-0.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.354019 hipscat_import-0.3.2/src/hipscat_import/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.358019 hipscat_import-0.3.2/src/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/run_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/sparse_histogram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.358019 hipscat_import-0.3.2/src/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/index/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/index/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/index/run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.358019 hipscat_import-0.3.2/src/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/pipeline_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/src/hipscat_import/soap/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/run_soap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/src/hipscat_import/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/verification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/verification/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/verification/run_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/src/hipscat_import.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/hipscat_import/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_run_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22142 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_run_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_sparse_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/hipscat_import/data/blank/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/blank/blank.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/input_01.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/input_02.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/schema.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.338019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.338019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.338019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.366019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.338019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.366019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.366019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.366019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/resume/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/resume/intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.374019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.374019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.374019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_10_of_05.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.374019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source/
+-rw-r--r--   0 runner    (1001) docker     (127)  1688789 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.378019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.378019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.378019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.382019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.386019 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/0_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/1_47.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_176.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_177.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_178.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_179.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_180.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_181.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_182.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_183.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_184.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_185.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_186.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_187.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.386019 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    33062 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    19958 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.390019 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/catalog.starr
+-rw-r--r--   0 runner    (1001) docker     (127)    45749 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_epoch.ecsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_minimum.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/hipscat_index.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/hipscat_index.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/macauff_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/pandasindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/pipe_delimited.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/small_sky.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.390019 hipscat_import-0.3.2/tests/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/index/test_index_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/index/test_index_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/index/test_run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.390019 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_round_trip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/tests/hipscat_import/soap/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/test_run_soap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/test_pipeline_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/test_runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/tests/hipscat_import/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/verification/test_run_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/verification/test_verification_arguments.py
```

### Comparing `hipscat_import-0.3.1/.copier-answers.yml` & `hipscat_import-0.3.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.gitattributes` & `hipscat_import-0.3.2/.gitattributes`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.github/pull_request_template.md` & `hipscat_import-0.3.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.github/workflows/build-documentation.yml` & `hipscat_import-0.3.2/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.github/workflows/pre-commit-ci.yml` & `hipscat_import-0.3.2/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.github/workflows/publish-to-pypi.yml` & `hipscat_import-0.3.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.github/workflows/smoke-test.yml` & `hipscat_import-0.3.2/.github/workflows/smoke-test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.9', '3.10', '3.11.8']
+        python-version: ['3.9', '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `hipscat_import-0.3.1/.github/workflows/testing-and-coverage.yml` & `hipscat_import-0.3.2/.github/workflows/testing-and-coverage.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.9', '3.10', '3.11.8']
+        python-version: ['3.9', '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `hipscat_import-0.3.1/.gitignore` & `hipscat_import-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.pre-commit-config.yaml` & `hipscat_import-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/.setup_dev.sh` & `hipscat_import-0.3.2/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/LICENSE` & `hipscat_import-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/PKG-INFO` & `hipscat_import-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.3.1
+Version: 0.3.2
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,22 +38,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask[complete]>=2024.3.0
 Requires-Dist: deprecated
 Requires-Dist: healpy
-Requires-Dist: hipscat>=0.2.9
+Requires-Dist: hipscat>=0.3.0
 Requires-Dist: ipykernel
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
 Requires-Dist: tqdm
 Requires-Dist: numpy
-Requires-Dist: fsspec<=2024.2.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `hipscat_import-0.3.1/README.md` & `hipscat_import-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/Makefile` & `hipscat_import-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/catalogs/arguments.rst` & `hipscat_import-0.3.2/docs/catalogs/arguments.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/catalogs/public/allwise.rst` & `hipscat_import-0.3.2/docs/catalogs/public/allwise.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/catalogs/public/index.rst` & `hipscat_import-0.3.2/docs/catalogs/public/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/catalogs/public/neowise.rst` & `hipscat_import-0.3.2/docs/catalogs/public/neowise.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/catalogs/public/panstarrs.rst` & `hipscat_import-0.3.2/docs/catalogs/public/panstarrs.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/catalogs/public/sdss.rst` & `hipscat_import-0.3.2/docs/catalogs/public/sdss.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/catalogs/public/tic.rst` & `hipscat_import-0.3.2/docs/catalogs/public/tic.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/catalogs/public/zubercal.rst` & `hipscat_import-0.3.2/docs/catalogs/public/zubercal.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/catalogs/temp_files.rst` & `hipscat_import-0.3.2/docs/catalogs/temp_files.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/conf.py` & `hipscat_import-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/guide/contact.rst` & `hipscat_import-0.3.2/docs/guide/contact.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/guide/contributing.rst` & `hipscat_import-0.3.2/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/guide/dask_on_ray.rst` & `hipscat_import-0.3.2/docs/guide/dask_on_ray.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/guide/index_table.rst` & `hipscat_import-0.3.2/docs/guide/index_table.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/guide/margin_cache.rst` & `hipscat_import-0.3.2/docs/guide/margin_cache.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/index.rst` & `hipscat_import-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/notebooks/estimate_pixel_threshold.ipynb` & `hipscat_import-0.3.2/docs/notebooks/estimate_pixel_threshold.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/notebooks/unequal_schema.ipynb` & `hipscat_import-0.3.2/docs/notebooks/unequal_schema.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/static/allwise_schema.parquet` & `hipscat_import-0.3.2/docs/static/allwise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/static/allwise_types.csv` & `hipscat_import-0.3.2/docs/static/allwise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/static/neowise_schema.parquet` & `hipscat_import-0.3.2/docs/static/neowise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/static/neowise_types.csv` & `hipscat_import-0.3.2/docs/static/neowise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/static/ps1_detections_types.csv` & `hipscat_import-0.3.2/docs/static/ps1_detections_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/static/ps1_otmo_types.csv` & `hipscat_import-0.3.2/docs/static/ps1_otmo_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/static/sdss_wget.bash` & `hipscat_import-0.3.2/docs/static/sdss_wget.bash`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/static/tic_schema.parquet` & `hipscat_import-0.3.2/docs/static/tic_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/docs/static/tic_types.csv` & `hipscat_import-0.3.2/docs/static/tic_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/pyproject.toml` & `hipscat_import-0.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,21 @@
     "Programming Language :: Python",
 ]
 dynamic = ["version"]
 dependencies = [
     "dask[complete]>=2024.3.0", # Includes dask expressions.
     "deprecated",
     "healpy",
-    "hipscat >= 0.2.9",
+    "hipscat >=0.3.0",
     "ipykernel", # Support for Jupyter notebooks
     "pandas",
     "pyarrow",
     "pyyaml",
     "tqdm",
     "numpy",
-    "fsspec <= 2024.2.0", # Remove when pyarrow updates to reflect api changes
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 dev = [
     "black", # Used for static linting of files
     "jupyter", # Clears output from Jupyter notebooks
```

### Comparing `hipscat_import-0.3.1/src/.pylintrc` & `hipscat_import-0.3.2/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/catalog/arguments.py` & `hipscat_import-0.3.2/src/hipscat_import/catalog/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             self.add_hipscat_index = False
             if self.sort_columns:
                 raise ValueError("When using _hipscat_index for position, no sort columns should be added")
 
         # Basic checks complete - make more checks and create directories where necessary
         self.input_paths = find_input_paths(
             self.input_path,
-            "**/**.*",
+            "**/*.*",
             self.input_file_list,
             storage_options=self.input_storage_options,
         )
         self.resume_plan = ResumePlan(
             resume=self.resume,
             progress_bar=self.progress_bar,
             input_paths=self.input_paths,
```

### Comparing `hipscat_import-0.3.1/src/hipscat_import/catalog/file_readers.py` & `hipscat_import-0.3.2/src/hipscat_import/catalog/file_readers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """File reading generators for common file types."""
 
 import abc
 from typing import Any, Dict, Union
 
 import pyarrow.parquet as pq
+from astropy.io import ascii as ascii_reader
 from astropy.table import Table
 from hipscat.io import FilePointer, file_io
 
 # pylint: disable=too-few-public-methods,too-many-arguments
 
 
 def get_file_reader(
@@ -34,22 +35,24 @@
         schema_file (str): path to a parquet schema file. if provided, header names
             and column types will be pulled from the parquet schema metadata.
         column_names (list[str]): for CSV files, the names of columns if no header
             is available. for fits files, a list of columns to *keep*.
         skip_column_names (list[str]): for fits files, a list of columns to remove.
         type_map (dict): for CSV files, the data types to use for columns
     """
-    if "csv" in file_format:
+    if file_format == "csv":
         return CsvReader(
             chunksize=chunksize,
             schema_file=schema_file,
             column_names=column_names,
             type_map=type_map,
             **kwargs,
         )
+    if file_format == "ecsv":
+        return AstropyEcsvReader(**kwargs)
     if file_format == "fits":
         return FitsReader(
             chunksize=chunksize,
             column_names=column_names,
             skip_column_names=skip_column_names,
             **kwargs,
         )
@@ -129,30 +132,31 @@
         self.header = header
         self.schema_file = schema_file
         self.column_names = column_names
         self.type_map = type_map
         self.parquet_kwargs = parquet_kwargs
         self.kwargs = kwargs
 
+        schema_parquet = None
         if self.schema_file:
             if self.parquet_kwargs is None:
                 self.parquet_kwargs = {}
             schema_parquet = file_io.load_parquet_to_pandas(
                 FilePointer(self.schema_file),
                 **self.parquet_kwargs,
             )
 
         if self.column_names:
             self.kwargs["names"] = self.column_names
-        elif not self.header and self.schema_file:
+        elif not self.header and schema_parquet is not None:
             self.kwargs["names"] = schema_parquet.columns
 
         if self.type_map:
             self.kwargs["dtype"] = self.type_map
-        elif self.schema_file:
+        elif schema_parquet is not None:
             self.kwargs["dtype"] = schema_parquet.dtypes.to_dict()
 
     def read(self, input_file, read_columns=None):
         self.regular_file_exists(input_file, **self.kwargs)
 
         if read_columns:
             self.kwargs["usecols"] = read_columns
@@ -176,14 +180,35 @@
             "column_names": self.column_names,
             "parquet_kwargs": self.parquet_kwargs,
             "kwargs": str_kwargs,
         }
         return provenance_info
 
 
+class AstropyEcsvReader(InputReader):
+    """Reads astropy ascii .ecsv files.
+
+    Note that this is NOT a chunked reader. Use caution when reading
+    large ECSV files with this reader."""
+
+    def __init__(self, **kwargs):
+        self.kwargs = kwargs
+
+    def read(self, input_file, read_columns=None):
+        self.regular_file_exists(input_file, **self.kwargs)
+        if read_columns:
+            self.kwargs["include_names"] = read_columns
+
+        astropy_table = ascii_reader.read(input_file, format="ecsv", **self.kwargs)
+        yield astropy_table.to_pandas()
+
+    def provenance_info(self):
+        return {"input_reader_type": "AstropyEcsvReader"}
+
+
 class FitsReader(InputReader):
     """Chunked FITS file reader.
 
     There are two column-level arguments for reading fits files:
     `column_names` and `skip_column_names`.
 
         - If neither is provided, we will read and process all columns in the fits file.
@@ -221,15 +246,26 @@
         elif self.skip_column_names:
             table.remove_columns(self.skip_column_names)
 
         total_rows = len(table)
         read_rows = 0
 
         while read_rows < total_rows:
-            yield table[read_rows : read_rows + self.chunksize].to_pandas()
+            df_chunk = table[read_rows : read_rows + self.chunksize].to_pandas()
+            for column in df_chunk.columns:
+                if (
+                    df_chunk[column].dtype == object
+                    and df_chunk[column].apply(lambda x: isinstance(x, bytes)).any()
+                ):
+                    df_chunk[column] = df_chunk[column].apply(
+                        lambda x: x.decode("utf-8") if isinstance(x, bytes) else x
+                    )
+
+            yield df_chunk
+
             read_rows += self.chunksize
 
     def provenance_info(self) -> dict:
         provenance_info = {
             "input_reader_type": "FitsReader",
             "chunksize": self.chunksize,
             "column_names": self.column_names,
```

### Comparing `hipscat_import-0.3.1/src/hipscat_import/catalog/map_reduce.py` & `hipscat_import-0.3.2/src/hipscat_import/catalog/map_reduce.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from hipscat import pixel_math
 from hipscat.io import FilePointer, file_io, paths
 from hipscat.pixel_math.healpix_pixel import HealpixPixel
 from hipscat.pixel_math.hipscat_id import HIPSCAT_ID_COLUMN, hipscat_id_to_healpix
 
 from hipscat_import.catalog.file_readers import InputReader
 from hipscat_import.catalog.resume_plan import ResumePlan
+from hipscat_import.catalog.sparse_histogram import SparseHistogram
 from hipscat_import.pipeline_resume_plan import get_pixel_cache_directory
 
 # pylint: disable=too-many-locals,too-many-arguments
 
 
 def _has_named_index(dataframe):
     """Heuristic to determine if a dataframe has some meaningful index.
@@ -89,28 +90,30 @@
     Returns:
         one-dimensional numpy array of long integers where the value at each index corresponds
         to the number of objects found at the healpix pixel.
     Raises:
         ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
         FileNotFoundError: if the file does not exist, or is a directory
     """
-    histo = pixel_math.empty_histogram(highest_order)
+    histo = SparseHistogram.make_empty(highest_order)
 
     if use_hipscat_index:
         read_columns = [HIPSCAT_ID_COLUMN]
     else:
         read_columns = [ra_column, dec_column]
 
     for _, _, mapped_pixels in _iterate_input_file(
         input_file, file_reader, highest_order, ra_column, dec_column, use_hipscat_index, read_columns
     ):
         mapped_pixel, count_at_pixel = np.unique(mapped_pixels, return_counts=True)
-        mapped_pixel = mapped_pixel.astype(np.int64)
-        histo[mapped_pixel] += count_at_pixel.astype(np.int64)
-    ResumePlan.write_partial_histogram(tmp_path=resume_path, mapping_key=mapping_key, histogram=histo)
+
+        partial = SparseHistogram.make_from_counts(mapped_pixel, count_at_pixel, healpix_order=highest_order)
+        histo.add(partial)
+
+    histo.to_file(ResumePlan.partial_histogram_file(tmp_path=resume_path, mapping_key=mapping_key))
 
 
 def split_pixels(
     input_file: FilePointer,
     file_reader: InputReader,
     splitting_key,
     highest_order,
@@ -156,15 +159,15 @@
             output_file = file_io.append_paths_to_pointer(
                 pixel_dir, f"shard_{splitting_key}_{chunk_number}.parquet"
             )
             if _has_named_index(filtered_data):
                 filtered_data.to_parquet(output_file, index=True)
             else:
                 filtered_data.to_parquet(output_file, index=False)
-        del filtered_data, data_indexes
+            del filtered_data, data_indexes
 
     ResumePlan.splitting_key_done(tmp_path=resume_path, splitting_key=splitting_key)
 
 
 def reduce_pixel_shards(
     cache_shard_path,
     resume_path,
```

### Comparing `hipscat_import-0.3.1/src/hipscat_import/catalog/resume_plan.py` & `hipscat_import-0.3.2/src/hipscat_import/catalog/resume_plan.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import List, Optional, Tuple
 
 import healpy as hp
-import numpy as np
-from hipscat import pixel_math
 from hipscat.io import FilePointer, file_io
 from hipscat.pixel_math.healpix_pixel import HealpixPixel
-from numpy import frombuffer
 from tqdm.auto import tqdm
 
+from hipscat_import.catalog.sparse_histogram import SparseHistogram
 from hipscat_import.pipeline_resume_plan import PipelineResumePlan
 
 
 @dataclass
 class ResumePlan(PipelineResumePlan):
     """Container class for holding the state of each file in the pipeline plan."""
 
@@ -29,15 +27,15 @@
     destination_pixel_map: Optional[List[Tuple[HealpixPixel, List[HealpixPixel], str]]] = None
     """Fully resolved map of destination pixels to constituent smaller pixels"""
 
     MAPPING_STAGE = "mapping"
     SPLITTING_STAGE = "splitting"
     REDUCING_STAGE = "reducing"
 
-    HISTOGRAM_BINARY_FILE = "mapping_histogram.binary"
+    HISTOGRAM_BINARY_FILE = "mapping_histogram.npz"
     HISTOGRAMS_DIR = "histograms"
 
     def __post_init__(self):
         """Initialize the plan."""
         self.gather_plan()
 
     def gather_plan(self):
@@ -88,99 +86,73 @@
             )
             step_progress.update(1)
 
     def get_remaining_map_keys(self):
         """Gather remaining keys, dropping successful mapping tasks from histogram names.
 
         Returns:
-            list of mapping keys *not* found in files like /resume/path/mapping_key.binary
+            list of mapping keys *not* found in files like /resume/path/mapping_key.npz
         """
         prefix = file_io.append_paths_to_pointer(self.tmp_path, self.HISTOGRAMS_DIR)
-        mapped_keys = self.get_keys_from_file_names(prefix, ".binary")
+        mapped_keys = self.get_keys_from_file_names(prefix, ".npz")
         return [
             (f"map_{i}", file_path)
             for i, file_path in enumerate(self.input_paths)
             if f"map_{i}" not in mapped_keys
         ]
 
     def read_histogram(self, healpix_order):
         """Return histogram with healpix_order'd shape
 
         - Try to find a combined histogram
         - Otherwise, combine histograms from partials
         - Otherwise, return an empty histogram
         """
         file_name = file_io.append_paths_to_pointer(self.tmp_path, self.HISTOGRAM_BINARY_FILE)
-        if file_io.does_file_or_directory_exist(file_name):
-            # Look for the single combined histogram file
-            with open(file_name, "rb") as file_handle:
-                full_histogram = frombuffer(file_handle.read(), dtype=np.int64)
-        else:
-            # Read the histogram from partial binaries
-            full_histogram = self.read_histogram_from_partials(healpix_order)
+        if not file_io.does_file_or_directory_exist(file_name):
+            # Read the histogram from partial histograms and combine.
+            remaining_map_files = self.get_remaining_map_keys()
+            if len(remaining_map_files) > 0:
+                raise RuntimeError(f"{len(remaining_map_files)} map stages did not complete successfully.")
+            histogram_files = file_io.find_files_matching_path(self.tmp_path, self.HISTOGRAMS_DIR, "*.npz")
+            aggregate_histogram = SparseHistogram.make_empty(healpix_order)
+            for partial_file_name in histogram_files:
+                aggregate_histogram.add(SparseHistogram.from_file(partial_file_name))
+
+            aggregate_histogram.to_file(file_name)
+            file_io.remove_directory(
+                file_io.append_paths_to_pointer(self.tmp_path, self.HISTOGRAMS_DIR),
+                ignore_errors=True,
+            )
+
+        full_histogram = SparseHistogram.from_file(file_name).to_array()
+
         if len(full_histogram) != hp.order2npix(healpix_order):
             raise ValueError(
                 "The histogram from the previous execution is incompatible with "
                 + "the highest healpix order. To start the importing pipeline "
                 + "from scratch with the current order set `resume` to False."
             )
         return full_histogram
 
-    def _get_partial_filenames(self):
-        remaining_map_files = self.get_remaining_map_keys()
-        if len(remaining_map_files) > 0:
-            raise RuntimeError(f"{len(remaining_map_files)} map stages did not complete successfully.")
-        histogram_files = file_io.find_files_matching_path(self.tmp_path, self.HISTOGRAMS_DIR, "**.binary")
-        return histogram_files
-
-    def read_histogram_from_partials(self, healpix_order):
-        """Combines the histogram partials to get the full histogram."""
-        histogram_files = self._get_partial_filenames()
-        full_histogram = pixel_math.empty_histogram(healpix_order)
-        # Read the partial histograms and make sure they are all the same size
-        for index, file_name in enumerate(histogram_files):
-            with open(file_name, "rb") as file_handle:
-                partial = frombuffer(file_handle.read(), dtype=np.int64)
-                if index == 0:
-                    full_histogram = partial
-                elif len(partial) != len(full_histogram):
-                    raise ValueError("The histogram partials have inconsistent sizes.")
-                else:
-                    full_histogram = np.add(full_histogram, partial)
-        self._write_combined_histogram(full_histogram)
-        return full_histogram
-
     @classmethod
-    def write_partial_histogram(cls, tmp_path, mapping_key: str, histogram):
-        """Write partial histogram to a special intermediate directory
+    def partial_histogram_file(cls, tmp_path, mapping_key: str):
+        """File name for writing a histogram file to a special intermediate directory.
+
+        As a side effect, this method may create the special intermediate directory.
 
         Args:
             tmp_path (str): where to write intermediate resume files.
             mapping_key (str): unique string for each mapping task (e.g. "map_57")
-            histogram (np.array): one-dimensional numpy array of long integers where
-                the value at each index corresponds to the number of objects found at
-                the healpix pixel.
         """
         file_io.make_directory(
             file_io.append_paths_to_pointer(tmp_path, cls.HISTOGRAMS_DIR),
             exist_ok=True,
         )
-        file_name = file_io.append_paths_to_pointer(tmp_path, cls.HISTOGRAMS_DIR, f"{mapping_key}.binary")
-        with open(file_name, "wb+") as file_handle:
-            file_handle.write(histogram.data)
-
-    def _write_combined_histogram(self, histogram):
-        """Writes the full histogram to disk, removing the pre-existing partials."""
-        file_name = file_io.append_paths_to_pointer(self.tmp_path, self.HISTOGRAM_BINARY_FILE)
-        with open(file_name, "wb+") as file_handle:
-            file_handle.write(histogram.data)
-        file_io.remove_directory(
-            file_io.append_paths_to_pointer(self.tmp_path, self.HISTOGRAMS_DIR),
-            ignore_errors=True,
-        )
+        return file_io.append_paths_to_pointer(tmp_path, cls.HISTOGRAMS_DIR, f"{mapping_key}.npz")
 
     def get_remaining_split_keys(self):
         """Gather remaining keys, dropping successful split tasks from done file names.
 
         Returns:
             list of splitting keys *not* found in files like /resume/path/split_key.done
         """
```

### Comparing `hipscat_import-0.3.1/src/hipscat_import/catalog/run_import.py` & `hipscat_import-0.3.2/src/hipscat_import/catalog/run_import.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/index/arguments.py` & `hipscat_import-0.3.2/src/hipscat_import/index/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/index/map_reduce.py` & `hipscat_import-0.3.2/src/hipscat_import/index/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/index/run_index.py` & `hipscat_import-0.3.2/src/hipscat_import/index/run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache.py` & `hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache_arguments.py` & `hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/margin_cache/margin_cache_map_reduce.py` & `hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/pipeline.py` & `hipscat_import-0.3.2/src/hipscat_import/pipeline.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/pipeline_resume_plan.py` & `hipscat_import-0.3.2/src/hipscat_import/pipeline_resume_plan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Utility to hold a pipeline's execution and resume plan."""
 
 from __future__ import annotations
 
 import re
-import warnings
 from dataclasses import dataclass
 from pathlib import Path
 
 from dask.distributed import as_completed
 from hipscat.io import FilePointer, file_io
 from hipscat.pixel_math.healpix_pixel import HealpixPixel
 from tqdm.auto import tqdm
@@ -34,17 +33,15 @@
         Raises:
             ValueError: if the tmp_path already exists and contains some files.
         """
         if file_io.directory_has_contents(self.tmp_path):
             if not self.resume:
                 self.clean_resume_files()
             else:
-                warnings.warn(
-                    f"tmp_path ({self.tmp_path}) contains intermediate files; resuming prior progress."
-                )
+                print(f"tmp_path ({self.tmp_path}) contains intermediate files; resuming prior progress.")
         file_io.make_directory(self.tmp_path, exist_ok=True)
 
     def done_file_exists(self, stage_name):
         """Is there a file at a given path?
         For a done file, the existence of the file is the only signal needed to indicate
         a pipeline segment is complete.
 
@@ -97,15 +94,15 @@
             directory: where to look for result files. this is NOT a recursive lookup
             extension (str): file suffix to look for and to remove from all file names.
                 if you expect a file like "map_01.csv", extension should be ".csv"
 
         Returns:
             list of keys taken from files like /resume/path/{key}{extension}
         """
-        result_files = file_io.find_files_matching_path(directory, f"**{extension}")
+        result_files = file_io.find_files_matching_path(directory, f"*{extension}")
         keys = []
         for file_path in result_files:
             result_file_name = file_io.get_basename_from_filepointer(file_path)
             match = re.match(r"(.*)" + extension, str(result_file_name))
             keys.append(match.group(1))
         return keys
 
@@ -130,16 +127,29 @@
             as_completed(futures),
             desc=formatted_stage_name,
             total=len(futures),
             disable=(not self.progress_bar),
         ):
             if future.status == "error":
                 some_error = True
-                print(f"{stage_name} task {future.key} failed with message:")
-                print(future.exception())
+                exception = future.exception()
+                trace_strs = [
+                    f"{stage_name} task {future.key} failed with message:",
+                    f"  {type(exception).__name__}: {exception}",
+                    "  Traceback (most recent call last):",
+                ]
+                stack_trace = exception.__traceback__
+                while stack_trace is not None:
+                    filename = stack_trace.tb_frame.f_code.co_filename
+                    method_name = stack_trace.tb_frame.f_code.co_name
+                    line_number = stack_trace.tb_lineno
+                    trace_strs.append(f'    File "{filename}", line {line_number}, in {method_name}')
+                    stack_trace = stack_trace.tb_next
+                print("\n".join(trace_strs))
+
         if some_error:
             raise RuntimeError(f"Some {stage_name} stages failed. See logs for details.")
 
     @staticmethod
     def get_formatted_stage_name(stage_name) -> str:
         """Create a stage name of consistent minimum length. Ensures that the tqdm
         progress bars can line up nicely when multiple stages must run.
```

### Comparing `hipscat_import-0.3.1/src/hipscat_import/runtime_arguments.py` & `hipscat_import-0.3.2/src/hipscat_import/runtime_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self._check_arguments()
 
     def _check_arguments(self):
         if not self.output_path:
             raise ValueError("output_path is required")
         if not self.output_artifact_name:
             raise ValueError("output_artifact_name is required")
-        if re.search(r"[^A-Za-z0-9_\-\\]", self.output_artifact_name):
+        if re.search(r"[^A-Za-z0-9\._\-\\]", self.output_artifact_name):
             raise ValueError("output_artifact_name contains invalid characters")
 
         if self.dask_n_workers <= 0:
             raise ValueError("dask_n_workers should be greather than 0")
         if self.dask_threads_per_worker <= 0:
             raise ValueError("dask_threads_per_worker should be greater than 0")
 
@@ -141,14 +141,15 @@
         file_matcher (str): matcher to use when searching for files
         input_file_list (List[str]): list of input paths
     Returns:
         matching files, if input_path is provided, otherwise, input_file_list
     Raises:
         FileNotFoundError: if no files are found at the input_path and the provided list is empty.
     """
+    input_paths = []
     if input_path:
         if not file_io.does_file_or_directory_exist(input_path, storage_options=storage_options):
             raise FileNotFoundError("input_path not found on local storage")
         input_paths = file_io.find_files_matching_path(
             input_path, file_matcher, include_protocol=True, storage_options=storage_options
         )
     elif input_file_list:
```

### Comparing `hipscat_import-0.3.1/src/hipscat_import/soap/arguments.py` & `hipscat_import-0.3.2/src/hipscat_import/soap/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/soap/map_reduce.py` & `hipscat_import-0.3.2/src/hipscat_import/soap/map_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         input_path(str): intermediate directory with partial result CSVs. likely, the
             directory used in the previous `count_joins` call as `cache_path`
         output_path(str): directory to write the combined results CSVs.
 
     Returns:
         integer that is the sum of all matched num_rows.
     """
-    partial_files = file_io.find_files_matching_path(input_path, "**.csv")
+    partial_files = file_io.find_files_matching_path(input_path, "*.csv")
     partials = []
 
     for partial_file in partial_files:
         partials.append(file_io.load_csv_to_pandas(partial_file))
 
     dataframe = pd.concat(partials)
 
@@ -190,15 +190,15 @@
     pixel_dir = get_pixel_cache_directory(soap_args.tmp_path, object_pixel)
     # If there's no directory, this implies there were no matches to this object pixel
     # earlier in the pipeline. Move on.
     if not file_io.does_file_or_directory_exist(pixel_dir):
         return
     # Find all of the constituent files / source pixels. Create a list of PyArrow Tables from those
     # parquet files. We need to know the schema before we create the ParquetWriter.
-    shard_file_list = file_io.find_files_matching_path(pixel_dir, "source**.parquet")
+    shard_file_list = file_io.find_files_matching_path(pixel_dir, "source*.parquet")
 
     if len(shard_file_list) == 0:
         return
 
     ## We want to order the row groups in a "breadth-first" sorting. Determine our sorting
     ## via the metadata, then read the tables in using that sorting.
     healpix_pixels = []
```

### Comparing `hipscat_import-0.3.1/src/hipscat_import/soap/resume_plan.py` & `hipscat_import-0.3.2/src/hipscat_import/soap/resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/soap/run_soap.py` & `hipscat_import-0.3.2/src/hipscat_import/soap/run_soap.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/verification/arguments.py` & `hipscat_import-0.3.2/src/hipscat_import/verification/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import/verification/run_verification.py` & `hipscat_import-0.3.2/src/hipscat_import/verification/run_verification.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/src/hipscat_import.egg-info/PKG-INFO` & `hipscat_import-0.3.2/src/hipscat_import.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.3.1
+Version: 0.3.2
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,22 +38,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask[complete]>=2024.3.0
 Requires-Dist: deprecated
 Requires-Dist: healpy
-Requires-Dist: hipscat>=0.2.9
+Requires-Dist: hipscat>=0.3.0
 Requires-Dist: ipykernel
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
 Requires-Dist: tqdm
 Requires-Dist: numpy
-Requires-Dist: fsspec<=2024.2.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `hipscat_import-0.3.1/src/hipscat_import.egg-info/SOURCES.txt` & `hipscat_import-0.3.2/src/hipscat_import.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 src/hipscat_import.egg-info/top_level.txt
 src/hipscat_import/catalog/__init__.py
 src/hipscat_import/catalog/arguments.py
 src/hipscat_import/catalog/file_readers.py
 src/hipscat_import/catalog/map_reduce.py
 src/hipscat_import/catalog/resume_plan.py
 src/hipscat_import/catalog/run_import.py
+src/hipscat_import/catalog/sparse_histogram.py
 src/hipscat_import/index/__init__.py
 src/hipscat_import/index/arguments.py
 src/hipscat_import/index/map_reduce.py
 src/hipscat_import/index/run_index.py
 src/hipscat_import/margin_cache/__init__.py
 src/hipscat_import/margin_cache/margin_cache.py
 src/hipscat_import/margin_cache/margin_cache_arguments.py
@@ -91,14 +92,15 @@
 tests/hipscat_import/test_runtime_arguments.py
 tests/hipscat_import/catalog/test_argument_validation.py
 tests/hipscat_import/catalog/test_file_readers.py
 tests/hipscat_import/catalog/test_map_reduce.py
 tests/hipscat_import/catalog/test_resume_plan.py
 tests/hipscat_import/catalog/test_run_import.py
 tests/hipscat_import/catalog/test_run_round_trip.py
+tests/hipscat_import/catalog/test_sparse_histogram.py
 tests/hipscat_import/data/blank/blank.csv
 tests/hipscat_import/data/mixed_schema/input_01.csv
 tests/hipscat_import/data/mixed_schema/input_02.csv
 tests/hipscat_import/data/mixed_schema/schema.parquet
 tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
 tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
 tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
@@ -139,14 +141,15 @@
 tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
 tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
 tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
 tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
 tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
 tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
 tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
+tests/hipscat_import/data/small_sky_parts/catalog_10_of_05.csv
 tests/hipscat_import/data/small_sky_source/small_sky_source.csv
 tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
 tests/hipscat_import/data/small_sky_source_catalog/_metadata
 tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
 tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
 tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
 tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
@@ -189,14 +192,15 @@
 tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet
 tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet
 tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet
 tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet
 tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet
 tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet
 tests/hipscat_import/data/test_formats/catalog.starr
+tests/hipscat_import/data/test_formats/gaia_epoch.ecsv
 tests/hipscat_import/data/test_formats/gaia_minimum.csv
 tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet
 tests/hipscat_import/data/test_formats/headers.csv
 tests/hipscat_import/data/test_formats/hipscat_index.csv
 tests/hipscat_import/data/test_formats/hipscat_index.parquet
 tests/hipscat_import/data/test_formats/macauff_metadata.yaml
 tests/hipscat_import/data/test_formats/pandasindex.parquet
```

### Comparing `hipscat_import-0.3.1/tests/.pylintrc` & `hipscat_import-0.3.2/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/conftest.py` & `hipscat_import-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_argument_validation.py` & `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_argument_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         output_artifact_name="catalog",
         input_path=small_sky_parts_dir,
         file_reader="csv",
         output_path=tmp_path,
         progress_bar=False,
     )
     assert args.input_path == small_sky_parts_dir
-    assert len(args.input_paths) == 5
+    assert len(args.input_paths) == 6
 
 
 def test_single_debug_file(formats_headers_csv, tmp_path):
     """Required arguments are provided, and paths are found."""
     args = ImportArguments(
         output_artifact_name="catalog",
         input_file_list=[formats_headers_csv],
```

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_file_readers.py` & `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_file_readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
 
 def test_read_fits_columns(formats_fits):
     """Success case - column filtering on reading fits file"""
     frame = next(FitsReader(column_names=["id", "ra", "dec"]).read(formats_fits))
     assert list(frame.columns) == ["id", "ra", "dec"]
 
     frame = next(FitsReader(skip_column_names=["ra_error", "dec_error"]).read(formats_fits))
-    assert list(frame.columns) == ["id", "ra", "dec"]
+    assert list(frame.columns) == ["id", "ra", "dec", "test_id"]
 
 
 def test_fits_reader_provenance_info(tmp_path, basic_catalog_info):
     """Test that we get some provenance info and it is parseable into JSON."""
     reader = FitsReader()
     provenance_info = reader.provenance_info()
     catalog_base_dir = os.path.join(tmp_path, "test_catalog")
```

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_map_reduce.py` & `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_map_reduce.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import healpy as hp
 import hipscat.pixel_math as hist
 import numpy as np
 import numpy.testing as npt
 import pandas as pd
 import pyarrow as pa
 import pytest
-from numpy import frombuffer
 
 import hipscat_import.catalog.map_reduce as mr
 from hipscat_import.catalog.file_readers import get_file_reader
+from hipscat_import.catalog.sparse_histogram import SparseHistogram
 
 
 def test_read_empty_filename():
     """Empty file name"""
     with pytest.raises(FileNotFoundError):
         mr.map_to_pixels(
             input_file="",
@@ -70,17 +70,17 @@
             resume_path="",
             mapping_key="map_0",
         )
 
 
 def read_partial_histogram(tmp_path, mapping_key):
     """Helper to read in the former result of a map operation."""
-    histogram_file = os.path.join(tmp_path, "histograms", f"{mapping_key}.binary")
-    with open(histogram_file, "rb") as file_handle:
-        return frombuffer(file_handle.read(), dtype=np.int64)
+    histogram_file = os.path.join(tmp_path, "histograms", f"{mapping_key}.npz")
+    hist = SparseHistogram.from_file(histogram_file)
+    return hist.to_array()
 
 
 def test_read_single_fits(tmp_path, formats_fits):
     """Success case - fits file that exists being read as fits"""
     os.makedirs(os.path.join(tmp_path, "histograms"))
     mr.map_to_pixels(
         input_file=formats_fits,
```

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_resume_plan.py` & `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_resume_plan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test catalog resume logic"""
 
-import hipscat.pixel_math as hist
 import numpy.testing as npt
 import pytest
 from hipscat.pixel_math.healpix_pixel import HealpixPixel
 
 from hipscat_import.catalog.resume_plan import ResumePlan
+from hipscat_import.catalog.sparse_histogram import SparseHistogram
 
 
 def test_mapping_done(tmp_path):
     """Verify expected behavior of mapping done file"""
     plan = ResumePlan(tmp_path=tmp_path, progress_bar=False)
     assert not plan.is_mapping_done()
     plan.touch_stage_done_file(ResumePlan.MAPPING_STAGE)
@@ -33,94 +33,86 @@
 def test_done_checks(tmp_path):
     """Verify that done files imply correct pipeline execution order:
     mapping > splitting > reducing
     """
     plan = ResumePlan(tmp_path=tmp_path, progress_bar=False, resume=True)
     plan.touch_stage_done_file(ResumePlan.REDUCING_STAGE)
 
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        with pytest.raises(ValueError, match="before reducing"):
-            plan.gather_plan()
+    with pytest.raises(ValueError, match="before reducing"):
+        plan.gather_plan()
 
     plan.touch_stage_done_file(ResumePlan.SPLITTING_STAGE)
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        with pytest.raises(ValueError, match="before reducing"):
-            plan.gather_plan()
+    with pytest.raises(ValueError, match="before reducing"):
+        plan.gather_plan()
 
     plan.clean_resume_files()
 
     plan = ResumePlan(tmp_path=tmp_path, progress_bar=False, resume=True)
     plan.touch_stage_done_file(ResumePlan.SPLITTING_STAGE)
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        with pytest.raises(ValueError, match="before splitting"):
-            plan.gather_plan()
+    with pytest.raises(ValueError, match="before splitting"):
+        plan.gather_plan()
 
 
 def test_same_input_paths(tmp_path, small_sky_single_file, formats_headers_csv):
     """Test that we can only resume if the input_paths are the same."""
     plan = ResumePlan(
         tmp_path=tmp_path,
         progress_bar=False,
         resume=True,
         input_paths=[small_sky_single_file, formats_headers_csv],
     )
     map_files = plan.map_files
     assert len(map_files) == 2
 
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        with pytest.raises(ValueError, match="Different file set"):
-            ResumePlan(
-                tmp_path=tmp_path,
-                progress_bar=False,
-                resume=True,
-                input_paths=[small_sky_single_file],
-            )
+    with pytest.raises(ValueError, match="Different file set"):
+        ResumePlan(
+            tmp_path=tmp_path,
+            progress_bar=False,
+            resume=True,
+            input_paths=[small_sky_single_file],
+        )
 
     ## List is the same length, but includes a duplicate
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        with pytest.raises(ValueError, match="Different file set"):
-            ResumePlan(
-                tmp_path=tmp_path,
-                progress_bar=False,
-                resume=True,
-                input_paths=[small_sky_single_file, small_sky_single_file],
-            )
-
-    ## Includes a duplicate file, but that's ok.
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        plan = ResumePlan(
+    with pytest.raises(ValueError, match="Different file set"):
+        ResumePlan(
             tmp_path=tmp_path,
             progress_bar=False,
             resume=True,
-            input_paths=[small_sky_single_file, small_sky_single_file, formats_headers_csv],
+            input_paths=[small_sky_single_file, small_sky_single_file],
         )
+
+    ## Includes a duplicate file, but that's ok.
+    plan = ResumePlan(
+        tmp_path=tmp_path,
+        progress_bar=False,
+        resume=True,
+        input_paths=[small_sky_single_file, small_sky_single_file, formats_headers_csv],
+    )
     map_files = plan.map_files
     assert len(map_files) == 2
 
 
 def test_read_write_histogram(tmp_path):
     """Test that we can read what we write into a histogram file."""
     plan = ResumePlan(tmp_path=tmp_path, progress_bar=False, input_paths=["foo1"])
 
     ## We're not ready to read the final histogram - missing partial histograms.
     with pytest.raises(RuntimeError, match="map stages"):
         result = plan.read_histogram(0)
 
-    expected = hist.empty_histogram(0)
-    expected[11] = 131
-
     remaining_keys = plan.get_remaining_map_keys()
     assert remaining_keys == [("map_0", "foo1")]
 
-    ResumePlan.write_partial_histogram(tmp_path=tmp_path, mapping_key="map_0", histogram=expected)
+    histogram = SparseHistogram.make_from_counts([11], [131], 0)
+    histogram.to_file(ResumePlan.partial_histogram_file(tmp_path=tmp_path, mapping_key="map_0"))
 
     remaining_keys = plan.get_remaining_map_keys()
     assert len(remaining_keys) == 0
     result = plan.read_histogram(0)
-    npt.assert_array_equal(result, expected)
+    npt.assert_array_equal(result, histogram.to_array())
 
 
 def never_fails():
     """Method never fails, but never marks intermediate success file."""
     return
 
 
@@ -131,18 +123,16 @@
 
     ## Method doesn't FAIL, but it doesn't write out the partial histogram either.
     ## Since the intermediate files aren't found, we throw an error.
     futures = [dask_client.submit(never_fails)]
     with pytest.raises(RuntimeError, match="map stages"):
         plan.wait_for_mapping(futures)
 
-    expected = hist.empty_histogram(0)
-    expected[11] = 131
-
-    ResumePlan.write_partial_histogram(tmp_path=tmp_path, mapping_key="map_0", histogram=expected)
+    histogram = SparseHistogram.make_from_counts([11], [131], 0)
+    histogram.to_file(ResumePlan.partial_histogram_file(tmp_path=tmp_path, mapping_key="map_0"))
 
     ## Method succeeds, *and* partial histogram is present.
     futures = [dask_client.submit(never_fails)]
     plan.wait_for_mapping(futures)
 
 
 def test_read_write_splitting_keys(tmp_path, small_sky_single_file, formats_headers_csv):
@@ -150,23 +140,21 @@
     input_paths = [small_sky_single_file, formats_headers_csv]
     plan = ResumePlan(tmp_path=tmp_path, progress_bar=False, resume=True, input_paths=input_paths)
     split_keys = plan.split_keys
     assert len(split_keys) == 2
 
     ResumePlan.touch_key_done_file(tmp_path, ResumePlan.SPLITTING_STAGE, "split_0")
 
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        plan.gather_plan()
+    plan.gather_plan()
     split_keys = plan.split_keys
     assert len(split_keys) == 1
     assert split_keys[0][0] == "split_1"
 
     ResumePlan.touch_key_done_file(tmp_path, ResumePlan.SPLITTING_STAGE, "split_1")
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        plan.gather_plan()
+    plan.gather_plan()
     split_keys = plan.split_keys
     assert len(split_keys) == 0
 
     plan.clean_resume_files()
     plan.gather_plan()
     split_keys = plan.split_keys
     assert len(split_keys) == 2
```

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/catalog/test_run_import.py` & `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_run_import.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Functional tests for catalog import"""
 
 import os
 import shutil
 
-import hipscat.pixel_math as hist
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pytest
 from hipscat.catalog.catalog import Catalog
 
 import hipscat_import.catalog.run_import as runner
 from hipscat_import.catalog.arguments import ImportArguments
 from hipscat_import.catalog.file_readers import CsvReader
 from hipscat_import.catalog.resume_plan import ResumePlan
+from hipscat_import.catalog.sparse_histogram import SparseHistogram
 
 
 def test_empty_args():
     """Runner should fail with empty arguments"""
     with pytest.raises(ValueError, match="args is required"):
         runner.run(None, None)
 
@@ -45,45 +45,45 @@
     shutil.copytree(
         os.path.join(resume_dir, "intermediate"),
         intermediate_dir,
     )
     ## Now set up our resume files to match previous work.
     resume_tmp = os.path.join(tmp_path, "tmp", "resume_catalog")
     plan = ResumePlan(tmp_path=resume_tmp, progress_bar=False)
-    histogram = hist.empty_histogram(0)
-    histogram[11] = 131
-    empty = hist.empty_histogram(0)
+    histogram = SparseHistogram.make_from_counts([11], [131], 0)
+    empty = SparseHistogram.make_empty(0)
     for file_index in range(0, 5):
         ResumePlan.touch_key_done_file(resume_tmp, ResumePlan.SPLITTING_STAGE, f"split_{file_index}")
-        ResumePlan.write_partial_histogram(
-            tmp_path=resume_tmp,
-            mapping_key=f"map_{file_index}",
-            histogram=histogram if file_index == 0 else empty,
+        histogram_file = ResumePlan.partial_histogram_file(
+            tmp_path=resume_tmp, mapping_key=f"map_{file_index}"
         )
+        if file_index == 0:
+            histogram.to_file(histogram_file)
+        else:
+            empty.to_file(histogram_file)
 
     ResumePlan.touch_key_done_file(resume_tmp, ResumePlan.REDUCING_STAGE, "0_11")
 
     shutil.copytree(
         os.path.join(resume_dir, "Norder=0"),
         os.path.join(tmp_path, "resume_catalog", "Norder=0"),
     )
 
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        args = ImportArguments(
-            output_artifact_name="resume_catalog",
-            input_path=small_sky_parts_dir,
-            file_reader="csv",
-            output_path=tmp_path,
-            dask_tmp=tmp_path,
-            tmp_dir=tmp_path,
-            resume_tmp=os.path.join(tmp_path, "tmp"),
-            highest_healpix_order=0,
-            pixel_threshold=1000,
-            progress_bar=False,
-        )
+    args = ImportArguments(
+        output_artifact_name="resume_catalog",
+        input_path=small_sky_parts_dir,
+        file_reader="csv",
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        tmp_dir=tmp_path,
+        resume_tmp=os.path.join(tmp_path, "tmp"),
+        highest_healpix_order=0,
+        pixel_threshold=1000,
+        progress_bar=False,
+    )
 
     runner.run(args, dask_client)
 
     # Check that the catalog metadata file exists
     catalog = Catalog.read_from_hipscat(args.catalog_path)
     assert catalog.on_disk
     assert catalog.catalog_path == args.catalog_path
@@ -150,47 +150,39 @@
         os.path.join(resume_dir, "intermediate"),
         intermediate_dir,
     )
 
     ## Now set up our resume files to match previous work.
     resume_tmp = os.path.join(tmp_path, "tmp", "resume_catalog")
     ResumePlan(tmp_path=resume_tmp, progress_bar=False)
-    histogram = hist.empty_histogram(0)
-    histogram[11] = 131
-    empty = hist.empty_histogram(0)
+    SparseHistogram.make_from_counts([11], [131], 0).to_file(
+        os.path.join(resume_tmp, "mapping_histogram.npz")
+    )
     for file_index in range(0, 5):
         ResumePlan.touch_key_done_file(resume_tmp, ResumePlan.SPLITTING_STAGE, f"split_{file_index}")
-        ResumePlan.write_partial_histogram(
-            tmp_path=resume_tmp,
-            mapping_key=f"map_{file_index}",
-            histogram=histogram if file_index == 0 else empty,
-        )
-
-    ResumePlan.touch_key_done_file(resume_tmp, ResumePlan.REDUCING_STAGE, "0_11")
 
     shutil.copytree(
         os.path.join(resume_dir, "Norder=0"),
         os.path.join(tmp_path, "resume_catalog", "Norder=0"),
     )
 
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        with pytest.raises(ValueError, match="incompatible with the highest healpix order"):
-            args = ImportArguments(
-                output_artifact_name="resume_catalog",
-                input_path=small_sky_parts_dir,
-                file_reader="csv",
-                output_path=tmp_path,
-                dask_tmp=tmp_path,
-                tmp_dir=tmp_path,
-                resume_tmp=os.path.join(tmp_path, "tmp"),
-                constant_healpix_order=1,
-                pixel_threshold=1000,
-                progress_bar=False,
-            )
-            runner.run(args, dask_client)
+    with pytest.raises(ValueError, match="incompatible with the highest healpix order"):
+        args = ImportArguments(
+            output_artifact_name="resume_catalog",
+            input_path=small_sky_parts_dir,
+            file_reader="csv",
+            output_path=tmp_path,
+            dask_tmp=tmp_path,
+            tmp_dir=tmp_path,
+            resume_tmp=os.path.join(tmp_path, "tmp"),
+            constant_healpix_order=1,
+            pixel_threshold=1000,
+            progress_bar=False,
+        )
+        runner.run(args, dask_client)
 
     # Running with resume set to "False" will start the pipeline from scratch
     args = ImportArguments(
         output_artifact_name="resume_catalog",
         input_path=small_sky_parts_dir,
         file_reader="csv",
         output_path=tmp_path,
@@ -228,40 +220,42 @@
     tmp_path,
 ):
     """Tests that the pipeline errors if the partial histograms have different sizes."""
     resume_tmp = os.path.join(tmp_path, "tmp", "resume_catalog")
     ResumePlan(tmp_path=resume_tmp, progress_bar=False)
 
     # We'll create mock partial histograms of size 0 and 2
-    histogram = hist.empty_histogram(0)
-    wrong_histogram = hist.empty_histogram(2)
+    histogram = SparseHistogram.make_empty(0)
+    wrong_histogram = SparseHistogram.make_empty(2)
 
     for file_index in range(0, 5):
         ResumePlan.touch_key_done_file(resume_tmp, ResumePlan.SPLITTING_STAGE, f"split_{file_index}")
-        ResumePlan.write_partial_histogram(
-            tmp_path=resume_tmp,
-            mapping_key=f"map_{file_index}",
-            histogram=histogram if file_index % 2 == 0 else wrong_histogram,
+
+        histogram_file = ResumePlan.partial_histogram_file(
+            tmp_path=resume_tmp, mapping_key=f"map_{file_index}"
         )
+        if file_index == 2:
+            histogram.to_file(histogram_file)
+        else:
+            wrong_histogram.to_file(histogram_file)
 
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        with pytest.raises(ValueError, match="histogram partials have inconsistent sizes"):
-            args = ImportArguments(
-                output_artifact_name="resume_catalog",
-                input_path=small_sky_parts_dir,
-                file_reader="csv",
-                output_path=tmp_path,
-                dask_tmp=tmp_path,
-                tmp_dir=tmp_path,
-                resume_tmp=os.path.join(tmp_path, "tmp"),
-                constant_healpix_order=1,
-                pixel_threshold=1000,
-                progress_bar=False,
-            )
-            runner.run(args, dask_client)
+    with pytest.raises(ValueError, match="histogram partials have incompatible sizes"):
+        args = ImportArguments(
+            output_artifact_name="resume_catalog",
+            input_path=small_sky_parts_dir,
+            file_reader="csv",
+            output_path=tmp_path,
+            dask_tmp=tmp_path,
+            tmp_dir=tmp_path,
+            resume_tmp=os.path.join(tmp_path, "tmp"),
+            constant_healpix_order=1,
+            pixel_threshold=1000,
+            progress_bar=False,
+        )
+        runner.run(args, dask_client)
 
 
 @pytest.mark.dask
 def test_dask_runner(
     dask_client,
     small_sky_parts_dir,
     assert_parquet_file_ids,
```

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/conftest.py` & `hipscat_import-0.3.2/tests/hipscat_import/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/mixed_schema/schema.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky/catalog.csv` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky/catalog.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/_metadata` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source/small_sky_source.csv` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source/small_sky_source.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/_metadata` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json` & `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/catalog.starr` & `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/catalog.starr`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/gaia_minimum.csv` & `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_minimum.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/hipscat_index.csv` & `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/hipscat_index.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/hipscat_index.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/hipscat_index.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/data/test_formats/pandasindex.parquet` & `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/pandasindex.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/index/test_index_argument.py` & `hipscat_import-0.3.2/tests/hipscat_import/index/test_index_argument.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/index/test_index_map_reduce.py` & `hipscat_import-0.3.2/tests/hipscat_import/index/test_index_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/index/test_run_index.py` & `hipscat_import-0.3.2/tests/hipscat_import/index/test_run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py` & `hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_cache.py` & `hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py` & `hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/margin_cache/test_margin_round_trip.py` & `hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_round_trip.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/soap/conftest.py` & `hipscat_import-0.3.2/tests/hipscat_import/soap/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/soap/test_run_soap.py` & `hipscat_import-0.3.2/tests/hipscat_import/soap/test_run_soap.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_arguments.py` & `hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_map_reduce.py` & `hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/soap/test_soap_resume_plan.py` & `hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_resume_plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,39 +90,36 @@
     """Verify expected behavior of counting keys file"""
     plan = SoapPlan(small_sky_soap_args)
     assert len(plan.count_keys) == 14
 
     ## Mark one done and check that there's one less key to count later.
     Path(small_sky_soap_args.tmp_path, "2_187.csv").touch()
 
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        plan.gather_plan(small_sky_soap_args)
+    plan.gather_plan(small_sky_soap_args)
     assert len(plan.count_keys) == 13
 
     ## Mark them ALL done and check that there are on keys later.
     plan.touch_stage_done_file(SoapPlan.COUNTING_STAGE)
 
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        plan.gather_plan(small_sky_soap_args)
+    plan.gather_plan(small_sky_soap_args)
     assert len(plan.count_keys) == 0
 
 
 @pytest.mark.timeout(2)
 def test_cached_map_file(small_sky_soap_args):
     """Verify that we cache the mapping file for later use.
     This can be expensive to compute for large survey cross-products!"""
     plan = SoapPlan(small_sky_soap_args)
     assert len(plan.count_keys) == 14
 
     ## The source partition mapping should be cached in a file.
     cache_map_file = os.path.join(small_sky_soap_args.tmp_path, SoapPlan.SOURCE_MAP_FILE)
     assert os.path.exists(cache_map_file)
 
-    with pytest.warns(UserWarning, match="resuming prior progress"):
-        plan = SoapPlan(small_sky_soap_args)
+    plan = SoapPlan(small_sky_soap_args)
     assert len(plan.count_keys) == 14
 
 
 def test_get_sources_to_count(small_sky_soap_args):
     """Test generation of remaining count items"""
     source_pixel_map = {HealpixPixel(0, 11): (131, [44, 45, 46])}
     plan = SoapPlan(small_sky_soap_args)
```

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/test_pipeline_resume_plan.py` & `hipscat_import-0.3.2/tests/hipscat_import/test_pipeline_resume_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,18 @@
 
     ## If there are no more intermediate files, we don't need to set resume.
     plan.clean_resume_files()
     plan.safe_to_resume()
 
 
 @pytest.mark.dask
-def test_wait_for_futures(tmp_path, dask_client):
-    """Test that we can wait around for futures to complete."""
+def test_wait_for_futures(tmp_path, dask_client, capsys):
+    """Test that we can wait around for futures to complete.
+
+    Additionally test that relevant parts of the traceback are printed to stdout."""
     plan = PipelineResumePlan(tmp_path=tmp_path, progress_bar=False, resume=False)
 
     def error_on_even(argument):
         """Silly little method used to test futures that fail under predictable conditions"""
         if argument % 2 == 0:
             raise RuntimeError("we are at odds with evens")
 
@@ -111,14 +113,18 @@
     plan.wait_for_futures(futures, "test")
 
     ## Throw an even in the mix, and we'll see some stages fail. Should cause whole stage to fail.
     futures = [dask_client.submit(error_on_even, 1), dask_client.submit(error_on_even, 2)]
     with pytest.raises(RuntimeError, match="Some test stages failed"):
         plan.wait_for_futures(futures, "test")
 
+        captured = capsys.readouterr()
+        assert "we are at odds with evens" in captured
+        assert "error_on_even" in captured
+
 
 def test_formatted_stage_name():
     """Test that we make pretty stage names for presenting in progress bars"""
     formatted = PipelineResumePlan.get_formatted_stage_name(None)
     assert formatted == "Progress  "
 
     formatted = PipelineResumePlan.get_formatted_stage_name("")
```

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/test_runtime_arguments.py` & `hipscat_import-0.3.2/tests/hipscat_import/test_runtime_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/verification/test_run_verification.py` & `hipscat_import-0.3.2/tests/hipscat_import/verification/test_run_verification.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.1/tests/hipscat_import/verification/test_verification_arguments.py` & `hipscat_import-0.3.2/tests/hipscat_import/verification/test_verification_arguments.py`

 * *Files identical despite different names*

