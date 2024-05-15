# Comparing `tmp/cornflow-client-1.0.9.tar.gz` & `tmp/cornflow-client-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cornflow-client-1.0.9.tar", last modified: Mon Mar  6 09:54:00 2023, max compression
+gzip compressed data, was "cornflow-client-1.1.0a1.tar", last modified: Wed May 15 17:14:43 2024, max compression
```

## Comparing `cornflow-client-1.0.9.tar` & `cornflow-client-1.1.0a1.tar`

### file list

```diff
@@ -1,74 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (116)    10766 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      139 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1754 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/
--rw-r--r--   0 runner    (1001) docker     (116)      411 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/airflow/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5264 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/airflow/api.py
--rw-r--r--   0 runner    (1001) docker     (116)    10497 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/airflow/dag_utilities.py
--rw-r--r--   0 runner    (1001) docker     (116)     7982 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/core/
--rw-r--r--   0 runner    (1001) docker     (116)      202 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8482 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/application.py
--rw-r--r--   0 runner    (1001) docker     (116)     1984 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/experiment.py
--rw-r--r--   0 runner    (1001) docker     (116)      839 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (116)    14662 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/instance_solution.py
--rw-r--r--   0 runner    (1001) docker     (116)     2824 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/read_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)      234 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/solution.py
--rw-r--r--   0 runner    (1001) docker     (116)      552 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     5496 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/cornflow_client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/data/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      121 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/empty_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)     2273 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/pulp_json_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)     5549 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/schema_validator.json
--rw-r--r--   0 runner    (1001) docker     (116)      819 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/solver_config.json
--rw-r--r--   0 runner    (1001) docker     (116)      476 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/vrp_solution_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)    30049 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/raw_cornflow_client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/schema/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10903 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/dictSchema.py
--rw-r--r--   0 runner    (1001) docker     (116)     3610 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/dict_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)     9404 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/manager.py
--rw-r--r--   0 runner    (1001) docker     (116)     2200 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5016 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/tests/data/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    30894 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/data_input_bad.json
--rw-r--r--   0 runner    (1001) docker     (116)     1319 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/data_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)     3425 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/gc_input.json
--rw-r--r--   0 runner    (1001) docker     (116)     1513 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/gc_output.json
--rw-r--r--   0 runner    (1001) docker     (116)      611 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/graph_coloring_input.json
--rw-r--r--   0 runner    (1001) docker     (116)      376 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/graph_coloring_output.json
--rw-r--r--   0 runner    (1001) docker     (116)    30946 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/hk_data_input.json
--rw-r--r--   0 runner    (1001) docker     (116)     1611 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/hk_data_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      437 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/hk_solution_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)     1495 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/instance-hackathon2.json
--rw-r--r--   0 runner    (1001) docker     (116)     1669 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/name_problem_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)   550476 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/pulp_example_data.json
--rw-r--r--   0 runner    (1001) docker     (116)      911 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/test_mps.mps
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2644 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/test_airflow_integration.py
--rw-r--r--   0 runner    (1001) docker     (116)    20676 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/test_cornflow_integration.py
--rw-r--r--   0 runner    (1001) docker     (116)    23785 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/test_raw_cornflow_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3739 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (116)     1734 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_dag_utilities.py
--rw-r--r--   0 runner    (1001) docker     (116)    14225 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_instance_solution_methods.py
--rw-r--r--   0 runner    (1001) docker     (116)     9473 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (116)     4852 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_varnames.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1754 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2415 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       64 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      983 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.127325 cornflow-client-1.1.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-15 17:14:43.127325 cornflow-client-1.1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.115325 cornflow-client-1.1.0a1/cornflow_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/airflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/airflow/dag_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14822 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/instance_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/read_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/cornflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/empty_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/pulp_json_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/schema_validator.json
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/solver_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/vrp_solution_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    29980 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/raw_cornflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/dictSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/dict_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.123325 cornflow-client-1.1.0a1/cornflow_client/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30894 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/data_input_bad.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/data_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/endpoints_access.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/endpoints_methods.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/gc_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/gc_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/graph_coloring_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/graph_coloring_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30946 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_data_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_data_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_solution_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/instance-hackathon2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/name_problem_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)   550476 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/pulp_example_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/schema_with_fk.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/schema_without_fk.json
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/test_mps.mps
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_with_access.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_with_fk.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_with_methods.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_without_fk.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.123325 cornflow-client-1.1.0a1/cornflow_client/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_airflow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21169 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_cornflow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24798 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_raw_cornflow_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.127325 cornflow-client-1.1.0a1/cornflow_client/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_dag_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15639 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_instance_solution_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_schema_from_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_varnames.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.115325 cornflow-client-1.1.0a1/cornflow_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:14:43.127325 cornflow-client-1.1.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cornflow-client-1.0.9/LICENSE` & `cornflow-client-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/PKG-INFO` & `cornflow-client-1.1.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cornflow-client
-Version: 1.0.9
+Version: 1.1.0a1
 Summary: Client to connect to a cornflow server
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow client
         ================
         
         The aim of this repository is to have a client to use to connect to a deployed cornflow webserver
         
         Requirements
         ~~~~~~~~~~~~
         
-        * python >= 3.6
+        * python >= 3.8
         
         Install cornflow-client
         ~~~~~~~~~~~~~~~~~~~~~~~~
         
         To install the package do::
         
             python3 -m pip install cornflow-client
@@ -43,10 +43,10 @@
             status = client.get_status(execution_id)
             results = client.get_results(execution_id)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `cornflow-client-1.0.9/README.rst` & `cornflow-client-1.1.0a1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ================
 
 The aim of this repository is to have a client to use to connect to a deployed cornflow webserver
 
 Requirements
 ~~~~~~~~~~~~
 
-* python >= 3.6
+* python >= 3.8
 
 Install cornflow-client
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 To install the package do::
 
     python3 -m pip install cornflow-client
```

### Comparing `cornflow-client-1.0.9/cornflow_client/airflow/api.py` & `cornflow-client-1.1.0a1/cornflow_client/airflow/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,22 @@
     def is_alive(self):
         try:
             response = requests.get(f"{self.url}/health")
         except (ConnectionError, HTTPError):
             return False
         try:
             data = response.json()
+            database = data["metadatabase"]["status"] == "healthy"
+            scheduler = data["scheduler"]["status"] == "healthy"
         except json.JSONDecodeError:
             return False
-        return (
-            data["metadatabase"]["status"] == "healthy"
-            and data["scheduler"]["status"] == "healthy"
-        )
+        except KeyError:
+            return False
+
+        return database and scheduler
 
     def request_headers_auth(self, status=200, **kwargs):
         def_headers = {"Content-type": "application/json", "Accept": "application/json"}
         headers = kwargs.get("headers", def_headers)
         response = requests.request(headers=headers, auth=self.auth, **kwargs)
         if status is None:
             return response
```

### Comparing `cornflow-client-1.0.9/cornflow_client/airflow/dag_utilities.py` & `cornflow-client-1.1.0a1/cornflow_client/airflow/dag_utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 """
 
 """
-# Full imports
+
 import json
-import logging
 import os
-
-# Partial imports
 from datetime import datetime, timedelta
 from urllib.parse import urlparse, urljoin
 
-
-# Imports from modules
 from cornflow_client import CornFlow, CornFlowApiError
 
-
 # TODO: convert everything to an object that encapsulates everything
 #  to make it clear and avoid all the arguments.
 # class DagApp(object):
 #
 #     def __init__(self, dag_name, secrets):
 #         self.name = dag_name
 #         self.secrets = secrets
@@ -41,28 +35,30 @@
     "email_on_retry": False,
     "retry_delay": timedelta(minutes=1),
     "schedule_interval": None,
 }
 
 
 def get_schemas_from_file(_dir, dag_name):
+    # TODO: check if in use
     with open(os.path.join(_dir, dag_name + "_input.json"), "r") as f:
         instance = json.load(f)
     with open(os.path.join(_dir, dag_name + "_output.json"), "r") as f:
         solution = json.load(f)
     return instance, solution
 
 
 def get_requirements(path):
     """
     Read requirements.txt from a project and return a list of packages.
 
     :param path: The path of the project
     :return: A list of required packages
     """
+    # TODO: check if in use
     req_path = f"{path}/requirements.txt"
 
     try:
         with open(req_path, "r") as file:
             req_list = file.read().splitlines()
     except:
         print("no requirement file in this path")
