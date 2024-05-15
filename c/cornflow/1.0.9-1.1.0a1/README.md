# Comparing `tmp/cornflow-1.0.9.tar.gz` & `tmp/cornflow-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornflow-1.0.9.tar", last modified: Wed Dec 27 10:12:58 2023, max compression
+gzip compressed data, was "cornflow-1.1.0a1.tar", last modified: Wed May 15 17:22:07 2024, max compression
```

## Comparing `cornflow-1.0.9.tar` & `cornflow-1.1.0a1.tar`

### file list

```diff
@@ -1,200 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.053682 cornflow-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-27 10:12:56.000000 cornflow-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10046 2023-12-27 10:12:58.053682 cornflow-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2023-12-27 10:12:56.000000 cornflow-1.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.025682 cornflow-1.0.9/airflow_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/airflow_local_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/airflow_config/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/airflow_config/plugins/XCom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/plugins/XCom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/plugins/XCom/gce_xcom_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/webserver_ldap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/cornflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/cornflow/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.033682 cornflow-1.0.9/cornflow/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16344 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/api_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12640 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/endpoint_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/models_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/schema_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/schemas_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.033682 cornflow-1.0.9/cornflow/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.037682 cornflow-1.0.9/cornflow/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/apiview.py
--rw-r--r--   0 runner    (1001) docker     (127)    18670 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/case.py
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/data_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    27951 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    11615 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/meta_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/signup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/gunicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.037682 cornflow-1.0.9/cornflow/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.041682 cornflow-1.0.9/cornflow/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/00757b557b02_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/1af47a419bbd_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/4aac5e0c6e66_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/7c3ea5ab5501_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/a472b5ad50b7_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/c2db9409cb5f_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/c8a6c762e818_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/ca449af8034c_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/d0e0700dcd8e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/d1b5be1f0549_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/e1a50dae1ac9_.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/e937a5234ce4_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/ebdd955fcc5e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/f3bee20314a2_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.041682 cornflow-1.0.9/cornflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/base_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/dag_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12000 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/meta_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.045682 cornflow-1.0.9/cornflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/case.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/model_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/solution_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/shared/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/shared/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18621 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/authentication/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/authentication/ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/query_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/utils_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/custom_liveServer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24777 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/custom_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/integration/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    20646 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/integration/test_cornflowclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/tests/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/ldap/test_ldap_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.053682 cornflow-1.0.9/cornflow/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_apiview.py
--rw-r--r--   0 runner    (1001) docker     (127)    23985 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_dags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_data_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_executions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15376 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_generate_from_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_instances_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_log_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16581 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_schema_from_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7177 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_sign_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    21677 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/cornflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10046 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-12-27 10:12:58.000000 cornflow-1.0.9/cornflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 10:12:58.053682 cornflow-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-27 10:12:56.000000 cornflow-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.271705 cornflow-1.1.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-15 17:22:07.271705 cornflow-1.1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/airflow_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/airflow_local_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/airflow_config/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/airflow_config/plugins/XCom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/plugins/XCom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/plugins/XCom/gce_xcom_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/webserver_ldap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/cornflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.251704 cornflow-1.1.0a1/cornflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.251704 cornflow-1.1.0a1/cornflow/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16344 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/api_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12640 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/endpoint_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/models_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/schema_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/schemas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.251704 cornflow-1.1.0a1/cornflow/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.255704 cornflow-1.1.0a1/cornflow/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/apiview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18670 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/data_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27998 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/meta_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/signup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/gunicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.255704 cornflow-1.1.0a1/cornflow/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.255704 cornflow-1.1.0a1/cornflow/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/00757b557b02_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/1af47a419bbd_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/4aac5e0c6e66_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/7c3ea5ab5501_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/991b98e24225_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/a472b5ad50b7_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/c2db9409cb5f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/c8a6c762e818_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/ca449af8034c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/d0e0700dcd8e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/d1b5be1f0549_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/e1a50dae1ac9_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/e937a5234ce4_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/ebdd955fcc5e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/f3bee20314a2_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.259704 cornflow-1.1.0a1/cornflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/base_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/dag_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/meta_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/model_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/solution_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/shared/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/authentication/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/authentication/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/query_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/utils_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/custom_liveServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25147 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/custom_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/integration/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20963 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/integration/test_cornflowclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.267705 cornflow-1.1.0a1/cornflow/tests/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/ldap/test_ldap_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.267705 cornflow-1.1.0a1/cornflow/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_apiview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25974 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_dags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_data_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17501 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_executions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15376 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_generate_from_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_instances_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_log_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_schema_from_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22430 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/cornflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-15 17:22:07.000000 cornflow-1.1.0a1/cornflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:22:07.271705 cornflow-1.1.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/setup.py
```

### Comparing `cornflow-1.0.9/PKG-INFO` & `cornflow-1.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cornflow
-Version: 1.0.9
+Version: 1.1.0a1
 Summary: Cornflow is an open source multi-solver optimization server with a REST API built using flask.
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: cornflow@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow
         =========
```

### Comparing `cornflow-1.0.9/README.rst` & `cornflow-1.1.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/airflow_config/airflow_local_settings.py` & `cornflow-1.1.0a1/airflow_config/airflow_local_settings.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/airflow_config/plugins/XCom/gce_xcom_backend.py` & `cornflow-1.1.0a1/airflow_config/plugins/XCom/gce_xcom_backend.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/airflow_config/webserver_ldap.py` & `cornflow-1.1.0a1/airflow_config/webserver_ldap.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/app.py` & `cornflow-1.1.0a1/cornflow/app.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/__init__.py` & `cornflow-1.1.0a1/cornflow/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/arguments.py` & `cornflow-1.1.0a1/cornflow/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/config.py` & `cornflow-1.1.0a1/cornflow/cli/config.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/migrations.py` & `cornflow-1.1.0a1/cornflow/cli/migrations.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/permissions.py` & `cornflow-1.1.0a1/cornflow/cli/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/schemas.py` & `cornflow-1.1.0a1/cornflow/cli/schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/service.py` & `cornflow-1.1.0a1/cornflow/cli/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from cornflow.app import create_app
 from cornflow.commands import (
     access_init_command,
     create_user_with_role,
     register_deployed_dags_command,
     register_dag_permissions_command,
     update_schemas_command,
+    update_dag_registry_command,
 )
 from cornflow.shared.const import AUTH_DB, ADMIN_ROLE, SERVICE_ROLE
 from cornflow.shared import db
 from cryptography.fernet import Fernet
 from flask_migrate import Migrate, upgrade
 
 
@@ -207,14 +208,17 @@
                     verbose=True,
                 )
             register_deployed_dags_command(
                 airflow_url, airflow_user, airflow_pwd, verbose=True
             )
             register_dag_permissions_command(open_deployment, verbose=True)
             update_schemas_command(airflow_url, airflow_user, airflow_pwd, verbose=True)
+            update_dag_registry_command(
+                airflow_url, airflow_user, airflow_pwd, verbose=True
+            )
 
         os.system(
             f"/usr/local/bin/gunicorn -c python:cornflow.gunicorn "
             f"\"$EXTERNAL_APP_MODULE:create_wsgi_app('$FLASK_ENV')\""
         )
 
     else:
```

### Comparing `cornflow-1.0.9/cornflow/cli/tools/api_generator.py` & `cornflow-1.1.0a1/cornflow/cli/tools/api_generator.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/tools/endpoint_tools.py` & `cornflow-1.1.0a1/cornflow/cli/tools/endpoint_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/tools/models_tools.py` & `cornflow-1.1.0a1/cornflow/cli/tools/models_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/tools/schema_generator.py` & `cornflow-1.1.0a1/cornflow/cli/tools/schema_generator.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/tools/schemas_tools.py` & `cornflow-1.1.0a1/cornflow/cli/tools/schemas_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/tools/tools.py` & `cornflow-1.1.0a1/cornflow/cli/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/users.py` & `cornflow-1.1.0a1/cornflow/cli/users.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/utils.py` & `cornflow-1.1.0a1/cornflow/cli/utils.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/cli/views.py` & `cornflow-1.1.0a1/cornflow/cli/views.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/commands/__init__.py` & `cornflow-1.1.0a1/cornflow/commands/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .actions import register_actions_command
 from .dag import register_deployed_dags_command
 from .permissions import (
     register_base_permissions_command,
     register_dag_permissions_command,
 )
 from .roles import register_roles_command
-from .schemas import update_schemas_command
+from .schemas import update_schemas_command, update_dag_registry_command
 from .users import (
     create_user_with_role,
     create_service_user_command,
     create_admin_user_command,
     create_planner_user_command,
 )
 from .views import register_views_command
```

### Comparing `cornflow-1.0.9/cornflow/commands/access.py` & `cornflow-1.1.0a1/cornflow/commands/access.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/commands/actions.py` & `cornflow-1.1.0a1/cornflow/commands/actions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/commands/dag.py` & `cornflow-1.1.0a1/cornflow/commands/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/commands/permissions.py` & `cornflow-1.1.0a1/cornflow/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/commands/roles.py` & `cornflow-1.1.0a1/cornflow/commands/roles.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/commands/schemas.py` & `cornflow-1.1.0a1/cornflow/commands/schemas.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,7 +23,38 @@
         if verbose:
             current_app.logger.info("DAGs schemas updated")
     else:
         if verbose:
             current_app.logger.info("The DAGs schemas were not updated properly")
 
     return True
