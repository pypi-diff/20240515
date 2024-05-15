# Comparing `tmp/pytest_fluent-0.3.0.tar.gz` & `tmp/pytest_fluent-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_fluent-0.3.0.tar", last modified: Tue May 14 08:51:32 2024, max compression
+gzip compressed data, was "pytest_fluent-0.3.1.tar", last modified: Wed May 15 13:01:19 2024, max compression
```

## Comparing `pytest_fluent-0.3.0.tar` & `pytest_fluent-0.3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.892866 pytest_fluent-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.880866 pytest_fluent-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.880866 pytest_fluent-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-05-14 08:51:32.892866 pytest_fluent-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.880866 pytest_fluent-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.880866 pytest_fluent-0.3.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/usage/stage_settings.md
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 08:51:32.892866 pytest_fluent-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.876866 pytest_fluent-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.884866 pytest_fluent-0.3.0/src/pytest_fluent/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/additional_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/content_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.884866 pytest_fluent-0.3.0/src/pytest_fluent/data/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/data/default.stage.json
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/data/schema.stage.json
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/importlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17309 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/setting_file_loader_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/src/pytest_fluent/test_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.888866 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 08:51:32.000000 pytest_fluent-0.3.0/src/pytest_fluent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.888866 pytest_fluent-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:51:32.888866 pytest_fluent-0.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/data/complex.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/data/default.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/data/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_additional_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_addoptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_content_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_importlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_ini_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_logging_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_reporting_patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tests/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-14 08:51:12.000000 pytest_fluent-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.746749 pytest_fluent-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.738750 pytest_fluent-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.738750 pytest_fluent-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-05-15 13:01:19.746749 pytest_fluent-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.742750 pytest_fluent-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.742750 pytest_fluent-0.3.1/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/docs/usage/stage_settings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-15 13:01:19.750750 pytest_fluent-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.738750 pytest_fluent-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.742750 pytest_fluent-0.3.1/src/pytest_fluent/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/additional_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/content_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.742750 pytest_fluent-0.3.1/src/pytest_fluent/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/data/default.stage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/data/schema.stage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/importlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17309 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/setting_file_loader_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/src/pytest_fluent/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.746749 pytest_fluent-0.3.1/src/pytest_fluent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-05-15 13:01:19.000000 pytest_fluent-0.3.1/src/pytest_fluent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-15 13:01:19.000000 pytest_fluent-0.3.1/src/pytest_fluent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:01:19.000000 pytest_fluent-0.3.1/src/pytest_fluent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 13:01:19.000000 pytest_fluent-0.3.1/src/pytest_fluent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 13:01:19.000000 pytest_fluent-0.3.1/src/pytest_fluent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 13:01:19.000000 pytest_fluent-0.3.1/src/pytest_fluent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.746749 pytest_fluent-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:01:19.746749 pytest_fluent-0.3.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/data/complex.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/data/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/data/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_additional_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_addoptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_content_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_importlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_ini_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_logging_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_reporting_patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tests/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-15 13:00:59.000000 pytest_fluent-0.3.1/tox.ini
```

### Comparing `pytest_fluent-0.3.0/.github/dependabot.yml` & `pytest_fluent-0.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/.github/workflows/linting.yml` & `pytest_fluent-0.3.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/.github/workflows/python-publish.yml` & `pytest_fluent-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/.github/workflows/tests.yml` & `pytest_fluent-0.3.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/.gitignore` & `pytest_fluent-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/.readthedocs.yaml` & `pytest_fluent-0.3.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/LICENSE` & `pytest_fluent-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/PKG-INFO` & `pytest_fluent-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-fluent
-Version: 0.3.0
+Version: 0.3.1
 Summary: A pytest plugin in order to provide logs via fluentd
 Author-email: "Rohde & Schwarz GmbH & Co. KG" <info@rohde-schwarz.com>
 Maintainer-email: Carsten Sauerbrey <carsten.sauerbrey@rohde-schwarz.com>, Nicola Lambiase <nicola.lambiase@rohde-schwarz.com>
 License: MIT
 Project-URL: project, https://github.com/Rohde-Schwarz/pytest-fluent
 Keywords: pytest,logging,fluent
 Platform: Unix