@@ -75,15 +71,15 @@
     """
     Create a connection to cornflow and log in with airflow admin user.
 
     :return: A logged and connected Cornflow class instance
     """
     # This secret comes from airflow configuration
     print("Getting connection information from ENV VAR=CF_URI")
-    uri = secrets.get_conn_uri("CF_URI")
+    uri = secrets.get_conn_value("CF_URI")
     conn = urlparse(uri)
     scheme = conn.scheme
     if scheme == "cornflow":
         scheme = "http"
     url = f"{scheme}://{conn.hostname}"
     if conn.port:
         url = f"{url}:{conn.port}"
@@ -95,32 +91,34 @@
 
 
 def try_to_save_error(client, exec_id, state=-1):
     """
     Attempt at saving that the execution failed
     """
     try:
-        client.put_api_for_id("dag/", id=exec_id, payload=dict(state=state))
+        client.raw.put_api_for_id("dag/", id=exec_id, payload=dict(state=state))
     except Exception as e:
         print(f"An exception trying to register the failed status: {e}")
 
 
 def try_to_save_airflow_log(client, exec_id, ti, base_log_folder):
     log_file = os.path.join(
         base_log_folder,
         f"{ti.dag_id}",
         f"{ti.task_id}",
         f"{ti.run_id}".replace("manual__", "").replace("scheduled__", ""),
-        f"{ti.try_number}.log"
+        f"{ti.try_number}.log",
     )
     if os.path.exists(log_file):
-        with open(log_file, 'r') as fd:
+        with open(log_file, "r") as fd:
             log_file_txt = fd.read()
         try:
-            client.put_api_for_id("dag/", id=exec_id, payload=dict(log_text=log_file_txt))
+            client.raw.put_api_for_id(
+                "dag/", id=exec_id, payload=dict(log_text=log_file_txt)
+            )
         except Exception as e:
             print(f"An exception occurred while trying to register airflow log: {e}")
 
 
 def try_to_write_solution(client, exec_id, payload):
     """
     Tries to write the payload into cornflow
@@ -146,14 +144,15 @@
             )
         except CornFlowApiError:
             try_to_save_error(client, exec_id, -6)
             raise AirflowDagException("The writing of the instance checks failed")
 
 
 def get_schema(dag_name):
+    # TODO: check if in use
     _file = os.path.join(os.path.dirname(__file__), f"{dag_name}_output.json")
     with open(_file, "r") as f:
         schema = json.load(f)
     return schema
 
 
 def cf_solve_app(app, secrets, **kwargs):
@@ -308,13 +307,45 @@
         client.update_status(exec_id, {"status": -1})
         try_to_save_airflow_log(client, exec_id, ti, base_log_folder)
         raise AirflowDagException(
             "There was an error during the verification of the data"
         )
 
 
+def callback_email(context):
+    from airflow.utils.email import send_email
+    from airflow.secrets.environment_variables import EnvironmentVariablesBackend
+
+    path_to_log = (
+        f"./logs/dag_id={context['dag'].dag_id}/run_id={context['run_id']}"
+        f"/task_id={context['ti'].task_id}/attempt=1.log"
+    )
+
+    environment = EnvironmentVariablesBackend().get_variable("ENVIRONMENT")
+    notification_email = EnvironmentVariablesBackend().get_variable(
+        "NOTIFICATION_EMAIL"
+    )
+    environment_name = os.getenv("AIRFLOW__WEBSERVER__INSTANCE_NAME", "CornflowEnv")
+
+    title = f"Airflow. {environment_name} ({environment}). DAG/task error: {context['dag'].dag_id}/{context['ti'].task_id} Failed"
+    body = f"""
+        The DAG/task {context['dag'].dag_id}/{context['ti'].task_id} has failed.
+        <br>
+        The log is attached.
+        """
+
+    send_email(
+        to=[
+            notification_email,
+        ],
+        subject=title,
+        html_content=body,
+        files=[path_to_log],
+    )
+
+
 class NoSolverException(Exception):
     pass
 
 
 class AirflowDagException(Exception):
     pass
```

### Comparing `cornflow-client-1.0.9/cornflow_client/core/application.py` & `cornflow-client-1.1.0a1/cornflow_client/core/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 """
 
 """
 # Partial imports
 from abc import ABC, abstractmethod
-from jsonschema import Draft7Validator
-from pytups import SuperDict
 from timeit import default_timer as timer
 from typing import Type, Dict, List, Tuple, Union
 
-# Imports from internal modules
-from .instance import InstanceCore
-from .solution import SolutionCore
-from .experiment import ExperimentCore
+from jsonschema import Draft7Validator
+from pytups import SuperDict
 
 from cornflow_client.constants import (
     STATUS_CONV,
     STATUS_OPTIMAL,
-    STATUS_NOT_SOLVED,
     STATUS_INFEASIBLE,
-    STATUS_UNDEFINED,
-    STATUS_TIME_LIMIT,
     SOLUTION_STATUS_FEASIBLE,
     SOLUTION_STATUS_INFEASIBLE,
     NoSolverException,
     BadConfiguration,
     BadSolution,
     BadInstance,
 )
+from .experiment import ExperimentCore
+
+# Imports from internal modules
+from .instance import InstanceCore
+from .solution import SolutionCore
 
 
 class ApplicationCore(ABC):
     """
     The application template.
     """
 
+    # We create a new attribute controlling the use of the notification mail function
+    def __init__(self):
+        self._notify = False
+
+    @property
+    def notify(self) -> bool:
+        return self._notify
+
     @property
     @abstractmethod
     def name(self) -> str:
         """
         Mandatory property
 
         :return: the name of the class.
@@ -59,14 +65,23 @@
         Optional property
 
         :return: the default args for the DAG
         """
         return None
 
     @property
+    def extra_args(self) -> Dict:
+        """
+        Optional property
+
+        :return: dictionary with optional arguments for the DAG
+        """
+        return None
+
+    @property
     @abstractmethod
     def instance(self) -> Type[InstanceCore]:
         """
         Mandatory property
 
         :return: the constructor for the instance.
         """
@@ -90,24 +105,34 @@
 
         :return: the configuration schema used for the solve() method.
         """
         raise NotImplementedError()
 
     @property
     @abstractmethod
-    def test_cases(self) -> List[Union[Dict, Tuple[Dict, Dict]]]:
+    def test_cases(
+        self,
+    ) -> Union[List[Dict[str, Union[str, Dict]]], List[Union[Dict, Tuple[Dict, Dict]]]]:
         """
         Mandatory property
 
         :return: a list of datasets following the json-schema.
           if each element in the list is:
 
           * **dict**: each element is an instance
           * **tuple**: the first part is the instance, the second its solution
+
+          it can also return a list of dicts, where the keys are:
+
+          * **name**: name of the test case.
+          * **description** optional field with a description of the test case.
+          * **instance**: the instance data.
+          * **solution**: the solution data (optional)
         """
+        # TODO: Phase out older list implementation
         raise NotImplementedError()
 
     @property
     @abstractmethod
     def solvers(self) -> Dict[str, Type[ExperimentCore]]:
         """
         Mandatory property
@@ -134,14 +159,15 @@
                 f"The configuration does not match the schema:\n{error_list}"
             )
 
         solver = config.get("solver")
         if solver is None:
             solver = self.get_default_solver_name()
         solver_class = self.get_solver(name=solver)
+        # TODO: I think this exception is unreachable
         if solver_class is None:
             raise NoSolverException(f"Solver {solver} is not available")
         inst = self.instance.from_dict(data)
         inst_errors = inst.check_schema()
         if inst_errors:
             raise BadInstance(f"The instance does not match the schema:\n{inst_errors}")
         sol = None
@@ -176,45 +202,49 @@
         output = algo.solve(config)
         sol = None
         # compatibility with previous format:
         if isinstance(output, int):
             output = dict(status=output)
         status = output.get("status")
         status_sol = output.get("status_sol")
-        log = dict(
-            time=timer() - start,
-            solver=solver,
-            status=STATUS_CONV.get(status, "Unknown"),
-            status_code=status,
-            sol_code=SOLUTION_STATUS_INFEASIBLE,
-        )
+
+        log_json = {
+            **output,
+            **{
+                "time": timer() - start,
+                "solver": solver,
+                "status": STATUS_CONV.get(status, "Unknown"),
+                "status_code": status,
+                "sol_code": SOLUTION_STATUS_INFEASIBLE,
+            },
+        }
 
         try:
             log_txt = algo.log
         except:
             log_txt = ""
 
         # check if there is a solution
         # TODO: we need to extract the solution status too
         #  because there may be already an initial solution in the solver
         # TODO: review whole status types and meaning
         if status_sol is not None:
-            log["sol_code"] = status_sol
+            log_json["sol_code"] = status_sol
         elif algo.solution is not None and len(algo.solution.data):
-            log["sol_code"] = SOLUTION_STATUS_FEASIBLE
+            log_json["sol_code"] = SOLUTION_STATUS_FEASIBLE
 
-        if log["sol_code"] > 0:
+        if log_json["sol_code"] > 0:
             sol = algo.solution.to_dict()
 
         if sol != {} and sol is not None:
             checks = algo.check_solution()
         else:
             checks = None
 
-        return sol, checks, instance_checks, log_txt, log
+        return sol, checks, instance_checks, log_txt, log_json
 
     def check(
         self, instance_data: dict, solution_data: dict, *args, **kwargs
     ) -> Tuple[Dict, Dict, Dict]:
         """
         Checks the instance and solution data
         :param instance_data: json data of the instance
