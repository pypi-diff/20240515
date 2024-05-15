# Comparing `tmp/audbcards-0.1.0.tar.gz` & `tmp/audbcards-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audbcards-0.1.0.tar", last modified: Wed Mar 27 14:16:49 2024, max compression
+gzip compressed data, was "audbcards-0.2.0.tar", last modified: Wed May 15 08:42:22 2024, max compression
```

## Comparing `audbcards-0.1.0.tar` & `audbcards-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.153947 audbcards-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.141947 audbcards-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.145947 audbcards-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-27 14:16:41.000000 audbcards-0.1.0/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-27 14:16:41.000000 audbcards-0.1.0/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-27 14:16:41.000000 audbcards-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-27 14:16:41.000000 audbcards-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-27 14:16:41.000000 audbcards-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-27 14:16:41.000000 audbcards-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-27 14:16:41.000000 audbcards-0.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-27 14:16:41.000000 audbcards-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-27 14:16:41.000000 audbcards-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-27 14:16:49.153947 audbcards-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-27 14:16:41.000000 audbcards-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.145947 audbcards-0.1.0/audbcards/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.145947 audbcards-0.1.0/audbcards/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11931 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/datacard.py
--rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.149947 audbcards-0.1.0/audbcards/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/templates/datacard.j2
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/templates/datacard_description.j2
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/templates/datacard_example.j2
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/templates/datacard_header.j2
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/templates/datacard_schemes.j2
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/templates/datacard_tables.j2
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/templates/datasets.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.149947 audbcards-0.1.0/audbcards/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-03-27 14:16:41.000000 audbcards-0.1.0/audbcards/sphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.153947 audbcards-0.1.0/audbcards.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-27 14:16:49.000000 audbcards-0.1.0/audbcards.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-27 14:16:49.000000 audbcards-0.1.0/audbcards.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:16:49.000000 audbcards-0.1.0/audbcards.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-27 14:16:49.000000 audbcards-0.1.0/audbcards.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-27 14:16:49.000000 audbcards-0.1.0/audbcards.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.149947 audbcards-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.149947 audbcards-0.1.0/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 14:16:41.000000 audbcards-0.1.0/docs/api-src/audbcards.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-27 14:16:41.000000 audbcards-0.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-27 14:16:41.000000 audbcards-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 14:16:41.000000 audbcards-0.1.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.149947 audbcards-0.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-27 14:16:41.000000 audbcards-0.1.0/docs/images/file-duration-distribution.png
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-27 14:16:41.000000 audbcards-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-27 14:16:41.000000 audbcards-0.1.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-27 14:16:41.000000 audbcards-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-03-27 14:16:41.000000 audbcards-0.1.0/docs/sphinx-extension.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-27 14:16:41.000000 audbcards-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-27 14:16:41.000000 audbcards-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 14:16:49.153947 audbcards-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.149947 audbcards-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-03-27 14:16:41.000000 audbcards-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 14:16:41.000000 audbcards-0.1.0/tests/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.145947 audbcards-0.1.0/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:16:49.153947 audbcards-0.1.0/tests/test_data/rendered_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-27 14:16:41.000000 audbcards-0.1.0/tests/test_data/rendered_templates/bare_db.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-27 14:16:41.000000 audbcards-0.1.0/tests/test_data/rendered_templates/medium_db.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-27 14:16:41.000000 audbcards-0.1.0/tests/test_data/rendered_templates/minimal_db.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-03-27 14:16:41.000000 audbcards-0.1.0/tests/test_datacard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9390 2024-03-27 14:16:41.000000 audbcards-0.1.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-27 14:16:41.000000 audbcards-0.1.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-27 14:16:41.000000 audbcards-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.836676 audbcards-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.824676 audbcards-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.828676 audbcards-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 08:42:16.000000 audbcards-0.2.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 08:42:16.000000 audbcards-0.2.0/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-15 08:42:16.000000 audbcards-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 08:42:16.000000 audbcards-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 08:42:16.000000 audbcards-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-15 08:42:16.000000 audbcards-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-15 08:42:16.000000 audbcards-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-15 08:42:16.000000 audbcards-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-15 08:42:16.000000 audbcards-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-15 08:42:22.836676 audbcards-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 08:42:16.000000 audbcards-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.828676 audbcards-0.2.0/audbcards/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.828676 audbcards-0.2.0/audbcards/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/datacard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22638 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.832676 audbcards-0.2.0/audbcards/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/templates/datacard.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/templates/datacard_description.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/templates/datacard_example.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/templates/datacard_header.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/templates/datacard_schemes.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/templates/datacard_tables.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/templates/datasets.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.832676 audbcards-0.2.0/audbcards/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-15 08:42:16.000000 audbcards-0.2.0/audbcards/sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.836676 audbcards-0.2.0/audbcards.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-15 08:42:22.000000 audbcards-0.2.0/audbcards.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-15 08:42:22.000000 audbcards-0.2.0/audbcards.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:42:22.000000 audbcards-0.2.0/audbcards.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 08:42:22.000000 audbcards-0.2.0/audbcards.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 08:42:22.000000 audbcards-0.2.0/audbcards.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.832676 audbcards-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.832676 audbcards-0.2.0/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-15 08:42:16.000000 audbcards-0.2.0/docs/api-src/audbcards.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 08:42:16.000000 audbcards-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-15 08:42:16.000000 audbcards-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 08:42:16.000000 audbcards-0.2.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.832676 audbcards-0.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 08:42:16.000000 audbcards-0.2.0/docs/images/file-duration-distribution.png
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-15 08:42:16.000000 audbcards-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-15 08:42:16.000000 audbcards-0.2.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-15 08:42:16.000000 audbcards-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-15 08:42:16.000000 audbcards-0.2.0/docs/sphinx-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-15 08:42:16.000000 audbcards-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 08:42:16.000000 audbcards-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:42:22.836676 audbcards-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.832676 audbcards-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-15 08:42:16.000000 audbcards-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 08:42:16.000000 audbcards-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.824676 audbcards-0.2.0/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:42:22.832676 audbcards-0.2.0/tests/test_data/rendered_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-15 08:42:16.000000 audbcards-0.2.0/tests/test_data/rendered_templates/bare_db.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-15 08:42:16.000000 audbcards-0.2.0/tests/test_data/rendered_templates/medium_db.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 08:42:16.000000 audbcards-0.2.0/tests/test_data/rendered_templates/minimal_db.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-15 08:42:16.000000 audbcards-0.2.0/tests/test_datacard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-05-15 08:42:16.000000 audbcards-0.2.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-15 08:42:16.000000 audbcards-0.2.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-15 08:42:16.000000 audbcards-0.2.0/tests/test_utils.py
```

### Comparing `audbcards-0.1.0/.github/workflows/doc.yml` & `audbcards-0.2.0/.github/workflows/doc.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,30 +12,30 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest ]
         python-version: [ '3.10' ]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Cache .cache/audbcards
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/.cache/audbcards
         key: audbcards-1
 
     - name: Cache audb
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb
         key: audb-1
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Ubuntu - install libsndfile
       run: |
         sudo apt-get update
         sudo apt-get install --no-install-recommends --yes libsndfile1
```

### Comparing `audbcards-0.1.0/.github/workflows/publish.yml` & `audbcards-0.2.0/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
     permissions:
       contents: write
       id-token: write
     concurrency:
       group: ${{ github.workflow }}-${{ github.ref }}
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 2
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build virtualenv
@@ -65,14 +65,14 @@
           echo 'body<<EOF'
           echo "$CHANGELOG"
           echo EOF
         } >> "$GITHUB_OUTPUT"
 
     - name: Create release on Github
       id: create_release
-      uses: softprops/action-gh-release@v1
+      uses: softprops/action-gh-release@v2
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ github.ref }}
         name: Release ${{ github.ref_name }}
         body: ${{ steps.changelog.outputs.body }}
