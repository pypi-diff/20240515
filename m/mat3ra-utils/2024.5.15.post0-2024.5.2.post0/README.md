# Comparing `tmp/mat3ra_utils-2024.5.15.post0.tar.gz` & `tmp/mat3ra_utils-2024.5.2.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra_utils-2024.5.15.post0.tar", last modified: Wed May 15 03:52:41 2024, max compression
+gzip compressed data, was "mat3ra_utils-2024.5.2.post0.tar", last modified: Thu May  2 03:14:23 2024, max compression
```

## Comparing `mat3ra_utils-2024.5.15.post0.tar` & `mat3ra_utils-2024.5.2.post0.tar`

### file list

```diff
@@ -1,99 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.850131 mat3ra_utils-2024.5.15.post0/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.eslintrc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.834131 mat3ra_utils-2024.5.15.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.838131 mat3ra_utils-2024.5.15.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.838131 mat3ra_utils-2024.5.15.post0/.husky/
--rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.nycrc
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-15 03:52:41.850131 mat3ra_utils-2024.5.15.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   314260 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 03:52:41.850131 mat3ra_utils-2024.5.15.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.834131 mat3ra_utils-2024.5.15.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.838131 mat3ra_utils-2024.5.15.post0/src/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.834131 mat3ra_utils-2024.5.15.post0/src/js/browser/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.838131 mat3ra_utils-2024.5.15.post0/src/js/browser/specific/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/browser/specific/codemirror.ts
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/index_browser.ts
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/index_server.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.838131 mat3ra_utils-2024.5.15.post0/src/js/server/
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/server/file.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.842131 mat3ra_utils-2024.5.15.post0/src/js/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/array.js
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/class.js
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/clone.js
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/constants.js
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/hash.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/math.ts
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/object.ts
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.842131 mat3ra_utils-2024.5.15.post0/src/js/shared/specific/
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/specific/filter.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/specific/github.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/specific/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/specific/timestampable.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/str.js
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/tree.js
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/url.js
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/js/shared/uuid.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.842131 mat3ra_utils-2024.5.15.post0/src/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.842131 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.842131 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.846131 mat3ra_utils-2024.5.15.post0/src/py/mat3ra_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-15 03:52:41.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-15 03:52:41.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:52:41.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-15 03:52:41.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 03:52:41.000000 mat3ra_utils-2024.5.15.post0/src/py/mat3ra_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.834131 mat3ra_utils-2024.5.15.post0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.846131 mat3ra_utils-2024.5.15.post0/tests/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/js/class.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/js/clone.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/js/file.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/js/filter.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/js/object.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/js/str.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/js/tree.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/js/url.tests.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.834131 mat3ra_utils-2024.5.15.post0/tests/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.846131 mat3ra_utils-2024.5.15.post0/tests/py/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.846131 mat3ra_utils-2024.5.15.post0/tests/py/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:41.846131 mat3ra_utils-2024.5.15.post0/tests/py/unit/fixtures/factory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/fixtures/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/fixtures/factory/factory_object_1.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/fixtures/factory/factory_object_2.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/fixtures/file_with_content.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/test_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tests/py/unit/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tsconfig-transpile.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 03:52:26.000000 mat3ra_utils-2024.5.15.post0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.eslintrc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/.husky/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.nycrc
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   314260 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/src/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/src/js/browser/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/src/js/browser/specific/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/browser/specific/codemirror.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/index_browser.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/index_server.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/src/js/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/server/file.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.173433 mat3ra_utils-2024.5.2.post0/src/js/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/array.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/class.js
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/clone.js
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/constants.js
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/hash.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/math.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/object.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.173433 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/filter.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/github.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/timestampable.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/str.js
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/tree.js
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/url.js
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/uuid.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.173433 mat3ra_utils-2024.5.2.post0/src/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.173433 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.177433 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.177433 mat3ra_utils-2024.5.2.post0/tests/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/class.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/clone.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/file.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/filter.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/object.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/str.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/tree.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/url.tests.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/tests/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/tests/py/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/factory/factory_object_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/factory/factory_object_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/file_with_content.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tsconfig-transpile.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tsconfig.json
```

### Comparing `mat3ra_utils-2024.5.15.post0/.github/workflows/cicd.yml` & `mat3ra_utils-2024.5.2.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/.gitignore` & `mat3ra_utils-2024.5.2.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/LICENSE.md` & `mat3ra_utils-2024.5.2.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/PKG-INFO` & `mat3ra_utils-2024.5.2.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-utils
-Version: 2024.5.15.post0
+Version: 2024.5.2.post0
 Summary: Utils.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2024 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra_utils-2024.5.15.post0/package-lock.json` & `mat3ra_utils-2024.5.2.post0/package-lock.json`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/package.json` & `mat3ra_utils-2024.5.2.post0/package.json`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/pyproject.toml` & `mat3ra_utils-2024.5.2.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/index.ts` & `mat3ra_utils-2024.5.2.post0/src/js/index.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/server/file.js` & `mat3ra_utils-2024.5.2.post0/src/js/server/file.js`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/array.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/array.js`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/class.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/class.js`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/constants.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/constants.js`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/hash.ts` & `mat3ra_utils-2024.5.2.post0/src/js/shared/hash.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/math.ts` & `mat3ra_utils-2024.5.2.post0/src/js/shared/math.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/object.ts` & `mat3ra_utils-2024.5.2.post0/src/js/shared/object.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/selector.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/selector.js`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/specific/filter.ts` & `mat3ra_utils-2024.5.2.post0/src/js/shared/specific/filter.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/specific/github.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/specific/github.js`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/str.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/str.js`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/js/shared/tree.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/tree.js`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/array.py` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/array.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import Any, List, Optional, Union
+from typing import List, Union
 
 
-def filter_by_slice_or_index_or_indices(
-    array: List, slice_or_index_or_indices: Optional[Union[slice, int, List[int]]] = None
-):
+def filter_by_slice_or_index_or_indices(array: List, slice_or_index_or_indices: Union[slice, int, List[int]] = None):
     if isinstance(slice_or_index_or_indices, list):
         return list(map(lambda x: array[x], slice_or_index_or_indices))
     if isinstance(slice_or_index_or_indices, slice):
         return array[slice_or_index_or_indices]
     if isinstance(slice_or_index_or_indices, int):
         return [array[slice_or_index_or_indices]]
     return array
 
 
-def convert_to_array_if_not(array_or_item: Union[List, Any]):
+def convert_to_array_if_not(array_or_item: Union[List, any]):
     return array_or_item if isinstance(array_or_item, list) else [array_or_item]
```

