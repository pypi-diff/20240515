# Comparing `tmp/ducktools_classbuilder-0.5.0.tar.gz` & `tmp/ducktools_classbuilder-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktools_classbuilder-0.5.0.tar", last modified: Fri Apr 26 14:13:31 2024, max compression
+gzip compressed data, was "ducktools_classbuilder-0.5.1.tar", last modified: Wed May 15 13:51:34 2024, max compression
```

## Comparing `ducktools_classbuilder-0.5.0.tar` & `ducktools_classbuilder-0.5.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.606230 ducktools_classbuilder-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-26 14:13:31.606230 ducktools_classbuilder-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.594230 ducktools_classbuilder-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/docs/approach_vs_tool.md
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    26324 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/docs/extension_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.594230 ducktools_classbuilder-0.5.0/docs/perf/
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/docs/perf/performance_tests.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.594230 ducktools_classbuilder-0.5.0/docs/prefab/
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/docs/prefab/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:13:31.606230 ducktools_classbuilder-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.594230 ducktools_classbuilder-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.594230 ducktools_classbuilder-0.5.0/src/ducktools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.598230 ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    20045 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28017 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/prefab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/prefab.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.606230 ducktools_classbuilder-0.5.0/src/ducktools_classbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-26 14:13:31.000000 ducktools_classbuilder-0.5.0/src/ducktools_classbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-26 14:13:31.000000 ducktools_classbuilder-0.5.0/src/ducktools_classbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:13:31.000000 ducktools_classbuilder-0.5.0/src/ducktools_classbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 14:13:31.000000 ducktools_classbuilder-0.5.0/src/ducktools_classbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 14:13:31.000000 ducktools_classbuilder-0.5.0/src/ducktools_classbuilder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.598230 ducktools_classbuilder-0.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.594230 ducktools_classbuilder-0.5.0/tests/prefab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.598230 ducktools_classbuilder-0.5.0/tests/prefab/dynamic/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_compare_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_construction.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_pre_post_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_slots_novalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_slotted_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.602230 ducktools_classbuilder-0.5.0/tests/prefab/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.602230 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/creation_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/dunders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:13:31.602230 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/fails/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/fails/creation_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/fails/creation_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/fails/creation_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/fails/creation_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/fails/inheritance_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/fails/inheritance_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/frozen_prefabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/funcs_prefabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/hint_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/init_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/kw_only.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/repr_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/test_dunders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/test_frozen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/test_hint_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/test_kw_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/prefab/shared/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/test_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-26 14:13:24.000000 ducktools_classbuilder-0.5.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.914924 ducktools_classbuilder-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-15 13:51:34.914924 ducktools_classbuilder-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.902924 ducktools_classbuilder-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/docs/approach_vs_tool.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26324 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/docs/extension_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.902924 ducktools_classbuilder-0.5.1/docs/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/docs/perf/performance_tests.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.902924 ducktools_classbuilder-0.5.1/docs/prefab/
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/docs/prefab/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:51:34.914924 ducktools_classbuilder-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.902924 ducktools_classbuilder-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.902924 ducktools_classbuilder-0.5.1/src/ducktools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.906925 ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/prefab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/prefab.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.914924 ducktools_classbuilder-0.5.1/src/ducktools_classbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-15 13:51:34.000000 ducktools_classbuilder-0.5.1/src/ducktools_classbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-15 13:51:34.000000 ducktools_classbuilder-0.5.1/src/ducktools_classbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:51:34.000000 ducktools_classbuilder-0.5.1/src/ducktools_classbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 13:51:34.000000 ducktools_classbuilder-0.5.1/src/ducktools_classbuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 13:51:34.000000 ducktools_classbuilder-0.5.1/src/ducktools_classbuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.906925 ducktools_classbuilder-0.5.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.902924 ducktools_classbuilder-0.5.1/tests/prefab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.906925 ducktools_classbuilder-0.5.1/tests/prefab/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_compare_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_pre_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_slots_novalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_slotted_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.910925 ducktools_classbuilder-0.5.1/tests/prefab/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.910925 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/creation_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/dunders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:51:34.914924 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/fails/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/fails/creation_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/fails/creation_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/fails/creation_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/fails/creation_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/fails/inheritance_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/fails/inheritance_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/frozen_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/funcs_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/init_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/repr_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/test_dunders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/test_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/test_hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/test_kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/prefab/shared/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/test_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-05-15 13:51:24.000000 ducktools_classbuilder-0.5.1/tests/test_core.py
```

### Comparing `ducktools_classbuilder-0.5.0/LICENSE.md` & `ducktools_classbuilder-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/PKG-INFO` & `ducktools_classbuilder-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.5.0
+Version: 0.5.1
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ducktools_classbuilder-0.5.0/README.md` & `ducktools_classbuilder-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/docs/Makefile` & `ducktools_classbuilder-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/docs/api.md` & `ducktools_classbuilder-0.5.1/docs/api.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/docs/approach_vs_tool.md` & `ducktools_classbuilder-0.5.1/docs/approach_vs_tool.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/docs/conf.py` & `ducktools_classbuilder-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/docs/extension_examples.md` & `ducktools_classbuilder-0.5.1/docs/extension_examples.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/docs/index.md` & `ducktools_classbuilder-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/docs/make.bat` & `ducktools_classbuilder-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/docs/perf/performance_tests.md` & `ducktools_classbuilder-0.5.1/docs/perf/performance_tests.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/docs/prefab/index.md` & `ducktools_classbuilder-0.5.1/docs/prefab/index.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/pyproject.toml` & `ducktools_classbuilder-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/__init__.py` & `ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import sys
 