```

### Comparing `audbcards-0.1.0/.github/workflows/test.yml` & `audbcards-0.2.0/.github/workflows/test.yml`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,23 @@
       matrix:
         os: [ ubuntu-latest, macOS-latest, windows-latest ]
         python-version: [ '3.10' ]
         include:
           - os: ubuntu-latest
             python-version: '3.9'
             tasks: tests
+          - os: ubuntu-latest
+            python-version: '3.11'
+            tasks: tests
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Ubuntu - install libsndfile
       run: |
         sudo apt-get update
         sudo apt-get install --no-install-recommends --yes libsndfile1
```

### Comparing `audbcards-0.1.0/.pre-commit-config.yaml` & `audbcards-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audbcards-0.1.0/CONTRIBUTING.rst` & `audbcards-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audbcards-0.1.0/LICENSE` & `audbcards-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audbcards-0.1.0/PKG-INFO` & `audbcards-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audbcards
-Version: 0.1.0
+Version: 0.2.0
 Summary: Create data cards for audb databases
 Author: BahaEddine Abrougui
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Christian Geng <cgeng@audeering.com>
 License: MIT License
         
         Copyright (c) 2023- audEERING GmbH and Contributors
         
@@ -38,20 +38,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: audb>=1.6.0
-Requires-Dist: audbackend>=1.0.1
+Requires-Dist: audb>=1.7.0
 Requires-Dist: audplot>=1.4.6
 Requires-Dist: jinja2
 Requires-Dist: pandas>=2.1.0
 Requires-Dist: toml
 
 =========
 audbcards
```

### Comparing `audbcards-0.1.0/audbcards/core/datacard.py` & `audbcards-0.2.0/audbcards/core/datacard.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import seaborn as sns
 
 import audb
 import audeer
 import audiofile
 import audplot
 
+from audbcards.core.config import config
 from audbcards.core.dataset import Dataset
 from audbcards.core.utils import set_plot_margins
 
 
 class Datacard(object):
     r"""Datacard of a dataset.
 
@@ -37,33 +38,39 @@
             and an interactive player
         sphinx_build_dir: build dir of sphinx.
             If not ``None``
             and ``example`` is ``True``,
             a call to :meth:`audbcards.Datacard.player`
             will store an example audio file
             under
-            ``<sphinx_build_dir>/<path>/<db-name>/<media-file-in-db>``
+            ``<sphinx_build_dir>/<path>/<dataset-name>/``
         sphinx_src_dir: source dir of sphinx.
             If not ``None``
             and ``example`` is ``True``,
             a call to :meth:`audbcards.Datacard.player`
-            will store a wavplot of the example audio file
+            will store a waveform plot of the example audio file
             under
-            ``<sphinx_src_dir>/<path>/<db-name>/<db-name>.png``
+            ``<sphinx_src_dir>/<path>/<dataset-name>/``
+        cache_root: cache folder.
+            If ``None``,
+            the environmental variable ``AUDBCARDS_CACHE_ROOT``,
+            or :attr:`audbcards.config.CACHE_ROOT`
+            is used
 
     """
 
     def __init__(
         self,
         dataset: Dataset,
         *,
         path: str = "datasets",
         example: bool = True,
         sphinx_build_dir: str = None,
         sphinx_src_dir: str = None,
+        cache_root: str = None,
     ):
         self.dataset = dataset
         """Dataset object."""
 
         self.path = path
         """Folder to store datacard."""
 
@@ -72,173 +79,246 @@
 
         self.sphinx_build_dir = sphinx_build_dir
         """Sphinx build dir."""
 
         self.sphinx_src_dir = sphinx_src_dir
         """Sphinx source dir."""
 
+        if cache_root is None:
+            cache_root = os.environ.get("AUDBCARDS_CACHE_ROOT") or config.CACHE_ROOT
+        self.cache_root = audeer.mkdir(cache_root)
+        r"""Cache root folder."""
+
         self.rst_preamble = ""
         """RST code added at top of data card."""
 
     @functools.cached_property
     def content(self):
         """Property Accessor for rendered jinja2 content."""
         return self._render_template()
 
     @property
-    def example_media(self) -> typing.Optional[str]:
-        r"""Select example media file.
-
-        This select a media file
-        based on the median duration
-        of all files
-        between 0.5 s and 300 s
-        and downloads it to the cache.
-
-        """
-        # Pick a meaningful duration for the example audio file
-        min_dur = 0.5
-        max_dur = 300  # 5 min
-        durations = self.dataset.file_durations
-        selected_durations = [d for d in durations if d >= min_dur and d <= max_dur]
-        if len(selected_durations) == 0:
-            return None
-        selected_duration = np.median(selected_durations)
-
-        # Get index for duration closest to selected duration
-        # see https://stackoverflow.com/a/9706105
-        # durations.index(selected_duration)
-        # is an alternative but fails due to rounding errors
-        index = min(
-            range(len(durations)),
-            key=lambda n: abs(durations[n] - selected_duration),
-        )
-        # Download of example data might fail
-        try:
-            media = self.dataset.deps.media[index]
-            audb.load_media(
-                self.dataset.name,
-                media,
-                version=self.dataset.version,
-                verbose=False,
-            )
-        except:  # noqa: E722
-            media = None
-        return media
-
-    @property
     def file_duration_distribution(self) -> str:
         r"""Minimum and maximum of files durations, and plotted distribution.
 
         This generates a single line
         containing the mininimum and maximum values
         of files durations.
 
-        If :attr:`audbcards.Datacard.self.sphinx_src_dir` is set
+        If :attr:`audbcards.Datacard.sphinx_src_dir` is not ``None``
         (e.g. when used in the sphinx extension),
-        an inline image is stored
-        in the sphinx source folder
-        under ``<dataset-name>/<dataset-name>-file-durations.png``
-        and displayed
+        an image is stored in the file
+        ``<dataset-name>-<dataset-version>-file-duration-distribution.png``,
+        which is cached in
+        ``<cache-root>/<dataset-name>/<dataset-version>/``
+        and copied to the sphinx source folder
+        into
+        ``<sphinx-src-dir>/<path><dataset-name>/``.
+        The image is displayed inline
         between the minimum and maximum values.
+        If all duration values are the same,
+        no distribution plot is created.
 
         """
+        file_name = (
+            f"{self.dataset.name}-{self.dataset.version}-file-duration-distribution.png"
+        )
+        # Cache is organized as `<cache_root>/<name>/<version>/`
+        cache_file = audeer.path(
+            self.cache_root,
+            self.dataset.name,
+            self.dataset.version,
+            file_name,
+        )
+
         min_ = 0
         max_ = 0
         unit = "s"
         durations = self.dataset.file_durations
         if len(durations) > 0:
             min_ = np.min(durations)
             max_ = np.max(durations)
+
+        # Skip creating a distribution plot,
+        # if all durations are the same
+        if min_ == max_:
+            return f"each file is {max_:.1f} {unit}"
+
         distribution_str = f"{min_:.1f} {unit} .. {max_:.1f} {unit}"
 
         # Save distribution plot
         if self.sphinx_src_dir is not None:
-            self._plot_distribution(durations)
-            name = "file-durations"
+            # Plot distribution to cache,
+            # if not found there already.
+            if not os.path.exists(cache_file):
+                audeer.mkdir(os.path.dirname(cache_file))
+                self._plot_distribution(durations)
+                plt.savefig(cache_file, transparent=True)
+                plt.close()
+
             image_file = audeer.path(
                 self.sphinx_src_dir,
                 self.path,
                 self.dataset.name,
-                f"{self.dataset.name}-{name}.png",
+                file_name,
             )
             audeer.mkdir(os.path.dirname(image_file))
-            plt.savefig(image_file, transparent=True)
-            plt.close()
+            shutil.copyfile(cache_file, image_file)
             distribution_str = self._inline_image(
                 f"{min_:.1f} {unit}",
-                f"./{self.dataset.name}/{self.dataset.name}-{name}.png",
+                f"./{self.dataset.name}/{file_name}",
                 f"{max_:.1f} {unit}",
             )
 
         return distribution_str
 