```

### Comparing `pytest_fluent-0.3.0/README.md` & `pytest_fluent-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/docs/conf.py` & `pytest_fluent-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/docs/usage/stage_settings.md` & `pytest_fluent-0.3.1/docs/usage/stage_settings.md`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/pyproject.toml` & `pytest_fluent-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent/__init__.py` & `pytest_fluent-0.3.1/src/pytest_fluent/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent/additional_information.py` & `pytest_fluent-0.3.1/src/pytest_fluent/additional_information.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent/content_patcher.py` & `pytest_fluent-0.3.1/src/pytest_fluent/content_patcher.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent/data/schema.stage.json` & `pytest_fluent-0.3.1/src/pytest_fluent/data/schema.stage.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'definitions'": "{'LogFormatter': {'additionalProperties': True}}"}*

```diff
@@ -77,15 +77,15 @@
                     "$ref": "#/definitions/RegexString",
                     "default": "<fluentd-tag>"
                 }
             },
             "type": "object"
         },
         "LogFormatter": {
-            "additionalProperties": false,
+            "additionalProperties": true,
             "properties": {
                 "recordFormatter": {
                     "additionalProperties": false,
                     "oneOf": [
                         {
                             "module": {
                                 "regex": "^([a-z_][a-z0-9_]*)+(\\.[a-z_][a-z0-9_]*)*$",
```

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent/event.py` & `pytest_fluent-0.3.1/src/pytest_fluent/event.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent/importlib_utils.py` & `pytest_fluent-0.3.1/src/pytest_fluent/importlib_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent/plugin.py` & `pytest_fluent-0.3.1/src/pytest_fluent/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent/setting_file_loader_action.py` & `pytest_fluent-0.3.1/src/pytest_fluent/setting_file_loader_action.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent/test_report.py` & `pytest_fluent-0.3.1/src/pytest_fluent/test_report.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent.egg-info/PKG-INFO` & `pytest_fluent-0.3.1/src/pytest_fluent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-fluent
-Version: 0.3.0
+Version: 0.3.1
 Summary: A pytest plugin in order to provide logs via fluentd
 Author-email: "Rohde & Schwarz GmbH & Co. KG" <info@rohde-schwarz.com>
 Maintainer-email: Carsten Sauerbrey <carsten.sauerbrey@rohde-schwarz.com>, Nicola Lambiase <nicola.lambiase@rohde-schwarz.com>
 License: MIT
 Project-URL: project, https://github.com/Rohde-Schwarz/pytest-fluent
 Keywords: pytest,logging,fluent
 Platform: Unix
```

### Comparing `pytest_fluent-0.3.0/src/pytest_fluent.egg-info/SOURCES.txt` & `pytest_fluent-0.3.1/src/pytest_fluent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/conftest.py` & `pytest_fluent-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/data/complex.json` & `pytest_fluent-0.3.1/tests/data/complex.json`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_additional_information.py` & `pytest_fluent-0.3.1/tests/test_additional_information.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_addoptions.py` & `pytest_fluent-0.3.1/tests/test_addoptions.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_content_patcher.py` & `pytest_fluent-0.3.1/tests/test_content_patcher.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_docstrings.py` & `pytest_fluent-0.3.1/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_fixtures.py` & `pytest_fluent-0.3.1/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_importlib_utils.py` & `pytest_fluent-0.3.1/tests/test_importlib_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_ini_configuration.py` & `pytest_fluent-0.3.1/tests/test_ini_configuration.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_logging_extension.py` & `pytest_fluent-0.3.1/tests/test_logging_extension.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_parser.py` & `pytest_fluent-0.3.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_reporting.py` & `pytest_fluent-0.3.1/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_reporting_patching.py` & `pytest_fluent-0.3.1/tests/test_reporting_patching.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tests/test_schema.py` & `pytest_fluent-0.3.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_fluent-0.3.0/tox.ini` & `pytest_fluent-0.3.1/tox.ini`

 * *Files identical despite different names*

