# Comparing `tmp/pyodmongo-0.9.0.tar.gz` & `tmp/pyodmongo-0.9.1.tar.gz`

## Comparing `pyodmongo-0.9.0.tar` & `pyodmongo-0.9.1.tar`

### file list

```diff
@@ -1,84 +1,85 @@
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/code_of_conduct.md
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/coverage.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/mkdocs.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyproject.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/requirements.txt
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/.github/workflows/black_formatter.yml
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/.github/workflows/publishing_docs_s3.yml
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/.github/workflows/python_publish.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    94192 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/assets/images/insomnia_request.png
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/assets/images/logo.png
--rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/assets/images/pyodmongo_Logo_BG_Dark.png
--rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/assets/images/pyodmongo_Logo_BG_White.png
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/aggregation.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/contributing.md
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/db_model.md
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/delete.md
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/fastapi.md
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/find.md
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/getting_started.md
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/index.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/indexes.md
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/query.md
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/en/save.md
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/aggregation.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/contributing.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/db_model.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/delete.md
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/fastapi.md
--rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/find.md
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/getting_started.md
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/index.md
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/indexes.md
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/query.md
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/pt-BR/save.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/docs/stylesheets/extras.css
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/version.py
--rw-r--r--   0        0        0    16992 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/async_engine/engine.py
--rw-r--r--   0        0        0    18792 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/engine/engine.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/engine/utils.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/models/db_field_info.py
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/models/db_model.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/models/fields.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/models/id_model.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/models/paginate.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/models/query_operators.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/models/responses.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/models/sort_operators.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/queries/__init__.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/queries/comparison_operators.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/queries/logical_operators.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/queries/query_string.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/queries/sort_operator.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/services/aggregate_stages.py
--rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/services/model_init.py
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyodmongo/services/query_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_async_aggregate.py
--rw-r--r--   0        0        0    19988 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_async_crud_db.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_class.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_db_field_info.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_db_index.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_dict_empty.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_fastapi.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_model_init_functions.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_object_id.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_project_pipeline.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_pydantic_validators.py
--rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_queries.py
--rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_reference_pipeline.py
--rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_save_dict.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_sync_aggregate.py
--rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_sync_crud_db.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/tests/test_version.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/LICENSE
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pyodmongo-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/code_of_conduct.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/coverage.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs_release_notes.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/mkdocs.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyproject.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/requirements.txt
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/workflows/black_formatter.yml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/workflows/publishing_docs_s3.yml
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    94192 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/insomnia_request.png
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/pyodmongo_Logo_BG_Dark.png
+-rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/pyodmongo_Logo_BG_White.png
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/aggregation.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/contributing.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/db_model.md
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/delete.md
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/fastapi.md
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/find.md
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/getting_started.md
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/index.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/indexes.md
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/query.md
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/save.md
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/aggregation.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/contributing.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/db_model.md
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/delete.md
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/fastapi.md
+-rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/find.md
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/getting_started.md
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/index.md
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/indexes.md
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/query.md
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/save.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/stylesheets/extras.css
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/version.py
+-rw-r--r--   0        0        0    16992 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/async_engine/engine.py
+-rw-r--r--   0        0        0    18792 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/engine/engine.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/engine/utils.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/db_field_info.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/db_model.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/fields.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/id_model.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/paginate.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/query_operators.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/responses.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/sort_operators.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/comparison_operators.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/logical_operators.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/query_string.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/sort_operator.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/services/aggregate_stages.py
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/services/model_init.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/services/query_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_async_aggregate.py
+-rw-r--r--   0        0        0    19988 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_async_crud_db.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_class.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_db_field_info.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_db_index.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_dict_empty.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_fastapi.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_model_init_functions.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_object_id.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_project_pipeline.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_pydantic_validators.py
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_queries.py
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_reference_pipeline.py
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_save_dict.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_sync_aggregate.py
+-rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_sync_crud_db.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_version.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/PKG-INFO
```

### Comparing `pyodmongo-0.9.0/code_of_conduct.md` & `pyodmongo-0.9.1/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/mkdocs.yml` & `pyodmongo-0.9.1/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     - find.md
     - delete.md
   - query.md
   - fastapi.md
   - indexes.md
   - aggregation.md
   - contributing.md
+  - release_notes.md
 
 extra:
   analytics:
     provider: google
     property: G-Q63PNQN3DY
 
 repo_url: https://github.com/mauro-andre/pyodmongo
