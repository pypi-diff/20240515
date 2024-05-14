# Comparing `tmp/sf_hamilton_sdk-0.3.5.tar.gz` & `tmp/sf_hamilton_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sf_hamilton_sdk-0.3.5.tar", last modified: Fri Apr 26 05:49:23 2024, max compression
+gzip compressed data, was "sf_hamilton_sdk-0.4.0.tar", last modified: Tue May 14 22:50:36 2024, max compression
```

## Comparing `sf_hamilton_sdk-0.3.5.tar` & `sf_hamilton_sdk-0.4.0.tar`

### file list

```diff
@@ -1,96 +1,99 @@
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.930543 sf_hamilton_sdk-0.3.5/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-04-26 05:49:23.930144 sf_hamilton_sdk-0.3.5/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2136 2024-04-25 22:55:11.000000 sf_hamilton_sdk-0.3.5/README.md
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1916 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/pyproject.toml
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       18 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/requirements-test.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      140 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/requirements.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2024-04-26 05:49:23.930648 sf_hamilton_sdk-0.3.5/setup.cfg
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/setup.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.892785 sf_hamilton_sdk-0.3.5/src/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.897841 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       24 2024-04-26 05:48:38.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    24683 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/adapters.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.900581 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/api/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    30765 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/api/clients.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       85 2024-04-24 23:04:38.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/api/constants.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      243 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/api/projecttypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.901621 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      960 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/cli.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5453 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/initialize.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.902015 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.904358 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/common/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/common/.env.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/common/README.md.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2702 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/common/run.py.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.904832 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.906396 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      352 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/components/common.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2529 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.906809 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/config/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.908204 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.908626 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.909285 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.910174 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.910573 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.912853 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      469 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3738 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      600 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2532 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1403 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.913310 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.916011 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1450 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      370 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      711 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      932 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      745 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.916414 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    32447 2024-04-26 05:48:38.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/driver.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.925272 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2401 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/dataframe_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4908 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/example_tracking.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1037 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/numpy_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5440 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/pandas_col_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4833 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/pandas_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6277 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/polars_col_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4683 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/polars_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8470 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      638 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/sql_utils.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6235 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1428 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/trackingtypes.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2024-04-25 22:55:11.000000 sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/utils.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.929232 sf_hamilton_sdk-0.3.5/src/sf_hamilton_sdk.egg-info/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-04-26 05:49:23.000000 sf_hamilton_sdk-0.3.5/src/sf_hamilton_sdk.egg-info/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3700 2024-04-26 05:49:23.000000 sf_hamilton_sdk-0.3.5/src/sf_hamilton_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2024-04-26 05:49:23.000000 sf_hamilton_sdk-0.3.5/src/sf_hamilton_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       58 2024-04-26 05:49:23.000000 sf_hamilton_sdk-0.3.5/src/sf_hamilton_sdk.egg-info/entry_points.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      109 2024-04-26 05:49:23.000000 sf_hamilton_sdk-0.3.5/src/sf_hamilton_sdk.egg-info/requires.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       13 2024-04-26 05:49:23.000000 sf_hamilton_sdk-0.3.5/src/sf_hamilton_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:49:23.928770 sf_hamilton_sdk-0.3.5/tests/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5387 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/tests/test_adapters.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/tests/test_driver.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9605 2024-04-24 06:06:48.000000 sf_hamilton_sdk-0.3.5/tests/test_tracking.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.027807 sf_hamilton_sdk-0.4.0/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3669 2024-05-14 22:50:36.027337 sf_hamilton_sdk-0.4.0/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2136 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/README.md
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1916 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       56 2024-05-14 22:46:21.000000 sf_hamilton_sdk-0.4.0/requirements-test.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      140 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/requirements.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2024-05-14 22:50:36.027903 sf_hamilton_sdk-0.4.0/setup.cfg
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/setup.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.983161 sf_hamilton_sdk-0.4.0/src/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.986588 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       24 2024-05-14 22:47:39.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    24683 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/adapters.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.990296 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/api/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    30765 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/api/clients.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       85 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/api/constants.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      243 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/api/projecttypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.991491 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      960 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/cli.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5453 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/initialize.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.991956 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.993896 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/common/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/common/.env.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2702 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.994383 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.996171 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      352 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2529 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.996781 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/config/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.998151 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.998597 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:35.999290 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.000137 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.000610 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.003167 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      469 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3738 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      600 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2532 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1403 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.003652 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.007396 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1450 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      370 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      711 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      932 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      745 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.008062 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    32949 2024-05-14 22:46:21.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/driver.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.021399 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2401 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/dataframe_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4908 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/example_tracking.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2376 2024-05-14 22:46:21.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/ibis_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1581 2024-05-14 22:46:21.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/langchain_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1037 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/numpy_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5440 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/pandas_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4833 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/pandas_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6277 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/polars_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4683 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/polars_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3380 2024-05-14 22:46:21.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/pyspark_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8538 2024-05-14 22:46:21.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      638 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/sql_utils.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6734 2024-05-14 22:46:21.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1428 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/trackingtypes.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/utils.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.025894 sf_hamilton_sdk-0.4.0/src/sf_hamilton_sdk.egg-info/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3669 2024-05-14 22:50:35.000000 sf_hamilton_sdk-0.4.0/src/sf_hamilton_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3828 2024-05-14 22:50:35.000000 sf_hamilton_sdk-0.4.0/src/sf_hamilton_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2024-05-14 22:50:35.000000 sf_hamilton_sdk-0.4.0/src/sf_hamilton_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       58 2024-05-14 22:50:35.000000 sf_hamilton_sdk-0.4.0/src/sf_hamilton_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      147 2024-05-14 22:50:35.000000 sf_hamilton_sdk-0.4.0/src/sf_hamilton_sdk.egg-info/requires.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       13 2024-05-14 22:50:35.000000 sf_hamilton_sdk-0.4.0/src/sf_hamilton_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-05-14 22:50:36.025183 sf_hamilton_sdk-0.4.0/tests/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5387 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/tests/test_adapters.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3535 2024-05-14 22:46:21.000000 sf_hamilton_sdk-0.4.0/tests/test_driver.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9605 2024-05-14 00:32:24.000000 sf_hamilton_sdk-0.4.0/tests/test_tracking.py
```

### Comparing `sf_hamilton_sdk-0.3.5/PKG-INFO` & `sf_hamilton_sdk-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-hamilton-sdk
-Version: 0.3.5
+Version: 0.4.0
 Summary: Hamilton SDK for reading and writing to the Hamilton backend APIs that support the UI.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://github.com/dagworks-inc/hamilton/
 Project-URL: Bug Reports, https://github.com/dagworks-inc/hamilton/issues
 Project-URL: Source, https://github.com/dagworks-inc/hamilton/ui/sdk
 Project-URL: Documenation, https://hamilton.dagworks.io/
 Keywords: hamilton,dagworks,observability