```

### Comparing `cornflow-client-1.0.9/cornflow_client/core/instance.py` & `cornflow-client-1.1.0a1/cornflow_client/core/instance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 
 """
-# Partial imports
+
 from abc import ABC, abstractmethod
 
-# Imports from internal modules
 from .instance_solution import InstanceSolutionCore
 
 
 class InstanceCore(InstanceSolutionCore, ABC):
     """
     The instance template.
     """
```

### Comparing `cornflow-client-1.0.9/cornflow_client/core/instance_solution.py` & `cornflow-client-1.1.0a1/cornflow_client/core/instance_solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 
 """
-# Full imports
-import json
 
-# Partial imports
+import json
 from abc import ABC, abstractmethod
+from datetime import datetime, timedelta
+from typing import List
+
 from genson import SchemaBuilder
 from jsonschema import Draft7Validator
 from pytups import SuperDict
-from typing import List
-from datetime import datetime, timedelta
 
-# Imports from internal modules
 from .read_tools import read_excel, is_xl_type
 
 
 class InstanceSolutionCore(ABC):
     """
     Common interface for the instance and solution templates
     """
@@ -331,30 +329,50 @@
 
     @staticmethod
     def add_time_to_ts(ts: datetime, weeks=0, days=0, minutes=0, seconds=0) -> datetime:
         """Adds time to a datetime"""
         return ts + timedelta(days=7 * weeks + days, minutes=minutes, seconds=seconds)
 
     @staticmethod
-    def add_time_to_date_string(string: str, weeks=0, days=0, minutes=0, seconds=0) -> str:
+    def add_time_to_date_string(
+        string: str, weeks=0, days=0, minutes=0, seconds=0
+    ) -> str:
         """Adds time to a date string"""
         date = datetime.strptime(string, "%Y-%m-%d").date()
-        return (date + timedelta(days=7 * weeks + days, minutes=minutes, seconds=seconds)).strftime("%Y-%m-%d")
+        return (
+            date + timedelta(days=7 * weeks + days, minutes=minutes, seconds=seconds)
+        ).strftime("%Y-%m-%d")
 
     @staticmethod
-    def add_time_to_datetime_string(string: str, weeks=0, days=0, minutes=0, seconds=0) -> str:
+    def add_time_to_datetime_string(
+        string: str, weeks=0, days=0, minutes=0, seconds=0
+    ) -> str:
         """Adds time to a datetime"""
         datetime_object = datetime.strptime(string, "%Y-%m-%dT%H:%M:%S")
-        return (datetime_object + timedelta(days=7 * weeks + days, minutes=minutes, seconds=seconds)).strftime("%Y-%m-%dT%H:%M:%S")
+        return (
+            datetime_object
+            + timedelta(days=7 * weeks + days, minutes=minutes, seconds=seconds)
+        ).strftime("%Y-%m-%dT%H:%M:%S")
 
     @staticmethod
-    def add_time_to_datetimesec_string(string: str, weeks=0, days=0, hours=0, minutes=0, seconds=0) -> str:
+    def add_time_to_datetimesec_string(
+        string: str, weeks=0, days=0, hours=0, minutes=0, seconds=0
+    ) -> str:
         """Adds time to a datetime"""
         datetime_object = datetime.strptime(string, "%Y-%m-%dT%H:%M:%S")
-        return (datetime_object + timedelta(weeks=weeks, days=7 * weeks + days, hours=hours, minutes=minutes, seconds=seconds)).strftime("%Y-%m-%dT%H:%M:%S")
+        return (
+            datetime_object
+            + timedelta(
+                weeks=weeks,
+                days=7 * weeks + days,
+                hours=hours,
+                minutes=minutes,
+                seconds=seconds,
+            )
+        ).strftime("%Y-%m-%dT%H:%M:%S")
 
     @staticmethod
     def get_week_from_ts(ts: datetime) -> int:
         """Returns the integer value of the week for the given time slot"""
         return ts.isocalendar()[1]
 
     @staticmethod
@@ -362,15 +380,15 @@
         """Returns the integer value of the week for the given string"""
         date_object = datetime.strptime(string, "%Y-%m-%d").date()
         return date_object.isocalendar()[1]
 
     @staticmethod
     def get_week_from_datetime_string(string: str) -> int:
         """Returns the integer value of the week for the given string"""
-        datetime_object = datetime.strptime(string, "%Y-%m-%dT%H:%M:%S")
+        datetime_object = datetime.strptime(string, "%Y-%m-%dT%H:%M")
         return datetime_object.isocalendar()[1]
 
     @staticmethod
     def get_week_from_datetimesec_string(string: str) -> int:
         """Returns the integer value of the week for the given string"""
         datetime_object = datetime.strptime(string, "%Y-%m-%dT%H:%M:%S")
         return datetime_object.isocalendar()[1]
@@ -379,33 +397,33 @@
     def get_weekday_from_ts(ts: datetime) -> int:
         """Returns the number of the weekday from a ts"""
         return ts.isocalendar()[2]
 
     @staticmethod
     def get_weekday_from_date_string(string: str) -> int:
         """Returns the number of the weekday from a date string in format 'YYYY-MM-DD'"""
-        date = datetime.strptime(string, '%Y-%m-%d').date()
+        date = datetime.strptime(string, "%Y-%m-%d").date()
         return date.isocalendar()[2]
 
     @staticmethod
     def get_weekday_from_datetime_string(string: str) -> int:
         """Returns the number of the weekday from a date string in format 'YYYY-MM-DDTh:m'"""
-        datetime_obj = datetime.strptime(string, '%Y-%m-%dT%H:%M:%S')
+        datetime_obj = datetime.strptime(string, "%Y-%m-%dT%H:%M:%S")
         return datetime_obj.isocalendar()[2]
 
     @staticmethod
     def get_weekday_from_datetimesec_string(string: str) -> int:
         """Returns the number of the weekday from a date string in format 'YYYY-MM-DDT:h:m:s'"""
-        datetime_obj = datetime.strptime(string, '%Y-%m-%dT%H:%M:%S')
+        datetime_obj = datetime.strptime(string, "%Y-%m-%dT%H:%M:%S")
         return datetime_obj.isocalendar()[2]
 
     @staticmethod
     def get_hour_from_datetime_string(string: str) -> float:
         """Returns the integer value of the hour (in number) from ts string in format 'YYYY-MM-DDTh:m'"""
-        datetime_obj = datetime.strptime(string, '%Y-%m-%dT%H:%M:%S')
+        datetime_obj = datetime.strptime(string, "%Y-%m-%dT%H:%M:%S")
         return datetime_obj.hour
 
     @staticmethod
     def get_hour_from_datetimesec_string(string: str) -> float:
         """Returns the integer value of the hour (in number) from ts string in format 'YYYY-MM-DDTh:m:s'"""
-        datetime_obj = datetime.strptime(string, '%Y-%m-%dT%H:%M:%S')
+        datetime_obj = datetime.strptime(string, "%Y-%m-%dT%H:%M:%S")
         return datetime_obj.hour