```

### Comparing `pyodmongo-0.9.0/pyproject.py` & `pyodmongo-0.9.1/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/requirements.txt` & `pyodmongo-0.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/.github/ISSUE_TEMPLATE/bug.yml` & `pyodmongo-0.9.1/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/.github/workflows/black_formatter.yml` & `pyodmongo-0.9.1/.github/workflows/black_formatter.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/.github/workflows/publishing_docs_s3.yml` & `pyodmongo-0.9.1/.github/workflows/publishing_docs_s3.yml`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,19 @@
       run: |
         python3 -m pip install --upgrade pip mkdocs-material mkdocs-static-i18n "mkdocs-material[imaging]"
 
     - name: Install Image processing Dependencies
       run: |
         sudo apt-get install -y libcairo2-dev libfreetype6-dev libffi-dev libjpeg-dev libpng-dev libz-dev
         sudo apt-get install -y pngquant
+
+    - name: Generate release notes
+      run: |
+        python docs_release_notes.py
+      if: ${{ success() }}
         
     - name: Install AWS CLI
       run: |
         sudo apt-get update
         sudo apt-get install awscli
   
     - name: Configuring AWS CLI
```

### Comparing `pyodmongo-0.9.0/.github/workflows/python_publish.yml` & `pyodmongo-0.9.1/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/.github/workflows/tests.yml` & `pyodmongo-0.9.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/assets/images/favicon.png` & `pyodmongo-0.9.1/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/assets/images/insomnia_request.png` & `pyodmongo-0.9.1/docs/assets/images/insomnia_request.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/assets/images/logo.png` & `pyodmongo-0.9.1/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/assets/images/pyodmongo_Logo_BG_Dark.png` & `pyodmongo-0.9.1/docs/assets/images/pyodmongo_Logo_BG_Dark.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/assets/images/pyodmongo_Logo_BG_White.png` & `pyodmongo-0.9.1/docs/assets/images/pyodmongo_Logo_BG_White.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/aggregation.md` & `pyodmongo-0.9.1/docs/en/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/contributing.md` & `pyodmongo-0.9.1/docs/en/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/db_model.md` & `pyodmongo-0.9.1/docs/en/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/delete.md` & `pyodmongo-0.9.1/docs/en/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/fastapi.md` & `pyodmongo-0.9.1/docs/en/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/find.md` & `pyodmongo-0.9.1/docs/en/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/getting_started.md` & `pyodmongo-0.9.1/docs/en/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/index.md` & `pyodmongo-0.9.1/docs/en/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/indexes.md` & `pyodmongo-0.9.1/docs/en/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/query.md` & `pyodmongo-0.9.1/docs/en/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/en/save.md` & `pyodmongo-0.9.1/docs/en/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/aggregation.md` & `pyodmongo-0.9.1/docs/pt-BR/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/contributing.md` & `pyodmongo-0.9.1/docs/pt-BR/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/db_model.md` & `pyodmongo-0.9.1/docs/pt-BR/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/delete.md` & `pyodmongo-0.9.1/docs/pt-BR/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/fastapi.md` & `pyodmongo-0.9.1/docs/pt-BR/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/find.md` & `pyodmongo-0.9.1/docs/pt-BR/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/getting_started.md` & `pyodmongo-0.9.1/docs/pt-BR/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/index.md` & `pyodmongo-0.9.1/docs/pt-BR/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/indexes.md` & `pyodmongo-0.9.1/docs/pt-BR/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/query.md` & `pyodmongo-0.9.1/docs/pt-BR/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/docs/pt-BR/save.md` & `pyodmongo-0.9.1/docs/pt-BR/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/async_engine/engine.py` & `pyodmongo-0.9.1/pyodmongo/async_engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/engine/engine.py` & `pyodmongo-0.9.1/pyodmongo/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/engine/utils.py` & `pyodmongo-0.9.1/pyodmongo/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/models/db_field_info.py` & `pyodmongo-0.9.1/pyodmongo/models/db_field_info.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/models/db_model.py` & `pyodmongo-0.9.1/pyodmongo/models/db_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,18 +100,18 @@
     model_config = ConfigDict(populate_by_name=True)
     _pipeline: ClassVar = []
 
     def __remove_empty_dict(self, dct: dict):
         if dct == {}:
             return None
         for key, value in dct.items():
-            if value == {}:
+            if value == {} or value == []:
                 dct[key] = None
             elif type(value) == dict:
-                self.__remove_empty_dict(dct=value)
+                dct[key] = self.__remove_empty_dict(dct=value)
         is_full_empty = all(v == None or v == {} or v == [] for v in dct.values())
         if is_full_empty:
             return None
         return dct
 
     def __init__(self, **attrs):
         for key, value in attrs.items():
