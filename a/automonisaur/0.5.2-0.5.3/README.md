# Comparing `tmp/automonisaur-0.5.2.tar.gz` & `tmp/automonisaur-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automonisaur-0.5.2.tar", last modified: Wed May  8 09:52:49 2024, max compression
+gzip compressed data, was "automonisaur-0.5.3.tar", last modified: Wed May 15 18:06:23 2024, max compression
```

## Comparing `automonisaur-0.5.2.tar` & `automonisaur-0.5.3.tar`

### file list

```diff
@@ -1,416 +1,416 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 09:52:45.000000 automonisaur-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-08 09:52:49.011735 automonisaur-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-08 09:52:45.000000 automonisaur-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.963735 automonisaur-0.5.2/automon/
--rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/assertions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/asyncioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/asyncioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/asyncioWrapper/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/cryptography/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/cryptography/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/cryptography/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/httpWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/mathWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/mathWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/mathWrapper/file_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/osWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/osWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/osWrapper/environ.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/sanitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.967735 automonisaur-0.5.2/automon/helpers/subprocessWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_sanitation.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_sleeper.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/tests/test_sleeper_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/helpers/threadingWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/threadingWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/threadingWrapper/initialize_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/helpers/threadingWrapper/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/integrations/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/integrations/beautifulsoupWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/beautifulsoupWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/beautifulsoupWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/integrations/cryptocurrency/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/accounting.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/robinhood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.971735 automonisaur-0.5.2/automon/integrations/cryptocurrency/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/cryptocurrency/tests/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datadogWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datadogWrapper/api/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/api/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/api/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/client_opentelemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/config_opentelemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_client_opentelemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_config_opentelemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datascience/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datascience/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/pandas/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/pandas/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/datascience/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/datascience/tests/test_datascience.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.975735 automonisaur-0.5.2/automon/integrations/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/facebook/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/flaskWrapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/auth_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/flaskWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/flaskWrapper/tests/test_flask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/geoip/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/geoip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/geoip/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/geoip/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/geoip/tests/test_geoip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/tests/test_config_Credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/auth/tests/test_google_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/gmail/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/gmail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.979735 automonisaur-0.5.2/automon/integrations/google/gmail/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/gmail/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/gmail/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/gmail/v1/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/people/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/people/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/tests/test_google_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/tests/test_google_contacts_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/people/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/sheets/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/sheets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets_clear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/google/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/tests/test_google_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/google/tests/test_google_contacts_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/grok/
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/grok/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/grok/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/grok/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/grok/tests/test_grok.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/instagram/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/stories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.983735 automonisaur-0.5.2/automon/integrations/instagram/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_browser_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/instagram/xpaths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/ldap/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/ldap/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/airport/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/airport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/ssid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/airport/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/tests/test_airport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/airport/tests/test_airport_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/macchanger/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/test_macchanger.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/test_set_mac_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/minioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.987735 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client_public.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/neo4jWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/cypher.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/nest_asyncioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nest_asyncioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nest_asyncioWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/nmap/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/nmap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/tests/test_nmap_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/nmap/tests/test_nmap_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/test_client_ready.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/test_memory_trace_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/test_memory_trace_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/test/test_pop_finished_spans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/openvpn/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openvpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/openvpn/openvpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.991735 automonisaur-0.5.2/automon/integrations/psutilWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/psutilWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/psutilWrapper/cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/requestsWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/test_rest_inherit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/scrapyWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/scrapyWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/scrapyWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/seleniumWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17113 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/config_window_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.995735 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser_headless.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_new_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/user_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/seleniumWrapper/webdriver_chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/sentryio/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/sentryio/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/tests/test_sentryio.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/sentryio/tests/test_sentryio_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/shodan/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/shodan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/shodan/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/shodan/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/shodan/tests/test_shodan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/slackWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/bots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/slack_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/slack_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/slackWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/slackWrapper/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/snmp/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/snmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/snmp/generate_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/splunk/
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:48.999735 automonisaur-0.5.2/automon/integrations/splunk/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/tests/test_splunk_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk/tests/test_splunk_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.003735 automonisaur-0.5.2/automon/integrations/splunk_soar/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/action_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    25563 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.003735 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.003735 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/ticket.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/phantom_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.003735 automonisaur-0.5.2/automon/integrations/splunk_soar/rest/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/rest/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   899665 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/dino.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_filter_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_get_action_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_by_playbook_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/splunk_soar/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/swift/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/iterables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/swift/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swift/tests/test_swift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.007735 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/api/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/integrations/vds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/integrations/vds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/integrations/vds/tests/test_vds.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/liveliness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/log/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automon/log/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-08 09:52:45.000000 automonisaur-0.5.2/automon/log/tests/test_logger_builtin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:52:49.011735 automonisaur-0.5.2/automonisaur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-08 09:52:48.000000 automonisaur-0.5.2/automonisaur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-08 09:52:48.000000 automonisaur-0.5.2/automonisaur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:52:48.000000 automonisaur-0.5.2/automonisaur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 09:52:48.000000 automonisaur-0.5.2/automonisaur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:52:49.011735 automonisaur-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 09:52:45.000000 automonisaur-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 18:06:19.000000 automonisaur-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-15 18:06:23.037043 automonisaur-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-15 18:06:19.000000 automonisaur-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/assertions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/asyncioWrapper/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/cryptography/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/cryptography/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/cryptography/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/httpWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/mathWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/mathWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/mathWrapper/file_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/osWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/osWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/osWrapper/environ.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/subprocessWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/test_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_sleeper_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/helpers/threadingWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/threadingWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/threadingWrapper/initialize_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/threadingWrapper/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/beautifulsoupWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/beautifulsoupWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/beautifulsoupWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/cryptocurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/accounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/robinhood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/cryptocurrency/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/tests/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/datadogWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datadogWrapper/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/api/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/client_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/config_opentelemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_client_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_config_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datascience/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datascience/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/pandas/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/pandas/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datascience/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/tests/test_datascience.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22254 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/facebook/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/flaskWrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/auth_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/flaskWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/tests/test_flask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/geoip/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/geoip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/geoip/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/geoip/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/geoip/tests/test_geoip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/tests/test_config_Credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/tests/test_google_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/gmail/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/gmail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/gmail/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/gmail/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/gmail/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/gmail/v1/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/people/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/google/people/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/tests/test_google_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/tests/test_google_contacts_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/google/sheets/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/google/sheets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets_clear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/google/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/tests/test_google_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/tests/test_google_contacts_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/grok/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/grok/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/grok/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/grok/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/grok/tests/test_grok.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/instagram/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/stories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/instagram/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_browser_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/xpaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/ldap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/ldap/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/airport/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/airport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/ssid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/airport/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/tests/test_airport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/tests/test_airport_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/macchanger/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/test_macchanger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/test_set_mac_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/minioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/neo4jWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/nest_asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nest_asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nest_asyncioWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/nmap/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/nmap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/tests/test_nmap_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/tests/test_nmap_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/test_client_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/test_memory_trace_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/test_memory_trace_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/test_pop_finished_spans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/openvpn/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openvpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openvpn/openvpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/psutilWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/psutilWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/psutilWrapper/cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/requestsWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/test_rest_inherit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/scrapyWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/scrapyWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/scrapyWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/seleniumWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17113 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/config_window_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser_headless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_new_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/user_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/webdriver_chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/sentryio/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/sentryio/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/tests/test_sentryio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/tests/test_sentryio_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/shodan/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/shodan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/shodan/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/shodan/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/shodan/tests/test_shodan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/slackWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/bots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/slack_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/slack_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/slackWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/snmp/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/snmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/snmp/generate_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/splunk/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/splunk/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/tests/test_splunk_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/tests/test_splunk_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.029043 automonisaur-0.5.3/automon/integrations/splunk_soar/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/action_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25563 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.029043 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.029043 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/ticket.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/phantom_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.029043 automonisaur-0.5.3/automon/integrations/splunk_soar/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/rest/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   899665 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_filter_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_get_action_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_by_playbook_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/swift/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/iterables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/swift/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/tests/test_swift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/api/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/integrations/vds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/integrations/vds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/tests/test_vds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/liveliness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/log/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/log/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/tests/test_logger_builtin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automonisaur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-15 18:06:22.000000 automonisaur-0.5.3/automonisaur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-15 18:06:22.000000 automonisaur-0.5.3/automonisaur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:06:22.000000 automonisaur-0.5.3/automonisaur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 18:06:22.000000 automonisaur-0.5.3/automonisaur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:06:23.037043 automonisaur-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-15 18:06:19.000000 automonisaur-0.5.3/setup.py
```

### Comparing `automonisaur-0.5.2/LICENSE` & `automonisaur-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/PKG-INFO` & `automonisaur-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.5.2
+Version: 0.5.3
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `automonisaur-0.5.2/README.md` & `automonisaur-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/assertions.py` & `automonisaur-0.5.3/automon/helpers/assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/markdown.py` & `automonisaur-0.5.3/automon/helpers/markdown.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/networking.py` & `automonisaur-0.5.3/automon/helpers/networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/osWrapper/environ.py` & `automonisaur-0.5.3/automon/helpers/osWrapper/environ.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/sanitation.py` & `automonisaur-0.5.3/automon/helpers/sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/sleeper.py` & `automonisaur-0.5.3/automon/helpers/sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/subprocessWrapper/run.py` & `automonisaur-0.5.3/automon/helpers/subprocessWrapper/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,105 +78,88 @@
     def which(self, program: str, *args, **kwargs) -> bool:
         """runs which
 
         :param program:
         :return:
         """
         logger.debug(str(dict(
-            program=program,
+            which=program,
             args=args,
             kwargs=kwargs,
         )))
-        if program:
-            return self.run(command=f'which {program}', *args, **kwargs)
-        return False
+        return self.run(command=f'which {program}', *args, **kwargs)
 
     def run_command(self, *args, **kwargs) -> bool:
         """alias to run"""
         logger.debug(str(dict(
             args=args,
             kwargs=kwargs,
         )))
         return self.run(*args, **kwargs)
 
     def run(
             self,
             command: str,
+            pipe: bool = False,
             text: bool = False,
-            inBackground: bool = False,
             shell: bool = False,
             sanitize_command: bool = True,
             **kwargs
     ) -> bool:
 
-        self.command = command
+        if not pipe:
+            self.command = command
 
-        if sanitize_command:
+        if sanitize_command and not shell:
             command = self.sanitize_command(command)
 
         if not command:
             logger.error(str(dict(
                 command=command,
                 text=text,
-                inBackground=inBackground,
                 shell=shell,
                 sanitize_command=sanitize_command,
                 kwargs=kwargs,
             )))
             raise SyntaxError(f'command cannot be empty, {command}')
 
         logger.debug(str(dict(
-            command=self.command,
+            command=command,
             text=text,
-            inBackground=inBackground,
             shell=shell,
             sanitize_command=sanitize_command,
             kwargs=kwargs,
         )))
 
         try:
-            if inBackground:
-                if 'text' in dir(subprocess.Popen):
-                    self.call = subprocess.Popen(args=command, text=text, shell=shell, **kwargs)
-                else:
-                    self.call = subprocess.Popen(args=command, shell=shell, **kwargs)
+
+            self.call = subprocess.Popen(
+                args=command,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                text=text,
+                shell=shell,
+                **kwargs)
+
+            stdout, stderr = self.call.communicate()
+            # self.call.wait()
+
+            timestamp = Dates.iso()
+
+            self.last_run = timestamp
+            self._stdout = stdout
+            self._stderr = stderr
+            self.returncode = self.call.returncode
+
+            if self.returncode == 0:
+                logger.debug(str(dict(
+                    stdout_KB=round(len(self.stdout) / 1024, 2),
+                    stderr_KB=round(len(self.stderr) / 1024, 2),
+                )))
                 return True
-            else:
-                if 'text' in dir(subprocess.Popen):
-                    self.call = subprocess.Popen(
-                        args=command,
-                        stdout=subprocess.PIPE,
-                        stderr=subprocess.PIPE,
-                        text=text,
-                        shell=shell,
-                        **kwargs)
-                else:
-                    self.call = subprocess.Popen(
-                        args=command,
-                        stdout=subprocess.PIPE,
-                        stderr=subprocess.PIPE,
-                        shell=shell,
-                        **kwargs)
-
-                stdout, stderr = self.call.communicate()
-                # call.wait()
-
-                timestamp = Dates.iso()
-
-                self.last_run = timestamp
-                self._stdout = stdout
-                self._stderr = stderr
-                self.returncode = self.call.returncode
-
-                if self.returncode == 0:
-                    logger.debug(str(dict(
-                        stdout_KB=round(len(self.stdout) / 1024, 2),
-                        stderr_KB=round(len(self.stderr) / 1024, 2),
-                    )))
-                    return True
 
         except Exception as error:
             self._stderr = f'{error}'.encode()
             logger.error(f'{error}')
             raise RuntimeError(error)
 
         logger.error(str(dict(
@@ -184,30 +167,41 @@
             stderr_KB=round(len(self.stderr) / 1024, 2),
         )))
         return False
 
     def sanitize_command(self, command: str) -> [str]:
 
         if isinstance(command, str):
-            split_command = f'{command}'.split(' ')
-            split_command = [str(x).strip() for x in split_command]
-            split_command = [x for x in split_command if x]
-            command = split_command
-
-            for arg in split_command:
-                if '|' in arg:
-                    error = f'Pipes are not supported! {split_command}'
-                    logger.error(error)
-                    raise NotSupportedCommand(error)
+
+            if '|' in command:
+                command = self.sanitize_command_pipe(command=command)
+                command = [self.sanitize_command_spaces(command=cmd) for cmd in command]
+            else:
+                command = self.sanitize_command_spaces(command=command)
 
         logger.debug(str(dict(
             command=command
         )))
         return command
 
+    def sanitize_command_pipe(self, command: str) -> [str]:
+        """support for shell command piping"""
+        error = f'Pipes are not supported! To use run(shell=True). {command}'
+        logger.error(error)
+        raise NotSupportedCommand(error)
+
+        split_command = f'{command}'.split('|')
+        return split_command
+
+    def sanitize_command_spaces(self, command: str) -> [str]:
+        split_command = f'{command}'.split(' ')
+        split_command = [str(x).strip() for x in split_command]
+        split_command = [x for x in split_command if x]
+        return split_command
+
     def __repr__(self) -> str:
         return str(dict(
             command=self.command,
             stdout=f'{round(len(self.stdout) / 1024, 2)} KB',
             stderr=f'{round(len(self.stderr) / 1024, 2)} KB',
         ))
```

