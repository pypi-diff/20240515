# Comparing `tmp/logfire-0.32.0.tar.gz` & `tmp/logfire-0.32.1.tar.gz`

## Comparing `logfire-0.32.0.tar` & `logfire-0.32.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.32.0/Makefile
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18465 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    56181 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/config.py
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/constants.py
--rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    55300 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/main.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/openai.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 logfire-0.32.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_backfill.py
--rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_configure.py
--rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_formatter.py
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_logfire.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_loguru.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_no_production.py
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_structlog.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    43200 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.32.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.32.0/LICENSE
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.32.0/README.md
--rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 logfire-0.32.0/pyproject.toml
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.32.0/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.32.1/Makefile
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    56181 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/config.py
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/constants.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    55429 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/main.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/openai.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_backfill.py
+-rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_configure.py
+-rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_formatter.py
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_logfire.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_loguru.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_no_production.py
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_structlog.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    43200 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.32.1/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.32.1/LICENSE
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.32.1/README.md
+-rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 logfire-0.32.1/pyproject.toml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.32.1/PKG-INFO
```

### Comparing `logfire-0.32.0/Makefile` & `logfire-0.32.1/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/__init__.py` & `logfire-0.32.1/logfire/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/propagate.py` & `logfire-0.32.1/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/testing.py` & `logfire-0.32.1/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/ast_utils.py` & `logfire-0.32.1/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/async_.py` & `logfire-0.32.1/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/auth.py` & `logfire-0.32.1/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/backfill.py` & `logfire-0.32.1/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/cli.py` & `logfire-0.32.1/logfire/_internal/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,14 +359,16 @@
         'protobuf': 5,
         # dependencies
         'rich': 6,
         # dependencies
         'typing-extensions': 7,
         # dependencies
         'tomli': 8,
+        # dependencies
+        'executing': 9,
     }
     otel_index = max(package_names.values(), default=0) + 1
     related_packages: list[tuple[int, str, str]] = []
 
     for dist in importlib_metadata.distributions():
         name = dist.metadata['Name']
         index = package_names.get(name)
```

### Comparing `logfire-0.32.0/logfire/_internal/config.py` & `logfire-0.32.1/logfire/_internal/config.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/config_params.py` & `logfire-0.32.1/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/constants.py` & `logfire-0.32.1/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/formatter.py` & `logfire-0.32.1/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/instrument.py` & `logfire-0.32.1/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/json_encoder.py` & `logfire-0.32.1/logfire/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/json_formatter.py` & `logfire-0.32.1/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/json_schema.py` & `logfire-0.32.1/logfire/_internal/json_schema.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/json_types.py` & `logfire-0.32.1/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/main.py` & `logfire-0.32.1/logfire/_internal/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1371,15 +1371,19 @@
             )
         )
         span.set_attributes(log_level_attributes('error'))
 
     attributes = {**(attributes or {})}
     if ValidationError is not None and isinstance(exception, ValidationError):
         # insert a more detailed breakdown of pydantic errors
-        err_json = exception.json(include_url=False)
+        try:
+            err_json = exception.json(include_url=False)
+        except TypeError:  # pragma: no cover
+            # pydantic v1
+            err_json = exception.json()
         span.set_attribute(ATTRIBUTES_VALIDATION_ERROR_KEY, err_json)
         attributes[ATTRIBUTES_VALIDATION_ERROR_KEY] = err_json
 
     if exception is not sys.exc_info()[1]:
         # OTEL's record_exception uses `traceback.format_exc()` which is for the current exception,
         # ignoring the passed exception.
         # So we override the stacktrace attribute with the correct one.
