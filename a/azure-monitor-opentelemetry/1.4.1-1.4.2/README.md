# Comparing `tmp/azure-monitor-opentelemetry-1.4.1.tar.gz` & `tmp/azure-monitor-opentelemetry-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-monitor-opentelemetry-1.4.1.tar", last modified: Fri Apr 26 19:16:06 2024, max compression
+gzip compressed data, was "azure-monitor-opentelemetry-1.4.2.tar", last modified: Tue May 14 23:27:18 2024, max compression
```

## Comparing `azure-monitor-opentelemetry-1.4.1.tar` & `azure-monitor-opentelemetry-1.4.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10928 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      199 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8273 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/NOTICE.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20095 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19172 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.909411 azure-monitor-opentelemetry-1.4.1/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      480 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      305 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3140 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/distro.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8768 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_configure.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1893 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_constants.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3582 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2157 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/status_logger.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      709 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_types.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.913411 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2065 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5914 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/configurations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      325 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_version.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.917411 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20095 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3081 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      295 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/entry_points.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      481 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-26 19:16:06.000000 azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      135 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.917411 azure-monitor-opentelemetry-1.4.1/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5377 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.917411 azure-monitor-opentelemetry-1.4.1/samples/logging/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1285 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/basic.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      845 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/correlated_logs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/custom_properties.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      818 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/exception_logs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/logging/logs_with_traces.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.917411 azure-monitor-opentelemetry-1.4.1/samples/metrics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      904 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/metrics/attributes.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1579 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/metrics/instruments.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      542 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/azure_core.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      740 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/db_psycopg2.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.909411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      157 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/admin.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      240 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/apps.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/migrations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/migrations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      151 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      154 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/tests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      262 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/urls.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      626 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/views.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1130 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/manage.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      871 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/asgi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3404 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/settings.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      820 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/urls.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/wsgi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2096 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/filter_spans.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1217 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_fastapi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1088 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_flask.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1302 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1106 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_urllib.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/http_urllib3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/instrumentation_options.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/manually_instrumented.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1306 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/modify_spans.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      801 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/sampling.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/samples/tracing/simple.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3719 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/tests/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/tests/autoinstrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2454 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/autoinstrumentation/test_configurator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6167 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/autoinstrumentation/test_distro.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      515 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/conftest.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/tests/diagnostics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6878 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/diagnostics/test_diagnostic_logging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5030 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/diagnostics/test_status_logger.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.921411 azure-monitor-opentelemetry-1.4.1/tests/exporter/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1365 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/exporter/test_exporter.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_django.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      849 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_fastapi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      839 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_flask.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      953 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_psycopg2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_urllib.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      769 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_urllib3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17585 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/test_configure.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-26 19:16:06.925412 azure-monitor-opentelemetry-1.4.1/tests/utils/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10091 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/utils/test_configurations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4396 2024-04-26 19:14:33.000000 azure-monitor-opentelemetry-1.4.1/tests/utils/test_utils.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11093 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      199 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8273 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/NOTICE.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20095 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19172 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.320917 azure-monitor-opentelemetry-1.4.2/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.320917 azure-monitor-opentelemetry-1.4.2/azure/monitor/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.320917 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      480 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      305 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3140 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/distro.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8768 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_configure.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1893 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_constants.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3611 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2282 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/status_logger.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      709 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_types.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2065 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5914 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/configurations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      325 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_version.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20095 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3081 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      295 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/entry_points.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      481 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      135 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5377 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.328917 azure-monitor-opentelemetry-1.4.2/samples/logging/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1285 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/basic.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      845 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/correlated_logs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/custom_properties.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      818 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/exception_logs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/logs_with_traces.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.328917 azure-monitor-opentelemetry-1.4.2/samples/metrics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      904 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/metrics/attributes.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1579 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/metrics/instruments.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.328917 azure-monitor-opentelemetry-1.4.2/samples/tracing/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      542 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/azure_core.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      740 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/db_psycopg2.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.316917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.328917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      157 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/admin.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      240 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/apps.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/migrations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/migrations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      151 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      154 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/tests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      262 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/urls.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      626 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/views.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1130 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/manage.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      871 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/asgi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3404 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/settings.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      820 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/urls.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/wsgi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2096 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/filter_spans.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1217 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_fastapi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1088 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_flask.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1302 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1106 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_urllib.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_urllib3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/instrumentation_options.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/manually_instrumented.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1306 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/modify_spans.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      801 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/sampling.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/simple.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3719 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/tests/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2454 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/test_configurator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6167 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/test_distro.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      515 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/conftest.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/tests/diagnostics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6878 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/diagnostics/test_diagnostic_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5886 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/diagnostics/test_status_logger.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/tests/exporter/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1365 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/exporter/test_exporter.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_django.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      849 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_fastapi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      839 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_flask.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      953 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_psycopg2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_urllib.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      769 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_urllib3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17585 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/test_configure.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/tests/utils/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10091 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/utils/test_configurations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4396 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/utils/test_utils.py
```

### Comparing `azure-monitor-opentelemetry-1.4.1/CHANGELOG.md` & `azure-monitor-opentelemetry-1.4.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Release History
 