+
+
+def update_dag_registry_command(url, user, pwd, verbose: bool = False):
+    import time
+    from flask import current_app
+
+    from cornflow_client.airflow.api import Airflow
+
+    af_client = Airflow(url, user, pwd)
+    max_attempts = 20
+    attempts = 0
+    while not af_client.is_alive() and attempts < max_attempts:
+        attempts += 1
+        if verbose == 1:
+            current_app.logger.info(f"Airflow is not reachable (attempt {attempts})")
+        time.sleep(15)
+
+    if not af_client.is_alive():
+        if verbose == 1:
+            current_app.logger.info("Airflow is not reachable")
+        return False
+
+    response = af_client.update_dag_registry()
+    if response.status_code == 200:
+        if verbose:
+            current_app.logger.info("DAGs schemas updated on cornflow")
+    else:
+        if verbose:
+            current_app.logger.info("The DAGs schemas were not updated properly")
+
+    return True
```

### Comparing `cornflow-1.0.9/cornflow/commands/users.py` & `cornflow-1.1.0a1/cornflow/commands/users.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/commands/views.py` & `cornflow-1.1.0a1/cornflow/commands/views.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/config.py` & `cornflow-1.1.0a1/cornflow/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,20 @@
     SERVICE_EMAIL_PASSWORD = os.getenv("SERVICE_EMAIL_PASSWORD", None)
     SERVICE_EMAIL_SERVER = os.getenv("SERVICE_EMAIL_SERVER", None)
     SERVICE_EMAIL_PORT = os.getenv("SERVICE_EMAIL_PORT", None)
 
     # Alarms endpoints
     ALARMS_ENDPOINTS = os.getenv("CF_ALARMS_ENDPOINT", 0)
 
+    # Token duration in hours
+    TOKEN_DURATION = os.getenv("TOKEN_DURATION", 24)
+
+    # Password rotation time in days
+    PWD_ROTATION_TIME = os.getenv("PWD_ROTATION_TIME", 120)
+
 
 class Development(DefaultConfig):
 
     """ """
 
     ENV = "development"
```

### Comparing `cornflow-1.0.9/cornflow/endpoints/__init__.py` & `cornflow-1.1.0a1/cornflow/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/action.py` & `cornflow-1.1.0a1/cornflow/endpoints/action.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/alarms.py` & `cornflow-1.1.0a1/cornflow/endpoints/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/apiview.py` & `cornflow-1.1.0a1/cornflow/endpoints/apiview.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/case.py` & `cornflow-1.1.0a1/cornflow/endpoints/case.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/dag.py` & `cornflow-1.1.0a1/cornflow/endpoints/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/data_check.py` & `cornflow-1.1.0a1/cornflow/endpoints/data_check.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/example_data.py` & `cornflow-1.1.0a1/cornflow/endpoints/example_data.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/execution.py` & `cornflow-1.1.0a1/cornflow/endpoints/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     ExecutionLogEndpointResponse,
     ExecutionStatusEndpointResponse,
     ExecutionStatusEndpointUpdate,
     ExecutionRequest,
     ExecutionEditRequest,
     QueryFiltersExecution,
     ReLaunchExecutionRequest,