-    def player(
-        self,
-        file: str = None,
-    ) -> str:
+    def player(self) -> str:
         r"""Create an audio player showing the waveform.
 
-        Args:
-            file: input audio file to be used in the player.
-                If ``None``,
-                :attr:`audbcards.Datacard.example_media`
-                is used
+        If :attr:`audbcards.Datacard.sphinx_build_dir`
+        or :attr:`audbcards.Datacard.sphinx_src_dir`
+        is not ``None``,
+        an example media file is cached in the folder
+        ``<dataset-name>-<dataset-version>-player-media/``
+        inside
+        ``<cache-root>/<dataset-name>/<dataset-version>/``,
+        using the same sub-folder structure
+        as the media file has inside its dataset.
+        If :attr:`audbcards.Datacard.sphinx_build_dir`
+        is not ``None``,
+        the media sub-folder structure
+        is also copied
+        to the sphinx build dir into
+        ``<sphinx-build-dir>/<path>/<dataset-name>/``,
+        and an audio element referencing this file
+        is added to the returned RST string.
+
+        If :attr:`audbcards.Datacard.sphinx_src_dir` is not ``None``,
+        a plot of the waveform of the media file
+        is cached under
+        ``<dataset-name>-<dataset-version>-player-waveform.png``
+        inside
+        ``<cache-root>/<dataset-name>/<dataset-version>/``.
+        It is also copied to the sphinx source folder into
+        ``<sphinx-src-dir>/<path>/<dataset-name>/``,
+        and referenced at the beginning of the returned RST string.
+
+        If :attr:`audbcards.Datacard.sphinx_build_dir`
+        and :attr:`audbcards.Datacard.sphinx_src_dir`
+        are ``None``,
+        an empty string is returned.
 
-        """
-        if file is None:
-            file = self.example_media
+        Returns:
+            String containing RST code to include the player
 