### Comparing `automonisaur-0.5.2/automon/helpers/subprocessWrapper/tests/test_runner.py` & `automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/tests/test_assertions.py` & `automonisaur-0.5.3/automon/helpers/tests/test_assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/tests/test_networking.py` & `automonisaur-0.5.3/automon/helpers/tests/test_networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/tests/test_sanitation.py` & `automonisaur-0.5.3/automon/helpers/tests/test_sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/tests/test_sleeper.py` & `automonisaur-0.5.3/automon/helpers/tests/test_sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/threadingWrapper/initialize_threading.py` & `automonisaur-0.5.3/automon/helpers/threadingWrapper/initialize_threading.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/helpers/threadingWrapper/worker_thread.py` & `automonisaur-0.5.3/automon/helpers/threadingWrapper/worker_thread.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/beautifulsoupWrapper/client.py` & `automonisaur-0.5.3/automon/integrations/beautifulsoupWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/cryptocurrency/accounting.py` & `automonisaur-0.5.3/automon/integrations/cryptocurrency/accounting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/cryptocurrency/coinbase.py` & `automonisaur-0.5.3/automon/integrations/cryptocurrency/coinbase.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/cryptocurrency/other.py` & `automonisaur-0.5.3/automon/integrations/cryptocurrency/other.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/cryptocurrency/robinhood.py` & `automonisaur-0.5.3/automon/integrations/cryptocurrency/robinhood.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/cryptocurrency/tests/test_crypto.py` & `automonisaur-0.5.3/automon/integrations/cryptocurrency/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/datadogWrapper/client.py` & `automonisaur-0.5.3/automon/integrations/datadogWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/datadogWrapper/client_opentelemetry.py` & `automonisaur-0.5.3/automon/integrations/datadogWrapper/client_opentelemetry.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/datadogWrapper/config.py` & `automonisaur-0.5.3/automon/integrations/datadogWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/datadogWrapper/config_opentelemetry.py` & `automonisaur-0.5.3/automon/integrations/datadogWrapper/config_opentelemetry.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/datadogWrapper/tests/test_log.py` & `automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/datascience/pandas/pandas.py` & `automonisaur-0.5.3/automon/integrations/datascience/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/datascience/tests/test_datascience.py` & `automonisaur-0.5.3/automon/integrations/datascience/tests/test_datascience.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/elasticsearch/cleanup.py` & `automonisaur-0.5.3/automon/integrations/elasticsearch/cleanup.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/elasticsearch/client.py` & `automonisaur-0.5.3/automon/integrations/elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/elasticsearch/config.py` & `automonisaur-0.5.3/automon/integrations/elasticsearch/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/elasticsearch/jvm.py` & `automonisaur-0.5.3/automon/integrations/elasticsearch/jvm.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/elasticsearch/metrics.py` & `automonisaur-0.5.3/automon/integrations/elasticsearch/metrics.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/elasticsearch/snapshots.py` & `automonisaur-0.5.3/automon/integrations/elasticsearch/snapshots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch.py` & `automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py` & `automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py` & `automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/facebook/groups.py` & `automonisaur-0.5.3/automon/integrations/facebook/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,33 +548,33 @@
         return self.url
 
     async def start(self, headless: bool = True, random_user_agent: bool = False, set_user_agent: str = None):
         """start new instance of selenium"""
         self._browser.config.webdriver_wrapper = ChromeWrapper()
 
         if headless:
-            await self._browser.config.webdriver_wrapper.enable_headless()
-            await self._browser.config.webdriver_wrapper.set_locale_experimental()
+            self._browser.config.webdriver_wrapper.enable_headless()
+            self._browser.config.webdriver_wrapper.set_locale_experimental()
         else:
-            await self._browser.config.webdriver_wrapper.set_locale_experimental()
+            self._browser.config.webdriver_wrapper.set_locale_experimental()
 
         if random_user_agent:
-            await self._browser.config.webdriver_wrapper.set_user_agent(
+            self._browser.config.webdriver_wrapper.set_user_agent(
                 await self._browser.get_random_user_agent()
             )
         elif set_user_agent:
-            await self._browser.config.webdriver_wrapper.set_user_agent(
+            self._browser.config.webdriver_wrapper.set_user_agent(
                 set_user_agent
             )
 
         logger.info(str(dict(
             browser=self._browser
         )))
         browser = await self._browser.run()
-        await self._browser.config.webdriver_wrapper.set_window_size(width=1920 * 0.6, height=1080)
+        self._browser.config.webdriver_wrapper.set_window_size(width=1920 * 0.6, height=1080)
         return browser
 
     async def stop(self):
         """alias to quit"""
         return await self.quit()
 
     async def to_dict(self):
```

### Comparing `automonisaur-0.5.2/automon/integrations/flaskWrapper/auth.py` & `automonisaur-0.5.3/automon/integrations/flaskWrapper/auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/flaskWrapper/boilerplate.py` & `automonisaur-0.5.3/automon/integrations/flaskWrapper/boilerplate.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/flaskWrapper/config.py` & `automonisaur-0.5.3/automon/integrations/flaskWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/flaskWrapper/tests/test_flask.py` & `automonisaur-0.5.3/automon/integrations/flaskWrapper/tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/auth/client.py` & `automonisaur-0.5.3/automon/integrations/google/auth/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/auth/config.py` & `automonisaur-0.5.3/automon/integrations/google/auth/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/gmail/v1/client.py` & `automonisaur-0.5.3/automon/integrations/google/gmail/v1/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/gmail/v1/config.py` & `automonisaur-0.5.3/automon/integrations/google/gmail/v1/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/people/client.py` & `automonisaur-0.5.3/automon/integrations/google/people/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/people/config.py` & `automonisaur-0.5.3/automon/integrations/google/people/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/people/person.py` & `automonisaur-0.5.3/automon/integrations/google/people/person.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/people/results.py` & `automonisaur-0.5.3/automon/integrations/google/people/results.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/people/urls.py` & `automonisaur-0.5.3/automon/integrations/google/people/urls.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/sheets/client.py` & `automonisaur-0.5.3/automon/integrations/google/sheets/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/sheets/config.py` & `automonisaur-0.5.3/automon/integrations/google/sheets/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets.py` & `automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py` & `automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/google/sheets/tests/test_google_sheets_clear.py` & `automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets_clear.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/grok/__init__.py` & `automonisaur-0.5.3/automon/integrations/grok/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/instagram/client.py` & `automonisaur-0.5.3/automon/integrations/instagram/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/instagram/client_browser.py` & `automonisaur-0.5.3/automon/integrations/instagram/client_browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/instagram/config.py` & `automonisaur-0.5.3/automon/integrations/instagram/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/instagram/stories.py` & `automonisaur-0.5.3/automon/integrations/instagram/stories.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_browser.py` & `automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/instagram/tests/test_instagram_browser_auth.py` & `automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_browser_auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/instagram/xpaths.py` & `automonisaur-0.5.3/automon/integrations/instagram/xpaths.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/ldap/client.py` & `automonisaur-0.5.3/automon/integrations/ldap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/mac/airport/airport.py` & `automonisaur-0.5.3/automon/integrations/mac/airport/airport.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/mac/airport/scan.py` & `automonisaur-0.5.3/automon/integrations/mac/airport/scan.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/mac/airport/ssid.py` & `automonisaur-0.5.3/automon/integrations/mac/airport/ssid.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/mac/airport/tests/test_airport.py` & `automonisaur-0.5.3/automon/integrations/mac/airport/tests/test_airport.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/mac/airport/tests/test_airport_neo4j.py` & `automonisaur-0.5.3/automon/integrations/mac/airport/tests/test_airport_neo4j.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/mac/macchanger/client.py` & `automonisaur-0.5.3/automon/integrations/mac/macchanger/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/mac/macchanger/tests/test_macchanger.py` & `automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/test_macchanger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/minioWrapper/client.py` & `automonisaur-0.5.3/automon/integrations/minioWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/minioWrapper/config.py` & `automonisaur-0.5.3/automon/integrations/minioWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/minioWrapper/object.py` & `automonisaur-0.5.3/automon/integrations/minioWrapper/object.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client.py` & `automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client_public.py` & `automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client_public.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py` & `automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/neo4jWrapper/client.py` & `automonisaur-0.5.3/automon/integrations/neo4jWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/neo4jWrapper/clientAsync.py` & `automonisaur-0.5.3/automon/integrations/neo4jWrapper/clientAsync.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/neo4jWrapper/config.py` & `automonisaur-0.5.3/automon/integrations/neo4jWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/neo4jWrapper/cypher.py` & `automonisaur-0.5.3/automon/integrations/neo4jWrapper/cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/neo4jWrapper/results.py` & `automonisaur-0.5.3/automon/integrations/neo4jWrapper/results.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py` & `automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py` & `automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py` & `automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/nest_asyncioWrapper/client.py` & `automonisaur-0.5.3/automon/integrations/nest_asyncioWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/nmap/client.py` & `automonisaur-0.5.3/automon/integrations/nmap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/nmap/config.py` & `automonisaur-0.5.3/automon/integrations/nmap/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/nmap/output.py` & `automonisaur-0.5.3/automon/integrations/nmap/output.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/nmap/tests/test_nmap_client.py` & `automonisaur-0.5.3/automon/integrations/nmap/tests/test_nmap_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/client.py` & `automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/openTelemetryWrapper/config.py` & `automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/openvpn/openvpn.py` & `automonisaur-0.5.3/automon/integrations/openvpn/openvpn.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/requestsWrapper/client.py` & `automonisaur-0.5.3/automon/integrations/requestsWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/requestsWrapper/rest.py` & `automonisaur-0.5.3/automon/integrations/requestsWrapper/rest.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/requestsWrapper/tests/test_requests.py` & `automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/actions.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/actions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/browser_types.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser_types.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/config.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/config_window_size.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/config_window_size.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser_headless.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser_headless.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/tests/test_user_agent.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_user_agent.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/user_agents.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/user_agents.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/seleniumWrapper/webdriver_chrome.py` & `automonisaur-0.5.3/automon/integrations/seleniumWrapper/webdriver_chrome.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         self._chrome_options = selenium.webdriver.ChromeOptions()
         self._chromedriver_path = environ_list('SELENIUM_CHROMEDRIVER_PATH')
         self._ChromeService = None
         self._window_size = set_window_size()
 
         self.update_paths(self.chromedriver_path)
 
-        logger.error('missing SELENIUM_CHROMEDRIVER_PATH')
+        if not self.chromedriver_path:
+            logger.error('missing SELENIUM_CHROMEDRIVER_PATH')
 
     def __repr__(self):
         if self._webdriver:
             return str(dict(
                 name=self.webdriver.name,
                 window_size=self.window_size,
                 browserVersion=self.browserVersion,
```

### Comparing `automonisaur-0.5.2/automon/integrations/sentryio/client.py` & `automonisaur-0.5.3/automon/integrations/sentryio/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/sentryio/config.py` & `automonisaur-0.5.3/automon/integrations/sentryio/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/sentryio/tests/test_sentryio.py` & `automonisaur-0.5.3/automon/integrations/sentryio/tests/test_sentryio.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/sentryio/tests/test_sentryio_callback.py` & `automonisaur-0.5.3/automon/integrations/sentryio/tests/test_sentryio_callback.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/shodan/__init__.py` & `automonisaur-0.5.3/automon/integrations/shodan/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/slackWrapper/bots.py` & `automonisaur-0.5.3/automon/integrations/slackWrapper/bots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/slackWrapper/client.py` & `automonisaur-0.5.3/automon/integrations/slackWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/slackWrapper/clientAsync.py` & `automonisaur-0.5.3/automon/integrations/slackWrapper/clientAsync.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/slackWrapper/config.py` & `automonisaur-0.5.3/automon/integrations/slackWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/slackWrapper/error.py` & `automonisaur-0.5.3/automon/integrations/slackWrapper/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/slackWrapper/slack_formatting.py` & `automonisaur-0.5.3/automon/integrations/slackWrapper/slack_formatting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/slackWrapper/slack_logger.py` & `automonisaur-0.5.3/automon/integrations/slackWrapper/slack_logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/slackWrapper/tests/test_slack.py` & `automonisaur-0.5.3/automon/integrations/slackWrapper/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/snmp/generate_maps.py` & `automonisaur-0.5.3/automon/integrations/snmp/generate_maps.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk/client.py` & `automonisaur-0.5.3/automon/integrations/splunk/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk/config.py` & `automonisaur-0.5.3/automon/integrations/splunk/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk/helpers.py` & `automonisaur-0.5.3/automon/integrations/splunk/helpers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk/tests/test_splunk_client.py` & `automonisaur-0.5.3/automon/integrations/splunk/tests/test_splunk_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk/tests/test_splunk_config.py` & `automonisaur-0.5.3/automon/integrations/splunk/tests/test_splunk_config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/client.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/config.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/datatypes.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/datatypes.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/integration/servicenow/ticket.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/ticket.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/phantom_unittest.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/phantom_unittest.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/responses.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/responses.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/rest/urls.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/rest/urls.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/rules.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/rules.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/dino.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/dino.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/splunk_soar/vault.py` & `automonisaur-0.5.3/automon/integrations/splunk_soar/vault.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swift/client.py` & `automonisaur-0.5.3/automon/integrations/swift/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swift/config.py` & `automonisaur-0.5.3/automon/integrations/swift/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swift/error.py` & `automonisaur-0.5.3/automon/integrations/swift/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swift/iterables.py` & `automonisaur-0.5.3/automon/integrations/swift/iterables.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swift/tests/test_swift.py` & `automonisaur-0.5.3/automon/integrations/swift/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/api/v2.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/api/v2.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/client.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/config.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_app.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_app.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py` & `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/vds/client.py` & `automonisaur-0.5.3/automon/integrations/vds/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/integrations/vds/config.py` & `automonisaur-0.5.3/automon/integrations/vds/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/log/__init__.py` & `automonisaur-0.5.3/automon/log/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/log/attributes.py` & `automonisaur-0.5.3/automon/log/attributes.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/log/logger.py` & `automonisaur-0.5.3/automon/log/logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automon/log/tests/test_logger_builtin.py` & `automonisaur-0.5.3/automon/log/tests/test_logger_builtin.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.2/automonisaur.egg-info/PKG-INFO` & `automonisaur-0.5.3/automonisaur.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.5.2
+Version: 0.5.3
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `automonisaur-0.5.2/automonisaur.egg-info/SOURCES.txt` & `automonisaur-0.5.3/automonisaur.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 automon/helpers/mathWrapper/file_size.py
 automon/helpers/osWrapper/__init__.py
 automon/helpers/osWrapper/environ.py
 automon/helpers/subprocessWrapper/__init__.py
 automon/helpers/subprocessWrapper/exceptions.py
 automon/helpers/subprocessWrapper/run.py
 automon/helpers/subprocessWrapper/tests/__init__.py
-automon/helpers/subprocessWrapper/tests/test_pipe.py
 automon/helpers/subprocessWrapper/tests/test_run.py
 automon/helpers/subprocessWrapper/tests/test_runner.py
 automon/helpers/subprocessWrapper/tests/test_sanitize.py
 automon/helpers/tests/__init__.py
 automon/helpers/tests/test_assertions.py
 automon/helpers/tests/test_healthcheck.py
 automon/helpers/tests/test_helpers.py
@@ -141,14 +140,15 @@
 automon/integrations/instagram/tests/test_instagram.py
 automon/integrations/instagram/tests/test_instagram_browser.py
 automon/integrations/instagram/tests/test_instagram_browser_auth.py
 automon/integrations/instagram/tests/test_instagram_config.py
 automon/integrations/ldap/__init__.py
 automon/integrations/ldap/client.py
 automon/integrations/mac/__init__.py
+automon/integrations/mac/check.py
 automon/integrations/mac/airport/__init__.py
 automon/integrations/mac/airport/airport.py
 automon/integrations/mac/airport/scan.py
 automon/integrations/mac/airport/ssid.py
 automon/integrations/mac/airport/tests/__init__.py
 automon/integrations/mac/airport/tests/test_airport.py
 automon/integrations/mac/airport/tests/test_airport_neo4j.py
```

### Comparing `automonisaur-0.5.2/setup.py` & `automonisaur-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="automonisaur",
-    version="0.5.2",
+    version="0.5.3",
     author="naisanza",
     author_email="naisanza@gmail.com",
     description="Core libraries for automonisaur",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheShellLand/automonisaur",
     packages=setuptools.find_packages(),
```