```

### Comparing `cornflow-client-1.0.9/cornflow_client/core/read_tools.py` & `cornflow-client-1.1.0a1/cornflow_client/core/read_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 """
 
 """
-# Full imports
+
 import math
+import numbers
 
-# Partial imports
 from pytups import TupList, SuperDict
-import numbers
 
 
-def read_excel(path: str, param_tables_names: list = None) -> dict:
+def read_excel(
+    path: str, param_tables_names: list = None, preserve_types=False
+) -> dict:
     """
-    Read an entire excel file.
+    Read an entire Excel file.
 
-    :param path: path of the excel file
-    :param param_tables_names: names of the parameter tables
+    :param path: path of the Excel file.
+    :param param_tables_names: names of the parameter tables.
+    :param preserve_types: if true pandas will not interpret type.
     :return: a dict with a list of dict (records format) for each table.
     """
     is_xl_type(path)
 
     try:
         import openpyxl
     except (ModuleNotFoundError, ImportError) as e:
         raise Exception("You must install openpyxl package to use this method")
 
     try:
         import pandas as pd
     except (ModuleNotFoundError, ImportError):
         raise Exception("You must install pandas package to use this method")
 
-    data = pd.read_excel(path, sheet_name=None)
+    dtype = "object" if preserve_types else None
+
+    data = pd.read_excel(path, sheet_name=None, dtype=dtype)
 
     data_tables = {
         name: TupList(content.to_dict(orient="records")).vapply(
             lambda v: SuperDict(v).vapply(lambda vv: format_value(vv))
         )
         for name, content in data.items()
         if name not in param_tables_names
```

### Comparing `cornflow-client-1.0.9/cornflow_client/core/tools.py` & `cornflow-client-1.1.0a1/cornflow_client/core/tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 
 """
-# Full imports
+
 import json
 import pickle
 
-# Partial imports
 from pytups import OrderSet
 
 
 def new_set(seq):
     """
     :param seq: a (hopefully unique) list of elements (tuples, strings, etc.)
     Returns a new ordered set
```

### Comparing `cornflow-client-1.0.9/cornflow_client/cornflow_client.py` & `cornflow-client-1.1.0a1/cornflow_client/cornflow_client.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/data/pulp_json_schema.json` & `cornflow-client-1.1.0a1/cornflow_client/data/pulp_json_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/data/schema_validator.json` & `cornflow-client-1.1.0a1/cornflow_client/data/schema_validator.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/data/solver_config.json` & `cornflow-client-1.1.0a1/cornflow_client/data/solver_config.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/raw_cornflow_client.py` & `cornflow-client-1.1.0a1/cornflow_client/raw_cornflow_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 
 """
-# Full imports
+
 import logging as log
 import re
-import requests
-
-# Partial imports
 from functools import wraps
 from urllib.parse import urljoin
 
+import requests
+
 
 class RawCornFlow(object):
     """
     Base class to access cornflow-server
     """
 
     def __init__(self, url, token=None):
@@ -405,15 +404,15 @@
         url = urljoin(urljoin(self.url, api) + "/", str(execution_id) + "/" + post_url)
         return requests.request(
             method="post",
             url=url,
             headers={
                 "Authorization": "access_token " + self.token,
                 "Content-Encoding": encoding,
-            }
+            },
         )
 
     @log_call
     @ask_token
     @prepare_encoding
     def create_instance_data_check(
         self,
@@ -435,25 +434,25 @@
         url = urljoin(urljoin(self.url, api) + "/", str(instance_id) + "/" + post_url)
         return requests.request(
             method="post",
             url=url,
             headers={
                 "Authorization": "access_token " + self.token,
                 "Content-Encoding": encoding,
-            }
+            },
         )
 
     @log_call
     @ask_token
     @prepare_encoding
     def create_case_data_check(
-            self,
-            case_id,
-            encoding=None,
-            run=True,
+        self,
+        case_id,
+        encoding=None,
+        run=True,
     ):
         """
         Creates an execution to check the instance and solution of a case
 
         :param str case_id: id for the case to check
         :param str encoding: the type of encoding used in the call. Defaults to 'br'
         :param bool run: if the execution should be run or not
@@ -465,15 +464,15 @@
         url = urljoin(urljoin(self.url, api) + "/", str(case_id) + "/" + post_url)
         return requests.request(
             method="post",
             url=url,
             headers={
                 "Authorization": "access_token " + self.token,
                 "Content-Encoding": encoding,
-            }
+            },
         )
 
     @ask_token
     @prepare_encoding
     def get_data(self, execution_id, encoding=None):
         """
         Downloads the data from an execution
@@ -550,17 +549,15 @@
     def get_results(self, execution_id, encoding=None):
         """
         Downloads results from an execution
 
         :param str execution_id: id for the execution
         :param str encoding: the type of encoding used in the call. Defaults to 'br'
         """
-        return self.get_api_for_id(
-            api="execution/", id=execution_id, encoding=encoding
-        )
+        return self.get_api_for_id(api="execution/", id=execution_id, encoding=encoding)
 
     @log_call
     @ask_token
     @prepare_encoding
     def get_status(self, execution_id, encoding=None):
         """
         Downloads the current status of an execution
@@ -684,17 +681,15 @@
         """
         Downloads header of an instance
 
         :param str reference_id: id for the instance
         :param str encoding: the type of encoding used in the call. Defaults to 'br'
 
         """
-        return self.get_api_for_id(
-            api="instance", id=reference_id, encoding=encoding
-        )
+        return self.get_api_for_id(api="instance", id=reference_id, encoding=encoding)
 
     @log_call
     @ask_token
     @prepare_encoding
     def get_one_instance_data(self, reference_id, encoding=None):
         """
         Downloads instance data
@@ -725,15 +720,17 @@
     def get_one_case_data(self, reference_id, encoding=None):
         """
         Downloads case data
 
         :param str reference_id: id for the case
         :param str encoding: the type of encoding used in the call. Defaults to 'br'
         """
-        return self.get_api_for_id(api="case", id=reference_id, post_url="data", encoding=encoding)
+        return self.get_api_for_id(
+            api="case", id=reference_id, post_url="data", encoding=encoding
+        )
 
     @log_call
     @ask_token
     @prepare_encoding
     def put_one_case(self, reference_id, payload, encoding=None):
         """
         Edits a case
@@ -811,17 +808,15 @@
     def delete_one_case(self, reference_id, encoding=None):
         """
         Deletes a case
 
         :param int reference_id: id for the case
         :param str encoding: the type of encoding used in the call. Defaults to 'br'
         """
-        return self.delete_api_for_id(
-            api="case", id=reference_id, encoding=encoding
-        )
+        return self.delete_api_for_id(api="case", id=reference_id, encoding=encoding)
 
     @log_call
     @ask_token
     @prepare_encoding
     def delete_one_execution(self, reference_id, encoding=None):
         """
         Deletes an execution
@@ -873,34 +868,36 @@
         name: str,
         instance_schema: dict,
         instance_checks_schema: dict,
         solution_schema: dict,
         solution_checks_schema: dict,
         config_schema: dict,
         description: str = None,
-        encoding=None
+        encoding=None,
     ):
         if name is None:
             return {"error": "No dag name was given"}
         payload = dict(
             id=name,
             description=description,
             instance_schema=instance_schema,
             solution_schema=solution_schema,
             instance_checks_schema=instance_checks_schema,
             solution_checks_schema=solution_checks_schema,
-            config_schema=config_schema
+            config_schema=config_schema,
         )
         return self.create_api("dag/deployed/", json=payload, encoding=encoding)
-    
+
     @log_call
     @ask_token
     @prepare_encoding
     def put_deployed_dag(self, dag_id, data, encoding=None):
-        return self.put_api_for_id("dag/deployed/", dag_id, payload=data, encoding=encoding)
+        return self.put_api_for_id(
+            "dag/deployed/", dag_id, payload=data, encoding=encoding
+        )
 
 
 class CornFlowApiError(Exception):
     """
     CornFlow returns an error
     """
```

### Comparing `cornflow-client-1.0.9/cornflow_client/schema/dictSchema.py` & `cornflow-client-1.1.0a1/cornflow_client/schema/dictSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 
 """
-# Full imports
 import re
 
-# Imports from internal modules
-from .dict_functions import gen_schema, ParameterSchema, sort_dict
 from cornflow_client.constants import JSON_TYPES, DATASCHEMA
