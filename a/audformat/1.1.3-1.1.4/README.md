# Comparing `tmp/audformat-1.1.3.tar.gz` & `tmp/audformat-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audformat-1.1.3.tar", last modified: Fri Apr 26 10:58:56 2024, max compression
+gzip compressed data, was "audformat-1.1.4.tar", last modified: Wed May 15 10:35:41 2024, max compression
```

## Comparing `audformat-1.1.3.tar` & `audformat-1.1.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.346547 audformat-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.326547 audformat-1.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.330547 audformat-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-26 10:58:48.000000 audformat-1.1.3/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-26 10:58:48.000000 audformat-1.1.3/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-26 10:58:48.000000 audformat-1.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-26 10:58:48.000000 audformat-1.1.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-26 10:58:48.000000 audformat-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-26 10:58:48.000000 audformat-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15990 2024-04-26 10:58:48.000000 audformat-1.1.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-26 10:58:48.000000 audformat-1.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-26 10:58:48.000000 audformat-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-26 10:58:56.346547 audformat-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-26 10:58:48.000000 audformat-1.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.330547 audformat-1.1.3/audformat/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    58342 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/define.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/media.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/rater.py
--rw-r--r--   0 runner    (1001) docker     (127)    17718 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/split.py
--rw-r--r--   0 runner    (1001) docker     (127)    49501 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    66906 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/define/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/define/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/audformat/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-26 10:58:48.000000 audformat-1.1.3/audformat/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.346547 audformat-1.1.3/audformat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 10:58:56.000000 audformat-1.1.3/audformat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.334547 audformat-1.1.3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-26 10:58:48.000000 audformat-1.1.3/benchmarks/benchmark_union.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.338547 audformat-1.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/accessing-data.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.338547 audformat-1.1.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.define.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.errors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.rst
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api/audformat.utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.342547 audformat-1.1.3/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.define.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.errors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.rst
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/api-src/audformat.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/combine-tables.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/create-database.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-example.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-format.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-header.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-misc-tables.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/data-tables.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/emodb-example.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/map-scheme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.342547 audformat-1.1.3/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/pics/audformat-database.dot
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/pics/audformat-misc-table.dot
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/pics/audformat-table.dot
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-26 10:58:48.000000 audformat-1.1.3/docs/update-database.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-26 10:58:48.000000 audformat-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 10:58:48.000000 audformat-1.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:58:56.346547 audformat-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:58:56.346547 audformat-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    27063 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    43614 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_database_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    46698 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_misc_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    22998 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    55994 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    71995 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54334 2024-04-26 10:58:48.000000 audformat-1.1.3/tests/test_utils_concat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.188822 audformat-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.168822 audformat-1.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.172822 audformat-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-15 10:35:32.000000 audformat-1.1.4/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 10:35:32.000000 audformat-1.1.4/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-15 10:35:32.000000 audformat-1.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-15 10:35:32.000000 audformat-1.1.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 10:35:32.000000 audformat-1.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-15 10:35:32.000000 audformat-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-05-15 10:35:32.000000 audformat-1.1.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-15 10:35:32.000000 audformat-1.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-15 10:35:32.000000 audformat-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-15 10:35:41.188822 audformat-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-15 10:35:32.000000 audformat-1.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.172822 audformat-1.1.4/audformat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.176822 audformat-1.1.4/audformat/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58489 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/rater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17718 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49501 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66906 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.176822 audformat-1.1.4/audformat/define/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/define/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.176822 audformat-1.1.4/audformat/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.176822 audformat-1.1.4/audformat/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.176822 audformat-1.1.4/audformat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-15 10:35:32.000000 audformat-1.1.4/audformat/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.184822 audformat-1.1.4/audformat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-15 10:35:41.000000 audformat-1.1.4/audformat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-15 10:35:41.000000 audformat-1.1.4/audformat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:35:41.000000 audformat-1.1.4/audformat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 10:35:41.000000 audformat-1.1.4/audformat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 10:35:41.000000 audformat-1.1.4/audformat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.176822 audformat-1.1.4/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-15 10:35:32.000000 audformat-1.1.4/benchmarks/benchmark_union.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.180822 audformat-1.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/accessing-data.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.180822 audformat-1.1.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api/audformat.define.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api/audformat.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api/audformat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api/audformat.testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api/audformat.utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.180822 audformat-1.1.4/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api-src/audformat.define.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api-src/audformat.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api-src/audformat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api-src/audformat.testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/api-src/audformat.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/combine-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/create-database.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/data-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/data-example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/data-format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/data-header.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/data-introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/data-misc-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/data-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/emodb-example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/map-scheme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.184822 audformat-1.1.4/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/pics/audformat-database.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/pics/audformat-misc-table.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/pics/audformat-table.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-15 10:35:32.000000 audformat-1.1.4/docs/update-database.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-15 10:35:32.000000 audformat-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 10:35:32.000000 audformat-1.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:35:41.188822 audformat-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:35:41.184822 audformat-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27063 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46217 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_database_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46698 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_misc_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22998 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55994 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71995 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54334 2024-05-15 10:35:32.000000 audformat-1.1.4/tests/test_utils_concat.py
```

### Comparing `audformat-1.1.3/.github/workflows/doc.yml` & `audformat-1.1.4/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/.github/workflows/publish.yml` & `audformat-1.1.4/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         pip install -r docs/requirements.txt
 
     - name: Build documentation
       run: |
         python -m sphinx docs/ docs/_build/ -b html
 
     - name: Deploy documentation to Github pages