@@ -25,15 +25,18 @@
 Requires-Dist: jinja2
 Requires-Dist: loguru
 Requires-Dist: posthog
 Requires-Dist: requests
 Requires-Dist: sf-hamilton>=1.43.0
 Requires-Dist: sqlglot
 Provides-Extra: test
+Requires-Dist: ibis-framework; extra == "test"
+Requires-Dist: langchain_core; extra == "test"
 Requires-Dist: polars; extra == "test"
+Requires-Dist: pyspark; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ray; extra == "test"
 
 # Hamilton UI SDK: Client Code &amp; Related
 
 Welcome to using the Hamilton UI!
```

### Comparing `sf_hamilton_sdk-0.3.5/README.md` & `sf_hamilton_sdk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/pyproject.toml` & `sf_hamilton_sdk-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/adapters.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/adapters.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/api/clients.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/api/clients.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/cli.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/initialize.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/common/run.py.jinja2` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/common/run.sh.jinja2` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/common/run.sh.jinja2`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/components/common.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/components/data_loader.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/data_processing/template_data.json` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/data_processing/template_data.json`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/components/transforms.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/hello_world/template_data.json` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/iris_loader.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/model_fitting.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/machine_learning/components/models.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/machine_learning/components/models.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/driver.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,30 @@
             hash_object.update(f.read())
     else:
         logger.debug(
             "Skipping hash for module %s because it has no __file__ attribute or it is None.",
             module,
         )
 
+    def safe_getmembers(module):
+        """Need this because some modules are lazily loaded and we can't get the members.
+        e.g. ibis.
+        """
+        try:
+            return inspect.getmembers(module)
+        except Exception as e:
+            if logger.isEnabledFor(logging.DEBUG):
+                logger.debug(
+                    f"Skipping hash for module {module.__name__} because we could not get the members. "
+                    f"Error: {e}"
+                )
+            return []
+
     # Loop through the module's attributes