-__version__ = "v0.5.0"
+__version__ = "v0.5.1"
 
 # Change this name if you make heavy modifications
 INTERNALS_DICT = "__classbuilder_internals__"
 
 
 # If testing, make Field classes frozen to make sure attributes are not
 # overwritten. When running this is a performance penalty so it is not required.
@@ -355,34 +355,57 @@
         :return: new field subclass instance
         """
         argument_dict = {**_get_inst_fields(fld), **kwargs}
 
         return cls(**argument_dict)
 
 
+class GatheredFields:
+    __slots__ = ("fields", "modifications")
+
+    def __init__(self, fields, modifications):
+        self.fields = fields
+        self.modifications = modifications
+
+    def __call__(self, cls):
+        return self.fields, self.modifications
+
+
 # Use the builder to generate __repr__ and __eq__ methods
-# and pretend `Field` was a built class all along.
+# for both Field and GatheredFields
 _field_internal = {
     "default": Field(default=NOTHING),
     "default_factory": Field(default=NOTHING),
     "type": Field(default=NOTHING),
     "doc": Field(default=None),
 }
 
+_gathered_field_internal = {
+    "fields": Field(default=NOTHING),
+    "modifications": Field(default=NOTHING),
+}
+
 _field_methods = {repr_maker, eq_maker}
 if _UNDER_TESTING:
     _field_methods.update({frozen_setattr_maker, frozen_delattr_maker})
 
 builder(
     Field,
-    gatherer=lambda cls_: (_field_internal, {}),
+    gatherer=GatheredFields(_field_internal, {}),
     methods=_field_methods,
     flags={"slotted": True, "kw_only": True},
 )
 
+builder(
+    GatheredFields,
+    gatherer=GatheredFields(_gathered_field_internal, {}),
+    methods={repr_maker, eq_maker},
+    flags={"slotted": True, "kw_only": False},
+)
+
 
 # Slot gathering tools
 # Subclass of dict to be identifiable by isinstance checks
 # For anything more complicated this could be made into a Mapping
 class SlotFields(dict):
     """
     A plain dict subclass.
@@ -426,14 +449,21 @@
             **cls.__dict__.get("__annotations__", {})
         }
 
         cls_fields = {}
         slot_replacement = {}
 
         for k, v in cls_slots.items():
+            # Special case __dict__ and __weakref__
+            # They should be included in the final `__slots__`
+            # But ignored as a value.
+            if k in {"__dict__", "__weakref__"}:
+                slot_replacement[k] = None
+                continue
+
             if isinstance(v, field_type):
                 attrib = v
                 if attrib.type is not NOTHING:
                     cls_annotations[k] = attrib.type
             else:
                 # Plain values treated as defaults
                 attrib = field_type(default=v)