-      uses: peaceiris/actions-gh-pages@v3
+      uses: peaceiris/actions-gh-pages@v4
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
         publish_dir: ./docs/_build
 
     # Github release
     - name: Read CHANGELOG
       id: changelog
```

### Comparing `audformat-1.1.3/.github/workflows/test.yml` & `audformat-1.1.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/.pre-commit-config.yaml` & `audformat-1.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/CHANGELOG.rst` & `audformat-1.1.4/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.1.4 (2024-05-15)
+--------------------------
+
+* Fixed: ``audformat.Database.get()``,
+  if its argument ``additional_schemes``
+  contains a non-existent scheme
+
+
 Version 1.1.3 (2024-04-26)
 --------------------------
 
 * Added: ``as_dataframe`` argument
   to ``audformat.utils.read_csv()``
 * Fixed: ``audformat.utils.read_csv()``
   now treats float/integer values
```

### Comparing `audformat-1.1.3/CONTRIBUTING.rst` & `audformat-1.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/LICENSE` & `audformat-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/PKG-INFO` & `audformat-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audformat
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python implementation of audformat
 Author: BahaEddine Abrougui
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>
 License: MIT License
         
         Copyright (c) 2018-present audEERING GmbH and Contributors
```

### Comparing `audformat-1.1.3/README.rst` & `audformat-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/__init__.py` & `audformat-1.1.4/audformat/__init__.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/attachment.py` & `audformat-1.1.4/audformat/core/attachment.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/column.py` & `audformat-1.1.4/audformat/core/column.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/common.py` & `audformat-1.1.4/audformat/core/common.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/conftest.py` & `audformat-1.1.4/audformat/core/conftest.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/database.py` & `audformat-1.1.4/audformat/core/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -852,24 +852,26 @@
         elif isinstance(obj, pd.Series):
             obj = obj.to_frame()
 
         # --- Append additional schemes
         objs = [obj]
         for scheme in additional_schemes:
             if len(obj) == 0:
-                obj = empty_frame(scheme)
+                # Skip searching for additional schemes,
+                # if main scheme does return empty frame
+                additional_obj = empty_frame(scheme)
             else:
-                obj = self.get(
+                additional_obj = self.get(
                     scheme,
                     strict=strict,
                     map=map,
                     original_column_names=original_column_names,
                     aggregate_function=aggregate_function,
                 )
-            objs.append(obj)
+            objs.append(additional_obj)
         if len(objs) > 1:
             obj = utils.concat(objs)
             obj = obj.loc[index]
             if len(obj) == 0:
                 obj.index = filewise_index()
 
         return obj
```

### Comparing `audformat-1.1.3/audformat/core/define.py` & `audformat-1.1.4/audformat/core/define.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/errors.py` & `audformat-1.1.4/audformat/core/errors.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/index.py` & `audformat-1.1.4/audformat/core/index.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/media.py` & `audformat-1.1.4/audformat/core/media.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/rater.py` & `audformat-1.1.4/audformat/core/rater.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/scheme.py` & `audformat-1.1.4/audformat/core/scheme.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/split.py` & `audformat-1.1.4/audformat/core/split.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/table.py` & `audformat-1.1.4/audformat/core/table.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/testing.py` & `audformat-1.1.4/audformat/core/testing.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/core/utils.py` & `audformat-1.1.4/audformat/core/utils.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat/utils/__init__.py` & `audformat-1.1.4/audformat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/audformat.egg-info/PKG-INFO` & `audformat-1.1.4/audformat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audformat
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python implementation of audformat
 Author: BahaEddine Abrougui
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>
 License: MIT License
         
         Copyright (c) 2018-present audEERING GmbH and Contributors
```

### Comparing `audformat-1.1.3/audformat.egg-info/SOURCES.txt` & `audformat-1.1.4/audformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/benchmarks/benchmark_union.py` & `audformat-1.1.4/benchmarks/benchmark_union.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/accessing-data.rst` & `audformat-1.1.4/docs/accessing-data.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/api/audformat.define.rst` & `audformat-1.1.4/docs/api/audformat.define.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/api/audformat.testing.rst` & `audformat-1.1.4/docs/api/audformat.testing.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/api-src/audformat.define.rst` & `audformat-1.1.4/docs/api-src/audformat.define.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/api-src/audformat.testing.rst` & `audformat-1.1.4/docs/api-src/audformat.testing.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/combine-tables.rst` & `audformat-1.1.4/docs/combine-tables.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/conf.py` & `audformat-1.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/create-database.rst` & `audformat-1.1.4/docs/create-database.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/data-conventions.rst` & `audformat-1.1.4/docs/data-conventions.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/data-example.rst` & `audformat-1.1.4/docs/data-example.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/data-format.rst` & `audformat-1.1.4/docs/data-format.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/data-header.rst` & `audformat-1.1.4/docs/data-header.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/data-introduction.rst` & `audformat-1.1.4/docs/data-introduction.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/data-misc-tables.rst` & `audformat-1.1.4/docs/data-misc-tables.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/data-tables.rst` & `audformat-1.1.4/docs/data-tables.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/emodb-example.rst` & `audformat-1.1.4/docs/emodb-example.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/index.rst` & `audformat-1.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/map-scheme.rst` & `audformat-1.1.4/docs/map-scheme.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/pics/audformat-database.dot` & `audformat-1.1.4/docs/pics/audformat-database.dot`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/docs/update-database.rst` & `audformat-1.1.4/docs/update-database.rst`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/pyproject.toml` & `audformat-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/conftest.py` & `audformat-1.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_attachment.py` & `audformat-1.1.4/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_column.py` & `audformat-1.1.4/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_common.py` & `audformat-1.1.4/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_database.py` & `audformat-1.1.4/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_database_get.py` & `audformat-1.1.4/tests/test_database_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,14 +383,84 @@
                         dtype="object",
                         name="non-existing",
                     ),
                 ],
                 axis=1,
             ),
         ),