-        # use audb cache instead of dataset.cache_root
-        media_src_dir = (
-            f"{audb.default_cache_root()}/"
-            f"{audb.flavor_path(self.dataset.name, self.dataset.version)}"
+        """
+        # Cache is organized as `<cache_root>/<name>/<version>/`
+        cache_folder = audeer.path(
+            self.cache_root,
+            self.dataset.name,
+            self.dataset.version,
         )
 
-        # Move file to build folder
+        def load_media_to_cache() -> str:
+            r"""Load media file with audb and copy to audbcards cache.
+
+            Load example media file to cache,
+            if not existent.
+
+            Returns:
+                full path to media file in cache
+
+            """
+            cache_example_media = audeer.path(
+                cache_folder,
+                f"{self.dataset.name}-{self.dataset.version}-player-media",
+                self.dataset.example_media,
+            )
+            if not os.path.exists(cache_example_media):
+                media = audb.load_media(
+                    self.dataset.name,
+                    self.dataset.example_media,
+                    version=self.dataset.version,
+                    verbose=False,
+                )[0]
+                audeer.mkdir(os.path.dirname(cache_example_media))
+                shutil.copy(media, cache_example_media)
+            return cache_example_media
+
+        def plot_waveform_to_cache(cache_example_media: str) -> str:
+            r"""Plot waveform of example media to cache.
+
+            Args:
+                cache_example_media: full path to media file in cache
+
+            Returns:
+                full path to waveform file in cache
+
+            """
+            cache_waveform_file = audeer.path(
+                cache_folder,
+                f"{self.dataset.name}-{self.dataset.version}-player-waveform.png",
+            )
+            if not os.path.exists(cache_waveform_file):
+                signal, sampling_rate = audiofile.read(
+                    cache_example_media,
+                    always_2d=True,
+                )
+                audeer.mkdir(os.path.dirname(cache_waveform_file))
+                plt.figure(figsize=[3, 0.5])
+                ax = plt.subplot(111)
+                audplot.waveform(signal[0, :], ax=ax)
+                set_plot_margins()
+                plt.savefig(cache_waveform_file)
+                plt.close()
+            return cache_waveform_file
+
+        # String holding the RST code to include the player
+        player_str = ""
+
+        # Add plot of waveform to Sphinx source folder (e.g. docs/)
+        if self.sphinx_src_dir is not None:
+            cache_example_media = load_media_to_cache()
+            cache_waveform_file = plot_waveform_to_cache(cache_example_media)
+            plot_dst_dir = audeer.path(
+                self.sphinx_src_dir,
+                self.path,
+                self.dataset.name,
+            )
+            audeer.mkdir(plot_dst_dir)
+            shutil.copy(
+                cache_waveform_file,
+                os.path.join(plot_dst_dir, os.path.basename(cache_waveform_file)),
+            )
+            waveform_src = (
+                f"./{self.dataset.name}/{os.path.basename(cache_waveform_file)}"
+            )
+            player_str += f".. image:: {waveform_src}\n\n"
+
+        # Copy media file to Sphinx build folder (e.g. build/)
         if self.sphinx_build_dir is not None:
+            cache_example_media = load_media_to_cache()
             media_dst_dir = audeer.path(
                 self.sphinx_build_dir,
                 self.path,
                 self.dataset.name,
             )
-            audeer.mkdir(os.path.join(media_dst_dir, os.path.dirname(file)))
+            audeer.mkdir(media_dst_dir, os.path.dirname(self.dataset.example_media))
             shutil.copy(
-                os.path.join(media_src_dir, file),
-                os.path.join(media_dst_dir, file),
+                cache_example_media,
+                os.path.join(media_dst_dir, self.dataset.example_media),
             )
 
-        # Add plot of waveform
-        if self.sphinx_src_dir is not None:
-            signal, sampling_rate = audiofile.read(
-                os.path.join(media_src_dir, file),
-                always_2d=True,
+            player_src = f"./{self.dataset.name}/{self.dataset.example_media}"
+            player_str += (
+                ".. raw:: html\n"
+                "\n"
+                f'    <p><audio controls src="{player_src}"></audio></p>'
             )
-            image_file = audeer.path(
-                self.sphinx_src_dir,
-                self.path,
-                self.dataset.name,
-                f"{self.dataset.name}.png",
-            )
-            audeer.mkdir(os.path.dirname(image_file))
-            plt.figure(figsize=[3, 0.5])
-            ax = plt.subplot(111)
-            audplot.waveform(signal[0, :], ax=ax)
-            set_plot_margins()
-            plt.savefig(image_file)
-            plt.close()
-
-        player_src = f"./{self.dataset.name}/{file}"
-        player_str = (
-            f".. image:: ./{self.dataset.name}/{self.dataset.name}.png\n"
-            "\n"
-            ".. raw:: html\n"
-            "\n"
-            f'    <p><audio controls src="{player_src}"></audio></p>'
-        )
+
         return player_str
 
     def save(self, file: str = None):
         """Save content of rendered template to rst.
 
         Args:
             file: name of output RST file.
@@ -353,22 +433,18 @@
 
         Returns:
             extended datasets dictionary
 
         """
         # Add path of datacard folder
         dataset["path"] = self.path
-        # Add audio player for example file
-        dataset["example"] = None
         if self.example:
-            example = self.example_media
-            if example is not None:
-                player = self.player(example)
+            if self.dataset.example_media is not None:
+                player = self.player()
                 dataset["player"] = player
-                dataset["example"] = example
         dataset["file_duration_distribution"] = self.file_duration_distribution
         return dataset
 
     def _render_template(self) -> str:
         r"""Render content of data card with Jinja2.
 
         It uses the dictionary representation
@@ -383,15 +459,15 @@
         environment = jinja2.Environment(
             loader=jinja2.FileSystemLoader(template_dir),
             trim_blocks=True,
         )
         template = environment.get_template("datacard.j2")
 
         # Convert dataset object to dictionary
-        dataset = self.dataset.properties()
+        dataset = self.dataset._cached_properties()
 
         # Add additional datacard only properties
         dataset = self._expand_dataset(dataset)
 
         content = template.render(dataset)
 
         # Add RST preamble
```

### Comparing `audbcards-0.1.0/audbcards/core/dataset.py` & `audbcards-0.2.0/audbcards/core/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,93 @@
 import functools
 import inspect
 import os
 import pickle
 import typing
 
-import dohq_artifactory
 import jinja2
+import numpy as np
 import pandas as pd
 
 import audb
 import audbackend
 import audeer
 import audformat
 
+from audbcards.core.config import config
 from audbcards.core.utils import format_schemes
 from audbcards.core.utils import limit_presented_samples
 
 
-def _getstate(self):
-    return self.name
-
-
-def _setstate(self, state):
-    self.name = state
-
-
-# Ensure we can pickle the repository
-dohq_artifactory.GenericRepository.__getstate__ = _getstate
-dohq_artifactory.GenericRepository.__setstate__ = _setstate
-
-
 class _Dataset:
     @classmethod
     def create(
         cls,
         name: str,
         version: str,
         *,
-        cache_root: str = "~/.cache/audbcards",
+        cache_root: str = None,
     ):
         r"""Instantiate Dataset Object."""
+        if cache_root is None:
+            cache_root = os.environ.get("AUDBCARDS_CACHE_ROOT") or config.CACHE_ROOT
         dataset_cache_filename = cls._dataset_cache_path(name, version, cache_root)
 
         if os.path.exists(dataset_cache_filename):
             obj = cls._load_pickled(dataset_cache_filename)
 
             return obj
 
         obj = cls(name, version, cache_root)
-        _ = obj.properties()
+        _ = obj._cached_properties()
 
         cls._save_pickled(obj, dataset_cache_filename)
         return obj
 
     def __init__(
         self,
         name: str,
         version: str,
-        cache_root: str = "~./cache/audbcards",
+        cache_root: str = None,
     ):
-        self.cache_root = audeer.mkdir(audeer.path(cache_root))
-        self.header = audb.info.header(
-            name,
-            version=version,
-            load_tables=True,  # ensure misc tables are loaded
-        )
-        self.deps = audb.dependencies(
-            name,
-            version=version,
-            verbose=False,
-        )
+        self.cache_root = audeer.mkdir(cache_root)
+        r"""Cache root folder."""
 
+        # Store name and version in private attributes here,
+        # ``self.name`` and ``self.version``
+        # are implemented as cached properties below
+        self._name = name
         self._version = version
-        self._repository = audb.repository(name, version)
-        self._backend = audbackend.access(
-            name=self._repository.backend,
-            host=self._repository.host,
-            repository=self._repository.name,
-        )
-        if isinstance(self._backend, audbackend.Artifactory):
-            self._backend._use_legacy_file_structure()  # pragma: nocover
+
+        # Private attributes,
+        # used inside corresponding properties.
+        self._header = self._load_header()
+        self._deps = self._load_dependencies()
+        self._repository_object = self._load_repository_object()  # load before backend
+        self._backend = self._load_backend()
 
         # Clean up cache
         # by removing all other versions of the same dataset
         # to reduce its storage size in CI runners
         versions = audeer.list_dir_names(
-            audeer.path(self.cache_root, name),
+            audeer.path(cache_root, name),
             basenames=True,
         )
         other_versions = [v for v in versions if v != version]
         for other_version in other_versions:
-            audeer.rmdir(audeer.path(self.cache_root, name, other_version))
+            audeer.rmdir(cache_root, name, other_version)
+
+    def __getstate__(self):
+        r"""Returns attributes to be pickled."""
+        return self._cached_properties()
 
     @staticmethod
     def _dataset_cache_path(name: str, version: str, cache_root: str) -> str:
         r"""Generate the name of the cache file."""
-        cache_dir = audeer.mkdir(audeer.path(cache_root, name, version))
+        cache_dir = audeer.mkdir(cache_root, name, version)
 
         cache_filename = audeer.path(
             cache_dir,
             f"{name}-{version}.pkl",
         )
         return cache_filename
 
@@ -116,14 +104,42 @@
     def _save_pickled(obj, path: str):
         """Save object instance to path as pickle."""
         audeer.mkdir(os.path.dirname(path))
 
         with open(path, "wb") as f:
             pickle.dump(obj, f, protocol=4)
 
+    @property
+    def backend(self) -> typing.Type[audbackend.interface.Base]:
+        r"""Dataset backend object."""
+        if not hasattr(self, "_backend"):  # when loaded from cache
+            self._backend = self._load_backend()
+        return self._backend
+
+    @property
+    def deps(self) -> audb.Dependencies:
+        r"""Dataset dependency table."""
+        if not hasattr(self, "_deps"):  # when loaded from cache
+            self._deps = self._load_dependencies()
+        return self._deps
+
+    @property
+    def header(self) -> audformat.Database:
+        r"""Dataset header."""
+        if not hasattr(self, "_header"):  # when loaded from cache
+            self._header = self._load_header()
+        return self._header
+
+    @property
+    def repository_object(self) -> audb.Repository:
+        r"""Repository object containing dataset."""
+        if not hasattr(self, "_repository_object"):  # when loaded from cache
+            self._repository_object = self._load_repository_object()
+        return self._repository_object
+
     @functools.cached_property
     def archives(self) -> int:
         r"""Number of archives of media files in dataset."""
         return len(set([self.deps.archive(file) for file in self.deps.media]))
 
     @functools.cached_property
     def author(self) -> typing.List[str]:
@@ -171,14 +187,47 @@
         durations = [self.deps.duration(file) for file in self.deps.media]
         return pd.to_timedelta(
             sum([d for d in durations if d is not None]),
             unit="s",
         )
 
     @functools.cached_property
+    def example_media(self) -> typing.Optional[str]:
+        r"""Example media file.
+
+        The media file is selected
+        by its median duration
+        from all files in the dataset
+        with a duration
+        between 0.5 s and 300 s.
+        If no media file meets this criterium,
+        ``None`` is returned instead.
+
+        """
+        # Pick a meaningful duration for the example audio file
+        min_dur = 0.5
+        max_dur = 300  # 5 min
+        durations = self.file_durations
+        selected_durations = [d for d in durations if d >= min_dur and d <= max_dur]
+
+        if len(selected_durations) == 0:
+            return None
+
+        selected_duration = np.median(selected_durations)
+        # Get index for duration closest to selected duration
+        # see https://stackoverflow.com/a/9706105
+        # durations.index(selected_duration)
+        # is an alternative but fails due to rounding errors
+        index = min(
+            range(len(durations)),
+            key=lambda n: abs(durations[n] - selected_duration),
+        )
+        return self.deps.media[index]
+
+    @functools.cached_property
     def files(self) -> int:
         r"""Number of media files in dataset."""
         return len(self.deps.media)
 
     @functools.cached_property
     def file_durations(self) -> typing.List:
         r"""File durations in dataset in seconds."""
@@ -221,52 +270,44 @@
             return None
         else:
             return self.header.license_url
 
     @functools.cached_property
     def name(self) -> str:
         r"""Name of dataset."""
-        return self.header.name
+        return self._name
 
     @functools.cached_property
     def publication_date(self) -> str:
         r"""Date dataset was uploaded to repository."""
-        path = self._backend.join("/", self.name, "db.yaml")
-        return self._backend.date(path, self._version)
+        with self.backend.backend:
+            path = self.backend.join("/", self.name, "db.yaml")
+            return self.backend.date(path, self.version)
 
     @functools.cached_property
     def publication_owner(self) -> str:
         r"""User who uploaded dataset to repository."""
-        path = self._backend.join("/", self.name, "db.yaml")
-        return self._backend.owner(path, self._version)
-
-    def properties(self):
-        """Get list of properties of the object."""
-        class_items = self.__class__.__dict__.items()
-        props = dict(
-            (k, getattr(self, k))
-            for k, v in class_items
-            if isinstance(v, functools.cached_property)
-        )
-        return props
+        with self.backend.backend:
+            path = self.backend.join("/", self.name, "db.yaml")
+            return self.backend.owner(path, self.version)
 
     @functools.cached_property
     def repository(self) -> str:
         r"""Repository containing the dataset."""
-        return f"{self._repository.name}"
+        return f"{self.repository_object.name}"
 
     @functools.cached_property
     def repository_link(self) -> str:
         r"""Link to repository in Artifactory web UI."""
         # NOTE: this needs to be changed
         # as we want to support different backends
         return (
-            f"{self._repository.host}/"
+            f"{self.repository_object.host}/"
             f"webapp/#/artifacts/browse/tree/General/"
-            f"{self._repository.name}/"
+            f"{self.repository}/"
             f"{self.name}"
         )
 
     @functools.cached_property
     def sampling_rates(self) -> typing.List[int]:
         r"""Sampling rates of media files in dataset."""
         return sorted(
@@ -283,14 +324,26 @@
 
     @functools.cached_property
     def schemes(self) -> typing.List[str]:
         r"""Schemes of dataset."""
         return list(self.header.schemes)
 
     @functools.cached_property
+    def schemes_summary(self) -> str:
+        r"""Summary of dataset schemes.
+
+        It lists all schemes in a string,
+        showing additional information
+        on schemes named ``'emotion'`` and ``'speaker'``,
+        e.g. ``'speaker: [age, gender, language]'``.
+
+        """
+        return format_schemes(self.header.schemes)
+
+    @functools.cached_property
     def schemes_table(self) -> typing.List[typing.List[str]]:
         """Schemes table with name, type, min, max, labels, mappings.
 
         The table is represented as a dictionary
         with column names as keys.
 
         """
@@ -354,14 +407,42 @@
         return self.header.usage
 
     @functools.cached_property
     def version(self) -> str:
         r"""Version of dataset."""
         return self._version
 
+    def _cached_properties(self):
+        """Get list of cached properties of the object."""
+        class_items = self.__class__.__dict__.items()
+        props = dict(
+            (k, getattr(self, k))
+            for k, v in class_items
+            if isinstance(v, functools.cached_property)
+        )
+        return props
+
+    def _load_backend(self) -> typing.Type[audbackend.interface.Base]:
+        r"""Load backend object containing dataset."""
+        backend_interface = self.repository_object.create_backend_interface()
+        return backend_interface
+
+    def _load_dependencies(self) -> audb.Dependencies:
+        r"""Load dataset dependencies."""
+        return audb.dependencies(self.name, version=self.version, verbose=False)
+
+    def _load_header(self) -> audformat.Database:
+        r"""Load dataset header."""
+        # Ensure misc tables are loaded
+        return audb.info.header(self.name, version=self.version, load_tables=True)
+
+    def _load_repository_object(self) -> audb.Repository:
+        r"""Load repository object containing dataset."""
+        return audb.repository(self.name, self.version)
+
     @functools.cached_property
     def _scheme_table_columns(self) -> typing.List[str]:
         """Column names for the scheme table.
 
         Column names always include ``'ID'`` and ``'Dtype'``,
         and if defined in any scheme
         ``'Min'``,
@@ -495,37 +576,53 @@
 
     Dataset object that represents a dataset
     that can be loaded with :func:`audb.load()`.
 
     Args:
         name: name of dataset
         version: version of dataset
-        cache_root: cache folder
+        cache_root: cache folder.
+            If ``None``,
+            the environmental variable ``AUDBCARDS_CACHE_ROOT``,
+            or :attr:`audbcards.config.CACHE_ROOT`
+            is used
 
     """
 
     def __new__(
         cls,
         name: str,
         version: str,
         *,
-        cache_root: str = "~/.cache/audbcards",
+        cache_root: str = None,
     ):
         r"""Create Dataset Instance."""
         instance = _Dataset.create(name, version, cache_root=cache_root)
         return instance
 
+    # Add an __init__() function,
+    # to allow documenting instance variables
+    def __init__(
+        self,
+        name: str,
+        version: str,
+        *,
+        cache_root: str = None,
+    ):
+        self.cache_root = audeer.mkdir(cache_root)
+        r"""Cache root folder."""
+
     # Copy attributes and methods
     # to include in documentation
-    for prop in [
+    for _prop in [  # use private variable `_prop` to avoid inclusion in API doc
         name
         for name, value in inspect.getmembers(_Dataset)
-        if isinstance(value, functools.cached_property) and not name.startswith("_")
+        if not name.startswith("_") and name not in ["create"]
     ]:
-        vars()[prop] = getattr(_Dataset, prop)
+        vars()[_prop] = getattr(_Dataset, _prop)
 
     @staticmethod
     def _map_iso_languages(*args):
         return _Dataset._map_iso_languages(*args)
 
     @staticmethod
     def _dataset_cache_path(*args):
@@ -578,15 +675,15 @@
     """
     tuples = [
         (
             f"`{dataset.name} <{datacards_path}/{dataset.name}.html>`__",
             dataset.short_description,
             f"`{dataset.license} <{dataset.license_link}>`__",
             dataset.version,
-            format_schemes(dataset.header.schemes),
+            dataset.schemes_summary,
         )
         for dataset in datasets
     ]
     df = pd.DataFrame.from_records(
         tuples,
         columns=["name", "description", "license", "version", "schemes"],
         index="name",
```

### Comparing `audbcards-0.1.0/audbcards/core/templates/datacard_header.j2` & `audbcards-0.2.0/audbcards/core/templates/datacard_header.j2`

 * *Files identical despite different names*

### Comparing `audbcards-0.1.0/audbcards/core/templates/datasets.j2` & `audbcards-0.2.0/audbcards/core/templates/datasets.j2`

 * *Files identical despite different names*

### Comparing `audbcards-0.1.0/audbcards/core/utils.py` & `audbcards-0.2.0/audbcards/core/utils.py`

 * *Files identical despite different names*

### Comparing `audbcards-0.1.0/audbcards/sphinx/__init__.py` & `audbcards-0.2.0/audbcards/sphinx/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 
 import sphinx
+import sphinx.application
 
 import audb
 import audeer
 
 from audbcards.core.datacard import Datacard
 from audbcards.core.dataset import Dataset
 from audbcards.core.dataset import create_datasets_page
@@ -35,15 +36,15 @@
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
 
 
 # ===== SPHINX EXTENSION FUNCTIONS ========================================
 #
-# All fctions defined here
+# All functions defined here
 # are added to the extension
 # via app.connect()
 # in setup()
 #
 def builder_inited(app: sphinx.application.Sphinx):
     r"""Emitted when the builder object has been created.
 
@@ -65,14 +66,19 @@
         audb.config.REPOSITORIES = audeer.to_list(repositories)
 
         print("Get list of available datasets... ", end="", flush=True)
         df = audb.available(only_latest=True)
         df = df.sort_index()
         print("done")
 
+        # Store list of datasets in app
+        # to make them accessible in `docs/conf.py`
+        app.audbcards = {}
+        app.audbcards["df"] = df
+
         # Iterate datasets and create data card pages
         names = list(df.index)
         versions = list(df["version"])
         datasets = []
         for name, version in zip(names, versions):
             print(f"Parse {name}-{version}... ", end="", flush=True)
             dataset = Dataset(name, version)
```

### Comparing `audbcards-0.1.0/audbcards.egg-info/PKG-INFO` & `audbcards-0.2.0/audbcards.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audbcards
-Version: 0.1.0
+Version: 0.2.0
 Summary: Create data cards for audb databases
 Author: BahaEddine Abrougui
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Christian Geng <cgeng@audeering.com>
 License: MIT License
         
         Copyright (c) 2023- audEERING GmbH and Contributors
         
@@ -38,20 +38,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: audb>=1.6.0
-Requires-Dist: audbackend>=1.0.1
+Requires-Dist: audb>=1.7.0
 Requires-Dist: audplot>=1.4.6
 Requires-Dist: jinja2
 Requires-Dist: pandas>=2.1.0
 Requires-Dist: toml
 
 =========
 audbcards
```

### Comparing `audbcards-0.1.0/audbcards.egg-info/SOURCES.txt` & `audbcards-0.2.0/audbcards.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 audbcards/__init__.py
 audbcards.egg-info/PKG-INFO
 audbcards.egg-info/SOURCES.txt
 audbcards.egg-info/dependency_links.txt
 audbcards.egg-info/requires.txt
 audbcards.egg-info/top_level.txt
 audbcards/core/__init__.py
+audbcards/core/config.py
 audbcards/core/datacard.py
 audbcards/core/dataset.py
 audbcards/core/utils.py
 audbcards/core/templates/datacard.j2
 audbcards/core/templates/datacard_description.j2
 audbcards/core/templates/datacard_example.j2
 audbcards/core/templates/datacard_header.j2
```

### Comparing `audbcards-0.1.0/docs/conf.py` & `audbcards-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audbcards-0.1.0/docs/index.rst` & `audbcards-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audbcards-0.1.0/docs/install.rst` & `audbcards-0.2.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `audbcards-0.1.0/docs/sphinx-extension.rst` & `audbcards-0.2.0/docs/sphinx-extension.rst`

 * *Files 11% similar despite different names*

```diff
@@ -138,8 +138,24 @@
     :ref:`data-public-emodb` shows the data card for emodb.
 
 Which will render as:
 
     :ref:`data-public-emodb` shows the data card for emodb.
 
 
+List of available datasets
+--------------------------
+
+The sphinx extension calls :func:`audb.available`
+to get an overview of all available datasets.
+This information can be reused inside ``docs/conf.py``
+as it is stored in the ``app.audbcards`` dictionary
+under the ``"df"`` key, e.g.
+
+.. code-block:: python
+
+    def setup(app: sphinx.application.Sphinx):
+        df = app.audbcards["df"]
+        # ...
+        
+
 .. _sphinx extension: https://www.sphinx-doc.org/en/master/usage/extensions/index.html
```

### Comparing `audbcards-0.1.0/pyproject.toml` & `audbcards-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,20 +24,20 @@
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering',
 ]
 requires-python = '>=3.9'
 dependencies = [
-    'audb >=1.6.0',
-    'audbackend >=1.0.1',
+    'audb >=1.7.0',
     'audplot >=1.4.6',
     'jinja2',
     'pandas >=2.1.0',
     'toml',
 ]
 # Get version dynamically from git
 # (needs setuptools_scm tools config below)
```

### Comparing `audbcards-0.1.0/tests/conftest.py` & `audbcards-0.2.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 @pytest.fixture
 def audb_cache(tmpdir, scope="session", autouse=True):
     """Local audb cache folder."""
     cache = audeer.mkdir(audeer.path(tmpdir, "audb-cache"))
     audb.config.CACHE_ROOT = cache
-    audb.config.SHARED_CACHE = cache
+    audb.config.SHARED_CACHE_ROOT = cache
 
 
 @pytest.fixture
 def repository(tmpdir, scope="session"):
     """Local audb repository only visible inside the tests."""
     name = "data-local"
     host = audeer.mkdir(audeer.path(tmpdir, "repo"))
@@ -51,14 +51,15 @@
     return repository
 
 
 @pytest.fixture
 def bare_db(
     tmpdir,
     repository,
+    audb_cache,
     scope="session",
     autouse=True,
 ):
     r"""Publish and load a bare database.
 
     The name of the database will be ``bare_db``.
 
@@ -72,21 +73,25 @@
     db_path = audeer.mkdir(audeer.path(tmpdir, name))
 
     db = audformat.Database(name=name)
     db.save(db_path)
 
     # Publish and load database
     audb.publish(db_path, pytest.VERSION, repository)
-    return audb.load(name, version=pytest.VERSION, verbose=False)
+    db = audb.load(name, version=pytest.VERSION, verbose=False)
+    tmp_root = str(tmpdir.parts()[1])
+    assert db.root.startswith(tmp_root)
+    return db
 
 
 @pytest.fixture
 def minimal_db(
     tmpdir,
     repository,
+    audb_cache,
     scope="session",
     autouse=True,
 ):
     r"""Publish and load a minimal database.
 
     The name of the database will be ``minimal_db``.
 
@@ -121,21 +126,25 @@
     # Create audio files and store database
     durations = [0.1]  # s
     create_audio_files(db, db_path, durations)
     db.save(db_path)
 
     # Publish and load database
     audb.publish(db_path, pytest.VERSION, repository)
-    return audb.load(name, version=pytest.VERSION, verbose=False)
+    db = audb.load(name, version=pytest.VERSION, verbose=False)
+    tmp_root = str(tmpdir.parts()[1])
+    assert db.root.startswith(tmp_root)
+    return db
 
 
 @pytest.fixture
 def medium_db(
     tmpdir,
     repository,
+    audb_cache,
     scope="session",
     autouse=True,
 ):
     r"""Publish and load a medium test database.
 
     The name of the database will be ``medium_db``.
 
@@ -151,15 +160,15 @@
 
     db = audformat.Database(
         name=name,
         source="https://github.com/audeering/audbcards",
         usage="unrestricted",
         expires=None,
         languages=["eng", "de"],
-        description="Medium database.",
+        description="Medium database. | Some description |.",
         author="H Wierstorf, C Geng, B E Abrougui",
         organization="audEERING",
         license=audformat.define.License.CC0_1_0,
     )
 
     # Misc table 'speaker'
     db.schemes["age"] = audformat.Scheme(
@@ -212,15 +221,18 @@
     # Create audio files and store database
     durations = [1, 301]
     create_audio_files(db, db_path, durations)
     db.save(db_path)
 
     # Publish and load database
     audb.publish(db_path, pytest.VERSION, repository)
-    return audb.load(name, version=pytest.VERSION, verbose=False)
+    db = audb.load(name, version=pytest.VERSION, verbose=False)
+    tmp_root = str(tmpdir.parts()[1])
+    assert db.root.startswith(tmp_root)
+    return db
 
 
 def create_audio_files(
     db: audformat.Database,
     db_path: str,
     durations: typing.Sequence[float],
     *,
```

### Comparing `audbcards-0.1.0/tests/test_data/rendered_templates/medium_db.rst` & `audbcards-0.2.0/tests/test_data/rendered_templates/medium_db.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. |medium_db-1.0.0-file-duration-distribution| image:: ./medium_db/medium_db-1.0.0-file-duration-distribution.png
+
 .. _datasets-medium_db:
 
 medium_db
 ---------
 
 Created by H Wierstorf, C Geng, B E Abrougui
 
@@ -12,30 +14,30 @@
 usage         unrestricted
 languages     eng, deu
 format        wav
 channel       1
 sampling rate 8000
 bit depth     16
 duration      0 days 00:05:02
-files         2, duration distribution: 1.0 s .. 301.0 s
+files         2, duration distribution: 1.0 s |medium_db-1.0.0-file-duration-distribution| 301.0 s
 repository    `data-local <.../data-local/medium_db>`__
 published     2023-04-05 by author
 ============= ======================
 
 Description
 ^^^^^^^^^^^
 
-Medium database.
+Medium database. \| Some description \|.
 
 Example
 ^^^^^^^
 
 :file:`data/f0.wav`
 
-.. image:: ./medium_db/medium_db.png
+.. image:: ./medium_db/medium_db-1.0.0-player-waveform.png
 
 .. raw:: html
 
     <p><audio controls src="./medium_db/data/f0.wav"></audio></p>
 
 Tables
 ^^^^^^
```

### Comparing `audbcards-0.1.0/tests/test_data/rendered_templates/minimal_db.rst` & `audbcards-0.2.0/tests/test_data/rendered_templates/minimal_db.rst`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 usage         unrestricted
 languages     
 format        wav
 channel       1
 sampling rate 8000
 bit depth     16
 duration      0 days 00:00:00.100000
-files         1, duration distribution: 0.1 s .. 0.1 s
+files         1, duration distribution: each file is 0.1 s
 repository    `data-local <.../data-local/minimal_db>`__
 published     2023-04-05 by author
 ============= ======================
 
 Description
 ^^^^^^^^^^^
```

### Comparing `audbcards-0.1.0/tests/test_datacard.py` & `audbcards-0.2.0/tests/test_datacard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
-import posixpath
 import re
 
 import matplotlib.pyplot as plt
-import numpy as np
 import pytest
 
 import audeer
 import audiofile
 import audplot
 
 import audbcards
@@ -19,19 +17,26 @@
     "db",
     [
         "bare_db",
         "minimal_db",
         "medium_db",
     ],
 )
-def test_datacard(db, cache, request):
+def test_datacard(tmpdir, db, cache, request):
     """Test datacard creation from jinja2 templates."""
     db = request.getfixturevalue(db)
     dataset = audbcards.Dataset(db.name, pytest.VERSION, cache_root=cache)
     datacard = audbcards.Datacard(dataset)
+
+    # Set sphinx src and build dir
+    build_dir = audeer.mkdir(tmpdir, "build", "html")
+    src_dir = audeer.mkdir(tmpdir, "docs")
+    datacard.sphinx_build_dir = build_dir
+    datacard.sphinx_src_dir = src_dir
+
     content = datacard._render_template()
     content = content.rstrip()
     expected_content = load_rendered_template(db.name)
 
     # Remove lines that depend on author/local machine
     for pattern in [
         re.compile("^published.*$", flags=(re.MULTILINE)),
@@ -41,46 +46,14 @@
         content = re.sub(pattern, "", content)
         expected_content = re.sub(pattern, "", expected_content)
 
     assert content == expected_content
 
 
 @pytest.mark.parametrize(
-    "db",
-    [
-        "medium_db",
-    ],
-)
-def test_datacard_example_media(db, cache, request):
-    r"""Test Datacard.example_media.
-
-    It checks that the desired audio file
-    is selected as example.
-
-    """
-    db = request.getfixturevalue(db)
-    dataset = audbcards.Dataset(db.name, pytest.VERSION, cache_root=cache)
-    datacard = audbcards.Datacard(dataset)
-
-    # Relative path to audio file from database
-    # as written in the dependencies table,
-    # for example data/file.wav
-    durations = [d.total_seconds() for d in db.files_duration(db.files)]
-    median_duration = np.median([d for d in durations if 0.5 < d < 300])
-    expected_example_index = min(
-        range(len(durations)), key=lambda n: abs(durations[n] - median_duration)
-    )
-    expected_example = audeer.path(db.files[expected_example_index]).replace(
-        os.sep, posixpath.sep
-    )
-    expected_example = "/".join(expected_example.split("/")[-2:])
-    assert datacard.example_media == expected_example
-
-
-@pytest.mark.parametrize(
     "db, expected_min, expected_max",
     [
         ("bare_db", 0, 0),
         ("medium_db", 1, 301),
     ],
 )
 def test_datacard_file_duration_distribution(
@@ -109,28 +82,34 @@
     distribution_str = datacard.file_duration_distribution
     build_dir = audeer.mkdir(tmpdir, "build", "html")
     src_dir = audeer.mkdir(tmpdir, "docs")
     image_file = audeer.path(
         build_dir,
         datacard.path,
         db.name,
-        f"{db.name}-file-durations.png",
+        f"{db.name}-{pytest.VERSION}-file-duration-distribution.png",
     )
     assert not os.path.exists(image_file)
-    expected_distribution_str = f"{expected_min:.1f} s .. {expected_max:.1f} s"
+    if expected_min == expected_max:
+        expected_distribution_str = f"each file is {expected_max:.1f} s"
+    else:
+        expected_distribution_str = f"{expected_min:.1f} s .. {expected_max:.1f} s"
     assert expected_distribution_str == distribution_str
 
     # Set sphinx src and build dir and execute again
     datacard.sphinx_build_dir = build_dir
     datacard.sphinx_src_dir = src_dir
     distribution_str = datacard.file_duration_distribution
-    assert os.path.exists(image_file)
-    expected_distribution_str = (
-        f"{expected_min:.1f} s |{db.name}-file-durations| {expected_max:.1f} s"
-    )
+    if expected_min != expected_max:
+        assert os.path.exists(image_file)
+        expected_distribution_str = (
+            f"{expected_min:.1f} s "
+            f"|{db.name}-{pytest.VERSION}-file-duration-distribution| "
+            f"{expected_max:.1f} s"
+        )
     assert expected_distribution_str == distribution_str
 
 
 @pytest.mark.parametrize(
     "db",
     [
         "medium_db",
@@ -149,38 +128,75 @@
     dataset = audbcards.Dataset(db.name, pytest.VERSION, cache_root=cache)
 
     datacard_path = audeer.mkdir(tmpdir, "datasets")
     datacard = audbcards.Datacard(dataset, path=datacard_path)
 
     # Execute player
     # without specifying sphinx src and build dirs
+    expected_player_str = ""
     player_str = datacard.player()
     build_dir = audeer.mkdir(tmpdir, "build", "html")
     src_dir = audeer.mkdir(tmpdir, "docs")
     media_file = audeer.path(
         build_dir,
         datacard.path,
         db.name,
-        datacard.example_media,
+        datacard.dataset.example_media,
     )
     image_file = audeer.path(
         src_dir,
         datacard.path,
         db.name,
-        f"{db.name}.png",
+        f"{db.name}-{pytest.VERSION}-player-waveform.png",
     )
     assert not os.path.exists(media_file)
     assert not os.path.exists(image_file)
+    assert player_str == expected_player_str
 
-    # Set sphinx src and build dir and execute again
+    # With sphinx source dir
+    expected_player_str = (
+        f".. image:: ./{db.name}/{db.name}-{pytest.VERSION}-player-waveform.png\n\n"
+    )
+    datacard.sphinx_src_dir = src_dir
+    player_str = datacard.player()
+    assert not os.path.exists(media_file)
+    assert os.path.exists(image_file)
+    assert player_str == expected_player_str
+    os.remove(image_file)
+
+    # With sphinx build dir
+    expected_player_str = (
+        ".. raw:: html\n"
+        "\n"
+        f'    <p><audio controls src="./{db.name}/{datacard.dataset.example_media}">'
+        f"</audio></p>"
+    )
+    datacard.sphinx_src_dir = None
+    datacard.sphinx_build_dir = build_dir
+    player_str = datacard.player()
+    assert os.path.exists(media_file)
+    assert not os.path.exists(image_file)
+    assert player_str == expected_player_str
+    os.remove(media_file)
+
+    # With sphinx source dir and build dir
+    expected_player_str = (
+        f".. image:: ./{db.name}/{db.name}-{pytest.VERSION}-player-waveform.png\n"
+        "\n"
+        ".. raw:: html\n"
+        "\n"
+        f'    <p><audio controls src="./{db.name}/{datacard.dataset.example_media}">'
+        f"</audio></p>"
+    )
     datacard.sphinx_build_dir = build_dir
     datacard.sphinx_src_dir = src_dir
-    player_str = datacard.player(datacard.example_media)
+    player_str = datacard.player()
     assert os.path.exists(media_file)
     assert os.path.exists(image_file)
+    assert expected_player_str == player_str
 
     # Expected waveform plot
     signal, sampling_rate = audiofile.read(
         media_file,
         always_2d=True,
     )
     plt.figure(figsize=[3, 0.5])
@@ -191,26 +207,14 @@
     plt.savefig(outfile)
     plt.close()
     expected_waveform = open(outfile, "rb").read()
     # Check if generated images are exactly the same (pixel-wise)
     waveform = open(image_file, "rb").read()
     assert waveform == expected_waveform
 
-    # Append audio to the expected player_str
-    expected_player_str = (
-        f".. image:: ./{db.name}/{db.name}.png\n"
-        "\n"
-        ".. raw:: html\n"
-        "\n"
-        f'    <p><audio controls src="./{db.name}/{datacard.example_media}">'
-        f"</audio></p>"
-    )
-    # Check if the generated player_str and the expected matches
-    assert expected_player_str == player_str
-
 
 @pytest.mark.parametrize(
     "dbs",
     [
         ["minimal_db", "medium_db"],
     ],
 )
```

### Comparing `audbcards-0.1.0/tests/test_dataset.py` & `audbcards-0.2.0/tests/test_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
+import posixpath
 
+import numpy as np
 import pandas as pd
 import pytest
 
 import audb
-import audbackend
 import audeer
 import audformat
 import audiofile
 
 import audbcards
 
 
@@ -25,15 +26,15 @@
     dataset_cache = audeer.mkdir(tmpdir, "cache")
     dataset = audbcards.Dataset(
         db.name,
         pytest.VERSION,
         cache_root=dataset_cache,
     )
 
-    props = [x for x in dataset.properties().keys()]
+    props = [x for x in dataset._cached_properties().keys()]
 
     # should not exist in local scope
     for prop in props:
         assert prop not in vars()
 
     # should not exist in global scope either
     for prop in props:
@@ -60,24 +61,24 @@
 
     dataset_cache = audeer.mkdir(tmpdir, "cache")
     dataset = audbcards.Dataset(
         db.name,
         pytest.VERSION,
         cache_root=dataset_cache,
     )
-    backend = audbackend.access(
-        name=repository.backend,
-        host=repository.host,
-        repository=repository.name,
-    )
+    backend_interface = repository.create_backend_interface()
 
     # __init__
     assert dataset.name == db.name
     assert dataset.version == pytest.VERSION
-    assert dataset._repository == repository
+    assert dataset.repository_object == repository
+    with backend_interface.backend:
+        # Compare only string,
+        # as backends are not identical
+        assert str(dataset.backend) == str(backend_interface)
     expected_header = audb.info.header(
         db.name,
         version=pytest.VERSION,
         cache_root=audb_cache,
     )
     assert str(dataset.header) == str(expected_header)
     expected_deps = audb.dependencies(
@@ -139,27 +140,28 @@
     # license link
     if db.license_url is None or len(db.license_url) == 0:
         expected_license_link = None
     else:
         expected_license_link = db.license_url
     assert dataset.license_link == expected_license_link
 
-    # publication_date:
-    expected_publication_date = backend.date(
-        backend.join("/", db.name, "db.yaml"),
-        pytest.VERSION,
-    )
-    assert dataset.publication_date == expected_publication_date
+    with backend_interface.backend:
+        # publication_date:
+        expected_publication_date = backend_interface.date(
+            backend_interface.join("/", db.name, "db.yaml"),
+            pytest.VERSION,
+        )
+        assert dataset.publication_date == expected_publication_date
 
-    # publication_owner
-    expected_publication_owner = backend.owner(
-        backend.join("/", db.name, "db.yaml"),
-        pytest.VERSION,
-    )
-    assert dataset.publication_owner == expected_publication_owner
+        # publication_owner
+        expected_publication_owner = backend_interface.owner(
+            backend_interface.join("/", db.name, "db.yaml"),
+            pytest.VERSION,
+        )
+        assert dataset.publication_owner == expected_publication_owner
 
     # repository
     assert dataset.repository == repository.name
 
     # repository_link : skipped for now
 
     # sampling_rates
@@ -253,14 +255,45 @@
 
     datasets = [
         audbcards.Dataset(db.name, pytest.VERSION, cache_root=cache) for db in dbs
     ]
     _ = [dataset.iso_languages for dataset in datasets]
 
 
+@pytest.mark.parametrize(
+    "db",
+    [
+        "medium_db",
+    ],
+)
+def test_dataset_example_media(db, cache, request):
+    r"""Test Dataset.example_media.
+
+    It checks that the desired audio file
+    is selected as example.
+
+    """
+    db = request.getfixturevalue(db)
+    dataset = audbcards.Dataset(db.name, pytest.VERSION, cache_root=cache)
+
+    # Relative path to audio file from database
+    # as written in the dependencies table,
+    # for example data/file.wav
+    durations = [d.total_seconds() for d in db.files_duration(db.files)]
+    median_duration = np.median([d for d in durations if 0.5 < d < 300])
+    expected_example_index = min(
+        range(len(durations)), key=lambda n: abs(durations[n] - median_duration)
+    )
+    expected_example = audeer.path(db.files[expected_example_index]).replace(
+        os.sep, posixpath.sep
+    )
+    expected_example = "/".join(expected_example.split("/")[-2:])
+    assert dataset.example_media == expected_example
+
+
 @pytest.fixture
 def constructor(tmpdir, medium_db, request):
     """Fixture to test Dataset constructor."""
     db = medium_db
     dataset_cache = audeer.mkdir(tmpdir, "cache")
     dataset_cache_filename = audbcards.Dataset._dataset_cache_path(
         db.name, pytest.VERSION, dataset_cache
@@ -300,21 +333,57 @@
         _, _, cache_file_existence = constructor
         expected_cache_file_existence = [False, True, True]
         assert cache_file_existence == expected_cache_file_existence
 
     def test_props_equal(self, constructor):
         """Cached and uncached datasets have equal props."""
         ds_uncached, ds_cached, _ = constructor
-        props_uncached = ds_uncached.properties()
-        props_cached = ds_cached.properties()
+        props_uncached = ds_uncached._cached_properties()
+        props_cached = ds_cached._cached_properties()
         list_props_uncached = list(props_uncached.keys())
         list_props_cached = list(props_cached.keys())
         assert list_props_uncached == list_props_cached
 
 
+@pytest.mark.parametrize(
+    "db",
+    [
+        "medium_db",
+    ],
+)
+def test_dataset_cache_root(tmpdir, request, db):
+    """Test configuration of cache root.
+
+    ``cache_root`` can be provided by different options,
+    in the following precedence:
+
+    * as argument to ``audbcards.Dataset()``
+    * as environment variable ``AUDBCARDS_CACHE_ROOT``
+    * as ``audbcards.config.CACHE_ROOT`` entry
+
+    """
+    db = request.getfixturevalue(db)
+    cache_root1 = audeer.mkdir(tmpdir, "cache1")
+    cache_root2 = audeer.mkdir(tmpdir, "cache2")
+    cache_root3 = audeer.mkdir(tmpdir, "cache3")
+    assert audbcards.config.CACHE_ROOT == "~/.cache/audbcards"
+    audbcards.config.CACHE_ROOT = cache_root1
+    dataset = audbcards.Dataset(db.name, pytest.VERSION)
+    assert dataset.cache_root == cache_root1
+    os.environ["AUDBCARDS_CACHE_ROOT"] = cache_root2
+    dataset = audbcards.Dataset(db.name, pytest.VERSION)
+    assert dataset.cache_root == cache_root2
+    dataset = audbcards.Dataset(
+        db.name,
+        pytest.VERSION,
+        cache_root=cache_root3,
+    )
+    assert dataset.cache_root == cache_root3
+
+
 def test_dataset_cache_path():
     """Test Value of default cache path."""
     cache_path_calculated = audbcards.core.dataset._Dataset._dataset_cache_path(
         "emodb",
         "1.2.1",
         "~/.cache/audbcards",
     )
@@ -324,7 +393,52 @@
         ".cache",
         "audbcards",
         "emodb",
         "1.2.1",
         "emodb-1.2.1.pkl",
     )
     assert cache_path_calculated == cache_path_expected
+
+
+@pytest.mark.parametrize(
+    "db",
+    [
+        "medium_db",
+    ],
+)
+def test_dataset_cache_loading(audb_cache, tmpdir, repository, db, request):
+    """Test cached properties after loading from cache.
+
+    We no longer store all attributes/properties
+    in cache as pickle files,
+    but limit ourselves to the cached properties.
+    This test ensures,
+    that other attributes will be re-calculated.
+
+    """
+    db = request.getfixturevalue(db)
+    cache_root = audeer.mkdir(tmpdir, "cache")
+    dataset = audbcards.Dataset(db.name, pytest.VERSION, cache_root=cache_root)
+    del dataset
+    dataset = audbcards.Dataset(db.name, pytest.VERSION, cache_root=cache_root)
+    deps = audb.dependencies(
+        db.name,
+        version=pytest.VERSION,
+        cache_root=audb_cache,
+    )
+    backend_interface = repository.create_backend_interface()
+    with backend_interface.backend:
+        header = audb.info.header(
+            db.name,
+            version=pytest.VERSION,
+            load_tables=True,
+            cache_root=audb_cache,
+        )
+        # Compare only string representation,
+        # as objects are not identical
+        assert str(dataset.backend) == str(backend_interface)
+        assert dataset.deps == deps
+        # The dataset header is a not fully loaded `audformat.Database` object,
+        # so we cannot directly use `audformat.Database.__eq__()`
+        # to compare it.
+        assert str(dataset.header) == str(header)
+        assert dataset.repository_object == repository
```

### Comparing `audbcards-0.1.0/tests/test_utils.py` & `audbcards-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