```

### Comparing `ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/__init__.pyi` & `ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -88,14 +88,33 @@
     def __repr__(self) -> str: ...
     def __eq__(self, other: Field | object) -> bool: ...
     def validate_field(self) -> None: ...
     @classmethod
     def from_field(cls, fld: Field, /, **kwargs: typing.Any) -> Field: ...
 
 
+class GatheredFields:
+    __slots__ = ("fields", "modifications")
+
+    fields: dict[str, Field]
+    modifications: dict[str, typing.Any]
+
+    __classbuilder_internals__: dict
+
+    def __init__(
+        self,
+        fields: dict[str, Field],
+        modifications: dict[str, typing.Any]
+    ) -> None: ...
+
+    def __repr__(self) -> str: ...
+    def __eq__(self, other) -> bool: ...
+    def __call__(self, cls: type) -> tuple[dict[str, Field], dict[str, typing.Any]]: ...
+
+
 class SlotFields(dict):
     ...
 
 def make_slot_gatherer(
         field_type: type[Field] = Field
 ) -> Callable[[type], tuple[dict[str, Field], dict[str, typing.Any]]]: ...
```

### Comparing `ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/prefab.py` & `ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/prefab.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Includes pre and post init functions along with other methods.
 """
 
 import sys
 
 from . import (
     INTERNALS_DICT, NOTHING,
-    Field, MethodMaker, SlotFields,
+    Field, MethodMaker, SlotFields, GatheredFields,
     builder, fieldclass, get_flags, get_fields, make_slot_gatherer,
     frozen_setattr_maker, frozen_delattr_maker, is_classvar,
 )
 
 PREFAB_FIELDS = "PREFAB_FIELDS"
 PREFAB_INIT_FUNC = "__prefab_init__"
 PRE_INIT_FUNC = "__prefab_pre_init__"
@@ -515,14 +515,15 @@
     eq=True,
     iter=False,
     match_args=True,
     kw_only=False,
     frozen=False,
     dict_method=False,
     recursive_repr=False,
+    gathered_fields=None,
 ):
     """
     Generate boilerplate code for dunder methods in a class.
 
     :param cls: Class to convert to a prefab
     :param init: generate __init__
     :param repr: generate __repr__
@@ -531,31 +532,36 @@
     :param match_args: generate __match_args__
     :param kw_only: Make all attributes keyword only
     :param frozen: Prevent attribute values from being changed once defined
                    (This does not prevent the modification of mutable attributes
                    such as lists)
     :param dict_method: Include an as_dict method for faster dictionary creation
     :param recursive_repr: Safely handle repr in case of recursion
+    :param gathered_fields: Pre-gathered fields callable, to skip re-collecting attributes
     :return: class with __ methods defined
     """
     cls_dict = cls.__dict__
 
     if INTERNALS_DICT in cls_dict:
         raise PrefabError(
             f"Decorated class {cls.__name__!r} "
             f"has already been processed as a Prefab."
         )
 
     slots = cls_dict.get("__slots__")
-    if isinstance(slots, SlotFields):
-        gatherer = slot_prefab_gatherer
-        slotted = True
+    if gathered_fields is None:
+        if isinstance(slots, SlotFields):
+            gatherer = slot_prefab_gatherer
+            slotted = True
+        else:
+            gatherer = attribute_gatherer
+            slotted = False
     else:
-        gatherer = attribute_gatherer
-        slotted = False
+        gatherer = gathered_fields
+        slotted = False if slots is None else True
 
     methods = set()
 
     if init and "__init__" not in cls_dict:
         methods.add(init_maker)
     else:
         methods.add(prefab_init_maker)
@@ -766,14 +772,15 @@
     eq=True,
     iter=False,
     match_args=True,
     kw_only=False,
     frozen=False,
     dict_method=False,
     recursive_repr=False,
+    slots=False,
 ):
     """
     Dynamically construct a (dynamic) prefab.
 
     :param class_name: name of the resulting prefab class
     :param attributes: list of (name, attribute()) pairs to assign to the class
                        for construction
@@ -786,32 +793,56 @@
     :param iter: generate __iter__
     :param match_args: generate __match_args__
     :param kw_only: make all attributes keyword only
     :param frozen: Prevent attribute values from being changed once defined
                    (This does not prevent the modification of mutable attributes such as lists)
     :param dict_method: Include an as_dict method for faster dictionary creation
     :param recursive_repr: Safely handle repr in case of recursion