```

### Comparing `pyodmongo-0.9.0/pyodmongo/models/fields.py` & `pyodmongo-0.9.1/pyodmongo/models/fields.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/models/id_model.py` & `pyodmongo-0.9.1/pyodmongo/models/id_model.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/models/paginate.py` & `pyodmongo-0.9.1/pyodmongo/models/paginate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/models/query_operators.py` & `pyodmongo-0.9.1/pyodmongo/models/query_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/models/responses.py` & `pyodmongo-0.9.1/pyodmongo/models/responses.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/queries/comparison_operators.py` & `pyodmongo-0.9.1/pyodmongo/queries/comparison_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/queries/logical_operators.py` & `pyodmongo-0.9.1/pyodmongo/queries/logical_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/queries/query_string.py` & `pyodmongo-0.9.1/pyodmongo/queries/query_string.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/queries/sort_operator.py` & `pyodmongo-0.9.1/pyodmongo/queries/sort_operator.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/services/aggregate_stages.py` & `pyodmongo-0.9.1/pyodmongo/services/aggregate_stages.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/services/model_init.py` & `pyodmongo-0.9.1/pyodmongo/services/model_init.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyodmongo/services/query_operators.py` & `pyodmongo-0.9.1/pyodmongo/services/query_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_async_aggregate.py` & `pyodmongo-0.9.1/tests/test_async_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_async_crud_db.py` & `pyodmongo-0.9.1/tests/test_async_crud_db.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_class.py` & `pyodmongo-0.9.1/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_db_field_info.py` & `pyodmongo-0.9.1/tests/test_db_field_info.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_db_index.py` & `pyodmongo-0.9.1/tests/test_db_index.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_dict_empty.py` & `pyodmongo-0.9.1/tests/test_dict_empty.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 from pyodmongo import DbModel, Id
 
 
 def test_empty_dict():
     class MyModel1(DbModel):
-        attr1: str
+        attr1: str | None
         _collection = "my_model_1"
 
     class MyModel2(DbModel):
-        attr2: str
-        my_model_1: MyModel1 | Id
+        attr2: str | None
+        my_model_1: MyModel1 | Id | None
         _collection = "my_model_2"
 
     class MyModel3(DbModel):
-        attr3: str
+        attr3: str | None
         my_model_2: MyModel2 | Id | None
         my_model_2_2: MyModel2 | Id | None
+        my_model_2_3: MyModel2 | Id | None
         _collection = "my_model_3"
 
-    dct = {"attr3": "attr3", "my_model_2": {}, "my_model_2_2": {"my_model_1": {}}}
+    dct = {
+        "attr3": "attr3",
+        "my_model_2": {"attr2": "Escrito", "my_model_1": {"attr1": {}}},
+        "my_model_2_2": {"my_model_1": {}},
+        "my_model_2_3": {},
+    }
     obj = MyModel3(**dct)
     assert obj.model_dump() == {
         "attr3": "attr3",
-        "my_model_2": None,
+        "my_model_2": {
+            "id": None,
+            "created_at": None,
+            "updated_at": None,
+            "attr2": "Escrito",
+            "my_model_1": None,
+        },
         "my_model_2_2": None,
+        "my_model_2_3": None,
         "id": None,
         "created_at": None,
         "updated_at": None,
     }
```

### Comparing `pyodmongo-0.9.0/tests/test_fastapi.py` & `pyodmongo-0.9.1/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_model_init_functions.py` & `pyodmongo-0.9.1/tests/test_model_init_functions.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_object_id.py` & `pyodmongo-0.9.1/tests/test_object_id.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_project_pipeline.py` & `pyodmongo-0.9.1/tests/test_project_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_pydantic_validators.py` & `pyodmongo-0.9.1/tests/test_pydantic_validators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_queries.py` & `pyodmongo-0.9.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_reference_pipeline.py` & `pyodmongo-0.9.1/tests/test_reference_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_save_dict.py` & `pyodmongo-0.9.1/tests/test_save_dict.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_sync_aggregate.py` & `pyodmongo-0.9.1/tests/test_sync_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/tests/test_sync_crud_db.py` & `pyodmongo-0.9.1/tests/test_sync_crud_db.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/.gitignore` & `pyodmongo-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/LICENSE` & `pyodmongo-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/README.md` & `pyodmongo-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.0/pyproject.toml` & `pyodmongo-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyodmongo"
-version = "0.9.0"
+version = "0.9.1"
 license = "MIT"
 authors = [
   { name="Mauro André", email="eng.mauroandre@gmail.com" },
 ]
 description = "A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `pyodmongo-0.9.0/PKG-INFO` & `pyodmongo-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodmongo
-Version: 0.9.0
+Version: 0.9.1
 Summary: A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic
 Project-URL: Homepage, https://github.com/mauro-andre/pyodmongo
 Project-URL: Documentation, https://pyodmongo.dev
 Author-email: Mauro André <eng.mauroandre@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