+    ExecutionDetailsWithIndicatorsAndLogResponse
 )
 from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.compress import compressed
 from cornflow.shared.const import (
     EXEC_STATE_RUNNING,
     EXEC_STATE_ERROR,
     EXEC_STATE_ERROR_START,
@@ -54,15 +55,15 @@
         super().__init__()
         self.model = ExecutionModel
         self.data_model = ExecutionModel
         self.foreign_data = {"instance_id": InstanceModel}
 
     @doc(description="Get all executions", tags=["Executions"])
     @authenticate(auth_class=Auth())
-    @marshal_with(ExecutionDetailsEndpointWithIndicatorsResponse(many=True))
+    @marshal_with(ExecutionDetailsWithIndicatorsAndLogResponse(many=True))
     @use_kwargs(QueryFiltersExecution, location="query")
     def get(self, **kwargs):
         """
         API method to get all the executions created by the user and its related info
         It requires authentication to be passed in the form of a token that has to be linked to
         an existing session (login) made by a user
```

### Comparing `cornflow-1.0.9/cornflow/endpoints/health.py` & `cornflow-1.1.0a1/cornflow/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/instance.py` & `cornflow-1.1.0a1/cornflow/endpoints/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/licenses.py` & `cornflow-1.1.0a1/cornflow/endpoints/licenses.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/login.py` & `cornflow-1.1.0a1/cornflow/endpoints/login.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 External endpoint for the user to login to the cornflow webserver
 """
 
 # Partial imports
 from flask import current_app
 from flask_apispec import use_kwargs, doc
 from sqlalchemy.exc import IntegrityError, DBAPIError
+from datetime import datetime, timedelta
 
 # Import from internal modules
 from cornflow.endpoints.meta_resource import BaseMetaResource
-from cornflow.models import PermissionsDAG, UserModel, UserRoleModel
+from cornflow.models import UserModel, UserRoleModel
 from cornflow.schemas.user import LoginEndpointRequest, LoginOpenAuthRequest
 from cornflow.shared import db
 from cornflow.shared.authentication import Auth, LDAPBase
 from cornflow.shared.const import (
     AUTH_DB,
     AUTH_LDAP,
     AUTH_OID,
@@ -43,30 +44,34 @@
 
         :param kwargs: keyword arguments passed for the login, these can be username, password or a token
         :return: the response of the login or it raises an error. The correct response is a dict
         with the newly issued token and the user id, and a status code of 200
         :rtype: dict
         """
         auth_type = current_app.config["AUTH_TYPE"]
+        response = {}
 
         if auth_type == AUTH_DB:
             user = self.auth_db_authenticate(**kwargs)
+            response.update({"change_password": check_last_password_change(user)})
         elif auth_type == AUTH_LDAP:
             user = self.auth_ldap_authenticate(**kwargs)
         elif auth_type == AUTH_OID:
             user = self.auth_oid_authenticate(**kwargs)
         else:
             raise ConfigurationError()
 
         try:
             token = self.auth_class.generate_token(user.id)
         except Exception as e:
             raise InvalidUsage(f"Error in generating user token: {str(e)}", 400)
 
-        return {"token": token, "id": user.id}, 200
+        response.update({"token": token, "id": user.id})
+
+        return response, 200
 
     def auth_db_authenticate(self, username, password):
         """
         Method in charge of performing the authentication against the database
 
         :param str username: the username of the user to log in
         :param str password:  the password of the user to log in
@@ -172,14 +177,21 @@
             )
 
             user_role.save()
 
         return user
 
 
+def check_last_password_change(user):
+    if user.pwd_last_change:
+        if user.pwd_last_change + timedelta(days=int(current_app.config["PWD_ROTATION_TIME"])) < datetime.utcnow():
+            return True
+    return False
+
+
 class LoginEndpoint(LoginBaseEndpoint):
     """
     Endpoint used to do the login to the cornflow webserver
     """
 
     def __init__(self):
         super().__init__()
@@ -194,19 +206,15 @@
         API (POST) method to log in in to the web server.
 
         :return: A dictionary with a message (either an error during login or the generated token for the user session)
           and an integer with the HTTP status code
         :rtype: Tuple(dict, integer)
         """
 
-        content, status = self.log_in(**kwargs)
-        if int(current_app.config["OPEN_DEPLOYMENT"]) == 1:
-            PermissionsDAG.delete_all_permissions_from_user(content["id"])
-            PermissionsDAG.add_all_permissions_to_user(content["id"])
-        return content, status
+        return self.log_in(**kwargs)
 
 
 class LoginOpenAuthEndpoint(LoginBaseEndpoint):
     """ """
 
     def __init__(self):
         super().__init__()
@@ -214,13 +222,8 @@
         self.auth_class = Auth
         self.user_role_association = UserRoleModel
 
     @doc(description="Log in", tags=["Users"])
     @use_kwargs(LoginOpenAuthRequest, location="json")
     def post(self, **kwargs):
         """ """
-
-        content, status = self.log_in(**kwargs)
-        if int(current_app.config["OPEN_DEPLOYMENT"]) == 1:
-            PermissionsDAG.delete_all_permissions_from_user(content["id"])
-            PermissionsDAG.add_all_permissions_to_user(content["id"])
-        return content, status
+        return self.log_in(**kwargs)
```

### Comparing `cornflow-1.0.9/cornflow/endpoints/main_alarms.py` & `cornflow-1.1.0a1/cornflow/endpoints/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/meta_resource.py` & `cornflow-1.1.0a1/cornflow/endpoints/meta_resource.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/permission.py` & `cornflow-1.1.0a1/cornflow/endpoints/permission.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/roles.py` & `cornflow-1.1.0a1/cornflow/endpoints/roles.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/schemas.py` & `cornflow-1.1.0a1/cornflow/endpoints/schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/signup.py` & `cornflow-1.1.0a1/cornflow/endpoints/signup.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/tables.py` & `cornflow-1.1.0a1/cornflow/endpoints/tables.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/token.py` & `cornflow-1.1.0a1/cornflow/endpoints/token.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/endpoints/user.py` & `cornflow-1.1.0a1/cornflow/endpoints/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,24 +166,24 @@
         ):
             raise EndpointNotImplemented(
                 "To edit a user, go to the OID provider",
                 log_txt=f"Error while user {self.get_user()} tries to edit user {user_id}. "
                 f"To edit a user, go to the OID provider.",
             )
 
-        if data.get("password"):
+        if data.get("password") is not None:
             check, msg = check_password_pattern(data.get("password"))
             if not check:
                 raise InvalidCredentials(
                     msg,
                     log_txt=f"Error while user {self.get_user()} tries to edit user {user_id}. "
                     f"The new password is not valid.",
                 )
 
-        if data.get("email"):
+        if data.get("email") is not None:
             check, msg = check_email_pattern(data.get("email"))
             if not check:
                 raise InvalidCredentials(
                     msg,
                     log_txt=f"Error while user {self.get_user()} tries to edit user {user_id}. "
                     f"The new email is not valid.",
                 )
```

### Comparing `cornflow-1.0.9/cornflow/endpoints/user_role.py` & `cornflow-1.1.0a1/cornflow/endpoints/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/alembic.ini` & `cornflow-1.1.0a1/cornflow/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/env.py` & `cornflow-1.1.0a1/cornflow/migrations/env.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/00757b557b02_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/00757b557b02_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/1af47a419bbd_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/1af47a419bbd_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/4aac5e0c6e66_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/4aac5e0c6e66_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/7c3ea5ab5501_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/7c3ea5ab5501_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/a472b5ad50b7_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/a472b5ad50b7_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/c2db9409cb5f_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/c2db9409cb5f_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/c8a6c762e818_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/c8a6c762e818_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/ca449af8034c_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/ca449af8034c_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/d0e0700dcd8e_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/d0e0700dcd8e_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/d1b5be1f0549_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/d1b5be1f0549_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/e1a50dae1ac9_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/e1a50dae1ac9_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/e937a5234ce4_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/e937a5234ce4_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/ebdd955fcc5e_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/ebdd955fcc5e_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/migrations/versions/f3bee20314a2_.py` & `cornflow-1.1.0a1/cornflow/migrations/versions/f3bee20314a2_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/action.py` & `cornflow-1.1.0a1/cornflow/models/action.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/alarms.py` & `cornflow-1.1.0a1/cornflow/models/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/base_data_model.py` & `cornflow-1.1.0a1/cornflow/models/base_data_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     name = db.Column(db.String(256), nullable=False)
     description = db.Column(TEXT, nullable=True)
     data_hash = db.Column(db.String(256), nullable=False)
     schema = db.Column(db.String(256), nullable=True)
 
     @declared_attr
     def user_id(self):
+        """
+        The foreign key for the user (:class:`UserModel<cornflow.models.UserModel>`).
+        """
         return db.Column(db.Integer, db.ForeignKey("users.id"), nullable=False)
 
     @declared_attr
     def user(self):
         return db.relationship("UserModel")
 
     def __init__(self, data):
```

### Comparing `cornflow-1.0.9/cornflow/models/dag.py` & `cornflow-1.1.0a1/cornflow/models/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/dag_permissions.py` & `cornflow-1.1.0a1/cornflow/models/dag_permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/execution.py` & `cornflow-1.1.0a1/cornflow/models/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cornflow.shared import db
 from cornflow.shared.const import DEFAULT_EXECUTION_CODE, EXECUTION_STATE_MESSAGE_DICT
 
 
 class ExecutionModel(BaseDataModel):
     """
     Model class for the Executions.
-    It inherits from :class:`BaseDataModel` to have the trace fields and user field
+    It inherits from :class:`BaseDataModel<cornflow.models.base_data_model.BaseDataModel>` to have the trace fields and user field.
 
     - **id**: str, the primary key for the executions, a hash generated upon creation of the execution
       and the id given back to the user.
       The hash is generated from the creation date, the user and the id of the parent instance.
     - **instance_id**: str, the foreign key for the instance (:class:`InstanceModel`). It links the execution to its
       parent instance.
     - **name**: str, the name of the execution given by the user.
```

### Comparing `cornflow-1.0.9/cornflow/models/instance.py` & `cornflow-1.1.0a1/cornflow/models/instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cornflow.models.base_data_model import BaseDataModel
 from cornflow.shared import db
 
 
 class InstanceModel(BaseDataModel):
     """
     Model class for the Instances
-    It inherits from :class:`BaseDataModel` to have the trace fields and user field
+    It inherits from :class:`BaseDataModel<cornflow.models.base_data_model.BaseDataModel>` to have the trace fields and user field
 
     The :class:`InstanceModel` has the following fields:
 
     - **id**: str, the primary key for the instances, a hash generated upon creation of the instance
       and the id given back to the user.The hash is generated from the creation time and the user id.
     - **data**: dict (JSON), the data structure of the instance (:class:`DataSchema`)
     - **name**: str, the name given to the instance by the user.
@@ -54,20 +54,22 @@
             information to create a new instance
         """
         super().__init__(data)
         self.id = hashlib.sha1(
             (str(self.created_at) + " " + str(self.user_id)).encode()
         ).hexdigest()
 
-    def update(self, data):
+    def update(self, data: dict):
         """
-        Method used to update an instance from the database
+        Method used to update an instance from the database.
+
+        This method is mainly used on PUT requests to update the instance.
 
         :param dict data: the data of the object
-        :return: None
+        :return: Nothing, it will update the instance in-place and on the database
         :rtype: None
         """
         # Delete the checks if the data has been modified since they are probably not valid anymore
         if "data" in data.keys():
             self.checks = None
             # Delete the checks of all the related executions since they are probably not valid anymore either
             for execution in self.executions:
```

### Comparing `cornflow-1.0.9/cornflow/models/main_alarms.py` & `cornflow-1.1.0a1/cornflow/models/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/meta_models.py` & `cornflow-1.1.0a1/cornflow/models/meta_models.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/permissions.py` & `cornflow-1.1.0a1/cornflow/models/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/role.py` & `cornflow-1.1.0a1/cornflow/models/role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/user.py` & `cornflow-1.1.0a1/cornflow/models/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This file contains the UserModel
 """
 # Imports from external libraries
 import random
 import string
+from datetime import datetime
 
 # Imports from internal modules
 from cornflow.models.meta_models import TraceAttributesModel
 from cornflow.models.user_role import UserRoleModel
 from cornflow.shared import (
     bcrypt,
     db,
@@ -47,14 +48,15 @@
 
     __tablename__ = "users"
     id = db.Column(db.Integer, primary_key=True, autoincrement=True)
     first_name = db.Column(db.String(128), nullable=True)
     last_name = db.Column(db.String(128), nullable=True)
     username = db.Column(db.String(128), nullable=False, unique=True)
     password = db.Column(db.String(128), nullable=True)
+    pwd_last_change = db.Column(db.DateTime, nullable=True)
     email = db.Column(db.String(128), nullable=False, unique=True)
 
     user_roles = db.relationship(
         "UserRoleModel", cascade="all,delete", backref="users"
     )
 
     instances = db.relationship(
@@ -89,14 +91,15 @@
         return {r.role.id: r.role.name for r in self.user_roles}
 
     def __init__(self, data):
         super().__init__()
         self.first_name = data.get("first_name")
         self.last_name = data.get("last_name")
         self.username = data.get("username")
+        self.pwd_last_change = datetime.utcnow()
         # TODO: handle better None passwords that can be found when using ldap
         check_pass, msg = check_password_pattern(data.get("password"))
         if check_pass:
             self.password = self.__generate_hash(data.get("password"))
         else:
             raise InvalidCredentials(
                 msg,
@@ -119,14 +122,15 @@
         :param dict data: the data to update the user
         """
         # First we create the hash of the new password and then we update the object
         new_password = data.get("password")
         if new_password:
             new_password = self.__generate_hash(new_password)
             data["password"] = new_password
+            data["pwd_last_change"] = datetime.utcnow()
         super().update(data)
 
     def comes_from_external_provider(self):
         """
         Returns a boolean if the user comes from an external_provider or not
         """
         return self.password is None
```

### Comparing `cornflow-1.0.9/cornflow/models/user_role.py` & `cornflow-1.1.0a1/cornflow/models/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/models/view.py` & `cornflow-1.1.0a1/cornflow/models/view.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/schemas/alarms.py` & `cornflow-1.1.0a1/cornflow/schemas/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/schemas/case.py` & `cornflow-1.1.0a1/cornflow/schemas/case.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/schemas/dag.py` & `cornflow-1.1.0a1/cornflow/schemas/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/schemas/execution.py` & `cornflow-1.1.0a1/cornflow/schemas/execution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Imports from libraries
 from marshmallow import fields, Schema, validate
 
 # Imports from internal modules
 from cornflow.shared.const import MIN_EXECUTION_STATUS_CODE, MAX_EXECUTION_STATUS_CODE
 from .common import QueryFilters, BaseDataEndpointResponse
-from .solution_log import LogSchema
+from .solution_log import LogSchema, BasicLogSchema
 
 
 class QueryFiltersExecution(QueryFilters):
     pass
     # status = fields.Int(required=False)
 
 
@@ -110,14 +110,20 @@
                 for key, val in sorted(temp.items()):
                     indicators_string = f"{indicators_string} {key}: {val};"
         return indicators_string[1:-1]
 
     indicators = fields.Method("get_indicators")
 
 
+class ExecutionDetailsWithIndicatorsAndLogResponse(
+    ExecutionDetailsEndpointWithIndicatorsResponse
+):
+    log = fields.Nested(BasicLogSchema, attribute="log_json")
+
+
 class ExecutionStatusEndpointResponse(Schema):
     id = fields.Str()
     state = fields.Int()
     message = fields.Str(attribute="state_message")
     data_hash = fields.Str(dump_only=True)
 
 
@@ -125,12 +131,13 @@
     id = fields.Str()
     status = fields.Int()
 
 
 class ExecutionDataEndpointResponse(ExecutionDetailsEndpointResponse):
     data = fields.Raw()
     checks = fields.Raw()
+    log = fields.Nested(BasicLogSchema, attribute="log_json")
 
 
 class ExecutionLogEndpointResponse(ExecutionDetailsEndpointWithIndicatorsResponse):
     log = fields.Nested(LogSchema, attribute="log_json")
     log_text = fields.Str(attribute="log_text")
```

### Comparing `cornflow-1.0.9/cornflow/schemas/instance.py` & `cornflow-1.1.0a1/cornflow/schemas/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/schemas/main_alarms.py` & `cornflow-1.1.0a1/cornflow/schemas/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/schemas/permissions.py` & `cornflow-1.1.0a1/cornflow/schemas/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/schemas/query.py` & `cornflow-1.1.0a1/cornflow/schemas/query.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/schemas/solution_log.py` & `cornflow-1.1.0a1/cornflow/schemas/solution_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from marshmallow import fields, Schema
+from marshmallow import fields, Schema, EXCLUDE
 
 options = dict(required=True, allow_none=True)
 log_options = dict(required=False, allow_none=True)
 pg_options = dict(many=True, required=True)
 list_of_strings = fields.List(fields.Str, required=False, many=True)
 
 
@@ -45,26 +45,32 @@
 class FirstSolution(Schema):
     Node = fields.Int(**options)
     NodesLeft = fields.Int(**options)
     BestInteger = fields.Float(**options)
     CutsBestBound = fields.Float(**options)
 
 
-class LogSchema(Schema):
+class BasicLogSchema(Schema):
+    status = fields.Str(**log_options)
+    status_code = fields.Int(**log_options)
+    sol_code = fields.Int(**log_options)
+
+
+class LogSchema(BasicLogSchema):
+    class Meta:
+        unknown = EXCLUDE
+
     version = fields.Str(**log_options)
     solver = fields.Str(**log_options)
-    status = fields.Str(**log_options)
     best_bound = fields.Float(**log_options)
     best_solution = fields.Float(**log_options)
     gap = fields.Float(**log_options)
     time = fields.Float(**log_options)
     matrix = fields.Nested(MatrixSchema, **log_options)
     matrix_post = fields.Nested(MatrixSchema, **log_options)
     rootTime = fields.Float(**log_options)
     presolve = fields.Nested(PresolveSchema, **log_options)
     first_relaxed = fields.Float(**log_options)
     first_solution = fields.Nested(FirstSolution, **log_options)
-    status_code = fields.Int(**log_options)
-    sol_code = fields.Int(**log_options)
     nodes = fields.Int(**log_options)
     progress = fields.Nested(ProgressSchema, required=False)
     cut_info = fields.Raw(**log_options)
```

### Comparing `cornflow-1.0.9/cornflow/schemas/user.py` & `cornflow-1.1.0a1/cornflow/schemas/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,22 +21,24 @@
 class UserEndpointResponse(Schema):
     id = fields.Int()
     username = fields.Str()
     first_name = fields.Str()
     last_name = fields.Str()
     email = fields.Str()
     created_at = fields.Str()
+    pwd_last_change = fields.Str()
 
 
 class UserDetailsEndpointResponse(Schema):
     id = fields.Int()
     first_name = fields.Str()
     last_name = fields.Str()
     username = fields.Str()
     email = fields.Str()
+    pwd_last_change = fields.Str()
 
 
 class TokenEndpointResponse(Schema):
     valid = fields.Int()
 
 
 class RecoverPasswordRequest(Schema):
@@ -45,14 +47,15 @@
 
 class UserEditRequest(Schema):
     username = fields.Str(required=False)
     first_name = fields.Str(required=False)
     last_name = fields.Str(required=False)
     email = fields.Str(required=False)
     password = fields.Str(required=False)
+    pwd_last_change = fields.DateTime(required=False)
 
 
 class LoginEndpointRequest(Schema):
     """
     This is the schema used by the login endpoint with auth db or ldap
     """
```

### Comparing `cornflow-1.0.9/cornflow/schemas/user_role.py` & `cornflow-1.1.0a1/cornflow/schemas/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/authentication/auth.py` & `cornflow-1.1.0a1/cornflow/shared/authentication/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         if user_id is None:
             err = "The user id passed to generate the token is not valid."
             raise InvalidUsage(
                 err, log_txt="Error while trying to generate token. " + err
             )
 
         payload = {
-            "exp": datetime.utcnow() + timedelta(days=1),
+            "exp": datetime.utcnow() + timedelta(hours=float(current_app.config["TOKEN_DURATION"])),
             "iat": datetime.utcnow(),
             "sub": user_id,
         }
 
         return jwt.encode(
             payload, current_app.config["SECRET_TOKEN_KEY"], algorithm="HS256"
         )
```

### Comparing `cornflow-1.0.9/cornflow/shared/authentication/decorators.py` & `cornflow-1.1.0a1/cornflow/shared/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/authentication/ldap.py` & `cornflow-1.1.0a1/cornflow/shared/authentication/ldap.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/compress.py` & `cornflow-1.1.0a1/cornflow/shared/compress.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/const.py` & `cornflow-1.1.0a1/cornflow/shared/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/email.py` & `cornflow-1.1.0a1/cornflow/shared/email.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/exceptions.py` & `cornflow-1.1.0a1/cornflow/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/log_config.py` & `cornflow-1.1.0a1/cornflow/shared/log_config.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/query_tools.py` & `cornflow-1.1.0a1/cornflow/shared/query_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/utils.py` & `cornflow-1.1.0a1/cornflow/shared/utils.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/utils_tables.py` & `cornflow-1.1.0a1/cornflow/shared/utils_tables.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/shared/validators.py` & `cornflow-1.1.0a1/cornflow/shared/validators.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/const.py` & `cornflow-1.1.0a1/cornflow/tests/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/custom_liveServer.py` & `cornflow-1.1.0a1/cornflow/tests/custom_liveServer.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/custom_test_case.py` & `cornflow-1.1.0a1/cornflow/tests/custom_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
 This file contains the different custom test classes used to generalize the unit testing of cornflow.
 """
 
 # Import from libraries
 import logging as log
 from datetime import datetime, timedelta
+
+from typing import List
+
 from flask import current_app
 from flask_testing import TestCase
 import json
 import jwt
 
 # Import from internal modules
 from cornflow.app import create_app
@@ -23,15 +26,14 @@
     LOGIN_URL,
     SIGNUP_URL,
     USER_URL,
     USER_ROLE_URL,
     TOKEN_URL,
 )
 
-
 try:
     date_from_str = datetime.fromisoformat
 except:
 
     def date_from_str(_string):
         return datetime.strptime(_string, "%Y-%m-%dT%H:%M:%S.%f")
 
@@ -168,52 +170,64 @@
 
         for key in self.get_keys_to_check(payload):
             getattr(row, key)
             if key in payload:
                 self.assertEqual(getattr(row, key), payload[key])
         return row.id
 
-    def get_rows(self, url, data, token=None, check_data=True):
+    def get_rows(
+        self, url, data, token=None, check_data=True, keys_to_check: List[str] = None
+    ):
         token = token or self.token
 
         codes = [
             self.create_new_row(url=url, model=self.model, payload=d) for d in data
         ]
         rows = self.client.get(
             url, follow_redirects=True, headers=self.get_header_with_auth(token)
         )
         # rows now come in desc order of date, so we reverse them:
         rows_data = list(reversed(rows.json))
         self.assertEqual(len(rows.json), len(data))
         if check_data:
             for i in range(len(data)):
                 self.assertEqual(rows_data[i]["id"], codes[i])
+                if keys_to_check:
+                    self.assertCountEqual(list(rows_data[i].keys()), keys_to_check)
                 for key in self.get_keys_to_check(data[i]):
                     self.assertIn(key, rows_data[i])
                     if key in data[i]:
                         self.assertEqual(rows_data[i][key], data[i][key])
         return rows
 
     def get_keys_to_check(self, payload):
         if len(self.items_to_check):
             return self.items_to_check
         return payload.keys()
 
     def get_one_row(
-        self, url, payload, expected_status=200, check_payload=True, token=None
+        self,
+        url,
+        payload,
+        expected_status=200,
+        check_payload=True,
+        token=None,
+        keys_to_check: List[str] = None,
     ):
         token = token or self.token
 
         row = self.client.get(
             url, follow_redirects=True, headers=self.get_header_with_auth(token)
         )
 
         self.assertEqual(expected_status, row.status_code)
         if not check_payload:
             return row.json
+        if keys_to_check:
+            self.assertCountEqual(list(row.json.keys()), keys_to_check)
         self.assertEqual(row.json["id"], payload["id"])
         for key in self.get_keys_to_check(payload):
             self.assertIn(key, row.json)
             if key in payload:
                 self.assertEqual(row.json[key], payload[key])
         return row.json
```

### Comparing `cornflow-1.0.9/cornflow/tests/integration/test_commands.py` & `cornflow-1.1.0a1/cornflow/tests/integration/test_commands.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/integration/test_cornflowclient.py` & `cornflow-1.1.0a1/cornflow/tests/integration/test_cornflowclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,32 @@
 
 
 class TestCornflowClientBasic(CustomTestCaseLive):
     def setUp(self, create_all=False):
         super().setUp()
         self.items_to_check = ["name", "description"]
 
+    def check_status_evolution(self, execution, end_state=EXEC_STATE_CORRECT):
+        statuses = [execution["state"]]
+        while end_state not in statuses and len(statuses) < 100:
+            time.sleep(1)
+            status = self.client.get_status(execution["id"])
+            statuses.append(status["state"])
+
+        self.assertIn(EXEC_STATE_QUEUED, statuses)
+        self.assertIn(EXEC_STATE_RUNNING, statuses)
+        self.assertIn(end_state, statuses)
+
+        queued_idx = statuses.index(EXEC_STATE_QUEUED)
+        running_idx = statuses.index(EXEC_STATE_RUNNING)
+        end_state_idx = statuses.index(end_state)
+
+        self.assertLess(queued_idx, running_idx)
+        self.assertLess(running_idx, end_state_idx)
+
     def create_new_instance_file(self, mps_file):
         name = "test_instance1"
         description = "description123"
         response = self.client.create_instance_file(
             filename=mps_file, name=name, description=description, minimize=True
         )
         self.assertTrue("id" in response)
@@ -137,15 +155,14 @@
             description="timer_exec_description",
             schema="timer",
         )
         return self.create_new_execution(payload)
 
 
 class TestCornflowClientOpen(TestCornflowClientBasic):
-
     # TODO: user management
     # TODO: infeasible execution
 
     def test_new_instance_file(self):
         self.create_new_instance_file("./cornflow/tests/data/test_mps.mps")
 
     def test_new_instance(self):
@@ -238,15 +255,14 @@
     def test_new_instance_with_schema_additional_data(self):
         payload = load_file(INSTANCE_PATH)
         payload["data"]["objective"]["inexistant_property"] = 1
         payload["schema"] = "solve_model_dag"
         self.client.create_instance(**payload)
 
     def test_new_instance_with_schema_good(self):
-
         payload = load_file(INSTANCE_PATH)
         payload["schema"] = "solve_model_dag"
         self.create_new_instance_payload(payload)
 
     def test_new_case_without_parent(self):
         payload = load_file(INSTANCE_PATH)
         self.create_new_case_payload(payload)
@@ -331,31 +347,21 @@
         status = self.client.get_status(execution["id"])
         results = self.client.get_results(execution["id"])
         self.assertEqual(status["state"], EXEC_STATE_STOPPED)
         self.assertEqual(results["state"], EXEC_STATE_STOPPED)
 
     def test_status_solving(self):
         execution = self.create_instance_and_execution()
-        time.sleep(10)
-        status = self.client.get_status(execution["id"])
-        self.assertEqual(status["state"], EXEC_STATE_CORRECT)
+        self.check_status_evolution(execution, EXEC_STATE_CORRECT)
 
     def test_status_solving_timer(self):
         execution = self.create_timer_instance_and_execution(10)
-        status = self.client.get_status(execution["id"])
-        self.assertEqual(status["state"], EXEC_STATE_QUEUED)
-        time.sleep(5)
-        status = self.client.get_status(execution["id"])
-        self.assertEqual(status["state"], EXEC_STATE_RUNNING)
-        time.sleep(12)
-        status = self.client.get_status(execution["id"])
-        self.assertEqual(status["state"], EXEC_STATE_CORRECT)
+        self.check_status_evolution(execution, EXEC_STATE_CORRECT)
 
     def test_manual_execution(self):
-
         instance_payload = load_file(INSTANCE_PATH)
         one_instance = self.create_new_instance_payload(instance_payload)
         name = "test_execution_name_123"
         description = "test_execution_description_123"
         # for the solution we can use the same standard than the instance data
         payload = dict(
             instance_id=one_instance["id"],
```

### Comparing `cornflow-1.0.9/cornflow/tests/ldap/test_ldap_authentication.py` & `cornflow-1.1.0a1/cornflow/tests/ldap/test_ldap_authentication.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_actions.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_alarms.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_apiview.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_apiview.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_cases.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_cases.py`

 * *Files 8% similar despite different names*

```diff
@@ -197,16 +197,37 @@
         self.payload["solution"] = self.payload["data"]
         self.create_new_row(self.url, self.model, self.payload)
 
     def test_new_case_without_solution(self):
         self.payload.pop("solution")
         self.items_to_check = ["name", "description", "schema", "data"]
         _id = self.create_new_row(self.url, self.model, self.payload)
+        keys_to_check = [
+            "data",
+            "solution_checks",
+            "updated_at",
+            "id",
+            "schema",
+            "data_hash",
+            "path",
+            "solution_hash",
+            "user_id",
+            "indicators",
+            "solution",
+            "is_dir",
+            "description",
+            "name",
+            "checks",
+            "created_at",
+        ]
         data = self.get_one_row(
-            self.url + "/" + str(_id) + "/data/", payload={}, check_payload=False
+            self.url + "/" + str(_id) + "/data/",
+            payload={},
+            check_payload=False,
+            keys_to_check=keys_to_check,
         )
         self.assertIsNone(data["solution"])
 
     def test_case_with_parent(self):
         payload = dict(self.payload)
         payload.pop("data")
         case_id = self.create_new_row(self.url, self.model, payload)
@@ -289,15 +310,29 @@
         self.payload = self.load_file(CASE_PATH)
         self.payloads = [self.load_file(f) for f in CASES_LIST]
         self.model = CaseModel
         self.items_to_check = ["name", "description", "path", "schema"]
         self.url = CASE_URL
 
     def test_get_rows(self):
-        self.get_rows(self.url, self.payloads)
+        keys_to_check = [
+            "data_hash",
+            "created_at",
+            "is_dir",
+            "path",
+            "schema",
+            "description",
+            "solution_hash",
+            "id",
+            "user_id",
+            "updated_at",
+            "name",
+            "indicators",
+        ]
+        self.get_rows(self.url, self.payloads, keys_to_check=keys_to_check)
 
 
 class TestCaseDetailEndpoint(BaseTestCases.DetailEndpoint):
     def setUp(self):
         super().setUp()
         self.payload = self.load_file(CASE_PATH)
         self.model = CaseModel
@@ -361,15 +396,27 @@
         response = self.client.post(
             CASE_URL + str(self.case_id) + "/instance/",
             follow_redirects=True,
             headers=self.get_header_with_auth(self.token),
         )
 
         payload = response.json
-        result = self.get_one_row(INSTANCE_URL + payload["id"] + "/", payload)
+        keys_to_check = [
+            "id",
+            "schema",
+            "data_hash",
+            "executions",
+            "user_id",
+            "description",
+            "name",
+            "created_at",
+        ]
+        result = self.get_one_row(
+            INSTANCE_URL + payload["id"] + "/", payload, keys_to_check=keys_to_check
+        )
         dif = self.response_items.symmetric_difference(result.keys())
         self.assertEqual(len(dif), 0)
 
         self.items_to_check = [
             "id",
             "name",
             "data",
@@ -378,15 +425,31 @@
             "schema",
             "user_id",
             "created_at",
             "description",
         ]
         self.response_items = set(self.items_to_check)
 
-        result = self.get_one_row(INSTANCE_URL + payload["id"] + "/data/", payload)
+        keys_to_check = [
+            "data",
+            "id",
+            "schema",
+            "data_hash",
+            "user_id",
+            "description",
+            "name",
+            "checks",
+            "created_at",
+        ]
+
+        result = self.get_one_row(
+            INSTANCE_URL + payload["id"] + "/data/",
+            payload,
+            keys_to_check=keys_to_check,
+        )
         dif = self.response_items.symmetric_difference(result.keys())
         self.assertEqual(len(dif), 0)
 
     def test_case_does_not_exist(self):
         response = self.client.post(
             CASE_URL + str(2) + "/instance/",
             follow_redirects=True,
@@ -535,19 +598,45 @@
             "name",
             "description",
             "schema",
             "data",
         ]
 
     def test_get_data(self):
-        self.get_one_row(self.url + str(self.payload["id"]) + "/data/", self.payload)
+        keys_to_check = [
+            "data",
+            "solution_checks",
+            "updated_at",
+            "id",
+            "schema",
+            "data_hash",
+            "path",
+            "solution_hash",
+            "user_id",
+            "indicators",
+            "solution",
+            "is_dir",
+            "description",
+            "name",
+            "checks",
+            "created_at",
+        ]
+        self.get_one_row(
+            self.url + str(self.payload["id"]) + "/data/",
+            self.payload,
+            keys_to_check=keys_to_check,
+        )
 
     def test_get_no_data(self):
         self.get_one_row(
-            self.url + str(500) + "/data/", {}, expected_status=404, check_payload=False
+            self.url + str(500) + "/data/",
+            {},
+            expected_status=404,
+            check_payload=False,
+            keys_to_check=["error"],
         )
 
     def test_get_compressed_data(self):
         headers = self.get_header_with_auth(self.token)
         headers["Accept-Encoding"] = "gzip"
 
         response = self.client.get(
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_cli.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_commands.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_commands.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_dags.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_dags.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     DAG_URL,
     DEPLOYED_DAG_URL,
     EXECUTION_URL_NORUN,
     INSTANCE_URL,
     LOGIN_URL,
     SIGNUP_URL,
     USER_URL,
+    EXECUTION_URL,
 )
 from cornflow.tests.unit.test_executions import TestExecutionsDetailEndpointMock
 from cornflow_client import get_pulp_jsonschema, get_empty_schema
 
 
 class TestDagEndpoint(TestExecutionsDetailEndpointMock):
     def test_manual_dag_service_user(self):
@@ -86,54 +87,100 @@
 
 
 class TestDagDetailEndpoint(TestExecutionsDetailEndpointMock):
     def test_put_dag(self):
         idx = self.create_new_row(EXECUTION_URL_NORUN, self.model, self.payload)
         with open(CASE_PATH) as f:
             payload = json.load(f)
+
+        log_json = {
+            "time": 10.3,
+            "solver": "dummy",
+            "status": "feasible",
+            "status_code": 2,
+            "sol_code": 1,
+            "some_other_key": "this should be excluded",
+        }
+
         data = dict(
             data=payload["data"],
             state=EXEC_STATE_CORRECT,
+            log_json={
+                "time": 10.3,
+                "solver": "dummy",
+                "status": "feasible",
+                "status_code": 2,
+                "sol_code": 1,
+                "some_other_key": "this should be excluded",
+            },
         )
         payload_to_check = {**self.payload, **data}
         token = self.create_service_user()
-        data = self.update_row(
+        self.update_row(
             url=DAG_URL + idx + "/",
             payload_to_check=payload_to_check,
             change=data,
             token=token,
             check_payload=False,
         )
 
+        data = self.get_one_row(
+            url=EXECUTION_URL + idx + "/log/",
+            token=token,
+            check_payload=False,
+            payload=self.payload,
+            expected_status=200,
+        )
+
+        for key in data["log"]:
+            self.assertEqual(data["log"][key], log_json[key])
+
+        self.assertNotIn("some_other_key", data["log"].keys())
+
     def test_get_dag(self):
         idx = self.create_new_row(EXECUTION_URL_NORUN, self.model, self.payload)
         token = self.create_service_user()
+        keys_to_check = ["id", "data", "solution_data", "config"]
         data = self.get_one_row(
             url=DAG_URL + idx + "/",
             token=token,
             check_payload=False,
             payload=self.payload,
+            keys_to_check=keys_to_check,
         )
+        keys_to_check = [
+            "data",
+            "id",
+            "schema",
+            "data_hash",
+            "user_id",
+            "description",
+            "name",
+            "checks",
+            "created_at",
+        ]
         instance_data = self.get_one_row(
             url=INSTANCE_URL + self.payload["instance_id"] + "/data/",
             payload=dict(),
             check_payload=False,
+            keys_to_check=keys_to_check,
         )
         self.assertEqual(data["data"], instance_data["data"])
         self.assertEqual(data["config"], self.payload["config"])
         return
 
     def test_get_no_dag(self):
         idx = self.create_new_row(EXECUTION_URL_NORUN, self.model, self.payload)
         data = self.get_one_row(
             url=DAG_URL + idx + "/",
             token=self.token,
             check_payload=False,
             payload=self.payload,
             expected_status=403,
+            keys_to_check=["error"],
         )
 
 
 class TestDeployedDAG(TestCase):
     def create_app(self):
         app = create_app("testing")
         return app
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_data_checks.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_data_checks.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_example_data.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_example_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 
 """
+
 # General imports
 import json
 
 # Partial imports
 from unittest.mock import patch
 
 
@@ -36,16 +37,18 @@
         }
         af_client.get_all_schemas.return_value = [{"name": self.schema_name}]
         return af_client
 
     @patch("cornflow.endpoints.example_data.Airflow.from_config")
     def test_get_example(self, airflow_init):
         af_client = self.patch_af_client(airflow_init)
