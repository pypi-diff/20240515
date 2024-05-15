# Comparing `tmp/data_prep_toolkit-0.0.1.dev4.tar.gz` & `tmp/data_prep_toolkit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_toolkit-0.0.1.dev4.tar", last modified: Sun May 12 08:55:41 2024, max compression
+gzip compressed data, was "data_prep_toolkit-0.1.0.tar", last modified: Wed May 15 16:26:42 2024, max compression
```

## Comparing `data_prep_toolkit-0.0.1.dev4.tar` & `data_prep_toolkit-0.1.0.tar`

### file list

```diff
@@ -1,126 +1,140 @@
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.566933 data_prep_toolkit-0.0.1.dev4/
--rw-r--r--   0 eres      (1000) eres      (1000)      357 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/.gitignore
--rw-r--r--   0 eres      (1000) eres      (1000)     2395 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/Makefile
--rw-r--r--   0 eres      (1000) eres      (1000)     1885 2024-05-12 08:55:41.566933 data_prep_toolkit-0.0.1.dev4/PKG-INFO
--rw-r--r--   0 eres      (1000) eres      (1000)      963 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/README.md
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.536934 data_prep_toolkit-0.0.1.dev4/doc/
--rw-r--r--   0 eres      (1000) eres      (1000)    12779 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/advanced-transform-tutorial.md
--rw-r--r--   0 eres      (1000) eres      (1000)     7617 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/architecture.md
--rw-r--r--   0 eres      (1000) eres      (1000)     5028 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/launcher-options.md
--rw-r--r--   0 eres      (1000) eres      (1000)    34920 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/logo-ibm-dark.png
--rw-r--r--   0 eres      (1000) eres      (1000)    35127 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/logo-ibm.png
--rw-r--r--   0 eres      (1000) eres      (1000)     1564 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/overview.md
--rw-r--r--   0 eres      (1000) eres      (1000)   137580 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/doc/processing-architecture.jpg
--rw-r--r--   0 eres      (1000) eres      (1000)     8840 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/simplest-transform-tutorial.md
--rw-r--r--   0 eres      (1000) eres      (1000)      193 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/doc/testing-e2e-transform.md
--rw-r--r--   0 eres      (1000) eres      (1000)     5888 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/testing-transforms.md
--rw-r--r--   0 eres      (1000) eres      (1000)    12175 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/doc/transform-external-resources.md
--rw-r--r--   0 eres      (1000) eres      (1000)    10775 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/transform-tutorials.md
--rw-r--r--   0 eres      (1000) eres      (1000)     1415 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/doc/transformer-utilities.md
--rw-r--r--   0 eres      (1000) eres      (1000)     3614 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/doc/using_s3_transformers.md
--rw-r--r--   0 eres      (1000) eres      (1000)     1333 2024-05-12 08:54:18.000000 data_prep_toolkit-0.0.1.dev4/pyproject.toml
--rw-r--r--   0 eres      (1000) eres      (1000)       38 2024-05-12 08:55:41.566933 data_prep_toolkit-0.0.1.dev4/setup.cfg
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/src/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.566933 data_prep_toolkit-0.0.1.dev4/src/data_prep_toolkit.egg-info/
--rw-r--r--   0 eres      (1000) eres      (1000)     1885 2024-05-12 08:55:41.000000 data_prep_toolkit-0.0.1.dev4/src/data_prep_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 eres      (1000) eres      (1000)     3992 2024-05-12 08:55:41.000000 data_prep_toolkit-0.0.1.dev4/src/data_prep_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 eres      (1000) eres      (1000)        1 2024-05-12 08:55:41.000000 data_prep_toolkit-0.0.1.dev4/src/data_prep_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 eres      (1000) eres      (1000)      249 2024-05-12 08:55:41.000000 data_prep_toolkit-0.0.1.dev4/src/data_prep_toolkit.egg-info/requires.txt
--rw-r--r--   0 eres      (1000) eres      (1000)       16 2024-05-12 08:55:41.000000 data_prep_toolkit-0.0.1.dev4/src/data_prep_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.536934 data_prep_toolkit-0.0.1.dev4/src/data_processing/
--rw-r--r--   0 eres      (1000) eres      (1000)        0 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/__init__.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.546934 data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/
--rw-r--r--   0 eres      (1000) eres      (1000)      427 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     8830 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/arrow_s3.py
--rw-r--r--   0 eres      (1000) eres      (1000)     8484 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access.py
--rw-r--r--   0 eres      (1000) eres      (1000)    11466 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access_factory.py
--rw-r--r--   0 eres      (1000) eres      (1000)     5647 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access_factory_base.py
--rw-r--r--   0 eres      (1000) eres      (1000)    15061 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access_local.py
--rw-r--r--   0 eres      (1000) eres      (1000)    13499 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access_s3.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.546934 data_prep_toolkit-0.0.1.dev4/src/data_processing/pure_python/
--rw-r--r--   0 eres      (1000) eres      (1000)      346 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/pure_python/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     4122 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/pure_python/python_launcher_configuration.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3800 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/pure_python/transform_launcher.py
--rw-r--r--   0 eres      (1000) eres      (1000)     4252 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/pure_python/transform_orchestrator.py
--rw-r--r--   0 eres      (1000) eres      (1000)     9237 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/pure_python/transform_table_processor.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.546934 data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/
--rw-r--r--   0 eres      (1000) eres      (1000)      576 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7404 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/ray_utils.py
--rw-r--r--   0 eres      (1000) eres      (1000)     5027 2024-05-12 08:53:50.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_launcher.py
--rw-r--r--   0 eres      (1000) eres      (1000)     6380 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_orchestrator.py
--rw-r--r--   0 eres      (1000) eres      (1000)     4574 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_orchestrator_configuration.py
--rw-r--r--   0 eres      (1000) eres      (1000)     4784 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_runtime.py
--rw-r--r--   0 eres      (1000) eres      (1000)     2883 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_statistics.py
--rw-r--r--   0 eres      (1000) eres      (1000)     9501 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_table_processor.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.546934 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/
--rw-r--r--   0 eres      (1000) eres      (1000)       62 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     8234 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/abstract_test.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.546934 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/data_access/
--rw-r--r--   0 eres      (1000) eres      (1000)       69 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/data_access/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     2666 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/data_access/data_access_factory_test.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/ray/
--rw-r--r--   0 eres      (1000) eres      (1000)       58 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/ray/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     4672 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/ray/transform_test.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/transform/
--rw-r--r--   0 eres      (1000) eres      (1000)      231 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/transform/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     5701 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/transform/noop_transform.py
--rw-r--r--   0 eres      (1000) eres      (1000)     4476 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/transform/transform_test.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/
--rw-r--r--   0 eres      (1000) eres      (1000)      368 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3067 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/execution_configuration.py
--rw-r--r--   0 eres      (1000) eres      (1000)     2521 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/launcher_configuration.py
--rw-r--r--   0 eres      (1000) eres      (1000)     2298 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/table_transform.py
--rw-r--r--   0 eres      (1000) eres      (1000)     1465 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/transform_statistics.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/
--rw-r--r--   0 eres      (1000) eres      (1000)      354 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3135 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/cli_utils.py
--rw-r--r--   0 eres      (1000) eres      (1000)     1695 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/config.py
--rw-r--r--   0 eres      (1000) eres      (1000)     2052 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/log.py
--rw-r--r--   0 eres      (1000) eres      (1000)     6029 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/params_utils.py
--rw-r--r--   0 eres      (1000) eres      (1000)     6740 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/transform_utils.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/test/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.566933 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/data_access/
--rw-r--r--   0 eres      (1000) eres      (1000)     1256 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/data_access/daf_local_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)    24597 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/data_access/data_access_local_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     5734 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/data_access/data_access_s3_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     1545 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/data_access/sample_input_data_test.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.566933 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/pure_python/
--rw-r--r--   0 eres      (1000) eres      (1000)     9106 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/pure_python/launcher_test.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.566933 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/ray/
--rw-r--r--   0 eres      (1000) eres      (1000)    11220 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/ray/launcher_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3288 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/ray/ray_util_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     1733 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/ray/test_noop_launch.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.566933 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/transform/
--rw-r--r--   0 eres      (1000) eres      (1000)     1678 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/transform/test_noop.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.566933 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/util/
--rw-r--r--   0 eres      (1000) eres      (1000)     1386 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/util/transform_utils_test.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/test-data/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/input/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/input/ds1/
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/input/ds1/sample1.parquet
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/input/ds1/sample2.parquet
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/input/ds2/
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/input/ds2/sample3.parquet
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/output/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/output/ds1/
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/output/ds1/sample1.parquet
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input/
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input/sample1.parquet
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input_multiple/
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input_multiple/sample1.parquet
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input_multiple/sample2.parquet
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input_multiple/sample3.parquet
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.526934 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/expected/
--rw-r--r--   0 eres      (1000) eres      (1000)     1128 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/expected/metadata.json
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/expected/sample1.parquet
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/expected/subdir/
--rw-r--r--   0 eres      (1000) eres      (1000)      753 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/input/
--rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/input/sample1.parquet
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 08:55:41.556933 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/input/subdir/
--rw-r--r--   0 eres      (1000) eres      (1000)      753 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/input/subdir/test1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.529639 data_prep_toolkit-0.1.0/
+-rw-r--r--   0 dawood     (501) staff       (20)      357 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/.gitignore
+-rw-r--r--   0 dawood     (501) staff       (20)     2572 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/Makefile
+-rw-r--r--   0 dawood     (501) staff       (20)     1880 2024-05-15 16:26:42.529334 data_prep_toolkit-0.1.0/PKG-INFO
+-rw-r--r--   0 dawood     (501) staff       (20)      963 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/README.md
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.501759 data_prep_toolkit-0.1.0/doc/
+-rw-r--r--   0 dawood     (501) staff       (20)    13397 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/doc/advanced-transform-tutorial.md
+-rw-r--r--   0 dawood     (501) staff       (20)     7687 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/doc/architecture.md
+-rw-r--r--   0 dawood     (501) staff       (20)     1418 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/overview.md
+-rw-r--r--   0 dawood     (501) staff       (20)   137580 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/doc/processing-architecture.jpg
+-rw-r--r--   0 dawood     (501) staff       (20)     3659 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/doc/python-launcher-options.md
+-rw-r--r--   0 dawood     (501) staff       (20)      531 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/python-runtime.md
+-rw-r--r--   0 dawood     (501) staff       (20)     5221 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/ray-launcher-options.md
+-rw-r--r--   0 dawood     (501) staff       (20)     7567 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/doc/ray-runtime.md
+-rw-r--r--   0 dawood     (501) staff       (20)     9369 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/doc/simplest-transform-tutorial.md
+-rw-r--r--   0 dawood     (501) staff       (20)      195 2024-05-14 11:51:27.000000 data_prep_toolkit-0.1.0/doc/testing-e2e-transform.md
+-rw-r--r--   0 dawood     (501) staff       (20)    12176 2024-05-14 11:51:27.000000 data_prep_toolkit-0.1.0/doc/transform-external-resources.md
+-rw-r--r--   0 dawood     (501) staff       (20)      436 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/transform-runtimes.md
+-rw-r--r--   0 dawood     (501) staff       (20)     3614 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/transform-s3-testing.md
+-rw-r--r--   0 dawood     (501) staff       (20)     5889 2024-05-14 11:51:27.000000 data_prep_toolkit-0.1.0/doc/transform-standalone-testing.md
+-rw-r--r--   0 dawood     (501) staff       (20)      472 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/transform-testing.md
+-rw-r--r--   0 dawood     (501) staff       (20)      674 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/transform-tutorial-examples.md
+-rw-r--r--   0 dawood     (501) staff       (20)     4595 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/doc/transform-tutorials.md
+-rw-r--r--   0 dawood     (501) staff       (20)     1418 2024-05-14 11:51:27.000000 data_prep_toolkit-0.1.0/doc/transformer-utilities.md
+-rw-r--r--   0 dawood     (501) staff       (20)     1329 2024-05-15 16:26:12.000000 data_prep_toolkit-0.1.0/pyproject.toml
+-rw-r--r--   0 dawood     (501) staff       (20)       38 2024-05-15 16:26:42.529696 data_prep_toolkit-0.1.0/setup.cfg
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.489934 data_prep_toolkit-0.1.0/src/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.528162 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/
+-rw-r--r--   0 dawood     (501) staff       (20)     1880 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 dawood     (501) staff       (20)     4693 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 dawood     (501) staff       (20)        1 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 dawood     (501) staff       (20)      249 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/requires.txt
+-rw-r--r--   0 dawood     (501) staff       (20)       16 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.503249 data_prep_toolkit-0.1.0/src/data_processing/
+-rw-r--r--   0 dawood     (501) staff       (20)        0 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/__init__.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.505781 data_prep_toolkit-0.1.0/src/data_processing/data_access/
+-rw-r--r--   0 dawood     (501) staff       (20)      427 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     8339 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/arrow_s3.py
+-rw-r--r--   0 dawood     (501) staff       (20)     8484 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access.py
+-rw-r--r--   0 dawood     (501) staff       (20)    11466 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_factory.py
+-rw-r--r--   0 dawood     (501) staff       (20)     5647 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_factory_base.py
+-rw-r--r--   0 dawood     (501) staff       (20)    15061 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_local.py
+-rw-r--r--   0 dawood     (501) staff       (20)    13499 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_s3.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.507122 data_prep_toolkit-0.1.0/src/data_processing/runtime/
+-rw-r--r--   0 dawood     (501) staff       (20)      370 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     3067 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/execution_configuration.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.508141 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/
+-rw-r--r--   0 dawood     (501) staff       (20)      378 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1143 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/runtime_configuration.py
+-rw-r--r--   0 dawood     (501) staff       (20)     3719 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_launcher.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4301 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_orchestrator.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2107 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_table_processor.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.510679 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/
+-rw-r--r--   0 dawood     (501) staff       (20)      763 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4572 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/execution_configuration.py
+-rw-r--r--   0 dawood     (501) staff       (20)     7404 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/ray_utils.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1788 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/runtime_configuration.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4801 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_launcher.py
+-rw-r--r--   0 dawood     (501) staff       (20)     6354 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_orchestrator.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2536 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_runtime.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2883 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_statistics.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2012 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_table_processor.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2777 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/runtime_configuration.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2889 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/transform_launcher.py
+-rw-r--r--   0 dawood     (501) staff       (20)     8328 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/transform_table_processor.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.511274 data_prep_toolkit-0.1.0/src/data_processing/test_support/
+-rw-r--r--   0 dawood     (501) staff       (20)       62 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     8234 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/abstract_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.511870 data_prep_toolkit-0.1.0/src/data_processing/test_support/data_access/
+-rw-r--r--   0 dawood     (501) staff       (20)       69 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/data_access/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2666 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/data_access/data_access_factory_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.512803 data_prep_toolkit-0.1.0/src/data_processing/test_support/launch/
+-rw-r--r--   0 dawood     (501) staff       (20)        0 2024-05-10 14:02:13.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/launch/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4821 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/launch/transform_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.513825 data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/
+-rw-r--r--   0 dawood     (501) staff       (20)      174 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     6140 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/noop_transform.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4476 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/transform_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.514667 data_prep_toolkit-0.1.0/src/data_processing/transform/
+-rw-r--r--   0 dawood     (501) staff       (20)      263 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/transform/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2298 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/transform/table_transform.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4394 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/transform/transform_configuration.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1465 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/transform/transform_statistics.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.515940 data_prep_toolkit-0.1.0/src/data_processing/utils/
+-rw-r--r--   0 dawood     (501) staff       (20)      354 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     3135 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/cli_utils.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1695 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/config.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2052 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/log.py
+-rw-r--r--   0 dawood     (501) staff       (20)     6029 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/params_utils.py
+-rw-r--r--   0 dawood     (501) staff       (20)     7916 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/transform_utils.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.493074 data_prep_toolkit-0.1.0/test/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.493712 data_prep_toolkit-0.1.0/test/data_processing_tests/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.524283 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/
+-rw-r--r--   0 dawood     (501) staff       (20)     1256 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/daf_local_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)    24597 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/data_access_local_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     5734 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/data_access_s3_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1545 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/sample_input_data_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.493505 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.524796 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/
+-rw-r--r--   0 dawood     (501) staff       (20)     6443 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/launcher_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2717 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/multi_launcher_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1852 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/test_noop_launch.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.525407 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/
+-rw-r--r--   0 dawood     (501) staff       (20)     7229 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/launcher_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2825 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/multi_launcher_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     3296 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/ray_util_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1856 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/test_noop_launch.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.525555 data_prep_toolkit-0.1.0/test/data_processing_tests/transform/
+-rw-r--r--   0 dawood     (501) staff       (20)     1678 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/transform/test_noop.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.525773 data_prep_toolkit-0.1.0/test/data_processing_tests/util/
+-rw-r--r--   0 dawood     (501) staff       (20)     1386 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/util/transform_utils_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.491391 data_prep_toolkit-0.1.0/test-data/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.492327 data_prep_toolkit-0.1.0/test-data/data_processing/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.491812 data_prep_toolkit-0.1.0/test-data/data_processing/daf/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.491712 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.516960 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/sample1.parquet
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/sample2.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.517853 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds2/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds2/sample3.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.491904 data_prep_toolkit-0.1.0/test-data/data_processing/daf/output/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.518578 data_prep_toolkit-0.1.0/test-data/data_processing/daf/output/ds1/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/daf/output/ds1/sample1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.519300 data_prep_toolkit-0.1.0/test-data/data_processing/input/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/input/sample1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.520896 data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample1.parquet
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample2.parquet
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample3.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.492474 data_prep_toolkit-0.1.0/test-data/data_processing/ray/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.492756 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.521548 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/
+-rw-r--r--   0 dawood     (501) staff       (20)     1128 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/metadata.json
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/sample1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.522163 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/subdir/
+-rw-r--r--   0 dawood     (501) staff       (20)      753 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.522365 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/sample1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.522594 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/subdir/
+-rw-r--r--   0 dawood     (501) staff       (20)      753 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/subdir/test1.parquet
```

### Comparing `data_prep_toolkit-0.0.1.dev4/Makefile` & `data_prep_toolkit-0.1.0/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
 
 # Here we run each test directory of tests and each ray launched test separately, because
 # it seems when running multiple ray launch tests in a single pytest run there is some sort of ray.init() duplication.
 # pytest-forked was tried, but then we get SIGABRT in pytest when running the s3 tests, some of which are skipped.. 
 test::  
 	@# Help: Use the already-built virtual environment to run pytest on the test directory. 