+from .dict_functions import gen_schema, ParameterSchema, sort_dict
 
 
 class DictSchema:
     """
     A json-schema to dict-schema parser
     """
```

### Comparing `cornflow-client-1.0.9/cornflow_client/schema/dict_functions.py` & `cornflow-client-1.1.0a1/cornflow_client/schema/dict_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 
 """
-# Partial imports
-
 from functools import partial
+
 from marshmallow import Schema, fields, INCLUDE
 
-# Imports from internal modules
 from cornflow_client.constants import (
     BOOLEAN_TYPE,
     STRING_TYPE,
     INTEGER_TYPE,
     FLOAT_TYPE,
     BASIC_TYPES,
 )
```

### Comparing `cornflow-client-1.0.9/cornflow_client/schema/manager.py` & `cornflow-client-1.1.0a1/cornflow_client/schema/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """
 Class to help create and manage data schema and to validate json files.
 """
-# Full imports
-import os
 
-# Partial imports
+import os
 from copy import deepcopy
+
 from genson import SchemaBuilder
 from jsonschema import Draft7Validator
 
-
-# Imports form internal modules
-from .dictSchema import DictSchema
 from cornflow_client.core.tools import load_json, save_json
+from .dictSchema import DictSchema
 
 
 class SchemaManager:
     """
     A schema manager between json-schema, dict-schema and marshmallow
     """
 
@@ -165,15 +162,15 @@
         """
         Print the schema_dict in a json file.
 
         :param path: the path where to save the dict.format
 
         :return: nothing
         """
-        self.save_json(self.to_dict_schema(), path)
+        save_json(self.to_dict_schema(), path)
 
     def draft_schema_from(self, path, save_path=None):
         """
         Create a draft jsonschema from a json file of data.
 
         :param path: path to the json file.
         :param save_path: path where to save the generated schema.