+        keys_to_check = ["name", "examples"]
         example = self.get_one_row(
             self.url + "{}/".format(self.schema_name),
             {},
             expected_status=200,
             check_payload=False,
+            keys_to_check=keys_to_check,
         )
         self.assertIn("examples", example)
         self.assertIn("name", example)
         self.assertEqual(example["examples"], self.example)
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_executions.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_executions.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,29 @@
             temp["instance_id"] = fk_id
             return temp
 
         self.payload = load_file_fk(EXECUTION_PATH)
         self.bad_payload = load_file_fk(BAD_EXECUTION_PATH)
         self.payloads = [load_file_fk(f) for f in EXECUTIONS_LIST]
         self.solution = load_file_fk(EXECUTION_SOLUTION_PATH)
+        self.keys_to_check = [
+            "data_hash",
+            "created_at",
+            "config",
+            "state",
+            "message",
+            "schema",
+            "description",
+            "id",
+            "user_id",
+            "log",
+            "instance_id",
+            "name",
+            "indicators",
+        ]
 
     def test_new_execution(self):
         self.create_new_row(self.url, self.model, payload=self.payload)
 
     @patch("cornflow.endpoints.execution.Airflow")
     def test_new_execution_run(self, af_client_class):
         patch_af_client(af_client_class)