+## 1.4.2 (2024-05-20)
+
+### Features Added
+
+- Add diagnostics for sdk detection and backoff
+    ([#35610](https://github.com/Azure/azure-sdk-for-python/pull/35610))
+
 ## 1.4.1 (2024-04-25)
 
 ### Features Added
 
 - Enable sampling for attach
     ([#35218](https://github.com/Azure/azure-sdk-for-python/pull/35218))
```

### Comparing `azure-monitor-opentelemetry-1.4.1/LICENSE` & `azure-monitor-opentelemetry-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/NOTICE.txt` & `azure-monitor-opentelemetry-1.4.2/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/PKG-INFO` & `azure-monitor-opentelemetry-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-opentelemetry
-Version: 1.4.1
+Version: 1.4.2
 Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `azure-monitor-opentelemetry-1.4.1/README.md` & `azure-monitor-opentelemetry-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py` & `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_autoinstrumentation/distro.py` & `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/distro.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_configure.py` & `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_configure.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_constants.py` & `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_constants.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py` & `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 _logger.setLevel(logging.INFO)
 _DIAGNOSTIC_LOG_PATH = _get_log_path()
 _DISTRO_DETECTS_ATTACH = "4100"
 _ATTACH_SUCCESS_DISTRO = "4200"
 _ATTACH_SUCCESS_CONFIGURATOR = "4201"
 _ATTACH_FAILURE_DISTRO = "4400"
 _ATTACH_FAILURE_CONFIGURATOR = "4401"
+_ATTACH_DETECTS_SDK = "4402"
 
 
 class AzureDiagnosticLogging:
     _initialized = False
     _lock = threading.Lock()
 
     @classmethod
```

### Comparing `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_diagnostics/status_logger.py` & `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/status_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,35 +23,37 @@
 
 def _get_status_logger_file_name(pid):
     return f"status_{_MACHINE_NAME}_{pid}.json"
 
 class AzureStatusLogger:
     @classmethod
     def _get_status_json(
-        cls, agent_initialized_successfully, pid, reason=None
+        cls, agent_initialized_successfully, pid, reason=None, sdk_present=None
     ):
         status_json = {
             "AgentInitializedSuccessfully": agent_initialized_successfully,
             "AppType": "python",
             "MachineName": _MACHINE_NAME,
             "PID": pid,
             "SdkVersion": VERSION,
             "Ikey": _get_customer_ikey_from_env_var(),
             "ExtensionVersion": _EXTENSION_VERSION,
         }
         if reason:
             status_json["Reason"] = reason
+        if sdk_present:
+            status_json["SDKPresent"] = sdk_present
         return status_json
 
     @classmethod
-    def log_status(cls, agent_initialized_successfully, reason=None):
+    def log_status(cls, agent_initialized_successfully, reason=None, sdk_present=None):
         if _IS_DIAGNOSTICS_ENABLED and _STATUS_LOG_PATH:
             pid = getpid()
             status_json = AzureStatusLogger._get_status_json(
-                agent_initialized_successfully, pid, reason
+                agent_initialized_successfully, pid, reason, sdk_present
             )
             if not exists(_STATUS_LOG_PATH):
                 makedirs(_STATUS_LOG_PATH)
             # Change to be hostname and pid
             status_logger_file_name = _get_status_logger_file_name(pid)
             with open(
                 join(_STATUS_LOG_PATH, status_logger_file_name),
```

### Comparing `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_types.py` & `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_types.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/__init__.py` & `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/azure/monitor/opentelemetry/_utils/configurations.py` & `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/configurations.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/PKG-INFO` & `azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-opentelemetry
-Version: 1.4.1
+Version: 1.4.2
 Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `azure-monitor-opentelemetry-1.4.1/azure_monitor_opentelemetry.egg-info/SOURCES.txt` & `azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/README.md` & `azure-monitor-opentelemetry-1.4.2/samples/README.md`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/logging/basic.py` & `azure-monitor-opentelemetry-1.4.2/samples/logging/basic.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/logging/correlated_logs.py` & `azure-monitor-opentelemetry-1.4.2/samples/logging/correlated_logs.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/logging/custom_properties.py` & `azure-monitor-opentelemetry-1.4.2/samples/logging/custom_properties.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/logging/exception_logs.py` & `azure-monitor-opentelemetry-1.4.2/samples/logging/exception_logs.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/logging/logs_with_traces.py` & `azure-monitor-opentelemetry-1.4.2/samples/logging/logs_with_traces.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/metrics/attributes.py` & `azure-monitor-opentelemetry-1.4.2/samples/metrics/attributes.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/metrics/instruments.py` & `azure-monitor-opentelemetry-1.4.2/samples/metrics/instruments.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/azure_core.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/azure_core.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/db_psycopg2.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/db_psycopg2.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/example/views.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/views.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/manage.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/manage.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/asgi.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/asgi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/settings.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/settings.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/urls.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/urls.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/django/sample/sample/wsgi.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/wsgi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/filter_spans.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/filter_spans.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_fastapi.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_fastapi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_flask.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_flask.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_requests.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_requests.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_urllib.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_urllib.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/http_urllib3.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/instrumentation_options.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/instrumentation_options.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/manually_instrumented.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/manually_instrumented.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/modify_spans.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/modify_spans.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/sampling.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/sampling.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/samples/tracing/simple.py` & `azure-monitor-opentelemetry-1.4.2/samples/tracing/simple.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/setup.py` & `azure-monitor-opentelemetry-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/autoinstrumentation/test_configurator.py` & `azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/test_configurator.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/autoinstrumentation/test_distro.py` & `azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/test_distro.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/conftest.py` & `azure-monitor-opentelemetry-1.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/diagnostics/test_diagnostic_logging.py` & `azure-monitor-opentelemetry-1.4.2/tests/diagnostics/test_diagnostic_logging.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/diagnostics/test_status_logger.py` & `azure-monitor-opentelemetry-1.4.2/tests/diagnostics/test_status_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,29 +62,33 @@
     ).start()
     patch(
         "azure.monitor.opentelemetry._diagnostics.status_logger._MACHINE_NAME",
         TEST_MACHINE_NAME,
     ).start()
 
 
-def check_file_for_messages(agent_initialized_successfully, file_path, reason=None):
+def check_file_for_messages(agent_initialized_successfully, file_path, reason=None, sdk_present=None):
     with open(file_path, "r") as f:
         f.seek(0)
         json = loads(f.readline())
         assert json["AgentInitializedSuccessfully"] == agent_initialized_successfully
         assert json["AppType"] == "python"
         assert json["MachineName"] == TEST_MACHINE_NAME
         assert json["PID"] == TEST_PID
         assert json["SdkVersion"] == TEST_VERSION
         assert json["Ikey"] == TEST_CUSTOMER_IKEY
         assert json["ExtensionVersion"] == TEST_EXTENSION_VERSION
         if reason:
             assert json["Reason"] == reason
         else:
             assert "Reason" not in json
+        if sdk_present:
+            assert json["SDKPresent"] == sdk_present
+        else:
+            assert "SDKPresent" not in json
         assert not f.read()
 
 
 def check_file_is_empty(file_path):
     with open(file_path, "r") as f:
         f.seek(0)
         assert not f.read()
@@ -106,14 +110,20 @@
 
     def test_log_status_no_reason(self, temp_file_path):
         set_up(temp_file_path, is_diagnostics_enabled=True)
         AzureStatusLogger.log_status(False, MESSAGE1)
         AzureStatusLogger.log_status(True)
         check_file_for_messages(True, temp_file_path)
 
+    def test_log_status_sdk_present(self, temp_file_path):
+        set_up(temp_file_path, is_diagnostics_enabled=True)
+        AzureStatusLogger.log_status(True, reason=MESSAGE1)
+        AzureStatusLogger.log_status(False, reason=MESSAGE2, sdk_present=True)
+        check_file_for_messages(agent_initialized_successfully=False, file_path=temp_file_path, reason=MESSAGE2, sdk_present=True)
+
     def test_disabled_log_status_success(self, temp_file_path):
         set_up(temp_file_path, is_diagnostics_enabled=False)
         AzureStatusLogger.log_status(False, MESSAGE1)
         AzureStatusLogger.log_status(True, MESSAGE2)
         check_file_is_empty(temp_file_path)
 
     def test_disabled_log_status_failed_initialization(self, temp_file_path):
@@ -124,13 +134,19 @@
 
     def test_disabled_log_status_no_reason(self, temp_file_path):
         set_up(temp_file_path, is_diagnostics_enabled=False)
         AzureStatusLogger.log_status(False, MESSAGE1)
         AzureStatusLogger.log_status(True)
         check_file_is_empty(temp_file_path)
 
+    def test_disabled_log_status_sdk_present(self, temp_file_path):
+        set_up(temp_file_path, is_diagnostics_enabled=False)
+        AzureStatusLogger.log_status(True, reason=MESSAGE1)
+        AzureStatusLogger.log_status(False, reason=MESSAGE2, sdk_present=True)
+        check_file_is_empty(temp_file_path)
+
     @patch(
         "azure.monitor.opentelemetry._diagnostics.status_logger._MACHINE_NAME",
         TEST_MACHINE_NAME,
     )
     def test_get_status_logger_file_name(self):
         assert _get_status_logger_file_name(TEST_PID) == f"status_{TEST_MACHINE_NAME}_{TEST_PID}.json"
```

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/exporter/test_exporter.py` & `azure-monitor-opentelemetry-1.4.2/tests/exporter/test_exporter.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_django.py` & `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_django.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_fastapi.py` & `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_flask.py` & `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_flask.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_psycopg2.py` & `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_psycopg2.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_requests.py` & `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_requests.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_urllib.py` & `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_urllib.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/instrumentation/test_urllib3.py` & `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_urllib3.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/test_configure.py` & `azure-monitor-opentelemetry-1.4.2/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/utils/test_configurations.py` & `azure-monitor-opentelemetry-1.4.2/tests/utils/test_configurations.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.1/tests/utils/test_utils.py` & `azure-monitor-opentelemetry-1.4.2/tests/utils/test_utils.py`

 * *Files identical despite different names*