-    for name, value in inspect.getmembers(module):
+    for name, value in safe_getmembers(module):
         # Check if the attribute is a module
         if inspect.ismodule(value):
             if value.__package__ is None:
                 logger.info(
                     f"Skipping hash for module {value.__name__} because it has no __package__ "
                     f"attribute or it is None. This happens with lazy loaders."
                 )
```

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/dataframe_stats.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/dataframe_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/example_tracking.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/example_tracking.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/numpy_stats.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/numpy_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/pandas_col_stats.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/pandas_col_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/pandas_stats.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/pandas_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/polars_col_stats.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/polars_col_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/polars_stats.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/polars_stats.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/runs.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import functools
+import importlib
 import logging
 import sys
 import time as py_time
 import traceback
 from contextlib import contextmanager
 from datetime import datetime, timezone
 from typing import Any, Callable, Dict, List, Optional
@@ -10,29 +11,25 @@
 from hamilton_sdk.tracking import stats
 from hamilton_sdk.tracking.trackingtypes import DAGRun, Status, TaskRun
 
 from hamilton import node as h_node
 from hamilton.data_quality import base as dq_base
 from hamilton.lifecycle import base as lifecycle_base
 
-try:
-    from hamilton_sdk.tracking import numpy_stats  # noqa: F401
-    from hamilton_sdk.tracking import pandas_stats  # noqa: F401
-
-except ImportError:
-    pass
-
-try:
-    from hamilton_sdk.tracking import polars_stats  # noqa: F401
-
-except ImportError:
-    pass
+_modules_to_import = ["numpy", "pandas", "polars", "pyspark", "ibis", "langchain"]
 
 logger = logging.getLogger(__name__)
 
+for module in _modules_to_import:
+    try:
+        importlib.import_module(f"hamilton_sdk.tracking.{module}_stats")
+    except ImportError:
+        logger.debug(f"Failed to import hamilton_sdk.tracking.{module}_stats")
+        pass
+
 
 def process_result(result: Any, node: h_node.Node) -> Any:
     """Processes result -- this is purely a by-type mapping.
     Note that this doesn't actually do anything yet -- the idea is that we can return DQ
     results, and do other stuff with other results -- E.G. summary stats on dataframes,
     pass small strings through, etc...
```

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/sql_utils.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/sql_utils.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/stats.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/stats.py`

 * *Files 7% similar despite different names*

```diff
@@ -110,14 +110,19 @@
                 "observability_type": "dict",
                 "observability_value": {
                     "type": str(type(result[1])),
                     "value": _metadata,
                 },
                 "observability_schema_version": "0.0.2",
             }