+    :param slots: Make the resulting class slotted
     :return: class with __ methods defined
     """
-    class_dict = {} if class_dict is None else class_dict
-    cls = type(class_name, bases, class_dict)
+    class_dict = {} if class_dict is None else class_dict.copy()
+
+    class_annotations = {}
+    class_slots = {}
+    fields = {}
+
     for name, attrib in attributes:
-        setattr(cls, name, attrib)
+        if isinstance(attrib, Attribute):
+            fields[name] = attrib
+        elif isinstance(attrib, Field):
+            fields[name] = Attribute.from_field(attrib)
+        else:
+            fields[name] = Attribute(default=attrib)
+
+        if attrib.type is not NOTHING:
+            class_annotations[name] = attrib.type
+
+        class_slots[name] = attrib.doc
+
+    if slots:
+        class_dict["__slots__"] = class_slots
+
+    class_dict["__annotations__"] = class_annotations
+    cls = type(class_name, bases, class_dict)
+
+    gathered_fields = GatheredFields(fields, {})
 
     cls = _make_prefab(
         cls,
         init=init,
         repr=repr,
         eq=eq,
         iter=iter,
         match_args=match_args,
         kw_only=kw_only,
         frozen=frozen,
         dict_method=dict_method,
         recursive_repr=recursive_repr,
+        gathered_fields=gathered_fields,
     )
 
     return cls
 
 
 # Extra Functions
 def is_prefab(o):
```

### Comparing `ducktools_classbuilder-0.5.0/src/ducktools/classbuilder/prefab.pyi` & `ducktools_classbuilder-0.5.1/src/ducktools/classbuilder/prefab.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     eq: bool = True,
     iter: bool = False,
     match_args: bool = True,
     kw_only: bool = False,
     frozen: bool = False,
     dict_method: bool = False,
     recursive_repr: bool = False,
+    gathered_fields: Callable[[type], tuple[dict[str, Attribute], dict[str, typing.Any]]] | None = None,
 ) -> type: ...
 
 _T = typing.TypeVar("_T")
 
 
 # For some reason PyCharm can't see 'attribute'?!?
 # noinspection PyUnresolvedReferences
@@ -142,14 +143,15 @@
     eq: bool = True,
     iter: bool = False,
     match_args: bool = True,
     kw_only: bool = False,
     frozen: bool = False,
     dict_method: bool = False,
     recursive_repr: bool = False,
+    slots: bool = False,
 ) -> type: ...
 
 def is_prefab(o: typing.Any) -> bool: ...
 
 def is_prefab_instance(o: object) -> bool: ...
 
 def as_dict(o) -> dict[str, typing.Any]: ...
```

### Comparing `ducktools_classbuilder-0.5.0/src/ducktools_classbuilder.egg-info/PKG-INFO` & `ducktools_classbuilder-0.5.1/src/ducktools_classbuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.5.0
+Version: 0.5.1
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ducktools_classbuilder-0.5.0/src/ducktools_classbuilder.egg-info/SOURCES.txt` & `ducktools_classbuilder-0.5.1/src/ducktools_classbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_construction.py` & `ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_construction.py`

 * *Files 22% similar despite different names*

```diff
@@ -87,7 +87,29 @@
 
     # This class should actually work because *all* attributes are kw_only
     @prefab(kw_only=True)
     class KeywordPrefab:
         a: int = 0
         b: int = attribute(kw_only=True)
         c: int = attribute()  # kw_only should be ignored
+
+
+def test_build_slotted():
+    SlottedClass = build_prefab(
+        "SlottedClass",
+        [
+            ("x", attribute(doc="x co-ordinate", type=float)),
+            ("y", attribute(default=0, doc="y co-ordinate", type=float))
+        ],
+        slots=True,
+    )
+
+    inst = SlottedClass(1)
+    assert inst.x == 1
+    assert inst.y == 0
+    assert SlottedClass.__slots__ == {'x': "x co-ordinate", 'y': "y co-ordinate"}
+
+    assert SlottedClass.__annotations__ == {'x': float, 'y': float}
+
+    # Test slots are functioning
+    with pytest.raises(AttributeError):
+        inst.z = 0
```

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_internals.py` & `ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_internals.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_pre_post_init.py` & `ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_pre_post_init.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/dynamic/test_slotted_class.py` & `ducktools_classbuilder-0.5.1/tests/prefab/dynamic/test_slotted_class.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/creation.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/creation.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/dunders.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/dunders.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/inheritance.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/inheritance.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/init_ex.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/init_ex.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/kw_only.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/kw_only.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/examples/repr_func.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/examples/repr_func.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/test_creation.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/test_creation.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/test_dunders.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/test_dunders.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/test_frozen.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/test_frozen.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/test_funcs.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/test_funcs.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/test_hint_syntax.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/test_hint_syntax.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/test_inheritance.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/test_init.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/test_init.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/test_kw_only.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/test_kw_only.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/prefab/shared/test_repr.py` & `ducktools_classbuilder-0.5.1/tests/prefab/shared/test_repr.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/test_annotated.py` & `ducktools_classbuilder-0.5.1/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.5.0/tests/test_core.py` & `ducktools_classbuilder-0.5.1/tests/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     init_maker,
     builder,
     Field,
     SlotFields,
     slot_gatherer,
     slotclass,
     fieldclass,
+    GatheredFields,
 )
 
 
 def test_get_fields_flags():
     local_fields = {"Example": Field()}
     resolved_fields = {"ParentField": Field(), "Example": Field()}
     flags = {"slotted": False}
@@ -295,14 +296,66 @@
             c=Field(default_factory=list, doc="a list"),
         )
 
     assert "__repr__" not in SlotClass.__dict__
     assert "__eq__" not in SlotClass.__dict__
 
 
+def test_slotclass_weakref():
+    import weakref
+
+    @slotclass
+    class WeakrefClass:
+        __slots__ = SlotFields(
+            a=1,
+            b=2,
+            __weakref__=None,
+        )
+
+    flds = get_fields(WeakrefClass)
+    assert 'a' in flds
+    assert 'b' in flds
+    assert '__weakref__' not in flds
+
+    slots = WeakrefClass.__slots__
+    assert 'a' in slots
+    assert 'b' in slots
+    assert '__weakref__' in slots
+
+    # Test weakrefs can be created
+    inst = WeakrefClass()
+    ref = weakref.ref(inst)
+    assert ref == inst.__weakref__
+
+
+def test_slotclass_dict():
+    @slotclass
+    class DictClass:
+        __slots__ = SlotFields(
+            a=1,
+            b=2,
+            __dict__=None,
+        )
+
+    flds = get_fields(DictClass)
+    assert 'a' in flds
+    assert 'b' in flds
+    assert '__dict__' not in flds
+
+    slots = DictClass.__slots__
+    assert 'a' in slots
+    assert 'b' in slots
+    assert '__dict__' in slots
+
+    # Test if __dict__ is included new values can be added
+    inst = DictClass()
+    inst.c = 42
+    assert inst.__dict__ == {"c": 42}
+
+
 def test_fieldclass():
     @fieldclass
     class NewField(Field):
         __slots__ = SlotFields(serialize=True)
         serialize: bool
 
     f = NewField()
@@ -370,7 +423,35 @@
     assert "__repr__" not in SlotClass.__dict__
     assert "__eq__" not in SlotClass.__dict__
 
     x = SlotClass(12)
     assert x.a == 12
     assert x.b == 2
     assert x.c == []
+
+
+def test_gatheredfields():
+    fields = {"x": Field(default=1)}
+    modifications = {"x": NOTHING}
+
+    alt_fields = {"x": Field(default=1), "y": Field(default=2)}
+
+    flds = GatheredFields(fields, modifications)
+    flds_2 = GatheredFields(fields, modifications)
+    flds_3 = GatheredFields(alt_fields, modifications)
+
+    class Ex:
+        pass
+
+    assert flds(Ex) == (fields, modifications)
+
+    assert flds == flds_2
+    assert flds != flds_3
+    assert flds != object()
+
+    assert repr(flds).endswith(
+        "GatheredFields("
+        "fields={'x': Field(default=1, default_factory=<NOTHING OBJECT>, type=<NOTHING OBJECT>, doc=None)}, "
+        "modifications={'x': <NOTHING OBJECT>}"
+        ")"
+    )
+
```