@@ -111,21 +126,21 @@
             follow_redirects=True,
             headers=self.get_header_with_auth(self.token),
         )
         self.assertEqual(404, response.status_code)
         self.assertTrue("error" in response.json)
 
     def test_get_executions(self):
-        self.get_rows(self.url, self.payloads)
+        self.get_rows(self.url, self.payloads, keys_to_check=self.keys_to_check)
 
     def test_get_no_executions(self):
         self.get_no_rows(self.url)
 
     def test_get_executions_superadmin(self):
-        self.get_rows(self.url, self.payloads)
+        self.get_rows(self.url, self.payloads, keys_to_check=self.keys_to_check)
         token = self.create_service_user()
         rows = self.client.get(
             self.url, follow_redirects=True, headers=self.get_header_with_auth(token)
         )
         self.assertEqual(len(rows.json), len(self.payloads))
 
 
@@ -271,23 +286,50 @@
             payload,
             expected_status=400,
             check_payload=False,
         )
 
     def test_create_delete_instance_load(self):
         idx = self.create_new_row(self.url + "?run=0", self.model, self.payload)
+        keys_to_check = [
+            "message",
+            "id",
+            "schema",
+            "data_hash",
+            "config",
+            "instance_id",
+            "user_id",
+            "indicators",
+            "description",
+            "name",
+            "created_at",
+            "state",
+        ]
         execution = self.get_one_row(
-            self.url + idx, payload={**self.payload, **dict(id=idx)}
+            self.url + idx,
+            payload={**self.payload, **dict(id=idx)},
+            keys_to_check=keys_to_check,
         )
         self.delete_row(self.url + idx + "/")