+        # Ensure that requesting a non-existing scheme
+        # before an existing scheme
+        # does return values for existing schemes.
+        # https://github.com/audeering/audformat/issues/426
+        (
+            "mono_db",
+            "gender",
+            ["non-existing", "sex"],
+            pd.concat(
+                [
+                    pd.Series(
+                        ["female", "", "male"],
+                        index=audformat.filewise_index(["f1.wav", "f2.wav", "f3.wav"]),
+                        dtype="string",
+                        name="gender",
+                    ),
+                    pd.Series(
+                        [],
+                        index=audformat.filewise_index(),
+                        dtype="object",
+                        name="non-existing",
+                    ),
+                    pd.Series(
+                        ["female", np.NaN, "male"],
+                        index=audformat.filewise_index(["f1.wav", "f2.wav", "f3.wav"]),
+                        dtype="object",
+                        name="sex",
+                    ),
+                ],
+                axis=1,
+            ),
+        ),
+        # Ensure that requesting a non-existing scheme
+        # before an existing scheme
+        # does return values for existing schemes.
+        # https://github.com/audeering/audformat/issues/426
+        (
+            "mono_db",
+            "gender",
+            ["numbers", "non-existing", "sex"],
+            pd.concat(
+                [
+                    pd.Series(
+                        ["female", "", "male"],
+                        index=audformat.filewise_index(["f1.wav", "f2.wav", "f3.wav"]),
+                        dtype="string",
+                        name="gender",
+                    ),
+                    pd.Series(
+                        [0, 1, 2],
+                        index=audformat.filewise_index(["f1.wav", "f2.wav", "f3.wav"]),
+                        dtype="Int64",
+                        name="numbers",
+                    ),
+                    pd.Series(
+                        [],
+                        index=audformat.filewise_index(),
+                        dtype="object",
+                        name="non-existing",
+                    ),
+                    pd.Series(
+                        ["female", np.NaN, "male"],
+                        index=audformat.filewise_index(["f1.wav", "f2.wav", "f3.wav"]),
+                        dtype="object",
+                        name="sex",
+                    ),
+                ],
+                axis=1,
+            ),
+        ),
         (
             "mono_db",
             "winner",
             [],
             pd.DataFrame(
                 {
                     "winner": ["w1", "w1", "w2", "w1", "w1", "w1", "w1"],
```

### Comparing `audformat-1.1.3/tests/test_eq.py` & `audformat-1.1.4/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_errors.py` & `audformat-1.1.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_index.py` & `audformat-1.1.4/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_misc_table.py` & `audformat-1.1.4/tests/test_misc_table.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_scheme.py` & `audformat-1.1.4/tests/test_scheme.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_table.py` & `audformat-1.1.4/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_utils.py` & `audformat-1.1.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `audformat-1.1.3/tests/test_utils_concat.py` & `audformat-1.1.4/tests/test_utils_concat.py`

 * *Files identical despite different names*