@@ -286,18 +283,14 @@
 
         :param path: the path of the json file.json
 
         return the json content.
         """
         return load_json(path)
 
-    @staticmethod
-    def save_json(data, path):
-        return save_json(data, path)
-
     """
     Aliases:
     """
     dict_to_flask = to_marshmallow
     load_schema = from_filepath
     jsonschema_to_flask = to_marshmallow
     jsonschema_to_dict = to_dict_schema
```

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/const.py` & `cornflow-client-1.1.0a1/cornflow_client/tests/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/data_input_bad.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/data_input_bad.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/data_schema.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/data_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/gc_input.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/gc_input.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/gc_output.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/gc_output.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/graph_coloring_input.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/graph_coloring_input.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/hk_data_input.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_data_input.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/hk_data_schema.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_data_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/instance-hackathon2.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/instance-hackathon2.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/name_problem_schema.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/name_problem_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/pulp_example_data.json` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/pulp_example_data.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/data/test_mps.mps` & `cornflow-client-1.1.0a1/cornflow_client/tests/data/test_mps.mps`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/integration/test_airflow_integration.py` & `cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_airflow_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from cornflow_client.airflow.api import Airflow
 from cornflow_client.constants import STATUS_OPTIMAL, STATUS_NOT_SOLVED
 from cornflow_client.tests.const import PULP_EXAMPLE
 
 # Constants
 path_to_tests_dir = os.path.dirname(os.path.abspath(__file__))
 
+
 # Helper functions
 def _load_file(_file):
     with open(_file) as f:
         temp = json.load(f)
     return temp
 
 
@@ -53,15 +54,15 @@
     def test_update_dag_registry(self):
         response = self.client.update_dag_registry()
         self.assertEqual(200, response.status_code)
 
     def test_run_dag(self):
         data = _load_file(PULP_EXAMPLE)
         cf_client = CornFlow(url="http://127.0.0.1:5050/")
-        cf_login = cf_client.login("user", "UserPassword1!")
+        cf_login = cf_client.login("admin", "Adminpassword1!")
         instance = cf_client.create_instance(data, "test_example", "test_description")
         execution = cf_client.create_execution(
             instance_id=instance["id"],
             config={"solver": "PULP_CBC_CMD", "timeLimit": 100},
             name="test_execution",
             description="execution_description",
             schema="solve_model_dag",
```

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/integration/test_cornflow_integration.py` & `cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_cornflow_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """
 Integration test for the Cornflow client
 Base, admin and service user get tested
 Integration between Airflow and cornflow through airflow client and cornflow client tested as well
 """
-# Full imports
+
 import json
 import os
-import pulp as pl
 import time
-
-# Partial imports
 from unittest import TestCase
 
-# Internal imports
+import pulp as pl
+
 from cornflow_client import CornFlow
 from cornflow_client.constants import STATUS_OPTIMAL, STATUS_NOT_SOLVED, STATUS_QUEUED
 from cornflow_client.schema.tools import get_pulp_jsonschema
 from cornflow_client.tests.const import PUBLIC_DAGS, PULP_EXAMPLE
 
 # Constants
 path_to_tests_dir = os.path.dirname(os.path.abspath(__file__))
 
+
 # Helper functions
 def _load_file(_file):
     with open(_file) as f:
         temp = json.load(f)
     return temp
 
 
@@ -40,14 +39,24 @@
         self.assertIn("id", login_result.keys())
         self.assertIn("token", login_result.keys())
         self.user_id = login_result["id"]
 
     def tearDown(self):
         pass
 
+    def check_execution_statuses(self, execution_id):
+        statuses = []
+        response = self.client.get_status(execution_id)
+        statuses.append(response["state"])
+        while STATUS_OPTIMAL not in statuses and len(statuses) < 100:
+            time.sleep(2)
+            response = self.client.get_status(execution_id)
+            statuses.append(response["state"])
+        return statuses
+
     def test_health_endpoint(self):
         response = self.client.is_alive()
         self.assertEqual(response["cornflow_status"], "healthy")
         self.assertEqual(response["airflow_status"], "healthy")
 
     def test_sign_up(self):
         response = self.client.sign_up(
@@ -167,23 +176,26 @@
         )
         self.assertEqual(STATUS_QUEUED, response["state"])
 
         return response
 
     def test_create_execution_data_check(self):
         exec_to_check = self.test_create_execution()
-        time.sleep(15)
+        statuses = self.check_execution_statuses(exec_to_check["id"])
+
         exec_to_check_id = exec_to_check["id"]
         execution = self.client.create_execution_data_check(exec_to_check_id)
         self.assertEqual(STATUS_QUEUED, execution["state"])
         return execution
 
     def test_execution_data_check_solution(self):
         execution = self.test_create_execution_data_check()
-        time.sleep(15)
+
+        statuses = self.check_execution_statuses(execution["id"])
+
         results = self.client.get_solution(execution["id"])
         self.assertEqual(results["state"], 1)
 
     def test_create_instance_data_check(self):
         inst_to_check = self.test_create_instance()
         inst_to_check_id = inst_to_check["id"]
         execution = self.client.create_instance_data_check(inst_to_check_id)
@@ -203,15 +215,16 @@
         response = self.client.get_one_instance_data(
             reference_id=execution["instance_id"], encoding="br"
         )
         self.assertIsNotNone(response["checks"])
 
     def test_execution_results(self):
         execution = self.test_create_execution()
-        time.sleep(10)
+        statuses = self.check_execution_statuses(execution["id"])
+
         response = self.client.get_results(execution["id"])
 
         items = [
             "id",
             "name",
             "description",
             "created_at",
@@ -224,32 +237,29 @@
             "message",
         ]
 
         for item in items:
             self.assertIn(item, response.keys())
 
         self.assertEqual(execution["id"], response["id"])
-        self.assertEqual(STATUS_OPTIMAL, response["state"])
+        self.assertIn(STATUS_NOT_SOLVED, statuses)
+        self.assertIn(STATUS_OPTIMAL, statuses)
 
     def test_execution_status(self):
         execution = self.test_create_execution()
-        self.assertEqual(STATUS_QUEUED, execution["state"])
 
-        time.sleep(4)
-        response = self.client.get_status(execution["id"])
-        items = ["id", "state", "message", "data_hash"]
-        for item in items:
-            self.assertIn(item, response.keys())
-        self.assertEqual(STATUS_NOT_SOLVED, response["state"])
+        statuses = self.check_execution_statuses(execution["id"])
+
+        self.assertIn(STATUS_NOT_SOLVED, statuses)
+        self.assertIn(STATUS_OPTIMAL, statuses)
 
-        time.sleep(10)
+        items = ["id", "state", "message", "data_hash"]
         response = self.client.get_status(execution["id"])
         for item in items:
             self.assertIn(item, response.keys())
-        self.assertEqual(STATUS_OPTIMAL, response["state"])
 
     def test_stop_execution(self):
         execution = self.test_create_execution()
         response = self.client.stop_execution(execution["id"])
         self.assertEqual(response["message"], "The execution has been stopped")
 
     def test_get_execution_log(self):
@@ -273,15 +283,17 @@
 
         for item in items:
             self.assertIn(item, response.keys())
         self.assertEqual(execution["id"], response["id"])
 
     def test_get_execution_solution(self):
         execution = self.test_create_execution()
-        time.sleep(15)
+        response = self.client.get_status(execution["id"])
+        statuses = self.check_execution_statuses(execution["id"])
+
         response = self.client.get_solution(execution["id"])
         items = [
             "id",
             "name",
             "description",
             "created_at",
             "user_id",
@@ -295,21 +307,24 @@
             "checks",
         ]
 
         for item in items:
             self.assertIn(item, response.keys())
 
         self.assertEqual(execution["id"], response["id"])
-        self.assertEqual(STATUS_OPTIMAL, response["state"])
+        self.assertIn(STATUS_NOT_SOLVED, statuses)
+        self.assertIn(STATUS_OPTIMAL, statuses)
 
         return response
 
     def test_put_one_execution(self):
         execution = self.test_create_execution()
-        response = self.client.put_one_execution(execution["id"], {"name": "new_execution_name"})
+        response = self.client.put_one_execution(
+            execution["id"], {"name": "new_execution_name"}
+        )
         self.assertEqual("Updated correctly", response["message"])
 
     def test_delete_one_execution(self):
         execution = self.test_create_execution()
         response = self.client.delete_one_execution(execution["id"])
         self.assertEqual("The object has been deleted", response["message"])
 
@@ -386,36 +401,38 @@
             "schema",
             "executions",
         ]
 
         for item in items:
             self.assertIn(item, response.keys())
             self.assertEqual(instance[item], response[item])
-            
+
     def test_get_one_instance_data(self):
         instance = self.test_create_instance()
         response = self.client.get_one_instance_data(instance["id"])
         items = [
             "id",
             "name",
             "description",
             "created_at",
             "user_id",
             "data_hash",
-            "schema"
+            "schema",
         ]
 
         self.assertIn("data", response.keys())
         for item in items:
             self.assertIn(item, response.keys())
             self.assertEqual(instance[item], response[item])
 
     def test_put_one_instance(self):
         instance = self.test_create_instance()
-        response = self.client.put_one_instance(instance["id"], {"name": "new_instance_name"})
+        response = self.client.put_one_instance(
+            instance["id"], {"name": "new_instance_name"}
+        )
         self.assertEqual("Updated correctly", response["message"])
 
     def test_get_one_case(self):
         case = self.test_create_case()
         response = self.client.get_one_case(case["id"])
         items = [
             "id",
@@ -430,15 +447,15 @@
             "updated_at",
             "is_dir",
         ]
 
         for item in items:
             self.assertIn(item, response.keys())
             self.assertEqual(case[item], response[item])
-            
+
     def test_get_one_case_data(self):
         case = self.test_create_case()
         response = self.client.get_one_case_data(case["id"])
         items = [
             "id",
             "name",
             "description",
@@ -504,15 +521,15 @@
             "instance": get_pulp_jsonschema(),
             "solution": get_pulp_jsonschema(),
         }
 
         schema["config"]["properties"]["solver"]["enum"] = pl.listSolvers()
         schema["config"]["properties"]["solver"]["default"] = "PULP_CBC_CMD"
 
-        for (key, value) in schema.items():
+        for key, value in schema.items():
             self.assertDictEqual(value, response[key])
 
     def test_get_all_schemas(self):
         response = self.client.get_all_schemas()
         read_schemas = [dag for v in response for (_, dag) in v.items()]
 
         for schema in PUBLIC_DAGS:
@@ -614,23 +631,22 @@
 
         deployed_dags = [v["id"] for v in response]
 
         for dag in PUBLIC_DAGS:
             self.assertIn(dag, deployed_dags)
 
     def test_post_deployed_dag(self):
-
         response = self.client.create_deployed_dag(
             name="test_dag",
             description="test_dag_description",
             instance_schema=dict(),
             instance_checks_schema=dict(),
             solution_schema=dict(),
             solution_checks_schema=dict(),
-            config_schema=dict()
+            config_schema=dict(),
         )
 
         items = ["id", "description"]
 
         for item in items:
             self.assertIn(item, response.keys())
         self.assertEqual("test_dag", response["id"])
```

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/integration/test_raw_cornflow_integration.py` & `cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_raw_cornflow_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """
 Integration test for the Cornflow client
 Base, admin and service user get tested
 Integration between Airflow and cornflow through airflow client and cornflow client tested as well
 """
-# Full imports
+
 import json
 import os
-import pulp as pl
 import time
-
-# Partial imports
 from unittest import TestCase
 
-# Internal imports
+import pulp as pl
+
 from cornflow_client import CornFlow
 from cornflow_client.constants import STATUS_OPTIMAL, STATUS_NOT_SOLVED, STATUS_QUEUED
 from cornflow_client.schema.tools import get_pulp_jsonschema
 from cornflow_client.tests.const import PUBLIC_DAGS, PULP_EXAMPLE
 
 # Constants
 path_to_tests_dir = os.path.dirname(os.path.abspath(__file__))
 
+
 # Helper functions
 def _load_file(_file):
     with open(_file) as f:
         temp = json.load(f)
     return temp
 
 
@@ -42,14 +41,40 @@
         self.assertIn("id", data.keys())
         self.assertIn("token", data.keys())
         self.user_id = data["id"]
 
     def tearDown(self):
         pass
 
+    def check_execution_statuses(
+        self, execution_id, end_state=STATUS_OPTIMAL, initial_state=None
+    ):
+        if initial_state is None:
+            statuses = [initial_state]
+        else:
+            statuses = []
+        response = self.client.raw.get_status(execution_id)
+        statuses.append(response.json()["state"])
+        while end_state not in statuses and len(statuses) < 100:
+            time.sleep(2)
+            response = self.client.raw.get_status(execution_id)
+            statuses.append(response.json()["state"])
+
+        self.assertIn(STATUS_QUEUED, statuses)
+        self.assertIn(STATUS_NOT_SOLVED, statuses)
+        self.assertIn(end_state, statuses)
+
+        queued_idx = statuses.index(STATUS_QUEUED)
+        not_solved_idx = statuses.index(STATUS_NOT_SOLVED)
+        end_state_idx = statuses.index(end_state)
+        self.assertLess(queued_idx, not_solved_idx)
+        self.assertLess(not_solved_idx, end_state_idx)
+
+        return statuses
+
     def test_health_endpoint(self):
         response = self.client.raw.is_alive()
         self.assertEqual(response.status_code, 200)
         data = response.json()
         self.assertEqual(data["cornflow_status"], "healthy")
         self.assertEqual(data["airflow_status"], "healthy")
 
@@ -60,15 +85,17 @@
         data = response.json()
         self.assertIn("id", data.keys())
         self.assertIn("token", data.keys())
         self.assertEqual(201, response.status_code)
 
     def test_create_instance(self):
         data = _load_file(PULP_EXAMPLE)
-        response = self.client.raw.create_instance(data, "test_example", "test_description")
+        response = self.client.raw.create_instance(
+            data, "test_example", "test_description"
+        )
         self.assertEqual(response.status_code, 201)
         instance = response.json()
 
         items = [
             "id",
             "name",
             "description",
@@ -179,24 +206,30 @@
         )
         self.assertEqual(STATUS_QUEUED, execution["state"])
 
         return execution
 
     def test_create_execution_data_check(self):
         exec_to_check = self.test_create_execution()
-        time.sleep(15)
+
+        statuses = self.check_execution_statuses(exec_to_check["id"])
+
         exec_to_check_id = exec_to_check["id"]
         response = self.client.raw.create_execution_data_check(exec_to_check_id)
         execution = response.json()
         self.assertEqual(STATUS_QUEUED, execution["state"])
         return execution
 
     def test_execution_data_check_solution(self):
         execution = self.test_create_execution_data_check()
-        time.sleep(15)
+
+        statuses = self.check_execution_statuses(
+            execution["id"], initial_state=execution["state"]
+        )
+
         results = self.client.raw.get_solution(execution["id"])
         self.assertEqual(results.status_code, 200)
         self.assertEqual(results.json()["state"], 1)
 
     def test_create_instance_data_check(self):
         inst_to_check = self.test_create_instance()
         inst_to_check_id = inst_to_check["id"]
@@ -221,15 +254,17 @@
             api="instance", id=execution["instance_id"], post_url="data", encoding="br"
         )
         self.assertEqual(response.status_code, 200)
         self.assertIsNotNone(response.json()["checks"])
 
     def test_execution_results(self):
         execution = self.test_create_execution()
-        time.sleep(10)
+
+        statuses = self.check_execution_statuses(execution["id"])
+
         response = self.client.raw.get_results(execution["id"])
         self.assertEqual(response.status_code, 200)
         response = response.json()
 
         items = [
             "id",
             "name",
@@ -244,35 +279,29 @@
             "message",
         ]
 
         for item in items:
             self.assertIn(item, response.keys())
 
         self.assertEqual(execution["id"], response["id"])
-        self.assertEqual(STATUS_OPTIMAL, response["state"])
+        self.assertIn(STATUS_NOT_SOLVED, statuses)
+        self.assertIn(STATUS_OPTIMAL, statuses)
 
     def test_execution_status(self):
         execution = self.test_create_execution()
-        self.assertEqual(STATUS_QUEUED, execution["state"])
 
-        time.sleep(4)
-        response = self.client.raw.get_status(execution["id"])
-        self.assertEqual(response.status_code, 200)
-        response = response.json()
-        items = ["id", "state", "message", "data_hash"]
-        for item in items:
-            self.assertIn(item, response.keys())
-        self.assertEqual(STATUS_NOT_SOLVED, response["state"])
+        statuses = self.check_execution_statuses(execution["id"])
+
+        self.assertIn(STATUS_NOT_SOLVED, statuses)
+        self.assertIn(STATUS_OPTIMAL, statuses)
 
-        time.sleep(10)
+        items = ["id", "state", "message", "data_hash"]
         response = self.client.raw.get_status(execution["id"])
-        self.assertEqual(response.status_code, 200)
         for item in items:
             self.assertIn(item, response.json().keys())
-        self.assertEqual(STATUS_OPTIMAL, response.json()["state"])
 
     def test_stop_execution(self):
         execution = self.test_create_execution()
         response = self.client.raw.stop_execution(execution["id"])
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.json()["message"], "The execution has been stopped")
 
@@ -298,15 +327,17 @@
 
         for item in items:
             self.assertIn(item, response.keys())
         self.assertEqual(execution["id"], response["id"])
 
     def test_get_execution_solution(self):
         execution = self.test_create_execution()
-        time.sleep(15)
+
+        statuses = self.check_execution_statuses(execution["id"])
+
         response = self.client.raw.get_solution(execution["id"])
         self.assertEqual(response.status_code, 200)
         response = response.json()
         items = [
             "id",
             "name",
             "description",
@@ -322,21 +353,24 @@
             "checks",
         ]
 
         for item in items:
             self.assertIn(item, response.keys())
 
         self.assertEqual(execution["id"], response["id"])
-        self.assertEqual(STATUS_OPTIMAL, response["state"])
+        self.assertIn(STATUS_NOT_SOLVED, statuses)
+        self.assertIn(STATUS_OPTIMAL, statuses)
 
         return response
 
     def test_put_one_execution(self):
         execution = self.test_create_execution()
-        response = self.client.raw.put_one_execution(execution["id"], {"name": "new_execution_name"})
+        response = self.client.raw.put_one_execution(
+            execution["id"], {"name": "new_execution_name"}
+        )
         self.assertEqual(200, response.status_code)
         self.assertEqual("Updated correctly", response.json()["message"])
 
     def test_delete_one_execution(self):
         execution = self.test_create_execution()
         response = self.client.raw.delete_one_execution(execution["id"])
         self.assertEqual(200, response.status_code)
@@ -436,25 +470,27 @@
         items = [
             "id",
             "name",
             "description",
             "created_at",
             "user_id",
             "data_hash",
-            "schema"
+            "schema",
         ]
 
         self.assertIn("data", response.keys())
         for item in items:
             self.assertIn(item, response.keys())
             self.assertEqual(instance[item], response[item])
 
     def test_put_one_instance(self):
         instance = self.test_create_instance()
-        response = self.client.raw.put_one_instance(instance["id"], {"name": "new_instance_name"})
+        response = self.client.raw.put_one_instance(
+            instance["id"], {"name": "new_instance_name"}
+        )
         self.assertEqual(response.status_code, 200)
         self.assertEqual("Updated correctly", response.json()["message"])
 
     def test_get_one_case(self):
         case = self.test_create_case()
         response = self.client.raw.get_one_case(case["id"])
         self.assertEqual(response.status_code, 200)
@@ -555,15 +591,15 @@
             "instance": get_pulp_jsonschema(),
             "solution": get_pulp_jsonschema(),
         }
 
         schema["config"]["properties"]["solver"]["enum"] = pl.listSolvers()
         schema["config"]["properties"]["solver"]["default"] = "PULP_CBC_CMD"
 
-        for (key, value) in schema.items():
+        for key, value in schema.items():
             self.assertDictEqual(value, response[key])
 
     def test_get_all_schemas(self):
         response = self.client.raw.get_all_schemas()
         read_schemas = [dag for v in response.json() for (_, dag) in v.items()]
 
         for schema in PUBLIC_DAGS:
@@ -610,15 +646,17 @@
     def tearDown(self):
         pass
 
     def test_get_execution_data(self):
         client = CornFlow(url="http://127.0.0.1:5050/")
         _ = client.login("user", "UserPassword1!")
         data = _load_file(PULP_EXAMPLE)
-        instance = client.raw.create_instance(data, "test_example", "test_description").json()
+        instance = client.raw.create_instance(
+            data, "test_example", "test_description"
+        ).json()
         execution = client.raw.create_execution(
             instance_id=instance["id"],
             config={"solver": "PULP_CBC_CMD", "timeLimit": 60},
             name="test_execution",
             description="execution_description",
             schema="solve_model_dag",
         ).json()
@@ -634,15 +672,17 @@
         self.assertEqual(data, response["data"])
         self.assertEqual(execution["config"], response["config"])
 
     def test_write_execution_solution(self):
         client = CornFlow(url="http://127.0.0.1:5050/")
         _ = client.login("user", "UserPassword1!")
         data = _load_file(PULP_EXAMPLE)
-        instance = client.raw.create_instance(data, "test_example", "test_description").json()
+        instance = client.raw.create_instance(
+            data, "test_example", "test_description"
+        ).json()
         execution = client.raw.create_execution(
             instance_id=instance["id"],
             config={"solver": "PULP_CBC_CMD", "timeLimit": 60},
             name="test_execution",
             description="execution_description",
             schema="solve_model_dag",
         ).json()
@@ -670,26 +710,25 @@
 
         deployed_dags = [v["id"] for v in response]
 
         for dag in PUBLIC_DAGS:
             self.assertIn(dag, deployed_dags)
 
     def test_post_deployed_dag(self):
-
         response = self.client.raw.create_deployed_dag(
             name="test_dag_2",
             description="test_dag_2_description",
             instance_schema=dict(),
             instance_checks_schema=dict(),
             solution_schema=dict(),
             solution_checks_schema=dict(),
-            config_schema=dict()
+            config_schema=dict(),
         )
         self.assertEqual(response.status_code, 201)
         response = response.json()
 
         items = ["id", "description"]
 
         for item in items:
             self.assertIn(item, response.keys())
         self.assertEqual("test_dag_2", response["id"])
-        self.assertEqual("test_dag_2_description", response["description"])
+        self.assertEqual("test_dag_2_description", response["description"])
```

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/unit/test_abc.py` & `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.assertRaises(BadInstance, must_fail)
 
     def test_check_data(self):
         inst_check, sol_check, log = GoodApp().check(dict(number=""), dict())
         self.assertIsInstance(inst_check, dict)
         self.assertIsInstance(sol_check, dict)
         self.assertIsInstance(log, dict)
-        self.assertEqual(log.get('status'), "Optimal")
+        self.assertEqual(log.get("status"), "Optimal")
 
 
 class GoodInstanceClass(InstanceCore):
     schema = get_empty_schema(dict(number=dict(type="number")))
     schema_checks = get_empty_schema()
 
     def check(self) -> dict:
```

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/unit/test_dag_utilities.py` & `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_dag_utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,14 @@
                 "http://airflow:airflow_test_password@localhost:5000",
                 ("airflow", "airflow_test_password"),
                 "http://localhost:5000",
             ),
         ]
         client_instance = CornFlow.return_value
         client_instance.login.return_value = ""
-        for (conn_str, user_info, url) in conn_uris:
-            secrets.get_conn_uri.return_value = conn_str
+        for conn_str, user_info, url in conn_uris:
+            secrets.get_conn_value.return_value = conn_str
             du.connect_to_cornflow(secrets)
             client_instance.login.assert_called_with(
                 username=user_info[0], pwd=user_info[1]
             )
             CornFlow.assert_called_with(url=url)
```

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/unit/test_instance_solution_methods.py` & `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_instance_solution_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import os
 import pickle
 from datetime import datetime, timedelta
 from unittest import TestCase
 from cornflow_client.core import InstanceSolutionCore
 
-from cornflow_client import InstanceCore
+from cornflow_client import InstanceCore, ExperimentCore
 
 from cornflow_client.schema.tools import get_empty_schema
 
 
 # Constants
 path_to_tests_dir = os.path.dirname(os.path.abspath(__file__))
 
@@ -274,15 +274,15 @@
     def test_get_week_from_date_string(self):
         string = "2022-01-01"
         result = InstanceSolutionCore.get_week_from_date_string(string)
         expected = 52
         self.assertEqual(result, expected)
 
     def test_get_week_from_datetime_string(self):
-        string = "2022-01-01T12:00:00"
+        string = "2022-01-01T12:00"
         result = InstanceSolutionCore.get_week_from_datetime_string(string)
         expected = 52
         self.assertEqual(result, expected)
 
     def test_get_week_from_datetimesec_string(self):
         string = "2022-01-01T12:00:00"
         result = InstanceSolutionCore.get_week_from_datetimesec_string(string)
@@ -343,14 +343,49 @@
     def test_instance_from_json(self):
         """Here as to be not equal as the data has been processed on the from_dict method"""
         instance = self.class_to_use.from_json(self.instance_filename)
         self.assertNotEqual(self.instance_data, instance.data)
         return instance
 
 
+class TestExperimentCore(TestCase):
+    def setUp(self):
+        self.class_to_use = SimpleExperiment
+        self.schema = get_empty_schema()
+
+    def test_get_solver_config_pulp(self):
+        initial_config = {
+            "solver": "mip.GUROBI_CMD",
+            "timeLimit": 10,
+            "iteration_limit": 10
+        }
+        res = self.class_to_use.get_solver_config(initial_config, lib="pulp")
+        self.assertEqual(res, {'timeLimit': 10, 'IterationLimit': 10})
+
+    def test_get_solver_config_pyomo(self):
+        initial_config = {
+            "solver": "mip.scip",
+            "timeLimit": 10,
+            "iteration_limit": 10
+        }
+        res = self.class_to_use.get_solver_config(initial_config)
+        self.assertEqual(res, {"limits/time": 10, "lp/iterlim": 10})
+
+    def test_get_solver_config_pyomo_2(self):
+        initial_config = {
+            "solver": "mip.scip",
+            "solver_config": {
+                "timeLimit": 10,
+                "iteration_limit": 10
+            }
+        }
+        res = self.class_to_use.get_solver_config(initial_config)
+        self.assertEqual(res, {"limits/time": 10, "lp/iterlim": 10})
+
+
 class SimpleInstance(InstanceCore):
     schema = get_empty_schema()
     schema_checks = get_empty_schema()
 
 
 class Instance(InstanceCore):
     schema = _load_file(_get_file("../data/graph_coloring_input.json"))
@@ -365,7 +400,20 @@
         return cls(data_p)
 
     def to_dict(self):
         tables = ["pairs"]
 
         data_p = {el: self.data[el].values_l() for el in tables}
         return pickle.loads(pickle.dumps(data_p, -1))
+
+
+class SimpleExperiment(ExperimentCore):
+    schema_checks = get_empty_schema()
+
+    def solve(self) -> dict:
+        return 0, 0
+
+    def get_objective(self) -> float:
+        return 0
+
+    def check_solution(self):
+        return dict()
```

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/unit/test_schema_manager.py` & `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client/tests/unit/test_varnames.py` & `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_varnames.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.9/cornflow_client.egg-info/PKG-INFO` & `cornflow-client-1.1.0a1/cornflow_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cornflow-client
-Version: 1.0.9
+Version: 1.1.0a1
 Summary: Client to connect to a cornflow server
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow client
         ================
         
         The aim of this repository is to have a client to use to connect to a deployed cornflow webserver
         
         Requirements
         ~~~~~~~~~~~~
         
-        * python >= 3.6
+        * python >= 3.8
         
         Install cornflow-client
         ~~~~~~~~~~~~~~~~~~~~~~~~
         
         To install the package do::
         
             python3 -m pip install cornflow-client
@@ -43,10 +43,10 @@
             status = client.get_status(execution_id)
             results = client.get_results(execution_id)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `cornflow-client-1.0.9/cornflow_client.egg-info/SOURCES.txt` & `cornflow-client-1.1.0a1/cornflow_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,38 @@
 cornflow_client/schema/manager.py
 cornflow_client/schema/tools.py
 cornflow_client/tests/__init__.py
 cornflow_client/tests/const.py
 cornflow_client/tests/data/__init__.py
 cornflow_client/tests/data/data_input_bad.json
 cornflow_client/tests/data/data_schema.json
+cornflow_client/tests/data/endpoints_access.json
+cornflow_client/tests/data/endpoints_methods.json
 cornflow_client/tests/data/gc_input.json
 cornflow_client/tests/data/gc_output.json
 cornflow_client/tests/data/graph_coloring_input.json
 cornflow_client/tests/data/graph_coloring_output.json
 cornflow_client/tests/data/hk_data_input.json
 cornflow_client/tests/data/hk_data_schema.json
 cornflow_client/tests/data/hk_solution_schema.json
 cornflow_client/tests/data/instance-hackathon2.json
 cornflow_client/tests/data/name_problem_schema.json
 cornflow_client/tests/data/pulp_example_data.json
+cornflow_client/tests/data/schema_with_fk.json
+cornflow_client/tests/data/schema_without_fk.json
 cornflow_client/tests/data/test_mps.mps
+cornflow_client/tests/data/xl_with_access.xlsx
+cornflow_client/tests/data/xl_with_fk.xlsx
+cornflow_client/tests/data/xl_with_methods.xlsx
+cornflow_client/tests/data/xl_without_fk.xlsx
 cornflow_client/tests/integration/__init__.py
 cornflow_client/tests/integration/test_airflow_integration.py
 cornflow_client/tests/integration/test_cornflow_integration.py
 cornflow_client/tests/integration/test_raw_cornflow_integration.py
 cornflow_client/tests/unit/__init__.py
 cornflow_client/tests/unit/test_abc.py
+cornflow_client/tests/unit/test_core.py
 cornflow_client/tests/unit/test_dag_utilities.py
 cornflow_client/tests/unit/test_instance_solution_methods.py
+cornflow_client/tests/unit/test_schema_from_excel.py
 cornflow_client/tests/unit/test_schema_manager.py
 cornflow_client/tests/unit/test_varnames.py
```

### Comparing `cornflow-client-1.0.9/setup.py` & `cornflow-client-1.1.0a1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,26 +8,26 @@
     required.append(fh.read().splitlines())
 
 extra_required = {"excel": ["openpyxl", "pandas"]}
 
 
 setuptools.setup(
     name="cornflow-client",
-    version="1.0.9",
+    version="1.1.0a1",
     author="baobab soluciones",
     author_email="sistemas@baobabsoluciones.es",
     description="Client to connect to a cornflow server",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/baobabsoluciones/cornflow",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     include_package_data=True,
     install_requires=required,
     extra_require=extra_required,
 )
```