```

### Comparing `logfire-0.32.0/logfire/_internal/metrics.py` & `logfire-0.32.1/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/scrubbing.py` & `logfire-0.32.1/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/stack_info.py` & `logfire-0.32.1/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/tracer.py` & `logfire-0.32.1/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/utils.py` & `logfire-0.32.1/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/auto_trace/__init__.py` & `logfire-0.32.1/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.32.1/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.32.1/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/auto_trace/types.py` & `logfire-0.32.1/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/exporters/console.py` & `logfire-0.32.1/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/exporters/fallback.py` & `logfire-0.32.1/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/exporters/file.py` & `logfire-0.32.1/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/exporters/otlp.py` & `logfire-0.32.1/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.32.1/logfire/_internal/exporters/processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/exporters/remove_pending.py` & `logfire-0.32.1/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/exporters/wrapper.py` & `logfire-0.32.1/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/integrations/executors.py` & `logfire-0.32.1/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/integrations/fastapi.py` & `logfire-0.32.1/logfire/_internal/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/integrations/openai.py` & `logfire-0.32.1/logfire/_internal/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/_internal/integrations/psycopg.py` & `logfire-0.32.1/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/integrations/logging.py` & `logfire-0.32.1/logfire/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/integrations/loguru.py` & `logfire-0.32.1/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/integrations/pydantic.py` & `logfire-0.32.1/logfire/integrations/pydantic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/logfire/integrations/structlog.py` & `logfire-0.32.1/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/conftest.py` & `logfire-0.32.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_auto_trace.py` & `logfire-0.32.1/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_backfill.py` & `logfire-0.32.1/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_cli.py` & `logfire-0.32.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_collect_package_resources.py` & `logfire-0.32.1/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_configure.py` & `logfire-0.32.1/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_console_exporter.py` & `logfire-0.32.1/tests/test_console_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_formatter.py` & `logfire-0.32.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_json_args.py` & `logfire-0.32.1/tests/test_json_args.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_json_args_formatting.py` & `logfire-0.32.1/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_logfire.py` & `logfire-0.32.1/tests/test_logfire.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_loguru.py` & `logfire-0.32.1/tests/test_loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_metrics.py` & `logfire-0.32.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_no_production.py` & `logfire-0.32.1/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_pydantic_plugin.py` & `logfire-0.32.1/tests/test_pydantic_plugin.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_sampling.py` & `logfire-0.32.1/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_secret_scrubbing.py` & `logfire-0.32.1/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_slow_async_callbacks.py` & `logfire-0.32.1/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_source_code_extraction.py` & `logfire-0.32.1/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_stdlib_logging.py` & `logfire-0.32.1/tests/test_stdlib_logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_structlog.py` & `logfire-0.32.1/tests/test_structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_testing.py` & `logfire-0.32.1/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/test_utils.py` & `logfire-0.32.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/utils.py` & `logfire-0.32.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/exporters/test_fallback_exporter.py` & `logfire-0.32.1/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/exporters/test_file_exporter.py` & `logfire-0.32.1/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/exporters/test_otlp_session.py` & `logfire-0.32.1/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/exporters/test_remove_pending.py` & `logfire-0.32.1/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.32.1/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.32.1/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_asgi.py` & `logfire-0.32.1/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_asyncpg.py` & `logfire-0.32.1/tests/otel_integrations/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_django.py` & `logfire-0.32.1/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_fastapi.py` & `logfire-0.32.1/tests/otel_integrations/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_flask.py` & `logfire-0.32.1/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_httpx.py` & `logfire-0.32.1/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_openai.py` & `logfire-0.32.1/tests/otel_integrations/test_openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_psycopg.py` & `logfire-0.32.1/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_requests.py` & `logfire-0.32.1/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.32.1/tests/otel_integrations/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_starlette.py` & `logfire-0.32.1/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/test_wsgi.py` & `logfire-0.32.1/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.32.1/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/LICENSE` & `logfire-0.32.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/README.md` & `logfire-0.32.1/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.32.0/pyproject.toml` & `logfire-0.32.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.32.0"
+version = "0.32.1"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
```

### Comparing `logfire-0.32.0/PKG-INFO` & `logfire-0.32.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.32.0
+Version: 0.32.1
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