+    # namedtuple -- this how we guide people to not have something tracked easily.
+    # so we skip it if it has a `secret_key`. This is hacky -- better choice would
+    # be to have an internal object or way to decorate a parameter to not track it.
+    if hasattr(result, "_asdict") and not hasattr(result, "secret_key"):
+        return compute_stats_dict(result._asdict(), node_name, node_tags)
     return {
         "observability_type": "unsupported",
         "observability_value": {
             "unsupported_type": str(type(result)),
             "action": "reach out to the DAGWorks team to add support for this type.",
         },
         "observability_schema_version": "0.0.1",
@@ -150,14 +155,16 @@
                     # it's a DF, Series -- so take full result.
                     v = v_result["observability_value"]
                 elif observed_type == "unsupported":
                     v = str(v)
                     # else just string it -- max 200 chars.
                     if len(v) > 200:
                         v = v[:200] + "..."
+                elif observed_type == "dict":
+                    v = v_result["observability_value"]
             result_values.append(v)
     return {
         # yes dict type -- that's so that we can display in the UI. It's a hack.
         "observability_type": "dict",
         "observability_value": {
             "type": str(type(result)),
             "value": result_values,
```

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/trackingtypes.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/trackingtypes.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/hamilton_sdk/tracking/utils.py` & `sf_hamilton_sdk-0.4.0/src/hamilton_sdk/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/src/sf_hamilton_sdk.egg-info/PKG-INFO` & `sf_hamilton_sdk-0.4.0/src/sf_hamilton_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-hamilton-sdk
-Version: 0.3.5
+Version: 0.4.0
 Summary: Hamilton SDK for reading and writing to the Hamilton backend APIs that support the UI.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://github.com/dagworks-inc/hamilton/
 Project-URL: Bug Reports, https://github.com/dagworks-inc/hamilton/issues
 Project-URL: Source, https://github.com/dagworks-inc/hamilton/ui/sdk
 Project-URL: Documenation, https://hamilton.dagworks.io/
 Keywords: hamilton,dagworks,observability
@@ -25,15 +25,18 @@
 Requires-Dist: jinja2
 Requires-Dist: loguru
 Requires-Dist: posthog
 Requires-Dist: requests
 Requires-Dist: sf-hamilton>=1.43.0
 Requires-Dist: sqlglot
 Provides-Extra: test
+Requires-Dist: ibis-framework; extra == "test"
+Requires-Dist: langchain_core; extra == "test"
 Requires-Dist: polars; extra == "test"
+Requires-Dist: pyspark; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ray; extra == "test"
 
 # Hamilton UI SDK: Client Code &amp; Related
 
 Welcome to using the Hamilton UI!
```

### Comparing `sf_hamilton_sdk-0.3.5/src/sf_hamilton_sdk.egg-info/SOURCES.txt` & `sf_hamilton_sdk-0.4.0/src/sf_hamilton_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,22 @@
 src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
 src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
 src/hamilton_sdk/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
 src/hamilton_sdk/cli/templates/time_series_feature_engineering/data/train_sample.csv
 src/hamilton_sdk/tracking/__init__.py
 src/hamilton_sdk/tracking/dataframe_stats.py
 src/hamilton_sdk/tracking/example_tracking.py
+src/hamilton_sdk/tracking/ibis_stats.py
+src/hamilton_sdk/tracking/langchain_stats.py
 src/hamilton_sdk/tracking/numpy_stats.py
 src/hamilton_sdk/tracking/pandas_col_stats.py
 src/hamilton_sdk/tracking/pandas_stats.py
 src/hamilton_sdk/tracking/polars_col_stats.py
 src/hamilton_sdk/tracking/polars_stats.py
+src/hamilton_sdk/tracking/pyspark_stats.py
 src/hamilton_sdk/tracking/runs.py
 src/hamilton_sdk/tracking/sql_utils.py
 src/hamilton_sdk/tracking/stats.py
 src/hamilton_sdk/tracking/trackingtypes.py
 src/hamilton_sdk/tracking/utils.py
 src/sf_hamilton_sdk.egg-info/PKG-INFO
 src/sf_hamilton_sdk.egg-info/SOURCES.txt
```

### Comparing `sf_hamilton_sdk-0.3.5/tests/test_adapters.py` & `sf_hamilton_sdk-0.4.0/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `sf_hamilton_sdk-0.3.5/tests/test_driver.py` & `sf_hamilton_sdk-0.4.0/tests/test_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """Tests that we successfully hash a simple package that imports a subpackage"""
     from tests.test_package_to_hash import submodule1
 
     hash_object = hashlib.sha256()
     seen_modules = set()
     result = _hash_module(submodule1, hash_object, seen_modules)
 
-    assert result.hexdigest() == "9f0b697b6b071d0ca6df18532031a8e553a8327531e249ff457d772b8bd392c7"
+    assert result.hexdigest() == "4466d1f61b2c57c2b5bfe8a9fec09acd53befcfdf2f5720075aef83e3d6c6bf8"
     assert len(seen_modules) == 2
     assert {m.__name__ for m in seen_modules} == {
         "tests.test_package_to_hash.subpackage",
         "tests.test_package_to_hash.submodule1",
     }
 
 
@@ -58,15 +58,15 @@
     """Tests that we successfully hash submodules and subpackages."""
     from tests import test_package_to_hash
 
     hash_object = hashlib.sha256()
     seen_modules = set()
     result = _hash_module(test_package_to_hash, hash_object, seen_modules)
 
-    assert result.hexdigest() == "fc568608a2f766eac3cbae4021fb367247c6aa36ac4ae72ea98104c1ba2a5e1c"
+    assert result.hexdigest() == "c22023a4fdc8564de1cda70d05a19d5e8c0ddaaa9dcccf644a2b789b80f19896"
     assert len(seen_modules) == 4
     assert {m.__name__ for m in seen_modules} == {
         "tests.test_package_to_hash",
         "tests.test_package_to_hash.submodule2",
         "tests.test_package_to_hash.submodule1",
         "tests.test_package_to_hash.subpackage",
     }
```

### Comparing `sf_hamilton_sdk-0.3.5/tests/test_tracking.py` & `sf_hamilton_sdk-0.4.0/tests/test_tracking.py`

 * *Files identical despite different names*