-	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/data_access;	
-	source venv/bin/activate; export PYTHONPATH=../src;  cd test; $(PYTEST)  data_processing_tests/transform;	
-	source venv/bin/activate; export PYTHONPATH=../src;  cd test; $(PYTEST)  data_processing_tests/pure_python;
-	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/ray/ray_util_test.py;
-	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/ray/launcher_test.py;	
-	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/ray/test_noop_launch.py;	
+	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/data_access;
+	source venv/bin/activate; export PYTHONPATH=../src;  cd test; $(PYTEST)  data_processing_tests/transform;
+	source venv/bin/activate; export PYTHONPATH=../src;  cd test; $(PYTEST)  data_processing_tests/launch/pure_python/launcher_test.py;
+	source venv/bin/activate; export PYTHONPATH=../src;  cd test; $(PYTEST)  data_processing_tests/launch/pure_python/test_noop_launch.py;
+	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/launch/ray/ray_util_test.py;
+	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/launch/ray/launcher_test.py;
+	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/launch/ray/test_noop_launch.py;
```

### Comparing `data_prep_toolkit-0.0.1.dev4/PKG-INFO` & `data_prep_toolkit-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit
-Version: 0.0.1.dev4
+Version: 0.1.0
 Summary: Data Preparation Toolkit Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
```

### Comparing `data_prep_toolkit-0.0.1.dev4/README.md` & `data_prep_toolkit-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/advanced-transform-tutorial.md` & `data_prep_toolkit-0.1.0/doc/advanced-transform-tutorial.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   in a single run of the transform.
 * How to implement custom `TransformRuntime` to create supporting Ray objects and supplement
   transform-specific metadata with the information about this statistics
 * How to define command line arguments that can be used to configure
   the operation of our _noop_ transform.
 
 The complete task involves the following:
+
 * EdedupTransform - class that implements the specific transformation
 * EdedupRuntime - class that implements custom TransformRuntime to create supporting Ray objects and enhance job output
   statistics
 * EdedupTableTransformConfiguration - class that provides configuration for the
   EdedupTransform and EdedupRuntime, including transform runtime class and the command line arguments used to
   configure them.
 * main() - simple creation and use of the TransformLauncher.
@@ -35,14 +36,15 @@
 
 ## EdedupTransform
 
 First, let's define the transform class.  To do this we extend
 the base abstract/interface class
 [AbstractTableTransform](../src/data_processing/transform/table_transform.py),
 which requires definition of the following:
+
 * an initializer (i.e. `init()`) that accepts a dictionary of configuration
   data.  For this example, the configuration data will only be defined by
   command line arguments (defined below).
 * the `transform()` method itself that takes an input table and produces an output
   table and any associated metadata for that table transformation.
 
 Other methods such as `flush()` need not be overridden/redefined for this example.
@@ -52,23 +54,25 @@
 
 ```python
 from argparse import ArgumentParser, Namespace
 from typing import Any
 
 import pyarrow as pa
 import ray
-from data_processing.data_access import DataAccessFactory
-from data_processing.ray import (
-  RayLauncherConfiguration,
+from data_processing.data_access import DataAccessFactoryBase
+from data_processing.runtime.ray import (
   DefaultTableTransformRuntimeRay,
-  RayUtils,
   RayTransformLauncher,
+  RayUtils,
+)
+from data_processing.runtime.ray.runtime_configuration import (
+  RayTransformRuntimeConfiguration,
 )
-from data_processing.transform import AbstractTableTransform
-from data_processing.utils import GB, TransformUtils
+from data_processing.transform import AbstractTableTransform, TransformConfiguration
+from data_processing.utils import GB, CLIArgumentProvider, TransformUtils, get_logger
 from ray.actor import ActorHandle
 
 
 class EdedupTransform(AbstractTableTransform):
 
   def __init__(self, config: dict):
     super().__init__(config)
@@ -132,16 +136,17 @@
 by the framework and reported as aggregated job statistics metadata.
 If there is no metadata then simply return an empty dictionary.
 
 ## EdedupRuntime
 
 First, let's define the transform runtime class.  To do this we extend
 the base abstract/interface class
-[DefaultTableTransformRuntime](../src/data_processing/ray/transform_runtime.py),
+[DefaultTableTransformRuntime](../src/data_processing/runtime/ray/transform_runtime.py),
 which requires definition of the following:
+
 * an initializer (i.e. `init()`) that accepts a dictionary of configuration
   data.  For this example, the configuration data will only be defined by
   command line arguments (defined below).
 * the `get_transform_config()` method that takes `data_access_factory`, `statistics actor`, and
   `list of files to process` and produces a dictionary of parameters used by transform.
 * the `compute_execution_stats()` method that takes take a dictionary of metadata, enhances it and
   produces an enhanced metadata dictionary.
@@ -198,32 +203,36 @@
     return {"number of hashes": sum_hash, "hash memory, GB": sum_hash_mem, "de duplication %": dedup_prst} | stats
 ```
 Input to this method is a dictionary of metadata collected by statistics object. It then enhances it by information
 collected by hash actors and custom computations based on statistics data.
 
 ## EdedupTableTransformConfiguration
 
-The final class we need to implement is `EdedupTableTransformConfiguration` class and its initializer that
-define the following:
+The final class we need to implement is `EdedupRayTransformConfiguration` class that provides configuration for 
+running our transform. Although we provide only Ray-based implementation, Ray-based configuration relies on Python-based
+configuration that we need to define first. So we first need to define `EdedupTableTransformConfiguration` class, 
+defining the following:
 
 * The short name for the transform
 * The class implementing the transform - in our case EdedupTransform
 * The transform runtime class be used - in our case EdedupRuntime
 * Command line argument support.
 
 First we define the class and its initializer,
 
 ```python
 short_name = "ededup"
 cli_prefix = f"{short_name}_"
 
-class EdedupTableTransformConfiguration(DefaultTableTransformConfiguration):
-    def __init__(self):
-        super().__init__(name=short_name, runtime_class=EdedupRuntime, transform_class=EdedupTransform)
-        self.params = {}
+class EdedupTableTransformConfiguration(TransformConfiguration):
+  def __init__(self):
+    super().__init__(
+      name=short_name,
+      transform_class=EdedupTransform,
+    )
 ```
 
 The initializer extends the DefaultTableTransformConfiguration which provides simple
 capture of our configuration data and enables picklability through the network.
 It also adds a `params` field that will be used below to hold the transform's
 configuration data (used in `EdedupRuntime.init()` above).
 
@@ -249,36 +258,44 @@
       self.params = self.params | captured
       if self.params["num_hashes"] <= 0:
         logger.info(f"Number of hashes should be greater then zero, provided {args.num_hashes}")
         return False
       logger.info(f"exact dedup params are {self.params}")
       return True
 ```
+Now we can implement `EdedupRayTransformConfiguration`with the following code
+```python
+class EdedupRayTransformConfiguration(RayTransformConfiguration):
+    def __init__(self):
+        super().__init__(transform_config=EdedupTableTransformConfiguration(), runtime_class=EdedupRuntime)
+
+```
 
 ## main()
 
 Next, we show how to launch the framework with the `EdedupTransform` using the
 framework's `TransformLauncher` class.
 
 ```python
 if __name__ == "__main__":