+        keys_to_check = [
+            "id",
+            "schema",
+            "description",
+            "name",
+            "user_id",
+            "executions",
+            "created_at",
+            "data_hash",
+        ]
         instance = self.get_one_row(
             INSTANCE_URL + execution["instance_id"] + "/",
             payload={},
             expected_status=200,
             check_payload=False,
+            keys_to_check=keys_to_check,
         )
         executions = [execution["id"] for execution in instance["executions"]]
         self.assertFalse(idx in executions)
 
     def test_delete_instance_deletes_execution(self):
         # we create a new instance
         with open(INSTANCE_PATH) as f:
@@ -347,48 +389,92 @@
 
 
 class TestExecutionsDataEndpoint(TestExecutionsDetailEndpointMock):
     def setUp(self):
         super().setUp()
         self.response_items = {"id", "name", "data"}
         self.items_to_check = ["name"]
+        self.keys_to_check = [
+            "created_at",
+            "checks",
+            "instance_id",
+            "schema",
+            "data",
+            "user_id",
+            "message",
+            "data_hash",
+            "log",
+            "config",
+            "description",
+            "state",
+            "name",
+            "id",
+        ]
 
     def test_get_one_execution(self):
         idx = self.create_new_row(EXECUTION_URL_NORUN, self.model, self.payload)
         self.url = EXECUTION_URL + idx + "/data/"
         payload = dict(self.payload)
         payload["id"] = idx
-        self.get_one_row(self.url, payload)
+        self.get_one_row(self.url, payload, keys_to_check=self.keys_to_check)
 
     def test_get_one_execution_superadmin(self):
         idx = self.create_new_row(EXECUTION_URL_NORUN, self.model, self.payload)
         payload = dict(self.payload)
         payload["id"] = idx
         token = self.create_service_user()