### Comparing `mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/factory.py` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/factory.py`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/regex.py` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/regex.py`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/py/mat3ra/utils/string.py` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/string.py`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/src/py/mat3ra_utils.egg-info/PKG-INFO` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-utils
-Version: 2024.5.15.post0
+Version: 2024.5.2.post0
 Summary: Utils.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2024 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra_utils-2024.5.15.post0/src/py/mat3ra_utils.egg-info/SOURCES.txt` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 src/js/shared/specific/github.js
 src/js/shared/specific/index.ts
 src/js/shared/specific/timestampable.ts
 src/py/__init__.py
 src/py/mat3ra/__init__.py
 src/py/mat3ra/utils/__init__.py
 src/py/mat3ra/utils/array.py
-src/py/mat3ra/utils/assertion.py
 src/py/mat3ra/utils/factory.py
 src/py/mat3ra/utils/file.py
 src/py/mat3ra/utils/mixins.py
 src/py/mat3ra/utils/object.py
 src/py/mat3ra/utils/regex.py
 src/py/mat3ra/utils/string.py
 src/py/mat3ra_utils.egg-info/PKG-INFO
@@ -59,15 +58,14 @@
 tests/js/filter.tests.ts
 tests/js/object.tests.ts
 tests/js/str.tests.ts
 tests/js/tree.tests.ts
 tests/js/url.tests.ts
 tests/py/unit/__init__.py
 tests/py/unit/test_array.py
-tests/py/unit/test_assertion.py
 tests/py/unit/test_factory.py
 tests/py/unit/test_file.py
 tests/py/unit/test_mixins.py
 tests/py/unit/test_object.py
 tests/py/unit/test_string.py
 tests/py/unit/fixtures/__init__.py
 tests/py/unit/fixtures/file_with_content.txt
```

### Comparing `mat3ra_utils-2024.5.15.post0/tests/js/class.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/class.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/tests/js/clone.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/clone.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/tests/js/filter.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/filter.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/tests/js/object.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/object.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/tests/js/str.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/str.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/tests/js/tree.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/tree.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/tests/py/unit/test_array.py` & `mat3ra_utils-2024.5.2.post0/tests/py/unit/test_array.py`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/tests/py/unit/test_mixins.py` & `mat3ra_utils-2024.5.2.post0/tests/py/unit/test_mixins.py`

 * *Files identical despite different names*

### Comparing `mat3ra_utils-2024.5.15.post0/tests/py/unit/test_object.py` & `mat3ra_utils-2024.5.2.post0/tests/py/unit/test_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 
 def test_omit():
     object_without_key1 = utils.omit(REFERENCE_OBJECT_1, ["key1"])
     assert object_without_key1 == REFERENCE_OBJECT_1_WITHOUT_KEY1
 
 
-def test_set_object_key():
+def test_set():
     object_with_key3 = utils.clone_deep(REFERENCE_OBJECT_1)
-    utils.set_object_key(object_with_key3, "key3", "value3")
+    utils.set(object_with_key3, "key3", "value3")
     assert object_with_key3 == REFERENCE_OBJECT_1_WITH_KEY3
 
 
 def test_clone_shallow():
     object_2_clone_shallow = utils.clone_shallow(REFERENCE_OBJECT_2_CLONE_SHALLOW)
     REFERENCE_OBJECT_2_CLONE_SHALLOW["key2"]["nested_key1"] = "nested_value2"
     assert object_2_clone_shallow["key2"]["nested_key1"] == "nested_value2"
```

### Comparing `mat3ra_utils-2024.5.15.post0/tests/py/unit/test_string.py` & `mat3ra_utils-2024.5.2.post0/tests/py/unit/test_string.py`

 * *Files identical despite different names*