-    launcher = TransformLauncher(transform_runtime_config=EdedupTransformConfiguration())
-    launcher.launch()
+  launcher = RayTransformLauncher(EdedupRayTransformConfiguration())
+  launcher.launch()
 ```
+
 The launcher requires only an instance of DefaultTableTransformConfiguration
-(our `EdedupTransformConfiguration` class).
+(our `EdedupRayTransformConfiguration` class).
 A single method `launch()` is then invoked to run the transform in a Ray cluster.
 
 ## Running
 
 Assuming the above `main()` is placed in `ededup_transform.py` we can run the transform on data
 in COS as follows:
 
 ```shell
 python ededup_transform.py --hash_cpu 0.5 --num_hashes 2 --doc_column "contents" \
   --run_locally True  \
   --s3_cred "{'access_key': 'KEY', 'secret_key': 'SECRET', 'cos_url': 'https://s3.us-east.cloud-object-storage.appdomain.cloud'}" \
   --s3_config "{'input_folder': 'cos-optimal-llm-pile/test/david/input/', 'output_folder': 'cos-optimal-llm-pile/test/david/output/'}"
 ```
 This is a minimal set of options to run locally.
-See the [launcher options](launcher-options.md) for a complete list of
+See the [launcher options](ray-launcher-options) for a complete list of
 transform-independent command line options.
```

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/architecture.md` & `data_prep_toolkit-0.1.0/doc/architecture.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,60 +9,64 @@
 The architecture is a "standard" implementation of [Embarrassingly parallel](https://en.wikipedia.org/wiki/Embarrassingly_parallel) to
 process many input files in parallel using a distribute network of RayWorkers.
 
 ![Processing Architecture](processing-architecture.jpg)
 
 The architecture includes the following core components: 
 
-* [RayLauncher](../src/data_processing/ray/transform_launcher.py) accepts and validates 
+* [RayLauncher](../src/data_processing/runtime/ray/transform_launcher.py) accepts and validates 
  CLI parameters to establish the Ray Orchestrator with the proper configuration. 
 It uses the following components, all of which can/do define CLI configuration parameters.:
-    * [Transform Orchestrator Configuration](../src/data_processing/ray/transform_orchestrator_configuration.py) is responsible 
+    * [Transform Orchestrator Configuration](../src/data_processing/runtime/ray/execution_configuration.py) is responsible 
      for defining and validating infrastructure parameters 
      (e.g., number of workers, memory and cpu, local or remote cluster, etc.). This class has very simple state
      (several dictionaries) and is fully pickleable. As a result framework uses its instance as a
      parameter in remote functions/actors invocation.
     * [DataAccessFactory](../src/data_processing/data_access/data_access_factory.py) - provides the
       configuration for the type of DataAccess to use when reading/writing the input/output data for
       the transforms.  Similar to Transform Orchestrator Configuration, this is a pickleable
       instance that is passed between Launcher, Orchestrator and Workers.
-    * [TransformConfiguration](../src/data_processing/ray/transform_runtime.py) - defines specifics
+    * [TransformConfiguration](../src/data_processing/runtime/ray/transform_runtime.py) - defines specifics
       of the transform implementation including transform implementation class, its short name, any transform-
       specific CLI parameters, and an optional TransformRuntime class, discussed below. 
      
     After all parameters are validated, the ray cluster is started and the DataAccessFactory, TransformOrchestratorConfiguraiton
     and TransformConfiguration are given to the Ray Orchestrator, via Ray remote() method invocation.
     The Launcher waits for the Ray Orchestrator to complete.
-* [Ray Orchestrator](../src/data_processing/ray/transform_orchestrator.py) is responsible for overall management of
+
+* documents with [Ray Orchestrator](../src/data_processing/runtime/ray/transform_orchestrator.py) is responsible for overall management of
   the data processing job. It creates the actors, determines the set of input data and distributes the 
   references to the data files to be processed by the workers. More specifically, it performs the following:
+
   1. Uses the DataAccess instance created by the DataAccessFactory to determine the set of the files 
   to be processed.  
   2. uses the TransformConfiguration to create the TransformRuntime instance 
   3. Uses the TransformRuntime to optionally apply additional configuration (ray object storage, etc) for the configuration
   and operation of the Transform.
-  3. uses the TransformOrchestratorConfiguration to determine the set of RayWorkers to create
+  4. uses the TransformOrchestratorConfiguration to determine the set of RayWorkers to create
   to execute transformers in parallel, providing the following to each worker:
       * Ray worker configuration
       * DataAccessFactory 
       * Transform class and its TransformConfiguration containing the CLI parameters and any TransformRuntime additions.
-  4. in a load-balanced, round-robin fashion, distributes the names of the input files to the workers for them to transform/process.
+  5. in a load-balanced, round-robin fashion, distributes the names of the input files to the workers for them to transform/process.
    
   Additionally, to provide monitoring of long-running transforms, the orchestrator is instrumented with 
   [custom metrics](https://docs.ray.io/en/latest/ray-observability/user-guides/add-app-metrics.html), that are exported to localhost:8080 (this is the endpoint that 
   Prometheus would be configured to scrape).
   Once all data is processed, the orchestrator will collect execution statistics (from the statistics actor) 
   and build and save it in the form of execution metadata (`metadata.json`). Finally, it will return the execution 
   result to the Launcher.
-* [Ray worker](../src/data_processing/ray/transform_table_processor.py) is responsible for 
+
+* [Ray worker](../src/data_processing/runtime/ray/transform_table_processor.py) is responsible for 
 reading files (as [PyArrow Tables](https://levelup.gitconnected.com/deep-dive-into-pyarrow-understanding-its-features-and-benefits-2cce8b1466c8))
 assigned by the orchestrator, applying the transform to the input table and writing out the 
 resulting table(s).  Metadata produced by each table transformation is aggregated into
 Transform Statistics (below).
-* [Transform Statistics](../src/data_processing/ray/transform_statistics.py) is a general 
+
+* [Transform Statistics](../src/data_processing/runtime/ray/transform_statistics.py) is a general 
 purpose data collector actor aggregating the numeric metadata from different places of 
 the framework (especially metadata produced by the transform).
 These statistics are reported as metadata (`metadata.json`) by the orchestrator upon completion.
 
 ## Core Components
 Some of the core components used by the architecture are definfed here:
 
@@ -88,17 +92,17 @@
 A brief discussion of the Transform components are provided here.
 For a more complete discussion, see the [tutorials](transform-tutorials.md).
 
 * [Transform](../src/data_processing/transform/table_transform.py) - defines the methods required
 of any transform implementation - `transform()` and `flush()` - and provides the bulk of any transform implementation
 convert one Table to 0 or more new Tables.   In general, this is not tied to the above Ray infrastructure 
 and so can usually be used independent of Ray. 
-* [TransformRuntime ](../src/data_processing/ray/transform_runtime.py) - this class only needs to be
+* [TransformRuntime ](../src/data_processing/runtime/ray/transform_runtime.py) - this class only needs to be
 extended/implemented when additional Ray components (actors, shared memory objects, etc.) are used
 by the transform. The main method `get_transform_config()` is used to enable these extensions.
-* [TransformConfiguration](../src/data_processing/ray/transform_runtime.py) - this is the bootstrap
+* [TransformConfiguration](../src/data_processing/runtime/ray/transform_runtime.py) - this is the bootstrap
   class provided to the Launcher that enables the instantiation of the Transform and the TransformRuntime within
   the architecture.  It is a CLIProvider, which allows it to define transform-specific CLI configuration
   that is made available to the Transform's initializer.
```

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/launcher-options.md` & `data_prep_toolkit-0.1.0/doc/ray-launcher-options.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,79 @@
-# Launcher Command Line Options
+# Ray Launcher Command Line Options
 A number of command line options are available when launching a transform.  
 
 The following is a current --help output (a work in progress) for 
-the `NOOPTransform` (note the --noop_sleep_sec option):
+the `NOOPTransform` (note the --noop_sleep_sec and --noop_pwd options):
 
 ```
-usage: noop_transform.py [-h] 
-                         [--run_locally RUN_LOCALLY]
-                         [--noop_sleep_sec NOOP_SLEEP_SEC] 
-                         [--data_s3_cred DATA_S3_CRED]
-                         [--data_s3_config DATA_S3_CONFIG]
-                         [--data_local_config DATA_LOCAL_CONFIG]
-                         [--data_max_files DATA_MAX_FILES]
-                         [--data_checkpointing DATA_CHECKPOINTING]
-                         [--data_data_sets DATA_DATA_SETS]
-                         [--data_max_files MAX_FILES]
-                         [--data_files_to_use DATA_FILES_TO_USE]
-                         [--data_num_samples DATA_NUM_SAMPLES]
-                         [--runtime_num_workers NUM_WORKERS] 
-                         [--runtime_worker_options WORKER_OPTIONS]
-                         [--runtime_pipeline_id PIPELINE_ID] [--job_id JOB_ID]
-                         [--runtime_creation_delay CREATION_DELAY]
-                         [--runtime_code_location CODE_LOCATION]
+usage: noop_transform.py [-h] [--run_locally RUN_LOCALLY] [--noop_sleep_sec NOOP_SLEEP_SEC] [--noop_pwd NOOP_PWD] [--data_s3_cred DATA_S3_CRED] [--data_s3_config DATA_S3_CONFIG] [--data_local_config DATA_LOCAL_CONFIG]
+                         [--data_max_files DATA_MAX_FILES] [--data_checkpointing DATA_CHECKPOINTING] [--data_data_sets DATA_DATA_SETS] [--data_files_to_use DATA_FILES_TO_USE] [--data_num_samples DATA_NUM_SAMPLES]
+                         [--runtime_num_workers RUNTIME_NUM_WORKERS] [--runtime_worker_options RUNTIME_WORKER_OPTIONS] [--runtime_creation_delay RUNTIME_CREATION_DELAY] [--runtime_pipeline_id RUNTIME_PIPELINE_ID]
+                         [--runtime_job_id RUNTIME_JOB_ID] [--runtime_code_location RUNTIME_CODE_LOCATION]
 
-Driver for NOOP processing
+Driver for noop processing
 
 options:
   -h, --help            show this help message and exit
   --run_locally RUN_LOCALLY
                         running ray local flag
   --noop_sleep_sec NOOP_SLEEP_SEC
                         Sleep actor for a number of seconds while processing the data frame, before writing the file to COS
-  --data_s3_cred S3_CRED     
-                        AST string of options for cos credentials. Only required for COS or Lakehouse.
+  --noop_pwd NOOP_PWD   A dummy password which should be filtered out of the metadata
+  --data_s3_cred DATA_S3_CRED
+                        AST string of options for s3 credentials. Only required for S3 data access.
                         access_key: access key help text
                         secret_key: secret key help text
-                        cos_url: COS url
-                        Example: { 'access_key': 'access', 'secret_key': 'secret', 's3_url': 'https://s3.us-east.cloud-object-storage.appdomain.cloud' }
-  --data_s3_config S3_CONFIG
+                        url: optional s3 url
+                        region: optional s3 region
+                        Example: { 'access_key': 'access', 'secret_key': 'secret', 
+                        'url': 'https://s3.us-east.cloud-object-storage.appdomain.cloud', 
+                        'region': 'us-east-1' }
+  --data_s3_config DATA_S3_CONFIG
                         AST string containing input/output paths.
                         input_folder: Path to input folder of files to be processed
                         output_folder: Path to output folder of processed files
-                        Example: { 'input_folder': 'your input folder', 'output_folder ': 'your output folder' }
-  --data_local_config LOCAL_CONFIG
+                        Example: { 'input_folder': 's3-path/your-input-bucket', 
+                        'output_folder': 's3-path/your-output-bucket' }
+  --data_local_config DATA_LOCAL_CONFIG
                         ast string containing input/output folders using local fs.
                         input_folder: Path to input folder of files to be processed
                         output_folder: Path to output folder of processed files
                         Example: { 'input_folder': './input', 'output_folder': '/tmp/output' }
-  --data_max_files MAX_FILES
+  --data_max_files DATA_MAX_FILES
                         Max amount of files to process
-  --data_checkpointing CHECKPOINTING
+  --data_checkpointing DATA_CHECKPOINTING
                         checkpointing flag
-  --data_data_sets DATA_SETS
-                        List of data sets
+  --data_data_sets DATA_DATA_SETS
+                        List of sub-directories of input directory to use for input. For example, ['dir1', 'dir2']
   --data_files_to_use DATA_FILES_TO_USE
-                        files extensions to use, default .parquet
+                        list of file extensions to choose for input.
   --data_num_samples DATA_NUM_SAMPLES
-                        number of randomply picked files to use
-  --runtime_num_workers NUM_WORKERS
+                        number of random input files to process
+  --runtime_num_workers RUNTIME_NUM_WORKERS
                         number of workers
-  --runtime_worker_options WORKER_OPTIONS
+  --runtime_worker_options RUNTIME_WORKER_OPTIONS
                         AST string defining worker resource requirements.
                         num_cpus: Required number of CPUs.
                         num_gpus: Required number of GPUs
                         resources: The complete list can be found at
                                    https://docs.ray.io/en/latest/ray-core/api/doc/ray.remote_function.RemoteFunction.options.html#ray.remote_function.RemoteFunction.options
                                    and contains accelerator_type, memory, name, num_cpus, num_gpus, object_store_memory, placement_group,
                                    placement_group_bundle_index, placement_group_capture_child_tasks, resources, runtime_env,
                                    scheduling_strategy, _metadata, concurrency_groups, lifetime, max_concurrency, max_restarts,
                                    max_task_retries, max_pending_calls, namespace, get_if_exists
-                        Example: { 'num_cpus': '8', 'num_gpus': '1', 'resources': '{"special_hardware": 1, "custom_label": 1}' }
-  --runtime_pipeline_id PIPELINE_ID
-                        pipeline id
-  --runtime_job_id JOB_ID       job id
-  --runtime_creation_delay CREATION_DELAY
+                        Example: { 'num_cpus': '8', 'num_gpus': '1', 
+                        'resources': '{"special_hardware": 1, "custom_label": 1}' }
+  --runtime_creation_delay RUNTIME_CREATION_DELAY
                         delay between actor' creation
-  --runtime_code_location CODE_LOCATION
+  --runtime_pipeline_id RUNTIME_PIPELINE_ID
+                        pipeline id
+  --runtime_job_id RUNTIME_JOB_ID
+                        job id
+  --runtime_code_location RUNTIME_CODE_LOCATION
                         AST string containing code location
                         github: Github repository URL.
                         commit_hash: github commit hash
                         path: Path within the repository
-                        Example: { 'github': 'https://github.com/somerepo', 'commit_hash': '13241231asdfaed', 'path': 'transforms/universal/ededup' }
+                        Example: { 'github': 'https://github.com/somerepo', 'commit_hash': '1324', 
+                        'path': 'transforms/universal/code' }
 ```
```

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/overview.md` & `data_prep_toolkit-0.1.0/doc/overview.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 more complex transformations requiring coordination among transforming nodes.
 This might include operations such as de-duplication, merging, and splitting.
 The framework uses a plugin-model for the primary functions.  The key ones for
 developers of data transformation are:
 
 * [Transformation](../src/data_processing/transform/table_transform.py) - a simple, easily-implemented interface defines
 the specifics of a given data transformation.
-* [Transform Configuration](../src/data_processing/ray/transform_runtime.py) - defines
-the transform implementation and runtime classes, the 
-command line arguments specific to transform, and the short name for the transform.
-* [Transformation Runtime](../src/data_processing/ray/transform_runtime.py) - allows for customization of the Ray environment for the transformer.
-This might include provisioning of shared memory objects or creation of additional actors.
+* [Transform Configuration](../src/data_processing/runtime/ray/transform_runtime.py) - defines
+the transform short name, its implementation class,  and command line configuration
+parameters.
 
 To learn more consider the following:
 
 * [Transform Tutorials](transform-tutorials.md)
-* [Testing transformers with S3](using_s3_transformers.md)
+* [Transform Runtimes](transform-runtimes.md)
+* [Transform Examples](transform-tutorial-examples.md)
+* [Testing Transforms](transform-testing.md)
+* [Utilities](transformer-utilities.md)
 * [Architecture Deep Dive](architecture.md)
 * [Transform project root readme](../../transforms/README.md)
```

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/processing-architecture.jpg` & `data_prep_toolkit-0.1.0/doc/processing-architecture.jpg`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/simplest-transform-tutorial.md` & `data_prep_toolkit-0.1.0/doc/simplest-transform-tutorial.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,59 +11,64 @@
 * How to define transform-specific metadata that can be associated
   with each table transformation and aggregated across all transformations
   in a single run of the transform.
 * How to define command line arguments that can be used to configure
   the operation of our _noop_ transform.
 
 We will **not** be showing the following:
-* The creation of a custom TransformRuntime that would enable more global
-  state and/or coordination among the transforms running in other ray actors.
+* The creation of a custom `TransformRuntime` that would enable more global
+  state and/or coordination among the transforms running in other Ray actors.
   This will be covered in an advanced tutorial.
 
 The complete task involves the following:
-* NOOPTransform - class that implements the specific transformation
-* NOOPTableTransformConfiguration - class that provides configuration for the
-  NOOPTransform, specifically the command line arguments used to configure it.
-* main() - simple creation and use of the TransformLauncher.
+
+* `NOOPTransform` - class that implements the specific transformation
+* `NOOPTableTransformConfiguration` - class that provides configuration for the
+  `NOOPTransform`, specifically the command line arguments used to configure it.
+* `main()` - simple creation and use of the `TransformLauncher`.
 
 (Currently, the complete code for the noop transform used for this
 tutorial can be found in the
 [noop transform](../../transforms/universal/noop) directory.
 
-Finally, we show to use the command line to run the transform in a local ray cluster
+Finally, we show how to use the command line to run the transform in a local ray cluster.
+
+> **Note:** You will need to run the setup commands in the [`../README`](..) before running the following examples.
+
 
-## NOOPTransform
+## `NOOPTransform`
 
 First, let's define the transform class.  To do this we extend
 the base abstract/interface class
-[AbstractTableTransform](../src/data_processing_ibm/transform/table_transform.py),
+[`AbstractTableTransform`](../src/data_processing_ibm/transform/table_transform.py),
 which requires definition of the following:
+
 * an initializer (i.e. `init()`) that accepts a dictionary of configuration
   data.  For this example, the configuration data will only be defined by
   command line arguments (defined below).
-* the `transform()` method itself that takes an input table produces an output
-  table and any associated metadata for that table transformation.
+* the `transform()` method itself that takes an input table and produces an output
+  table with any associated metadata for that table transformation.
 
 Other methods such as `flush()` need not be overridden/redefined for this simple example.
 
 We start with the simple definition of the class, its initializer and the imports required
 by subsequent code:
 
 ```python
 import time
 from argparse import ArgumentParser, Namespace
 from typing import Any
 
 import pyarrow as pa
-from data_processing.ray import (
-  RayLauncherConfiguration,
-  DefaultTableTransformRuntimeRay,
-  RayTransformLauncher,
+from data_processing.runtime.ray import RayTransformLauncher
+from data_processing.runtime.ray.runtime_configuration import (
+  RayTransformRuntimeConfiguration,
 )
-from data_processing.transform import AbstractTableTransform
+from data_processing.transform import AbstractTableTransform, TransformConfiguration
+from data_processing.utils import CLIArgumentProvider, get_logger
 
 
 class NOOPTransform(AbstractTableTransform):
 
   def __init__(self, config: dict[str, Any]):
     self.sleep = config.get("sleep", 1)
 ```
@@ -71,128 +76,146 @@
 
 For purposes of the tutorial and to simulate a more complex processing
 job, our initializer allows our transform to be configurable
 with an amount of seconds to sleep/delay during the call to `transform()`.
 Configuration is provided by the framework in a dictionary provided to the initializer.
 Below we will cover how this `sleep` argument is made available to the initializer.
 
-Note that in more complex transforms that might, for example, load a hugging face or other model,
+Note that in more complex transforms that might, for example, load a Hugging Face or other model,
 or perform other deep initializations, these can be done in the initializer.
 
 Next we define the `transform()` method itself, which includes the addition of some
 almost trivial metadata.
 
 ```python
     def transform(self, table: pa.Table) -> tuple[list[pa.Table], dict[str, Any]]:
         if self.sleep is not None:
             time.sleep(self.sleep)
         # Add some sample metadata.
         metadata = {"nfiles": 1, "nrows": len(table)}
         return [table], metadata
 ```
 The single input to this method is the in-memory pyarrow table to be transformed.
-The return of this function is a list of tables and optional metadata.  In this
-case of simple 1:1 table conversion the list will contain a single table, the input.
+The return value of this method is a list of tables and optional metadata.  In this
+case, we are doing a simple 1:1 table conversion, so the list will contain a single table, the input table.
 The metadata is a free-form dictionary of keys with numeric values that will be aggregated
 by the framework and reported as aggregated job statistics metadata.
 If there is no metadata then simply return an empty dictionary.
 
-## NOOPTransformConfiguration
+## `NOOPTransformConfiguration`
 
-Next we define the `NOOPTransformConfiguration` class and its initializer that define the following:
+Next we define the `NOOPTransformConfiguration` class and its initializer that defines the following:
 
 * The short name for the transform
-* The class implementing the transform - in our case NOOPTransform
+* The class implementing the transform - in our case `NOOPTransform`
 * Command line argument support.
-* The transform runtime class be used.  We will use the `DefaultTableTransformRuntime`
-  which is sufficient for most 1:1 table transforms.  Extensions to this class can be
-  used when more complex interactions among transform is required.*
+ 
+We also define the `NOOPRayTransformationConfiguration` so we can run the transform
+in the Ray runtime as well.  This adds allows the option to add a transform-specific
+Ray runtime class allowing more complex distributed memory and data sharing operations.
+The NOOP transform will not make use of this so is a simple extension.:
 
-First we define the class and its initializer,
+First we define the pure python transform configuration  class and its initializer,
 
 ```python
-short_name = "NOOP"
+short_name = "noop"
 cli_prefix = f"{short_name}_"
+pwd_key = "pwd"
 
-class NOOPTransformConfiguration(DefaultTableTransformConfiguration):
-    
+class NOOPTransformConfiguration(TransformConfiguration):
     def __init__(self):
-        super().__init__(name=short_name, transform_class=NOOPTransform)
-        self.params = {}
+        super().__init__(
+            name=short_name,
+            transform_class=NOOPTransform,
+            remove_from_metadata=[pwd_key],
+        )
 ```
-The initializer extends the DefaultTableTransformConfiguration which provides simple
-capture of our configuration data and enables picklability through the network.
+
+The initializer extends the `TransformConfiguration` that provides simple
+capture of our configuration data and enables the ability to pickle through the network.
 It also adds a `params` field that will be used below to hold the transform's
 configuration data (used in `NOOPTransform.init()` above).
 
 Next, we provide two methods that define and capture the command line configuration that
-is specific to the `NOOPTransform`, in this case the number of seconds to sleep during transformation
-and an example command line, `pwd`, option holding sensitive data that we don't want reported
-in the job metadata produced by the ray orchestrator.
-First we define the method establishes the command line arguments.
-This method is given a global argument parser to which the `NOOPTransform` arguments are added.
-It is good practice to include a common prefix to all transform-specific options (i.e. pii, lang, etc).
+is specific to the `NOOPTransform`, in this case the parameters are the number of seconds to sleep during transformation
+and an example command line parameter, `pwd` ("password"), option holding sensitive data that we don't want reported
+in the job metadata produced by the Ray orchestrator.
+
+The first method establishes the command line arguments.
+It is given a global argument parser to which the `NOOPTransform` arguments are added.
+It is a good practice to include a common prefix to all transform-specific options (i.e. pii, lang, etc).
 In our case we will use `noop_`.
 
 ```python
     def add_input_params(self, parser: ArgumentParser) -> None:
         parser.add_argument(
-            f"--{cli_prefix}noop_sleep_sec",
+            f"--{sleep_cli_param}",
             type=int,
             default=1,
-            help="Sleep actor for a number of seconds while processing the data frame",
+            help="Sleep actor for a number of seconds while processing the data frame, before writing the file to COS",
         )
-        # An example of a command line option that we don't want included in the metadata collected by the Ray orchestrator
-        # See below for remove_from_metadata addition so that it is not reported.
         parser.add_argument(
-            f"--{cli_prefix}noop_pwd",
+            f"--{pwd_cli_param}",
             type=str,
             default="nothing",
             help="A dummy password which should be filtered out of the metadata",
         )
+
+
+
 ```
-Next we implement a method that is called after the framework has parsed the CLI args
-and which allows us to capture the `NOOPTransform`-specific arguments, optionally validate them
-and flag that the `pwd` parameter should not be reported in the metadata.
+Next we implement a method that is called after the CLI args are parsed (usually by one
+of the runtimes) and which allows us to capture the `NOOPTransform`-specific arguments. 
+ 
 
 ```python
+
     def apply_input_params(self, args: Namespace) -> bool:
         captured = CLIArgumentProvider.capture_parameters(args, cli_prefix, False)
         if captured.get(sleep_key) < 0:
-          print(f"Parameter noop_sleep_sec should be non-negative. you specified {args.noop_sleep_sec}")
-          return False
-      
-        self.params = self.params | captured
-        logger.info(f"noop parameters are : {self.params}")
-        # Don't publish this in the metadata produced by the ray orchestrator.
-        self.remove_from_metadata.append(pwd_key)
+            print(f"Parameter noop_sleep_sec should be non-negative. you specified {args.noop_sleep_sec}")
+            return False
+        self.params = captured
         return True
 ```
+## Runtime Launching
+To run the transform on a set of input data, we use one of the runtimes, each described below.
 
-## main()
-
-Next, we show how to launch the framework with the `NOOPTransform` using the
-framework's `TransformLauncher` class.
+### Python Runtime
+To run in the python runtime, we need to create the instance of `PythonTransformLauncher`
+using the `NOOPTransformConfiguration`, and launch it as follows:
 
 ```python
 if __name__ == "__main__":
-    launcher = TransformLauncher(transform_runtime_config=NOOPTransformConfiguration())
+    launcher = PythonTransformLauncher(transform_config=NOOPTransformConfiguration())
     launcher.launch()
 ```
-The launcher requires only an instance of DefaultTableTransformConfiguration
-(our `NOOPTransformConfiguration` class).
-A single method `launch()` is then invoked to run the transform in a Ray cluster.
 
 ## Running
 
-Assuming the above `main()` is placed in `noop_main.py` we can run the transform on data
-in COS as follows:
-
+Assuming the above `main` code is placed in `noop_main.py` we can run the transform on some test data. We'll use data in the repo for the noop transform
+and create a temporary directory to hold the output:
+```shell
+export DPK_REPOROOT=...
+export NOOP_INPUT=$DPK_REPOROOT/transforms/universal/noop/test-data/input
+```
+To run
 ```shell
 python noop_main.py --noop_sleep_msec 2 \
-  --run_locally True  \
-  --s3_cred "{'access_key': 'KEY', 'secret_key': 'SECRET', 'cos_url': 'https://s3.us-east.cloud-object-storage.appdomain.cloud'}" \
-  --s3_config "{'input_folder': 'cos-optimal-llm-pile/test/david/input/', 'output_folder': 'cos-optimal-llm-pile/test/david/output/'}"
+  --data_local_config "{'input_folder': '"$NOOP_INPUT"', 'output_folder': '/tmp/noop-output'}"
+```
+See the [python launcher options](python-launcher-options.md) for a complete list of
+transform-independent command line options.
+
+### Ray Runtime
+To run in the Ray runtime, instead of creating the `PythonTransformLauncher`
+we use the `RayTransformLauncher`.
+as follows:
+```python
+if __name__ == "__main__":
+    launcher = RayTransformLauncher(transform_config=NOOPRayTransformConfiguration())
+    launcher.launch()
 ```
-This is a minimal set of options to run locally.
-See the [launcher options](launcher-options.md) for a complete list of
+We can run this with the same command as for the python runtime but to run in local Ray
+add the `--run_locally True` option.
+See the [ray launcher options](ray-launcher-options.md) for a complete list of
 transform-independent command line options.
```

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/testing-transforms.md` & `data_prep_toolkit-0.1.0/doc/transform-standalone-testing.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 `get_test_*_fixtures()` method that must be implemented by the specific
 transform implementation test to define the various sets of inputs tested.
 This approach allows the definition of new generic transform tests that existing
 transform implementation tests will easily leverage.
 
 The first (currently only test) is a the `test_transform()` method that takes the
 following inputs:
+
 * the transform implementation being tested, properly configured with the configuration
 dictionary for the associated test data.
 * a list of N (1 or more) input tables to be processed with the transform's `transform(Table)` method.
 * The expected list of accumulated tables across the N calls to 
 `transform(Table)` and the single finalizing call to the transform's `flush()` method.
 In the case where the `transform()` returns an empty list, no associated expected Table 
 should be included in this list.
```

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/transform-external-resources.md` & `data_prep_toolkit-0.1.0/doc/transform-external-resources.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 (e.g. models, configuration, etc.) to complete its job.  For example, the Blocklist transform
 loads a list of domains to block.  Resources can be loaded from either S3 or local storage or a 
 custom location defined by the transform (i.e. hugging face, etc).
 In addition to actually loading the resource(s), the transform needs to define the configuration that 
 defines the location of the domain list. 
 
 In the next sections we cover the following:
+
    1. How to define the transform-specific resource location(s) as command line arguments
    2. How to load the transform-specific resources, either or both of:
       1. During transform initialization - this is useful for testing outside of ray, and optionally
       2. During transform configuration in the Ray orchestrator.  This may not be feasible if a resource 
          is not picklable.
```

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/transform-tutorials.md` & `data_prep_toolkit-0.1.0/doc/ray-runtime.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,94 @@
-# Transform Tutorials
+# Ray Runtime 
+The Ray runtime includes the following set of components:
 
-All transforms operate on a [pyarrow Table](https://arrow.apache.org/docs/python/generated/pyarrow.Table.html)
-and produce zero or more transformed tables and transform specific metadata.
-The Transform itself need only be concerned with the conversion of one in memory table at a time.  
-
-When running in the Ray worker (i.e. [TransformTableProcessor](../src/data_processing/ray/transform_table_processor.py) ), the input
-tables are read from parquet files and the transform table(s) is/are stored in destination parquet files.
-Metadata accumulated across calls to all transforms is stored in the destination.
-
-### Transform Basics
-In support of this model the class 
-[AbstractTableTransform](../src/data_processing/transform/table_transform.py) 
-is expected to be extended when implementing a transform.
-The following methods are defined:
-
-* ```__init__(self, config:dict)``` - an initializer through which the transform can be created 
-with implementation-specific configuration.  For example, the location of a model, maximum number of
-rows in a table, column(s) to use, etc. 
-* ```transform(self, table:pyarrow.Table) -> tuple(list[pyarrow.Table], dict)``` - this method is responsible
-for the actual transformation of a given table to zero or more output tables, and optional 
-metadata regarding the transformation applied.  Zero tables might be returned when
-merging tables across calls to `transform()` and more than 1 table might be returned
-when splitting tables by size or other criteria.
-  * _output tables list_ - the RayWork handles the various number of returned tables as follows: 
-    * 0 - no file will be written out and the input file name will not be used in the output directory.
-    * 1 - one parquet file will be written to the output directory with 
-    * N - N parquet files are written to the output with `_<index>` appended to the base file name
-  * _dict_ - is a dictionary of transform-specific data keyed to numeric values.  The RayWorker will
-         accumulate/add dictionaries across all calls to transform across all RayWorkers.  As an example, a
-         transform might wish to track the number of instances of PII entities detected and might return 
-        this as `{ "entities" : 1234 }`.
-* ```flush() -> tuple(list[pyarrow.Table], dict)``` - this is provided for transforms that
-make use of buffering (e.g. [coalesce](../../transforms/universal/coalesce/src/coalesce_transform.py)) across calls 
-to `transform()` and need to be flushed of all buffered data at the end of processing of input tables.  
-The return values are handled the same waa as the return values for `transform()`.  Since most transforms will likely
-not need this feature, a default implementation is provided to return an empty list and empty dictionary.
-
-### Running in Ray
-When a transform is run using the Ray-based framework a number of other capabilities are involved:
-
-* [Transform Runtime](../src/data_processing/ray/transform_runtime.py) - this provides the ability for the
-transform implementor to create additional Ray resources 
+* [RayTransformLauncher](../src/data_processing/runtime/ray/transform_launcher.py) - this is a 
+class generally used to implement `main()` that makes use of a `TransformConfiguration` to 
+start the Ray runtime and execute the transform over the specified set of input files.
+The RayTransformLauncher is created using a `RayTransformConfiguration` instance.
+* [RayTransformConfiguration](../src/data_processing/runtime/ray/runtime_configuration.py) - this 
+class extends transform's base TransformConfiguration implementation to add an optional 
+`TranformRuntime` (see next) class to be used by the transform implementation.
+* [TransformRuntime](../src/data_processing/runtime/ray/transform_runtime.py) - 
+this provides the ability for the transform implementor to create additional Ray resources 
 and include them in the configuration used to create a transform
-(see, for example, [exact dedup](../../transforms/universal/ededup/src/ededup_transform.py) 
-or [blocklist](../../transforms/universal/blocklisting/src/blocklist_transform.py)).
+(see, for example, [exact dedup](../../transforms/universal/ededup/src/ededup_transform.py)).
 This also provide the ability to supplement the statics collected by
-[Statistics](../src/data_processing/ray/transform_statistics.py) (see below).
-* [Transform Configuration](../src/data_processing/ray/transform_runtime.py) - defines the following:
-  * the transform class to be used, 
-  * command line arguments used to initialize the Transform Runtime and generally, the Transform.
-  * Transform Runtime class to use
-  * transform short name 
-* [Transform Launcher](../src/data_processing/ray/transform_launcher.py) - this is a class generally used to 
-implement `main()` that makes use of a Transform Configuration to start the Ray runtime and execute the transforms.
+[Statistics](../src/data_processing/runtime/ray/transform_statistics.py) (see below).
 
 Roughly speaking the following steps are completed to establish transforms in the RayWorkers
 
 1. Launcher parses the CLI parameters using an ArgumentParser configured with its own CLI parameters 
 along with those of the Transform Configuration, 
-2. Launcher passes the Transform Configuration and CLI parameters to the [RayOrchestrator](../src/data_processing/ray/transform_orchestrator.py)
+2. Launcher passes the Transform Configuration and CLI parameters to the [RayOrchestrator](../src/data_processing/runtime/ray/transform_orchestrator.py)
 3. RayOrchestrator creates the Transform Runtime using the Transform Configuration and its CLI parameter values
 4. Transform Runtime creates transform initialization/configuration including the CLI parameters,  
 and any Ray components need by the transform.
-5. [RayWorker](../src/data_processing/ray/transform_table_processor.py) is started with configuration from the Transform Runtime.
+5. [RayWorker](../src/data_processing/runtime/ray/transform_table_processor.py) is started with configuration from the Transform Runtime.
 6. RayWorker creates the Transform using the configuration provided by the Transform Runtime.
 7. Statistics is used to collect the statistics submitted by the individual transform, that 
 is used for building execution metadata.
 
 ![Processing Architecture](processing-architecture.jpg)
 
-#### Transform Launcher
-The [TransformLauncher](../src/data_processing/ray/transform_launcher.py) uses the Transform Configuration
+## Ray Transform Launcher
+The [RayTransformLauncher](../src/data_processing/runtime/ray/transform_launcher.py) uses the Transform Configuration
 and provides a single method, `launch()`, that kicks off the Ray environment and transform execution coordinated 
-by [orchestrator](../src/data_processing/ray/transform_orchestrator.py).
+by [orchestrator](../src/data_processing/runtime/ray/transform_orchestrator.py).
 For example,
 ```python
-launcher = TransformLauncher(MyTransformConfiguration())
+launcher = RayTransformLauncher(YourTransformConfiguration())
 launcher.launch()
 ```
 Note that the launcher defines some additional CLI parameters that are used to control the operation of the 
-[orchestrator and workers](../src/data_processing/ray/transform_orchestrator_configuration.py) and 
+[orchestrator and workers](../src/data_processing/runtime/ray/execution_configuration.py) and 
 [data access](../src/data_processing/data_access/data_access_factory.py).  Things such as data access configuration,
 number of workers, worker resources, etc.
 Discussion of these options is beyond the scope of this document 
-(see [Launcher Options](launcher-options.md) for a list of available options.)
+(see [Launcher Options](ray-launcher-options) for a list of available options.)
 
-#### Transform Configuration
-The 
-[DefaultTableTransformConfiguration](../src/data_processing/ray/transform_runtime.py)
-class is sub-classed and initialized with transform-specific name, and implementation 
-and runtime classes. In addition, it is responsible for providing transform-specific
-methods to define and filter optional command line arguments.
-Finally, it creates the Transform Runtime, for which a default
-implementation uses the class available in the Transform Configuration.
+## Ray Transform Configuration
+In general, a transform should be able to run in both the python and Ray runtimes.
+As such we first define the python-only transform configuration, which will then
+be used by the Ray-runtime-specific transform configuration. 
+The python transform configuration implements  
+[TransformConfiguration](../src/data_processing/runtime/runtime_configuration.py)
+and deifnes with transform-specific name, and implementation 
+and class. In addition, it is responsible for providing transform-specific
+methods to define and capture optional command line arguments.
 ```python
 
-class MyTransformConfiguration(DefaultTableTransformConfiguration):
+class YourTransformConfiguration(TransformConfiguration):
 
     def __init__(self):
-        super().__init__(name="MyTransform", transform_class=MyTransform,
-                          runtime_class=MyTransformRuntime
+        super().__init__(name="YourTransform", transform_class=YourTransform)
         self.params = {}
+        
     def add_input_params(self, parser: ArgumentParser) -> None:
         ...
     def apply_input_params(self, args: Namespace) -> bool:
         ...
-    def create_transform_runtime(self) -> DefaultTableTransformRuntime:
-        ...
 ```
-Details are covered in the samples below.
+Next we define the Ray-runtime specific transform configuration as an exension of
+the RayTransformConfiguration and uses the `YourTransformConfiguration` above.
+```python
+    
+class YourTransformConfiguration(RayTransformConfiguration):
+    def __init__(self):
+        super().__init__(YourTransformConfiguration(),
+                         runtime_class=YourTransformRuntime
+```
+This class provides the ability to create the instance of `YourTransformRuntime` class (see below)
+as needed by the Ray runtime.  Note, that not all transforms will require a `runtime_class`
+and can omit this parameter to default to an acceptable runtime class.
+Details are covered in the [advanced transform tutorial](advanced-transform-tutorial.md).
 
-#### Transform Runtime
+## Transform Runtime
 The 
-[DefaultTableTransformRuntime](../src/data_processing/ray/transform_runtime.py)
+[DefaultTableTransformRuntime](../src/data_processing/runtime/ray/transform_runtime.py)
 class is provided and will be 
 sufficient for many use cases, especially 1:1 table transformation.
 However, some transforms will require use of the Ray environment, for example,
 to create additional workers, establish a shared memory object, etc.
 Of course, these transforms will generally not run outside of Ray environment. 
 
 ```python
@@ -145,15 +117,15 @@
 For those transforms that don't need this support, the default implementation
 simpy returns the CLI parameters used to initialize the runtime instance.
 
 The `computed_execution_stats()` provides an opportunity to augment the statistics
 collected and aggregated by the TransformStatistics actor. It is called by the RayOrchestrator
 after all files have been processed.
 
-### Exceptions
+## Exceptions
 A transform may find that it needs to signal error conditions.
 For example, if a referenced model could not be loaded or
 a given table does not have the expected column.
 In general, it should identify such conditions by raising an exception. 
 With this in mind, there are two types of exceptions:
 
 1. Those that would not allow any tables to be processed (e.g. model loading problem).
@@ -165,30 +137,7 @@
 should throw an exception from the associated method.  This will cause only the
 error-causing
 table to be ignored and not written out, but allow continued processing of tables by 
 the transform.
 In both cases, the framework will log the exception as an error.
 
 
-### Tutorial Examples
-With these basic concepts in mind, we start with a simple example and 
-progress to more complex transforms. 
-Before getting started  you may want to consult the 
-[transform project root readme](../../transforms/README.md) documentation.
-
-* [Simplest transform](simplest-transform-tutorial.md) - 
-Here we will take a simple example to show the basics of creating a simple transform
-that takes a single input Table, and produces a single Table.
-* [External resources transform](transform-external-resources.md) - shows how to load additional
-resources (models, configuration, etc) for a transform.
-* [Advanced transform](advanced-transform-tutorial.md)
-
-Once a transform has been built, testing can be enabled with the testing framework:
-
-* [Transform Testing](testing-transforms.md) - shows how to test a transform
-independent of the Ray framework.
-* [End-to-End Testing](testing-e2e-transform.md) - shows how to test the
-transform running in the Ray environment.
-
-### Additional transform support
-
-We also strted a library of [transform utilities](transformer-utilities.md)
```

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/transformer-utilities.md` & `data_prep_toolkit-0.1.0/doc/transformer-utilities.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Transform Utilities
 
 A class [TransformUtils](../src/data_processing/utils/transform_utils.py) provides several methods that simplify 
 transformer's implementation. Currently it includes the following methods:
+
 * `deep_get_size` is the method to get the complete size of the Python object based on
   https://www.askpython.com/python/built-in-methods/variables-memory-size-in-python
   It supports Python structures: list, tuple and set
 * `normalize_string` normalizes string, converting it to lower case and removing spaces, punctuation and CR
 * `str_to_hash`convert string to 259 bit hash
 * `str_to_int` getting an integer representing string by calculating string's hash
 * `validate_columns` check whether required columns exist in the table
@@ -13,12 +14,13 @@
 be removed before it is added
 * `validate_path` cleans up s3 path - Removes white spaces from the input/output paths
   removes schema prefix (s3://, http:// https://), if exists
   adds the "/" character at the end, if it doesn't exist
   removes URL encoding
 
 It also contain two variables:
+
 * `RANDOM_SEED` number that is used for methods that require seed
 * `LOCAL_TO_DISK` rough local size to size on disk/S3
 
 This class should be extended with additional methods, generally useful across multiple transformers and documentation 
-should be added here 
+should be added here
```

### Comparing `data_prep_toolkit-0.0.1.dev4/doc/using_s3_transformers.md` & `data_prep_toolkit-0.1.0/doc/transform-s3-testing.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/pyproject.toml` & `data_prep_toolkit-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "data_prep_toolkit"
-version = "0.0.1-dev4"
+version = "0.1.0"
 requires-python = ">=3.10"
 description = "Data Preparation Toolkit Library"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "David Wood", email = "dawood@us.ibm.com" },
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
@@ -41,12 +41,12 @@
 package_dir = ["src","test"]
 
 [options.packages.find]
 where = ["src/data_processing"]
 
 [tool.pytest.ini_options]
 # Currently we use low coverage since we have to run tests separately (see makefile)
-addopts = "--cov --cov-report term-missing --cov-fail-under 25"
+#addopts = "--cov --cov-report term-missing --cov-fail-under 25"
 markers = ["unit: unit tests", "integration: integration tests"]
 
 [tool.coverage.run]
 include = ["src/*"]
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_prep_toolkit.egg-info/PKG-INFO` & `data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit
-Version: 0.0.1.dev4
+Version: 0.1.0
 Summary: Data Preparation Toolkit Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_prep_toolkit.egg-info/SOURCES.txt` & `data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,73 @@
 .gitignore
 Makefile
 README.md
 pyproject.toml
 doc/advanced-transform-tutorial.md
 doc/architecture.md
-doc/launcher-options.md
-doc/logo-ibm-dark.png
-doc/logo-ibm.png
 doc/overview.md
 doc/processing-architecture.jpg
+doc/python-launcher-options.md
+doc/python-runtime.md
+doc/ray-launcher-options.md
+doc/ray-runtime.md
 doc/simplest-transform-tutorial.md
 doc/testing-e2e-transform.md
-doc/testing-transforms.md
 doc/transform-external-resources.md
+doc/transform-runtimes.md
+doc/transform-s3-testing.md
+doc/transform-standalone-testing.md
+doc/transform-testing.md
+doc/transform-tutorial-examples.md
 doc/transform-tutorials.md
 doc/transformer-utilities.md
-doc/using_s3_transformers.md
 src/data_prep_toolkit.egg-info/PKG-INFO
 src/data_prep_toolkit.egg-info/SOURCES.txt
 src/data_prep_toolkit.egg-info/dependency_links.txt
 src/data_prep_toolkit.egg-info/requires.txt
 src/data_prep_toolkit.egg-info/top_level.txt
 src/data_processing/__init__.py
 src/data_processing/data_access/__init__.py
 src/data_processing/data_access/arrow_s3.py
 src/data_processing/data_access/data_access.py
 src/data_processing/data_access/data_access_factory.py
 src/data_processing/data_access/data_access_factory_base.py
 src/data_processing/data_access/data_access_local.py
 src/data_processing/data_access/data_access_s3.py
-src/data_processing/pure_python/__init__.py
-src/data_processing/pure_python/python_launcher_configuration.py
-src/data_processing/pure_python/transform_launcher.py
-src/data_processing/pure_python/transform_orchestrator.py
-src/data_processing/pure_python/transform_table_processor.py
-src/data_processing/ray/__init__.py
-src/data_processing/ray/ray_utils.py
-src/data_processing/ray/transform_launcher.py
-src/data_processing/ray/transform_orchestrator.py
-src/data_processing/ray/transform_orchestrator_configuration.py
-src/data_processing/ray/transform_runtime.py
-src/data_processing/ray/transform_statistics.py
-src/data_processing/ray/transform_table_processor.py
+src/data_processing/runtime/__init__.py
+src/data_processing/runtime/execution_configuration.py
+src/data_processing/runtime/runtime_configuration.py
+src/data_processing/runtime/transform_launcher.py
+src/data_processing/runtime/transform_table_processor.py
+src/data_processing/runtime/pure_python/__init__.py
+src/data_processing/runtime/pure_python/runtime_configuration.py
+src/data_processing/runtime/pure_python/transform_launcher.py
+src/data_processing/runtime/pure_python/transform_orchestrator.py
+src/data_processing/runtime/pure_python/transform_table_processor.py
+src/data_processing/runtime/ray/__init__.py
+src/data_processing/runtime/ray/execution_configuration.py
+src/data_processing/runtime/ray/ray_utils.py
+src/data_processing/runtime/ray/runtime_configuration.py
+src/data_processing/runtime/ray/transform_launcher.py
+src/data_processing/runtime/ray/transform_orchestrator.py
+src/data_processing/runtime/ray/transform_runtime.py
+src/data_processing/runtime/ray/transform_statistics.py
+src/data_processing/runtime/ray/transform_table_processor.py
 src/data_processing/test_support/__init__.py
 src/data_processing/test_support/abstract_test.py
 src/data_processing/test_support/data_access/__init__.py
 src/data_processing/test_support/data_access/data_access_factory_test.py
-src/data_processing/test_support/ray/__init__.py
-src/data_processing/test_support/ray/transform_test.py
+src/data_processing/test_support/launch/__init__.py
+src/data_processing/test_support/launch/transform_test.py
 src/data_processing/test_support/transform/__init__.py
 src/data_processing/test_support/transform/noop_transform.py
 src/data_processing/test_support/transform/transform_test.py
 src/data_processing/transform/__init__.py
-src/data_processing/transform/execution_configuration.py
-src/data_processing/transform/launcher_configuration.py
 src/data_processing/transform/table_transform.py
+src/data_processing/transform/transform_configuration.py
 src/data_processing/transform/transform_statistics.py
 src/data_processing/utils/__init__.py
 src/data_processing/utils/cli_utils.py
 src/data_processing/utils/config.py
 src/data_processing/utils/log.py
 src/data_processing/utils/params_utils.py
 src/data_processing/utils/transform_utils.py
@@ -75,13 +84,16 @@
 test-data/data_processing/ray/noop/expected/subdir/test1.parquet
 test-data/data_processing/ray/noop/input/sample1.parquet
 test-data/data_processing/ray/noop/input/subdir/test1.parquet
 test/data_processing_tests/data_access/daf_local_test.py
 test/data_processing_tests/data_access/data_access_local_test.py
 test/data_processing_tests/data_access/data_access_s3_test.py
 test/data_processing_tests/data_access/sample_input_data_test.py
-test/data_processing_tests/pure_python/launcher_test.py
-test/data_processing_tests/ray/launcher_test.py
-test/data_processing_tests/ray/ray_util_test.py
-test/data_processing_tests/ray/test_noop_launch.py
+test/data_processing_tests/launch/pure_python/launcher_test.py
+test/data_processing_tests/launch/pure_python/multi_launcher_test.py
+test/data_processing_tests/launch/pure_python/test_noop_launch.py
+test/data_processing_tests/launch/ray/launcher_test.py
+test/data_processing_tests/launch/ray/multi_launcher_test.py
+test/data_processing_tests/launch/ray/ray_util_test.py
+test/data_processing_tests/launch/ray/test_noop_launch.py
 test/data_processing_tests/transform/test_noop.py
 test/data_processing_tests/util/transform_utils_test.py
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/arrow_s3.py` & `data_prep_toolkit-0.1.0/src/data_processing/data_access/arrow_s3.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # limitations under the License.
 ################################################################################
 
 from typing import Any
 
 import boto3
 import pyarrow as pa
-import pyarrow.parquet as pq
 from botocore.config import Config
-from data_processing.utils import get_logger
+from data_processing.utils import TransformUtils, get_logger
 
 
 logger = get_logger(__name__)
 
 
 class ArrowS3:
     """
@@ -154,39 +153,28 @@
         :param schema: Schema used for reading table, default None
         :return: table or None if the read failed
         """
         # Read file as bytes
         data = self.read_file(key)
         if data is None:
             return None
-        try:
-            # convert bytes to arrow table.
-            reader = pa.BufferReader(data)
-            table = pq.read_table(reader, schema=schema)
-            return table
-        except Exception as e:
-            logger.error(f"Failed to convert file {key} to arrow table, exception {e}. Skipping it")
-            return None
+        return TransformUtils.convert_binary_to_arrow(data=data, schema=schema)
 
     def save_table(self, key: str, table: pa.Table) -> tuple[int, dict[str, Any]]:
         """
         Save an arrow table to a file with a name
         :param key: complete path
         :param table: table to save
         :return: table size and a dictionary as
         defined https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/client/put_object.html
         in the case of failure len is -1 and dict is None
         """
-        try:
-            # convert table to bytes
-            writer = pa.BufferOutputStream()
-            pq.write_table(table=table, where=writer)
-            data = bytes(writer.getvalue())
-        except Exception as e:
-            logger.error(f"Failed to convert arrow table to byte array for key {key}, exception {e}. Skipping it")
+        # convert to bytes
+        data = TransformUtils.convert_arrow_to_binary(table=table)
+        if data is None:
             return -1, None
         # save bytes
         return len(data), self.save_file(key, data)
 
     def delete_file(self, key: str) -> None:
         """
         Delete file from S3
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access.py` & `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access_factory.py` & `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_factory.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access_factory_base.py` & `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_factory_base.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access_local.py` & `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_local.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/data_access/data_access_s3.py` & `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/pure_python/transform_launcher.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_launcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,64 +10,63 @@
 # limitations under the License.
 ################################################################################
 
 import argparse
 import time
 
 from data_processing.data_access import DataAccessFactory, DataAccessFactoryBase
-from data_processing.pure_python import orchestrate
-from data_processing.transform import (
-    TransformExecutionConfiguration,
+from data_processing.runtime import TransformExecutionConfiguration
+from data_processing.runtime.pure_python import (
+    PythonTransformRuntimeConfiguration,
+    orchestrate,
 )
-from data_processing.pure_python import PythonLauncherConfiguration
+from data_processing.runtime.transform_launcher import AbstractTransformLauncher
 from data_processing.utils import get_logger
 
 
 logger = get_logger(__name__)
 
 
-class PythonTransformLauncher:
+class PythonTransformLauncher(AbstractTransformLauncher):
     """
     Driver class starting Filter execution
     """
 
     def __init__(
         self,
-        transform_runtime_config: PythonLauncherConfiguration,
+        runtime_config: PythonTransformRuntimeConfiguration,
         data_access_factory: DataAccessFactoryBase = DataAccessFactory(),
     ):
         """
         Creates driver
-        :param transform_runtime_config: transform runtime factory
+        :param runtime_config: transform runtime factory
         :param data_access_factory: the factory to create DataAccess instances.
         """
-        self.name = transform_runtime_config.get_name()
-        self.transform_runtime_config = transform_runtime_config
-        self.data_access_factory = data_access_factory
-        self.execution_config = TransformExecutionConfiguration(name=transform_runtime_config.get_name())
+        super().__init__(runtime_config, data_access_factory)
+        self.execution_config = TransformExecutionConfiguration(name=runtime_config.get_name())
 
     def __get_parameters(self) -> bool:
         """
         This method creates arg parser, fill it with the parameters
         and does parameters validation
         :return: True id validation passe or False, if not
         """
         parser = argparse.ArgumentParser(
             description=f"Driver for {self.name} processing",
             # RawText is used to allow better formatting of ast-based arguments
             # See uses of ParamsUtils.dict_to_str()
             formatter_class=argparse.RawTextHelpFormatter,
         )
         # add additional arguments
-        self.transform_runtime_config.add_input_params(parser=parser)
+        self.runtime_config.add_input_params(parser=parser)
         self.data_access_factory.add_input_params(parser=parser)
         self.execution_config.add_input_params(parser=parser)
         args = parser.parse_args()
         return (
-            self.transform_runtime_config.apply_input_params(args=args)
+            self.runtime_config.apply_input_params(args=args)
             and self.execution_config.apply_input_params(args=args)
             and self.data_access_factory.apply_input_params(args=args)
         )
 
     def _submit_for_execution(self) -> int:
         """
         Submit for execution
@@ -75,15 +74,15 @@
         """
         res = 1
         start = time.time()
         try:
             logger.debug("Starting orchestrator")
             res = orchestrate(
                 data_access_factory=self.data_access_factory,
-                transform_config=self.transform_runtime_config,
+                runtime_config=self.runtime_config,
                 execution_config=self.execution_config,
             )
             logger.debug("Completed orchestrator")
         except Exception as e:
             logger.info(f"Exception running orchestration\n{e}")
         finally:
             logger.info(f"Completed execution in {(time.time() - start)/60.} min, execution result {res}")
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/pure_python/transform_orchestrator.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_orchestrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,39 +11,40 @@
 ################################################################################
 
 import time
 import traceback
 from datetime import datetime
 
 from data_processing.data_access import DataAccessFactoryBase
-from data_processing.pure_python import TransformTableProcessor
-from data_processing.transform import (
+from data_processing.runtime import (
     TransformExecutionConfiguration,
-    TransformStatistics,
+    TransformRuntimeConfiguration,
 )
-from data_processing.pure_python import PythonLauncherConfiguration
+from data_processing.runtime.pure_python import TransformTableProcessor
+from data_processing.transform import TransformStatistics
 from data_processing.utils import get_logger
 
 
 logger = get_logger(__name__)
 
 
 def orchestrate(
     data_access_factory: DataAccessFactoryBase,
-    transform_config: PythonLauncherConfiguration,
+    runtime_config: TransformRuntimeConfiguration,
     execution_config: TransformExecutionConfiguration,
 ) -> int:
     """
     orchestrator for transformer execution
     :param data_access_factory: data access factory
-    :param transform_config: transformer configuration
+    :param runtime_config: transformer configuration
+    :param execution_config: execution configuration
     :return: 0 - success or 1 - failure
     """
     start_ts = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-    logger.info(f"orchestrator {transform_config.get_name()} started at {start_ts}")
+    logger.info(f"orchestrator {runtime_config.get_name()} started at {start_ts}")
     try:
         # create data access
         data_access = data_access_factory.create_data_access()
         if data_access is None:
             logger.error("No DataAccess instance provided - exiting")
             return 1
         # Get files to process
@@ -56,18 +57,18 @@
         print_interval = int(len(files) / 100)
         if print_interval == 0:
             print_interval = 1
         # create statistics
         statistics = TransformStatistics()
         # create executor
         executor = TransformTableProcessor(
-            data_access_factory=data_access_factory, statistics=statistics, params=transform_config
+            data_access_factory=data_access_factory, statistics=statistics, params=runtime_config
         )
         # process data
-        logger.debug(f"{transform_config.get_name()} Begin processing files")
+        logger.debug(f"{runtime_config.get_name()} Begin processing files")
         t_start = time.time()
         completed = 0
         for path in files:
             executor.process_data(path)
             completed += 1
             if completed % print_interval == 0:
                 logger.info(f"Completed {completed} files in {(time.time() - t_start)/60} min")
@@ -77,15 +78,15 @@
         executor.flush()
         logger.info(f"done flushing in {time.time() - start} sec")
         # Compute execution statistics
         logger.debug("Computing execution stats")
         stats = statistics.get_execution_stats()
         # build and save metadata
         logger.debug("Building job metadata")
-        input_params = transform_config.get_transform_metadata()
+        input_params = runtime_config.get_transform_metadata()
         metadata = {
             "pipeline": execution_config.pipeline_id,
             "job details": execution_config.job_details
             | {
                 "start_time": start_ts,
                 "end_time": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                 "status": "success",
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/pure_python/transform_table_processor.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/transform_table_processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,180 +11,166 @@
 ################################################################################
 
 import time
 import traceback
 from typing import Any
 
 import pyarrow as pa
-from data_processing.data_access import DataAccessFactoryBase
-from data_processing.transform import TransformStatistics
 from data_processing.utils import TransformUtils, get_logger
-from data_processing.pure_python import PythonLauncherConfiguration
 
-logger = get_logger(__name__)
 
-
-class TransformTableProcessor:
+class AbstractTransformTableProcessor:
     """
-    This is the class implementing the worker class processing of a single pyarrow file
+    This is the the base class implementing processing of a single pyarrow file
     """
 
-    def __init__(
-        self,
-        data_access_factory: DataAccessFactoryBase,
-        statistics: TransformStatistics,
-        params: PythonLauncherConfiguration,
-    ):
+    def __init__(self):
         """
         Init method
-        :param data_access_factory - data access factory
-        :param statistics - reference to statistics class
-        :param params: transform configuration class
-        """
-        # Create data access
-        self.data_access = data_access_factory.create_data_access()
-        # Add data access and statistics to the processor parameters
-        transform_params = dict(params.get_transform_params())
-        transform_params["data_access"] = self.data_access
-        transform_params["statistics"] = statistics
-        # Create local processor
-        self.transform = params.get_transform_class()(transform_params)
-        # Create statistics
-        self.stats = statistics
-        self.last_fname = None
-        self.last_fname_next_index = None
+        """
+        self.data_access = None
+        self.transform = None
+        self.stats = None
+        self.last_file_name = None
+        self.last_file_name_next_index = None
+        self.logger = get_logger(__name__)
 
     def process_data(self, f_name: str) -> None:
         """
-        Method processing an individual file
+        Method processing an individual table
         :param f_name: file name
         :return: None
         """
-        logger.debug(f"Begin processing file {f_name}")
+        self.logger.debug(f"Begin processing file {f_name}")
         if self.data_access is None:
-            logger.warning("No data_access found. Returning.")
+            self.logger.warning("No data_access found. Returning.")
             return
         t_start = time.time()
         # Read source table
         table = self.data_access.get_table(path=f_name)
         if table is None:
-            logger.warning("File read resulted in None. Returning.")
-            self.stats.add_stats({"failed_reads": 1})
+            self.logger.warning("File read resulted in None. Returning.")
+            self._publish_stats({"failed_reads": 1})
             return
-        self.stats.add_stats({"source_files": 1, "source_size": table.nbytes})
+        self._publish_stats({"source_files": 1, "source_size": table.nbytes})
         # Process input table
         try:
             if table.num_rows > 0:
                 # execute local processing
-                logger.debug(f"Begin transforming table from {f_name}")
+                self.logger.debug(f"Begin transforming table from {f_name}")
                 out_tables, stats = self.transform.transform(table=table)
-                logger.debug(f"Done transforming table from {f_name}")
+                self.logger.debug(f"Done transforming table from {f_name}")
+                self.last_file_name = TransformUtils.get_file_extension(f_name)[0]
+                self.last_file_name_next_index = None
             else:
-                logger.info(f"table: {f_name} is empty, skipping processing")
-                self.stats.add_stats({"skipped empty tables": 1})
+                self.logger.info(f"table: {f_name} is empty, skipping processing")
+                self._publish_stats({"skipped empty tables": 1})
                 return
             # save results
-            self._submit_table(f_name=f_name, t_start=t_start, out_tables=out_tables, stats=stats)
+            self._submit_table(t_start=t_start, out_tables=out_tables, stats=stats)
         except Exception as e:
-            logger.warning(f"Exception {e} processing file {f_name}: {traceback.format_exc()}")
-            self.stats.add_stats({"transform execution exception": 1})
+            self.logger.warning(f"Exception {e} processing file {f_name}: {traceback.format_exc()}")
+            self._publish_stats({"transform execution exception": 1})
 
     def flush(self) -> None:
         """
         This is supporting method for transformers, that implement buffering of tables, for example coalesce.
         These transformers can have buffers containing tables that were not written to the output. Flush is
         the hook for them to return back locally stored tables and their statistics.
         :return: None
         """
         t_start = time.time()
-        if self.last_fname is None:
+        if self.last_file_name is None:
             # for some reason a given worker never processed anything. Happens in testing
             # when the amount of workers is greater then the amount of files
-            logger.debug("skipping flush, no name for file is defined")
+            self.logger.debug("skipping flush, no name for file is defined")
             return
         try:
             # get flush results
-            logger.debug(f"Begin flushing transform")
+            self.logger.debug(f"Begin flushing transform")
             out_tables, stats = self.transform.flush()
-            logger.debug(f"Done flushing transform, got {len(out_tables)} tables")
-            # Here we are using the name of the last table, that did not return anything
-            output_file_name = self.last_fname.removesuffix(".parquet")
-            if self.last_fname_next_index is None:
-                # The filename was NOT used to write out a file yet.
-                # This happens when _submit() is called with a filename, but with no tables.
-                # In this case, we can use the filename w/o an index.
-                output_file_name = f"{output_file_name}.parquet"
-            else:
-                # The filename was used to write out a file, so we need to include an index.
-                output_file_name = f"{output_file_name}_{self.last_fname_next_index}.parquet"
-            self._submit_table(f_name=output_file_name, t_start=t_start, out_tables=out_tables, stats=stats)
+            self.logger.debug(f"Done flushing transform, got {len(out_tables)} tables")
+            # Here we are using the name of the last table, that we were processing
+            self._submit_table(t_start=t_start, out_tables=out_tables, stats=stats)
         except Exception as e:
-            logger.warning(f"Exception {e} flushing: {traceback.format_exc()}")
-            self.stats.add_stats({"transform execution exception": 1})
+            self.logger.warning(f"Exception {e} flushing: {traceback.format_exc()}")
+            self._publish_stats({"transform execution exception": 1})
 
-    def _submit_table(self, f_name: str, t_start: float, out_tables: list[pa.Table], stats: dict[str, Any]) -> None:
+    def _submit_table(self, t_start: float, out_tables: list[pa.Table], stats: dict[str, Any]) -> None:
         """
         This is a helper method writing output tables and statistics
-        :param f_name: input file n
         :param t_start: execution start time
         :param out_tables: list of tables to write
         :param stats: execution statistics to populate
         :return: None
         """
-        logger.debug(f"submitting tables under file named {f_name}, number of tables {len(out_tables)}")
+        self.logger.debug(
+            f"submitting tables under file named {self.last_file_name}.parquet, " f"number of tables {len(out_tables)}"
+        )
         # Compute output file location. Preserve sub folders for Wisdom
-        self.last_fname = f_name
-        self.last_fname_next_index = None
         match len(out_tables):
             case 0:
                 # no tables - save input file name for flushing
-                logger.debug(f"Transform did not produce a transformed table for file {f_name}")
+                self.logger.debug(
+                    f"Transform did not produce a transformed table for " f"file {self.last_file_name}.parquet"
+                )
             case 1:
                 # we have exactly 1 table
-                output_name = self.data_access.get_output_location(path=f_name)
-                logger.debug(f"Writing transformed file {f_name} to {output_name}")
+                output_name = self.data_access.get_output_location(path=f"{self.last_file_name}.parquet")
+                self.logger.debug(f"Writing transformed file {self.last_file_name}.parquet to {output_name}")
                 if TransformUtils.verify_no_duplicate_columns(table=out_tables[0], file=output_name):
                     output_file_size, save_res = self.data_access.save_table(path=output_name, table=out_tables[0])
                     if save_res is not None:
                         # Store execution statistics. Doing this async
-                        self.stats.add_stats(
+                        self._publish_stats(
                             {
                                 "result_files": 1,
                                 "result_size": out_tables[0].nbytes,
                                 "table_processing": time.time() - t_start,
                             }
                         )
                     else:
-                        logger.warning(f"Failed to write file {output_name}")
-                        self.stats.add_stats({"failed_writes": 1})
-                self.last_fname_next_index = 1
+                        self.logger.warning(f"Failed to write file {output_name}")
+                        self._publish_stats({"failed_writes": 1})
+                self.last_file_name_next_index = 0
             case _:
                 # we have more then 1 table
                 table_sizes = 0
-                output_name = self.data_access.get_output_location(path=f_name)
-                output_file_name = output_name.removesuffix(".parquet")
+                output_file_name = self.data_access.get_output_location(path=self.last_file_name)
+                start_index = self.last_file_name_next_index
+                if start_index is None:
+                    start_index = 0
                 count = len(out_tables)
                 for index in range(count):
-                    if TransformUtils.verify_no_duplicate_columns(table=out_tables[index], file=output_name):
-                        output_name_indexed = f"{output_file_name}_{index}.parquet"
+                    output_name_indexed = f"{output_file_name}_{start_index + index}.parquet"
+                    if TransformUtils.verify_no_duplicate_columns(table=out_tables[index], file=output_name_indexed):
                         table_sizes += out_tables[index].nbytes
-                        logger.debug(
-                            f"Writing transformed file {f_name}, {index + 1} of {count}  to {output_name_indexed}"
+                        self.logger.debug(
+                            f"Writing transformed file {self.last_file_name}.parquet, {index + 1} "
+                            f"of {count}  to {output_name_indexed}"
                         )
                         output_file_size, save_res = self.data_access.save_table(
                             path=output_name_indexed, table=out_tables[index]
                         )
                         if save_res is None:
-                            logger.warning(f"Failed to write file {output_name_indexed}")
-                            self.stats.add_stats({"failed_writes": 1})
+                            self.logger.warning(f"Failed to write file {output_name_indexed}")
+                            self._publish_stats({"failed_writes": 1})
                             break
-                self.last_fname_next_index = count
-                self.stats.add_stats(
+                self.last_file_name_next_index = start_index + count
+                self._publish_stats(
                     {
                         "result_files": len(out_tables),
                         "result_size": table_sizes,
                         "table_processing": time.time() - t_start,
                     }
                 )
         # save transformer's statistics
         if len(stats) > 0:
-            self.stats.add_stats(stats)
+            self._publish_stats(stats)
+
+    def _publish_stats(self, stats: dict[str, Any]) -> None:
+        """
+        Publishing execution statistics
+        :param stats: Statistics
+        :return: None
+        """
+        raise ValueError("must be implemented by subclass")
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/__init__.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from data_processing.ray.ray_utils import RayUtils
-from data_processing.ray.transform_statistics import TransformStatisticsRay
-from data_processing.ray.transform_table_processor import TransformTableProcessorRay
-from data_processing.ray.transform_runtime import (
-    RayLauncherConfiguration,
-    DefaultTableTransformRuntimeRay,
-)
-from data_processing.ray.transform_orchestrator_configuration import TransformOrchestratorConfiguration
-from data_processing.ray.transform_orchestrator import orchestrate
-from data_processing.ray.transform_launcher import RayTransformLauncher
+from data_processing.runtime.ray.ray_utils import RayUtils
+from data_processing.runtime.ray.transform_statistics import TransformStatisticsRay
+from data_processing.runtime.ray.transform_runtime import DefaultTableTransformRuntimeRay
+from data_processing.runtime.ray.runtime_configuration import RayTransformRuntimeConfiguration
+from data_processing.runtime.ray.transform_table_processor import TransformTableProcessorRay
+from data_processing.runtime.ray.execution_configuration import RayTransformExecutionConfiguration
+from data_processing.runtime.ray.transform_orchestrator import orchestrate
+from data_processing.runtime.ray.transform_launcher import RayTransformLauncher
+from data_processing.runtime.runtime_configuration import TransformRuntimeConfiguration
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/ray_utils.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/ray_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_launcher.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_launcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,45 +12,42 @@
 
 import argparse
 import sys
 import time
 
 import ray
 from data_processing.data_access import DataAccessFactory, DataAccessFactoryBase
-from data_processing.ray import (
-    RayLauncherConfiguration,
-    TransformOrchestratorConfiguration,
-    orchestrate,
+from data_processing.runtime.ray import RayTransformExecutionConfiguration, orchestrate
+from data_processing.runtime.ray.runtime_configuration import (
+    RayTransformRuntimeConfiguration,
 )
+from data_processing.runtime.transform_launcher import AbstractTransformLauncher
 from data_processing.utils import get_logger, str2bool
 
 
 logger = get_logger(__name__)
 
 
-class RayTransformLauncher:
+class RayTransformLauncher(AbstractTransformLauncher):
     """
     Driver class starting Filter execution
     """
 
     def __init__(
-            self,
-            transform_runtime_config: RayLauncherConfiguration,
-            data_access_factory: DataAccessFactoryBase = DataAccessFactory(),
+        self,
+        runtime_config: RayTransformRuntimeConfiguration,
+        data_access_factory: DataAccessFactoryBase = DataAccessFactory(),
     ):
         """
         Creates driver
-        :param transform_runtime_config: transform runtime factory
+        :param runtime_config: transform runtime factory
         :param data_access_factory: the factory to create DataAccess instances.
         """
-        self.run_locally = False
-        self.name = transform_runtime_config.get_name()
-        self.transform_runtime_config = transform_runtime_config
-        self.data_access_factory = data_access_factory
-        self.ray_orchestrator = TransformOrchestratorConfiguration(name=self.name)
+        super().__init__(runtime_config, data_access_factory)
+        self.execution_config = RayTransformExecutionConfiguration(name=self.name)
 
     def __get_parameters(self) -> bool:
         """
         This method creates arg parser, fill it with the parameters
         and does parameters validation
         :return: True id validation passe or False, if not
         """
@@ -60,30 +57,27 @@
             # See uses of ParamsUtils.dict_to_str()
             formatter_class=argparse.RawTextHelpFormatter,
         )
         parser.add_argument(
             "--run_locally", type=lambda x: bool(str2bool(x)), default=False, help="running ray local flag"
         )
         # add additional arguments
-        self.transform_runtime_config.add_input_params(parser=parser)
+        self.runtime_config.add_input_params(parser=parser)
         self.data_access_factory.add_input_params(parser=parser)
-        self.ray_orchestrator.add_input_params(parser=parser)
-        try:
-            args = parser.parse_args()
-        except SystemExit:
-            return False
+        self.execution_config.add_input_params(parser=parser)
+        args = parser.parse_args()
         self.run_locally = args.run_locally
         if self.run_locally:
             logger.info("Running locally")
         else:
             logger.info("connecting to existing cluster")
         return (
-                self.transform_runtime_config.apply_input_params(args=args)
-                and self.data_access_factory.apply_input_params(args=args)
-                and self.ray_orchestrator.apply_input_params(args=args)
+            self.runtime_config.apply_input_params(args=args)
+            and self.data_access_factory.apply_input_params(args=args)
+            and self.execution_config.apply_input_params(args=args)
         )
 
     def _submit_for_execution(self) -> int:
         """
         Submit for Ray execution
         :return:
         """
@@ -97,17 +91,17 @@
             else:
                 # connect to the existing cluster
                 logger.info("Connecting to the existing Ray cluster")
                 ray.init(f"ray://localhost:10001", ignore_reinit_error=True)
             logger.debug("Starting orchestrator")
             res = ray.get(
                 orchestrate.remote(
-                    preprocessing_params=self.ray_orchestrator,
+                    preprocessing_params=self.execution_config,
                     data_access_factory=self.data_access_factory,
-                    transform_runtime_config=self.transform_runtime_config,
+                    runtime_config=self.runtime_config,
                 )
             )
             logger.debug("Completed orchestrator")
             time.sleep(10)
         except Exception as e:
             logger.info(f"Exception running ray remote orchestration\n{e}")
         finally:
@@ -116,18 +110,15 @@
             return res
 
     def launch(self) -> int:
         """
         Execute method orchestrates driver invocation
         :return: launch result
         """
-        print("testing execution11")
         if self.__get_parameters():
             res = self._submit_for_execution()
         else:
             res = 1
-        print(f"hmmm {self.run_locally} {res}")
         if not self.run_locally and res > 0:
-            print("hehe")
             # if we are running in kfp exit to signal kfp that we failed
             sys.exit(1)
         return res
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_orchestrator.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_orchestrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,40 +12,40 @@
 
 import time
 import traceback
 from datetime import datetime
 
 import ray
 from data_processing.data_access import DataAccessFactoryBase
-from data_processing.ray import (
+from data_processing.runtime.ray import (
+    RayTransformExecutionConfiguration,
+    RayTransformRuntimeConfiguration,
     RayUtils,
-    RayLauncherConfiguration,
-    TransformOrchestratorConfiguration,
     TransformStatisticsRay,
     TransformTableProcessorRay,
 )
 from data_processing.utils import get_logger
 from ray.util import ActorPool
 from ray.util.metrics import Gauge
 
 
 logger = get_logger(__name__)
 
 
 @ray.remote(num_cpus=1, scheduling_strategy="SPREAD")
 def orchestrate(
-    preprocessing_params: TransformOrchestratorConfiguration,
+    preprocessing_params: RayTransformExecutionConfiguration,
     data_access_factory: DataAccessFactoryBase,
-    transform_runtime_config: RayLauncherConfiguration,
+    runtime_config: RayTransformRuntimeConfiguration,
 ) -> int:
     """
     orchestrator for transformer execution
     :param preprocessing_params: orchestrator configuration
     :param data_access_factory: data access factory
-    :param transform_runtime_config: transformer runtime configuration
+    :param runtime_config: transformer runtime configuration
     :return: 0 - success or 1 - failure
     """
     start_ts = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     logger.info(f"orchestrator started at {start_ts}")
     try:
         # create data access
         data_access = data_access_factory.create_data_access()
@@ -66,21 +66,21 @@
         resources = RayUtils.get_cluster_resources()
         logger.info(f"Cluster resources: {resources}")
         # print execution params
         logger.info(
             f"Number of workers - {preprocessing_params.n_workers} " f"with {preprocessing_params.worker_options} each"
         )
         # create transformer runtime
-        runtime = transform_runtime_config.create_transform_runtime()
+        runtime = runtime_config.create_transform_runtime()
         # create statistics
         statistics = TransformStatisticsRay.remote({})
         # create executors
         processor_params = {
             "data_access_factory": data_access_factory,
-            "transform_class": transform_runtime_config.get_transform_class(),
+            "transform_class": runtime_config.get_transform_class(),
             "transform_params": runtime.get_transform_config(
                 data_access_factory=data_access_factory, statistics=statistics, files=files
             ),
             "statistics": statistics,
         }
         logger.debug("Creating actors")
         processors = RayUtils.create_actors(
@@ -124,15 +124,15 @@
         # build and save metadata
         logger.debug("Building job metadata")
         metadata = {
             "pipeline": preprocessing_params.pipeline_id,
             "job details": preprocessing_params.job_details
             | {"start_time": start_ts, "end_time": datetime.now().strftime("%Y-%m-%d %H:%M:%S"), "status": "success"},
             "code": preprocessing_params.code_location,
-            "job_input_params": transform_runtime_config.get_transform_metadata()
+            "job_input_params": runtime_config.get_transform_metadata()
             | data_access_factory.get_input_params()
             | preprocessing_params.get_input_params(),
             "execution_stats": resources,
             "job_output_stats": stats,
         }
         logger.debug(f"Saved job metadata: {metadata}.")
         data_access.save_job_metadata(metadata)
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_orchestrator_configuration.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/execution_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 # limitations under the License.
 ################################################################################
 
 import argparse
 import ast
 from typing import Any
 
-from data_processing.transform import TransformExecutionConfiguration
+from data_processing.runtime import TransformExecutionConfiguration
 from data_processing.utils import CLIArgumentProvider, ParamsUtils, get_logger
 
 
 logger = get_logger(__name__)
 
 
 cli_prefix = "runtime_"
 
 
-class TransformOrchestratorConfiguration(TransformExecutionConfiguration):
+class RayTransformExecutionConfiguration(TransformExecutionConfiguration):
     """
     A class specifying and validating Ray orchestrator configuration
     """
 
     def __init__(self, name: str):
         """
         Initialization
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_runtime.py` & `data_prep_toolkit-0.1.0/src/data_processing/transform/transform_configuration.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,100 +6,99 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
+from argparse import ArgumentParser
 from typing import Any
 
-from data_processing.data_access import DataAccessFactoryBase
-from data_processing.transform import (
-    AbstractTableTransform,
-    LauncherConfiguration,
-)
-from data_processing.pure_python import PythonLauncherConfiguration
-from ray.actor import ActorHandle
+from data_processing.transform import AbstractTableTransform
+from data_processing.utils import CLIArgumentProvider
 
 
-class DefaultTableTransformRuntimeRay:
+class TransformConfiguration(CLIArgumentProvider):
     """
-    Transformer runtime used by processor to to create Transform specific environment
+    This is a base transform configuration class defining transform's input/output parameter
     """
 
-    def __init__(self, params: dict[str, Any]):
+    def __init__(self, name: str, transform_class: type[AbstractTableTransform], remove_from_metadata: list[str] = []):
         """
-        Create/config this runtime.
-        :param params: parameters, often provided by the CLI arguments as defined by a TableTansformConfiguration.
-        """
-        self.params = params
-
-    def get_transform_config(
-        self, data_access_factory: DataAccessFactoryBase, statistics: ActorHandle, files: list[str]
-    ) -> dict[str, Any]:
-        """
-        Get the dictionary of configuration that will be provided to the transform's initializer.
-        This is the opportunity for this runtime to create a new set of configuration based on the
-        config/params provided to this instance's initializer.  This may include the addition
-        of new configuration data such as ray shared memory, new actors, etc, that might be needed and
-        expected by the transform in its initializer and/or transform() methods.
-        :param data_access_factory - data access factory class being used by the RayOrchestrator.
-        :param statistics - reference to statistics actor
-        :param files - list of files to process
-        :return: dictionary of transform init params
-        """
-        return self.params
+        Initialization
+        :param name: transformer name
+        :param transform_class: transform implementation class
+        :param remove_from_metadata - list of parameters to remove from metadata
+        """
+        self.name = name
+        self.transform_class = transform_class
+        self.remove_from_metadata = remove_from_metadata
+        self.params = {}
+
+    def get_transform_class(self) -> type[AbstractTableTransform]:
+        """
+        Get the class extending AbstractTableTransform which implements a specific transformation.
+        The class will generally be instantiated with a dictionary of configuration produced by
+        the associated TransformRuntime get_transform_config() method.
+        :return: class extending AbstractTableTransform
+        """
+        return self.transform_class
+
+    def get_name(self):
+        return self.name
+
+    def get_transform_metadata(self) -> dict[str, Any]:
+        """
+        Get transform metadata. Before returning remove all parameters key accumulated in
+        self.remove_from metadata. This allows transform developer to mark any input parameters
+        that should not make it to the metadata. This can be parameters containing sensitive
+        information, access keys, secrets, passwords, etc
+        :return parameters for metadata:
+        """
+        # get input parameters
+        parameters = self.get_input_params()
+        # remove everything that user marked as to be removed
+        for key in self.remove_from_metadata:
+            del self.params[key]
+        return parameters
 
-    def compute_execution_stats(self, stats: dict[str, Any]) -> dict[str, Any]:
+    def get_transform_params(self) -> dict[str, Any]:
         """
-        Update/augment the given stats object with runtime-specific additions/modifications.
-        :param stats: output of statistics as aggregated across all calls to all transforms.
-        :return: job execution statistics.  These are generally reported as metadata by the Ray Orchestrator.
+         Get transform parameters
+        :return: transform parameters
         """
-        return stats
+        return self.params
 
 
-class RayLauncherConfiguration(PythonLauncherConfiguration):
+def get_transform_config(
+    transform_configuration: TransformConfiguration, argv: list[str], parser: ArgumentParser = None
+):
     """
-    Provides support the configuration of a transformer running in the ray environment.
-    It holds the following:
-        1) The type of the concrete AbstractTransform class, that is created by a the ray worker with a
-            dictionary of parameters to perform that table transformations.
-        2) The type of the of DefaultTableTransformRuntime that supports operation of the transform
-            on the ray orchestrator side.  It is create with an initializer that takes the dictionary
-            of CLI arguments, optionally defined in this class.
-    Sub-classes may extend this class to override the following:
-        1) add_input_params() to add CLI argument definitions used in creating both the AbstractTransform
-            and the DefaultTableTransformRuntime.
+    Create a transform configuration dictionary  using the given Configuration class and dictionary of
+    values that should be treated as command line options.
+    Example:
+
+        config = self._get_transform_config(YourTransformConfiguration(), ...)\n
+        transform = YourTransform(config)   \n
+
+    :param transform_configuration: The configuration class used to define and apply input parameters.
+        and the values are the command line values.
+    :param parser: optional parser to use.  If not provided one is created internally.  if provided and argv
+        contains args that will be parsed by the parser, then they will be in the returned dictionary.
+    :param argv: list of parameters string
+    :return:  the configuration dictionary as produced by the given transform configuration after all args
+        have been defined and applied.
     """
-
-    def __init__(
-        self,
-        name: str,
-        transform_class: type[AbstractTableTransform],
-        launcher_configuration: LauncherConfiguration,
-        remove_from_metadata: list[str] = [],
-        runtime_class: type[DefaultTableTransformRuntimeRay] = DefaultTableTransformRuntimeRay,
-    ):
-        super().__init__(
-            name=name,
-            transform_class=transform_class,
-            launcher_configuration=launcher_configuration,
-            remove_from_metadata=remove_from_metadata,
-        )
-        """
-        Initialization
-        :param transform_class: implementation of the transform
-        :param runtime_class: implementation of the transform runtime
-        :param base: base transform configuration class
-        :param name: transform name
-        :param remove_from_metadata: list of parameters to remove from metadata
-        :return:
-        """
-        self.runtime_class = runtime_class
-
-    def create_transform_runtime(self) -> DefaultTableTransformRuntimeRay:
-        """
-        Create transform runtime with the parameters captured during apply_input_params()
-        :return: transform runtime object
-        """
-        return self.runtime_class(self.params)
+    # Create and add our arguments to the parser
+    if parser is None:
+        parser = ArgumentParser()
+    transform_configuration.add_input_params(parser)
+
+    # Create the command line and parse it.
+    if "python" in argv[0]:
+        argv = argv[1:0]
+    args = parser.parse_args(argv)
+    dargs = vars(args)
+
+    transform_configuration.apply_input_params(args)
+    config = transform_configuration.get_input_params()  # This is the transform configuration, for this test.
+    return dargs | config
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/ray/transform_statistics.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_statistics.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/abstract_test.py` & `data_prep_toolkit-0.1.0/src/data_processing/test_support/abstract_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/data_access/data_access_factory_test.py` & `data_prep_toolkit-0.1.0/src/data_processing/test_support/data_access/data_access_factory_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/ray/transform_test.py` & `data_prep_toolkit-0.1.0/src/data_processing/test_support/launch/transform_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,74 +10,76 @@
 # limitations under the License.
 ################################################################################
 
 import sys
 import tempfile
 from typing import Any
 
-from data_processing.ray import RayLauncherConfiguration, RayTransformLauncher
+from data_processing.runtime.ray import RayTransformLauncher
+from data_processing.runtime.transform_launcher import AbstractTransformLauncher
 from data_processing.test_support.abstract_test import AbstractTest
 from data_processing.utils import ParamsUtils
 
 
 class AbstractTransformLauncherTest(AbstractTest):
     """
     The Ray-based test class for all/most AbstractTransform implementations.
     Generic tests are provided here, and sub-classes must implement the _get*_fixture() method(s)
     to provide the test data for a given test method.  For example,  get_test_transform_fixtures()
     provides the test data for the test_transform() test method.
 
     """
 
     @staticmethod
-    def _get_argv(cli_params: dict[str, Any], in_table_path: str, out_table_path: str):
+    def _get_argv(
+        launcher: AbstractTransformLauncher, cli_params: dict[str, Any], in_table_path: str, out_table_path: str
+    ):
         args = {} | cli_params
         local_ast = {"input_folder": in_table_path, "output_folder": out_table_path}
         args["data_local_config"] = local_ast
-        args["run_locally"] = "True"
+        if isinstance(launcher, RayTransformLauncher):
+            args["run_locally"] = "True"
         argv = ParamsUtils.dict_to_req(args)
         return argv
 
     def test_transform(
         self,
-        transform_config: RayLauncherConfiguration,
+        launcher: AbstractTransformLauncher,
         cli_params: dict[str, Any],
         in_table_path: str,
         expected_out_table_path: str,
     ):
         """
         Test the given transform and its runtime using the given CLI arguments, input directory of data files and expected output directory.
         Data is processed into a temporary output directory which is then compared with the directory of expected output.
-        :param transform_config:
+        :param launcher: launcher configured to run the transform being tested
         :param cli_params: a map of the simulated CLI arguments (w/o --).  This includes both the transform-specific CLI parameters and  the Ray launching args.
         :param in_table_path: a directory containing the input parquet files to be processed and results compared against the expected output table path.
         :param expected_out_table_path: directory contain parquet and metadata.json that is expected to match the processed input directory.
         :return:
         """
-
-        launcher = RayTransformLauncher(transform_config)
-        prefix = transform_config.get_name()
+        prefix = launcher.get_transform_name()
         with tempfile.TemporaryDirectory(prefix=prefix, dir="/tmp") as temp_dir:
             print(f"Using temporary output path {temp_dir}")
-            sys.argv = self._get_argv(cli_params, in_table_path, temp_dir)
+            sys.argv = self._get_argv(launcher, cli_params, in_table_path, temp_dir)
             launcher.launch()
             AbstractTest.validate_directory_contents(temp_dir, expected_out_table_path)
 
     def _install_test_fixtures(self, metafunc):
         # Apply the fixtures for the method with these input names (i.e. test_transform()).
         if (
-            "transform_config" in metafunc.fixturenames
+            "launcher" in metafunc.fixturenames
             and "cli_params" in metafunc.fixturenames
             and "in_table_path" in metafunc.fixturenames
             and "expected_out_table_path" in metafunc.fixturenames
         ):
             # Let the sub-class define the specific tests and test data for the transform under test.
             f = self.get_test_transform_fixtures()
             # Install the fixture, matching the parameter names used by test_transform() method.
-            metafunc.parametrize("transform_config,cli_params,in_table_path,expected_out_table_path", f)
+            metafunc.parametrize("launcher,cli_params,in_table_path,expected_out_table_path", f)
 
     def get_test_transform_fixtures(self) -> list[tuple]:
         """
         Get the test data for the test_transform() test.  The returned list contains 0 or more tuples
         containing the following:
             |  Item 0: The DefaultTableTransformConfiguration to be tested. This defines the Transform being tested and the Runtime required to run it.
             |  Item 1: The dictionary of command line args to simulate when running the transform.
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/transform/noop_transform.py` & `data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/noop_transform.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 ################################################################################
 
 import time
 from argparse import ArgumentParser, Namespace
 from typing import Any
 
 import pyarrow as pa
-from data_processing.pure_python import PythonTransformLauncher
-from data_processing.ray import RayLauncherConfiguration
-from data_processing.transform import (
-    AbstractTableTransform,
-    LauncherConfiguration,
+from data_processing.runtime.pure_python.runtime_configuration import (
+    PythonTransformRuntimeConfiguration,
 )
-from data_processing.pure_python import PythonLauncherConfiguration
+from data_processing.runtime.ray import RayTransformLauncher
+from data_processing.runtime.ray.runtime_configuration import (
+    RayTransformRuntimeConfiguration,
+)
+from data_processing.transform import AbstractTableTransform, TransformConfiguration
 from data_processing.utils import CLIArgumentProvider, get_logger
 
 
 logger = get_logger(__name__)
 
 short_name = "noop"
 cli_prefix = f"{short_name}_"
@@ -66,26 +67,29 @@
             logger.info("Sleep completed - continue")
         # Add some sample metadata.
         logger.debug(f"Transformed one table with {len(table)} rows")
         metadata = {"nfiles": 1, "nrows": len(table)}
         return [table], metadata
 
 
-class NOOPLauncherConfiguration(LauncherConfiguration):
+class NOOPTransformConfiguration(TransformConfiguration):
 
     """
     Provides support for configuring and using the associated Transform class include
     configuration with CLI args.
     """
 
     def __init__(self):
-        super().__init__()
+        super().__init__(
+            name=short_name,
+            transform_class=NOOPTransform,
+            remove_from_metadata=[pwd_key],
+        )
 
-    @staticmethod
-    def add_input_params(parser: ArgumentParser) -> None:
+    def add_input_params(self, parser: ArgumentParser) -> None:
         """
         Add Transform-specific arguments to the given  parser.
         This will be included in a dictionary used to initialize the NOOPTransform.
         By convention a common prefix should be used for all transform-specific CLI args
         (e.g, noop_, pii_, etc.)
         """
         parser.add_argument(
@@ -116,31 +120,40 @@
             return False
 
         self.params = self.params | captured
         logger.info(f"noop parameters are : {self.params}")
         return True
 
 
-class NOOPTransformConfigurationRayLauncherConfiguration(RayLauncherConfiguration):
+class NOOPPythonTransformConfiguration(PythonTransformRuntimeConfiguration):
+    """
+    Implements the PythonTransformConfiguration for NOOP as required by the PythonTransformLauncher.
+    NOOP does not use a RayRuntime class so the superclass only needs the base
+    python-only configuration.
+    """
+
     def __init__(self):
-        super().__init__(
-            name=short_name,
-            transform_class=NOOPTransform,
-            launcher_configuration=NOOPLauncherConfiguration(),
-            remove_from_metadata=[pwd_key],
-        )
+        """
+        Initialization
+        """
+        super().__init__(transform_config=NOOPTransformConfiguration())
 
 
-class NOOPPythonLauncherConfigurationPython(PythonLauncherConfiguration):
+class NOOPRayTransformConfiguration(RayTransformRuntimeConfiguration):
+    """
+    Implements the RayTransformConfiguration for NOOP as required by the RayTransformLauncher.
+    NOOP does not use a RayRuntime class so the superclass only needs the base
+    python-only configuration.
+    """
+
     def __init__(self):
-        super().__init__(
-            name=short_name,
-            transform_class=NOOPTransform,
-            launcher_configuration=NOOPLauncherConfiguration(),
-            remove_from_metadata=[pwd_key],
-        )
+        """
+        Initialization
+        """
+        super().__init__(transform_config=NOOPTransformConfiguration())
 
 
 if __name__ == "__main__":
-    launcher = PythonTransformLauncher(transform_runtime_config=NOOPPythonLauncherConfigurationPython())
+    # launcher = NOOPRayLauncher()
+    launcher = RayTransformLauncher(NOOPRayTransformConfiguration())
     logger.info("Launching noop transform")
     launcher.launch()
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/test_support/transform/transform_test.py` & `data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/execution_configuration.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/execution_configuration.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/launcher_configuration.py` & `data_prep_toolkit-0.1.0/src/data_processing/runtime/runtime_configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,57 +6,59 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
+from typing import Any
 
+from data_processing.transform import AbstractTableTransform, TransformConfiguration
 from data_processing.utils import CLIArgumentProvider
 
 
-class LauncherConfiguration(CLIArgumentProvider):
-    """
-    This is a base transform configuration class defining transform's input/output parameter
-    """
-
-    def __init__(self):
+class TransformRuntimeConfiguration(CLIArgumentProvider):
+    def __init__(self, transform_config: TransformConfiguration):
         """
         Initialization
+        :param transform_config - base configuration class
+        """
+        self.transform_config = transform_config
+
+    def add_input_params(self, parser: ArgumentParser) -> None:
+        self.transform_config.add_input_params(parser)
+
+    def apply_input_params(self, args: Namespace) -> bool:
+        return self.transform_config.apply_input_params(args)
+
+    def get_input_params(self) -> dict[str, Any]:
+        return self.transform_config.get_input_params()
+
+    def get_transform_class(self) -> type[AbstractTableTransform]:
         """
-        self.params = {}
+        Get the class extending AbstractTableTransform which implements a specific transformation.
+        The class will generally be instantiated with a dictionary of configuration produced by
+        the associated TransformRuntime get_transform_config() method.
+        :return: class extending AbstractTableTransform
+        """
+        return self.transform_config.get_transform_class()
+
+    def get_name(self):
+        return self.transform_config.get_name()
 
+    def get_transform_metadata(self) -> dict[str, Any]:
+        """
+        Get transform metadata. Before returning remove all parameters key accumulated in
+        self.remove_from metadata. This allows transform developer to mark any input parameters
+        that should not make it to the metadata. This can be parameters containing sensitive
+        information, access keys, secrets, passwords, etc
+        :return parameters for metadata:
+        """
+        return self.transform_config.get_transform_metadata()
 
-def get_transform_config(
-    transform_configuration: LauncherConfiguration, argv: list[str], parser: ArgumentParser = None
-):
-    """
-    Create a transform configuration dictionary  using the given Configuration class and dictionary of
-    values that should be treated as command line options.
-    Example:
-
-        config = self._get_transform_config(YourTransformConfiguration(), ...)\n
-        transform = YourTransform(config)   \n
-
-    :param transform_configuration: The configuration class used to define and apply input parameters.
-        and the values are the command line values.
-    :param parser: optional parser to use.  If not provided one is created internally.  if provided and argv
-        contains args that will be parsed by the parser, then they will be in the returned dictionary.
-    :param argv: list of parameters string
-    :return:  the configuration dictionary as produced by the given transform configuration after all args
-        have been defined and applied.
-    """
-    # Create and add our arguments to the parser
-    if parser is None:
-        parser = ArgumentParser()
-    transform_configuration.add_input_params(parser)
-
-    # Create the command line and parse it.
-    if "python" in argv[0]:
-        argv = argv[1:0]
-    args = parser.parse_args(argv)
-    dargs = vars(args)
-
-    transform_configuration.apply_input_params(args)
-    config = transform_configuration.get_input_params()  # This is the transform configuration, for this test.
-    return dargs | config
+    def get_transform_params(self) -> dict[str, Any]:
+        """
+         Get transform parameters
+        :return: transform parameters
+        """
+        return self.transform_config.get_transform_params()
```

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/table_transform.py` & `data_prep_toolkit-0.1.0/src/data_processing/transform/table_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/transform/transform_statistics.py` & `data_prep_toolkit-0.1.0/src/data_processing/transform/transform_statistics.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/cli_utils.py` & `data_prep_toolkit-0.1.0/src/data_processing/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/config.py` & `data_prep_toolkit-0.1.0/src/data_processing/utils/config.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/log.py` & `data_prep_toolkit-0.1.0/src/data_processing/utils/log.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/params_utils.py` & `data_prep_toolkit-0.1.0/src/data_processing/utils/params_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/src/data_processing/utils/transform_utils.py` & `data_prep_toolkit-0.1.0/src/data_processing/utils/transform_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import os
 import string
 import sys
 from typing import Any
 
 import mmh3
 import pyarrow as pa
+import pyarrow.parquet as pq
 from data_processing.utils import get_logger
 
 
 logger = get_logger(__name__)
 
 
 RANDOM_SEED = 42
@@ -92,25 +93,21 @@
             content_string = content_bytes.decode(encoding)
             return content_string
         except Exception as e:
             logger.error(f"Error -> {e}")
             return ""
 
     @staticmethod
-    def get_file_extension(file_path) -> str:
+    def get_file_extension(file_path) -> list[str]:
         """
-        Get the file extension from the given file path.
+        Get the file's root and extension from the given file path.
         :param file_path : The path of the file.
         :return: str: The file extension including the dot ('.') if present, otherwise an empty string.
         """
-        ext = os.path.splitext(file_path)[1]
-        if len(ext) > 0:
-            return ext
-        else:
-            return ""
+        return os.path.splitext(file_path)
 
     @staticmethod
     def validate_columns(table: pa.Table, required: list[str]) -> bool:
         """
         Check if required columns exist in the table
         :param table: table
         :param required: list of required columns
@@ -123,14 +120,46 @@
                 result = False
                 break
         if not result:
             logger.error(f"Not all required columns are present in the table - required {required}, present {columns}")
         return result
 
     @staticmethod
+    def convert_binary_to_arrow(data: bytes, schema: pa.schema = None) -> pa.Table:
+        """
+        Convert byte array to table
+        :param data: byte array
+        :param schema: optional Arrow table schema used for reading table, default None
+        :return: table or None if the conversion failed
+        """
+        try:
+            reader = pa.BufferReader(data)
+            table = pq.read_table(reader, schema=schema)
+            return table
+        except Exception as e:
+            logger.error(f"Failed to convert byte array to arrow table, exception {e}. Skipping it")
+            return None
+
+    @staticmethod
+    def convert_arrow_to_binary(table: pa.Table) -> bytes:
+        """
+        Convert Arrow table to byte array
+        :param table: Arrow table
+        :return: byte array or None if conversion fails
+        """
+        try:
+            # convert table to bytes
+            writer = pa.BufferOutputStream()
+            pq.write_table(table=table, where=writer)
+            return bytes(writer.getvalue())
+        except Exception as e:
+            logger.error(f"Failed to convert arrow table to byte array, exception {e}. Skipping it")
+            return None
+
+    @staticmethod
     def add_column(table: pa.Table, name: str, content: list[Any]) -> pa.Table:
         """
         Add column to the table
         :param table: original table
         :param name: column name
         :param content: content of the column
         :return: updated table, containing new column
```

### Comparing `data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/data_access/daf_local_test.py` & `data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/daf_local_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/data_access/data_access_local_test.py` & `data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/data_access_local_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/data_access/data_access_s3_test.py` & `data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/data_access_s3_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/data_access/sample_input_data_test.py` & `data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/sample_input_data_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/pure_python/launcher_test.py` & `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/launcher_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,19 +9,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 import os
 import sys
 
-from data_processing.pure_python import PythonTransformLauncher, PythonLauncherConfiguration
-from data_processing.transform import (
-    AbstractTableTransform,
-    LauncherConfiguration,
-)
+from data_processing.runtime.ray import RayTransformLauncher
+from data_processing.test_support.transform import NOOPRayTransformConfiguration
 from data_processing.utils import ParamsUtils
 
 
 """
  see: https://stackoverflow.com/questions/55259371/pytest-testing-parser-error-unrecognised-arguments
  to run test using argparse we can simply overwrite sys.argv to supply required arguments
 """
@@ -35,192 +32,158 @@
     "output_folder": "output_folder",
 }
 local_conf = {
     "input_folder": os.path.join(os.sep, "tmp", "input"),
     "output_folder": os.path.join(os.sep, "tmp", "output"),
 }
 
+worker_options = {"num_cpu": 0.8}
 code_location = {"github": "github", "commit_hash": "12345", "path": "path"}
 
 
-class TestLauncherPython(PythonTransformLauncher):
+class TestLauncherRay(RayTransformLauncher):
     """
     Test driver for validation of the functionality
     """
 
+    def __init__(self):
+        super().__init__(NOOPRayTransformConfiguration())
+
     def _submit_for_execution(self) -> int:
         """
         Overwrite this method to just print all parameters to make sure that everything works
         :return:
         """
         print("\n\nPrinting preprocessing parameters")
+        print(f"Run locally {self.run_locally}")
         return 0
 
 
 def test_launcher():
     params = {
+        "run_locally": True,
         "data_max_files": -1,
         "data_checkpointing": False,
+        "runtime_worker_options": ParamsUtils.convert_to_ast(worker_options),
+        "runtime_num_workers": 5,
         "runtime_pipeline_id": "pipeline_id",
         "runtime_job_id": "job_id",
+        "runtime_creation_delay": 0,
         "runtime_code_location": ParamsUtils.convert_to_ast(code_location),
     }
     # s3 not defined
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 0 == res
     # Add S3 configuration
     params["data_s3_config"] = ParamsUtils.convert_to_ast(s3_conf)
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 1 == res
     # Add S3 credentials
     params["data_s3_cred"] = ParamsUtils.convert_to_ast(s3_cred)
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
+
     assert 0 == res
     # Add local config, should fail because now three different configs exist
     params["data_local_config"] = ParamsUtils.convert_to_ast(local_conf)
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 1 == res
     # remove local config, should still fail, because two configs left
     del params["data_local_config"]
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 0 == res
 
 
 def test_local_config():
     # test that the driver works with local configuration
     params = {
+        "run_locally": True,
         "data_local_config": ParamsUtils.convert_to_ast(local_conf),
         "data_max_files": -1,
         "data_checkpointing": False,
+        "runtime_worker_options": ParamsUtils.convert_to_ast(worker_options),
+        "runtime_num_workers": 5,
         "runtime_pipeline_id": "pipeline_id",
         "runtime_job_id": "job_id",
+        "runtime_creation_delay": 0,
         "runtime_code_location": ParamsUtils.convert_to_ast(code_location),
     }
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 0 == res
 
 
 def test_local_config_validate():
     # test the validation of the local configuration
     params = {
+        "run_locally": True,
         "data_max_files": -1,
         "data_checkpointing": False,
+        "runtime_worker_options": ParamsUtils.convert_to_ast(worker_options),
+        "runtime_num_workers": 5,
         "runtime_pipeline_id": "pipeline_id",
         "runtime_job_id": "job_id",
+        "runtime_creation_delay": 0,
         "runtime_code_location": ParamsUtils.convert_to_ast(code_location),
     }
     # invalid local configurations, driver launch should fail with any of these
     local_conf_empty = {}
     local_conf_no_input = {"output_folder": "output_folder"}
     local_conf_no_output = {"input_folder": "input_folder"}
     params["data_local_config"] = ParamsUtils.convert_to_ast(local_conf_empty)
     sys.argv = ParamsUtils.dict_to_req(d=params)
     print(f"parameters {sys.argv}")
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 1 == res
     params["data_local_config"] = ParamsUtils.convert_to_ast(local_conf_no_input)
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 1 == res
     params["data_local_config"] = ParamsUtils.convert_to_ast(local_conf_no_output)
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 1 == res
     params["data_local_config"] = ParamsUtils.convert_to_ast(local_conf)
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 0 == res
 
 
 def test_s3_config_validate():
     # test the validation of the local configuration
     params = {
+        "run_locally": True,
         "data_max_files": -1,
         "data_checkpointing": False,
         "data_s3_cred": ParamsUtils.convert_to_ast(s3_cred),
+        "runtime_worker_options": ParamsUtils.convert_to_ast(worker_options),
+        "runtime_num_workers": 5,
         "runtime_pipeline_id": "pipeline_id",
         "runtime_job_id": "job_id",
+        "runtime_creation_delay": 0,
         "runtime_code_location": ParamsUtils.convert_to_ast(code_location),
     }
     # invalid local configurations, driver launch should fail with any of these
     s3_conf_empty = {}
     s3_conf_no_input = {"output_folder": "output_folder"}
     s3_conf_no_output = {"input_folder": "input_folder"}
     params["data_s3_config"] = ParamsUtils.convert_to_ast(s3_conf_empty)
     sys.argv = ParamsUtils.dict_to_req(d=params)
     print(f"parameters {sys.argv}")
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 1 == res
     params["data_s3_config"] = ParamsUtils.convert_to_ast(s3_conf_no_input)
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 1 == res
     params["data_s3_config"] = ParamsUtils.convert_to_ast(s3_conf_no_output)
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 1 == res
     params["data_s3_config"] = ParamsUtils.convert_to_ast(s3_conf)
     sys.argv = ParamsUtils.dict_to_req(d=params)
-    res = TestLauncherPython(
-        transform_runtime_config=PythonLauncherConfiguration(
-            name="test", transform_class=AbstractTableTransform, launcher_configuration=LauncherConfiguration()
-        ),
-    ).launch()
+    res = TestLauncherRay().launch()
     assert 0 == res
```

### Comparing `data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/ray/ray_util_test.py` & `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/ray_util_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 import pyarrow as pa
 import ray
-from data_processing.ray import RayUtils, TransformStatisticsRay
+from data_processing.runtime.ray import RayUtils, TransformStatisticsRay
 from data_processing.utils import GB, TransformUtils
 
 
 params = {}
 actor_options = {"num_cpus": 1, "memory": GB, "max_task_retries": 10}
```

### Comparing `data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/ray/test_noop_launch.py` & `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/test_noop_launch.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 import os
 
 import pyarrow as pa
-from data_processing.test_support.ray import AbstractTransformLauncherTest
-from data_processing.test_support.transform import NOOPTransformConfigurationRayLauncherConfiguration
+from data_processing.runtime.pure_python import PythonTransformLauncher
+from data_processing.test_support.launch.transform_test import (
+    AbstractTransformLauncherTest,
+)
+from data_processing.test_support.transform import NOOPPythonTransformConfiguration
 
 
 table = pa.Table.from_pydict({"name": pa.array(["Tom"]), "age": pa.array([23])})
 expected_table = table  # We're a noop after all.
 expected_metadata_list = [{"nfiles": 1, "nrows": 1}, {}]  # transform() result  # flush() result
 
 
 class TestRayNOOPTransform(AbstractTransformLauncherTest):
     """
     Extends the super-class to define the test data for the tests defined there.
     The name of this class MUST begin with the word Test so that pytest recognizes it as a test class.
     """
 
     def get_test_transform_fixtures(self) -> list[tuple]:
-        basedir = "../../../test-data/data_processing/ray/noop/"
+        basedir = "../../../../test-data/data_processing/ray/noop/"
         basedir = os.path.abspath(os.path.join(os.path.dirname(__file__), basedir))
-        fixtures = [(NOOPTransformConfigurationRayLauncherConfiguration(), {"noop_sleep_sec": 0}, basedir + "/input", basedir + "/expected")]
+        launcher = PythonTransformLauncher(NOOPPythonTransformConfiguration())
+        fixtures = [(launcher, {"noop_sleep_sec": 0}, basedir + "/input", basedir + "/expected")]
         return fixtures
```

### Comparing `data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/transform/test_noop.py` & `data_prep_toolkit-0.1.0/test/data_processing_tests/transform/test_noop.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test/data_processing_tests/util/transform_utils_test.py` & `data_prep_toolkit-0.1.0/test/data_processing_tests/util/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/input/ds1/sample1.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/input/ds1/sample2.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/sample2.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/input/ds2/sample3.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds2/sample3.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/daf/output/ds1/sample1.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/daf/output/ds1/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input/sample1.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input_multiple/sample1.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input_multiple/sample2.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample2.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/input_multiple/sample3.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample3.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/expected/metadata.json` & `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/metadata.json`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/expected/sample1.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/expected/subdir/test1.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/subdir/test1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/input/sample1.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1.dev4/test-data/data_processing/ray/noop/input/subdir/test1.parquet` & `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/subdir/test1.parquet`

 * *Files identical despite different names*