-        self.get_one_row(EXECUTION_URL + idx + "/data/", payload, token=token)
+        self.get_one_row(
+            EXECUTION_URL + idx + "/data/",
+            payload,
+            token=token,
+            keys_to_check=self.keys_to_check,
+        )
 
 
 class TestExecutionsLogEndpoint(TestExecutionsDetailEndpointMock):
     def setUp(self):
         super().setUp()
         self.response_items = {"id", "name", "log", "indicators"}
         self.items_to_check = ["name"]
+        self.keys_to_check = [
+            "created_at",
+            "id",
+            "log_text",
+            "instance_id",
+            "state",
+            "message",
+            "description",
+            "data_hash",
+            "name",
+            "log",
+            "schema",
+            "user_id",
+            "config",
+            "indicators",
+        ]
 
     def test_get_one_execution(self):
         idx = self.create_new_row(EXECUTION_URL_NORUN, self.model, self.payload)
         payload = dict(self.payload)
         payload["id"] = idx
-        self.get_one_row(EXECUTION_URL + idx + "/log/", payload)
+        self.get_one_row(
+            EXECUTION_URL + idx + "/log/", payload, keys_to_check=self.keys_to_check
+        )
 
     def test_get_one_execution_superadmin(self):
         idx = self.create_new_row(EXECUTION_URL_NORUN, self.model, self.payload)
         payload = dict(self.payload)
         payload["id"] = idx
         token = self.create_service_user()
-        self.get_one_row(EXECUTION_URL + idx + "/log/", payload, token=token)
+        self.get_one_row(
+            EXECUTION_URL + idx + "/log/",
+            payload,
+            token=token,
+            keys_to_check=self.keys_to_check,
+        )
 
 
 class TestExecutionsStatusEndpoint(TestExecutionsDetailEndpointMock):
     def setUp(self):
         super().setUp()
         self.response_items = {"id", "name", "status"}
         self.items_to_check = []
@@ -396,16 +482,20 @@
     @patch("cornflow.endpoints.execution.Airflow")
     def test_get_one_status(self, af_client_class):
         patch_af_client(af_client_class)
 
         idx = self.create_new_row(EXECUTION_URL, self.model, self.payload)
         payload = dict(self.payload)
         payload["id"] = idx
+        keys_to_check = ["state", "message", "id", "data_hash"]
         data = self.get_one_row(
-            EXECUTION_URL + idx + "/status/", payload, check_payload=False
+            EXECUTION_URL + idx + "/status/",
+            payload,
+            check_payload=False,
+            keys_to_check=keys_to_check,
         )
         self.assertEqual(data["state"], 1)
 
     @patch("cornflow.endpoints.execution.Airflow")
     def test_put_one_status(self, af_client_class):
         patch_af_client(af_client_class)
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_generate_from_schema.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_generate_from_schema.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_health.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_health.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_instances.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_instances.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,23 @@
         def load_file(_file):
             with open(_file) as f:
                 temp = json.load(f)
             return temp
 
         self.payload = load_file(INSTANCE_PATH)
         self.payloads = [load_file(f) for f in INSTANCES_LIST]
+        self.keys_to_check = [
+            "data_hash",
+            "created_at",
+            "schema",
+            "description",
+            "id",
+            "user_id",
+            "name",
+        ]
 
     def test_new_instance(self):
         self.create_new_row(self.url, self.model, self.payload)
 
     def test_new_instance_missing_info(self):
         del self.payload["data"]["parameters"]
         self.create_new_row(
@@ -61,18 +70,18 @@
                 "Authorization": "Bearer " + self.token,
             },
         )
         self.assertEqual(400, response.status_code)
         self.assertTrue("error" in response.json)
 
     def test_get_instances(self):
-        self.get_rows(self.url, self.payloads)
+        self.get_rows(self.url, self.payloads, keys_to_check=self.keys_to_check)
 
     def test_get_instances_superadmin(self):
-        self.get_rows(self.url, self.payloads)
+        self.get_rows(self.url, self.payloads, keys_to_check=self.keys_to_check)
         token = self.create_service_user()
         rows = self.client.get(
             self.url, follow_redirects=True, headers=self.get_header_with_auth(token)
         )
         self.assertEqual(len(rows.json), len(self.payloads))
 
     def test_get_no_instances(self):
@@ -169,15 +178,28 @@
         self.response_items.add("checks")
         self.response_items.remove("executions")
         self.items_to_check += ["data", "checks"]
 
     def test_get_one_instance(self):
         idx = self.create_new_row(self.url, self.model, self.payload)
         payload = {**self.payload, **dict(id=idx)}
-        result = self.get_one_row(INSTANCE_URL + idx + "/data/", payload)
+        keys_to_check = [
+            "data",
+            "id",
+            "schema",
+            "data_hash",
+            "user_id",
+            "description",
+            "name",
+            "checks",
+            "created_at",
+        ]
+        result = self.get_one_row(
+            INSTANCE_URL + idx + "/data/", payload, keys_to_check=keys_to_check
+        )
         dif = self.response_items.symmetric_difference(result.keys())
         self.assertEqual(len(dif), 0)
 
     def test_instance_compression(self):
         idx = self.create_new_row(self.url, self.model, self.payload)
         headers = {
             "Content-Type": "application/json",
@@ -204,14 +226,15 @@
 
         self.get_one_row(
             INSTANCE_URL + idx + "/data/",
             payload=None,
             expected_status=404,
             check_payload=False,
             token=token,
+            keys_to_check=["error"],
         )
 
     def test_get_none_instance_planner_all(self):
         # Test planner users cannot access objects of other users
         self.create_new_row(self.url, self.model, self.payload)
         token = self.create_planner()
         self.get_no_rows(INSTANCE_URL, token=token)
@@ -228,16 +251,31 @@
         self.model = InstanceModel
 
     def test_get_one_instance_planner(self):
         # Test planner users can access objects of other users
         idx = self.create_new_row(self.url, self.model, self.payload)
         token = self.create_planner()
         payload = {**self.payload, **dict(id=idx)}
-
-        self.get_one_row(INSTANCE_URL + idx + "/data/", payload, token=token)
+        keys_to_check = [
+            "data",
+            "id",
+            "schema",
+            "data_hash",
+            "user_id",
+            "description",
+            "name",
+            "checks",
+            "created_at",
+        ]
+        self.get_one_row(
+            INSTANCE_URL + idx + "/data/",
+            payload,
+            token=token,
+            keys_to_check=keys_to_check,
+        )
 
     def test_get_all_instance_planner(self):
         # Test planner users can access objects of other users
         self.create_new_row(self.url, self.model, self.payload)
         token = self.create_planner()
         row = self.client.get(
             INSTANCE_URL,
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_instances_file.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_instances_file.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_licenses.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_licenses.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     @staticmethod
     def read_requirements():
         with open(_get_file("../../requirements.txt")) as req:
             content = req.read()
             requirements = content.split("\n")
 
         requirements = [
-            r.split("=")[0].split(">")[0].split("<")[0].lower()
+            r.split("=")[0].split(">")[0].split("<")[0].split("@")[0].lower()
             for r in requirements
-            if r != ""
+            if r != "" and not r.startswith("#")
         ]
         return requirements
 
     def setUp(self):
         super().setUp()
         self.roles_with_access = LicensesEndpoint.ROLES_WITH_ACCESS
         self.libraries = self.read_requirements()
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_log_in.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_log_in.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_main_alarms.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_main_alarms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 
 """
+
 import json
 
 # Imports from internal modules
 from cornflow.models import MainAlarmsModel, AlarmsModel
 from cornflow.tests.const import MAIN_ALARMS_URL, ALARMS_URL
 from cornflow.tests.custom_test_case import CustomTestCase
 
@@ -15,49 +16,48 @@
         self.url = MAIN_ALARMS_URL
         self.model = MainAlarmsModel
         self.response_items = {"id", "message", "criticality", "schema", "id_alarm"}
         self.items_to_check = ["message", "schema", "criticality", "id_alarm"]
         payload = {
             "name": "Alarm 1",
             "description": "Description Alarm 1",
-            "criticality": 1
+            "criticality": 1,
         }
         self.id_alarm = self.client.post(
             ALARMS_URL,
             data=json.dumps(payload),
             follow_redirects=True,
             headers=self.get_header_with_auth(self.token),
         ).json["id"]
 
     def test_post_main_alarm(self):
         payload = {
             "message": "Message Main Alarm 1",
             "criticality": 1,
-            "id_alarm": self.id_alarm
+            "id_alarm": self.id_alarm,
         }
         self.create_new_row(self.url, self.model, payload)
 
     def test_get_main_alarms(self):
         data = [
             {
                 "message": "Message Main Alarm 1",
                 "criticality": 1,
-                "id_alarm": self.id_alarm
+                "id_alarm": self.id_alarm,
             },
             {
                 "message": "Message Main Alarm 2",
                 "criticality": 2,
                 "schema": "solve_model_dag",
-                "id_alarm": self.id_alarm
+                "id_alarm": self.id_alarm,
             },
         ]
+        keys_to_check = ["schema", "id_alarm", "criticality", "id", "message"]
         rows = self.get_rows(
-            self.url,
-            data,
-            check_data=False
+            self.url, data, check_data=False, keys_to_check=keys_to_check
         )
         rows_data = list(rows.json)
         for i in range(len(data)):
             for key in self.get_keys_to_check(data[i]):
                 self.assertIn(key, rows_data[i])
                 if key in data[i]:
-                    self.assertEqual(rows_data[i][key], data[i][key])
+                    self.assertEqual(rows_data[i][key], data[i][key])
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_permissions.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_roles.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_roles.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_schema_from_models.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_schema_from_models.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_schemas.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_schemas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 
 """
+
 # General imports
 import unittest
 
 # Partial imports
 from marshmallow import ValidationError, Schema, fields
 from unittest.mock import patch
 
@@ -155,34 +156,43 @@
         super().setUp()
         self.schema = get_pulp_jsonschema()
         self.config = get_empty_schema(solvers=["cbc", "PULP_CBC_CMD"])
         self.url = SCHEMA_URL
         self.schema_name = "solve_model_dag"
 
     def test_get_schema(self):
+        keys_to_check = [
+            "solution_checks",
+            "instance_checks",
+            "config",
+            "solution",
+            "name",
+            "instance",
+        ]
         schemas = self.get_one_row(
             self.url + "{}/".format(self.schema_name),
             {},
             expected_status=200,
             check_payload=False,
+            keys_to_check=keys_to_check,
         )
         self.assertIn("instance", schemas)
         self.assertIn("solution", schemas)
         self.assertEqual(schemas["instance"], self.schema)
         self.assertEqual(schemas["solution"], self.schema)
         self.assertEqual(schemas["config"], self.config)
 
 
 class TestNewSchemaEndpointOpen(CustomTestCase):
     def setUp(self):
         super().setUp()
         self.url = SCHEMA_URL
 
     def test_get_all_schemas(self):
-        schemas = self.get_one_row(self.url, {}, 200, False)
+        schemas = self.get_one_row(self.url, {}, 200, False, keys_to_check=["name"])
         dags = [{"name": dag} for dag in ["solve_model_dag", "gc", "timer"]]
 
         self.assertEqual(dags, schemas)
 
 
 class TestNewSchemaEndpointNotOpen(CustomTestCase):
     def create_app(self):
@@ -201,14 +211,15 @@
 
     def test_get_one_schema(self):
         schema = self.get_one_row(
             self.url + "{}/".format(self.schema_name),
             {},
             expected_status=403,
             check_payload=False,
+            keys_to_check=["error"],
         )
         self.assertEqual(
             {"error": "User does not have permission to access this dag"}, schema
         )
 
 
 if __name__ == "__main__":
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_sign_up.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_sign_up.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_tables.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_tables.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_token.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_token.py`

 * *Files 19% similar despite different names*

```diff
@@ -37,14 +37,31 @@
             headers={"Content-Type": "application/json"},
         ).json["token"]
 
         self.get_check_token()
         self.assertEqual(200, self.response.status_code)
         self.assertEqual(1, self.response.json["valid"])
 
+    def test_token_duration(self):
+        durations = [0.000000000001, 1]
+        asserts = [0, 1]
+        payload = self.data
+        for i in range(2):
+            current_app.config["TOKEN_DURATION"] = durations[i]
+            self.token = self.client.post(
+                LOGIN_URL,
+                data=json.dumps(payload),
+                follow_redirects=True,
+                headers={"Content-Type": "application/json"},
+            ).json["token"]
+
+            self.get_check_token()
+            self.assertEqual(200, self.response.status_code)
+            self.assertEqual(asserts[i], self.response.json["valid"])
+
     def test_get_invalid_token(self):
         self.token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2Mzk4MjAwNzMsImlhdCI6MTYzOTczMzY3Mywic3ViIjoxfQ"
         self.token += ".KzAYFDSrAJoCrnxGqKL2v6fE3oxT2muBgYztF1wcuN8"
 
         self.get_check_token()
 
         self.assertEqual(200, self.response.status_code)
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/test_users.py` & `cornflow-1.1.0a1/cornflow/tests/unit/test_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 
+from flask import current_app
 from flask_testing import TestCase
+from datetime import datetime, timedelta
 from cornflow.app import create_app
 from cornflow.commands.access import access_init_command
 from cornflow.commands.dag import register_deployed_dags_command_test
 from cornflow.commands.permissions import register_dag_permissions_command
 from cornflow.models import (
     CaseModel,
     ExecutionModel,
@@ -355,14 +357,28 @@
         response = self.modify_info(self.viewer, self.viewer, payload)
         self.assertEqual(200, response.status_code)
         self.viewer["password"] = payload["password"]
         response = self.log_in(self.viewer)
         self.assertEqual(200, response.status_code)
         self.assertIsNotNone(response.json["token"])
 
+    def test_change_password_rotation(self):
+        current_app.config["PWD_ROTATION_TIME"] = 1  # in days
+        payload = {"pwd_last_change": (datetime.utcnow() - timedelta(days=2)).strftime("%Y-%m-%dT%H:%M:%SZ")}
+        self.modify_info(self.planner, self.planner, payload)
+        response = self.log_in(self.planner)
+        self.assertEqual(True, response.json["change_password"])
+
+        payload = {"password": "Newtestpassword1!"}
+        self.modify_info(self.planner, self.planner, payload)
+        self.planner.update(payload)
+        print(self.planner)
+        response = self.log_in(self.planner)
+        self.assertEqual(False, response.json["change_password"])
+
 
 class TestUserModel(TestCase):
     def create_app(self):
         app = create_app("testing")
         return app
 
     def setUp(self):
```

### Comparing `cornflow-1.0.9/cornflow/tests/unit/tools.py` & `cornflow-1.1.0a1/cornflow/tests/unit/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.9/cornflow.egg-info/PKG-INFO` & `cornflow-1.1.0a1/cornflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cornflow
-Version: 1.0.9
+Version: 1.1.0a1
 Summary: Cornflow is an open source multi-solver optimization server with a REST API built using flask.
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: cornflow@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow
         =========
```

### Comparing `cornflow-1.0.9/cornflow.egg-info/SOURCES.txt` & `cornflow-1.1.0a1/cornflow.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 cornflow/migrations/alembic.ini
 cornflow/migrations/env.py
 cornflow/migrations/script.py.mako
 cornflow/migrations/versions/00757b557b02_.py
 cornflow/migrations/versions/1af47a419bbd_.py
 cornflow/migrations/versions/4aac5e0c6e66_.py
 cornflow/migrations/versions/7c3ea5ab5501_.py
+cornflow/migrations/versions/991b98e24225_.py
 cornflow/migrations/versions/a472b5ad50b7_.py
 cornflow/migrations/versions/c2db9409cb5f_.py
 cornflow/migrations/versions/c8a6c762e818_.py
 cornflow/migrations/versions/ca449af8034c_.py
 cornflow/migrations/versions/d0e0700dcd8e_.py
 cornflow/migrations/versions/d1b5be1f0549_.py
 cornflow/migrations/versions/e1a50dae1ac9_.py
```

### Comparing `cornflow-1.0.9/cornflow.egg-info/requires.txt` & `cornflow-1.1.0a1/cornflow.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 alembic==1.9.2
 apispec<=6.2.0
 click<=8.1.3
-cornflow-client<=1.0.16
-cryptography<=39.0.2
+cornflow-client==1.1.0a1
+cryptography<=42.0.5
 disposable-email-domains>=0.0.86
 Flask==2.3.2
 flask-apispec<=0.11.4
 Flask-Bcrypt<=1.0.1
 Flask-Compress<=1.13
-flask-cors<=3.0.10
+flask-cors<=4.0.1
 flask-inflate<=0.3
 Flask-Migrate<=4.0.4
 Flask-RESTful<=0.3.9
 Flask-SQLAlchemy==2.5.1
 gevent==23.9.1
-gunicorn<=20.1.0
+gunicorn<=22.0.0
 jsonpatch<=1.32
 ldap3<=2.9.1
 marshmallow<=3.19.0
 PuLP<=2.7.0
 psycopg2<=2.95
 PyJWT<=2.6.0
 pytups>=0.86.2
-requests<=2.29.0
+requests<=2.31.0
 SQLAlchemy==1.3.21
 webargs<=8.2.0
-Werkzeug<=2.3.3
+Werkzeug<=3.0.3
 
 [:python_version < "3.11"]
 greenlet<=2.0.2
 
 [:python_version >= "3.11"]
 greenlet==3.0.0
```

### Comparing `cornflow-1.0.9/setup.py` & `cornflow-1.1.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 required = []
 with open("requirements.txt", "r") as fh:
     required.append(fh.read().splitlines())
 
 setuptools.setup(
     name="cornflow",
-    version="1.0.9",
+    version="1.1.0a1",
     author="baobab soluciones",
     author_email="cornflow@baobabsoluciones.es",
     description="Cornflow is an open source multi-solver optimization server with a REST API built using flask.",
     long_description=long_description,
     url="https://github.com/baobabsoluciones/cornflow",
     packages=setuptools.find_packages(),
     install_requires=required,
```

