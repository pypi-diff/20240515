# Comparing `tmp/compas_fea2-0.2.0.tar.gz` & `tmp/compas_fea2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_fea2-0.2.0.tar", last modified: Mon May 13 20:49:01 2024, max compression
+gzip compressed data, was "compas_fea2-0.2.1.tar", last modified: Wed May 15 08:25:00 2024, max compression
```

## Comparing `compas_fea2-0.2.0.tar` & `compas_fea2-0.2.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.418388 compas_fea2-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-13 20:49:01.418388 compas_fea2-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:49:01.418388 compas_fea2-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.402387 compas_fea2-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.406387 compas_fea2-0.2.0/src/compas_fea2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.406387 compas_fea2-0.2.0/src/compas_fea2/UI/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/UI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.406387 compas_fea2-0.2.0/src/compas_fea2/UI/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/UI/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/UI/viewer/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/UI/viewer/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.406387 compas_fea2-0.2.0/src/compas_fea2/job/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/job/input_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.410387 compas_fea2-0.2.0/src/compas_fea2/model/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/bcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    17204 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/ics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.410387 compas_fea2-0.2.0/src/compas_fea2/model/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/materials/concrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/materials/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/materials/steel.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/materials/timber.py
--rw-r--r--   0 runner    (1001) docker     (127)    38772 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    56602 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/parts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/releases.py
--rw-r--r--   0 runner    (1001) docker     (127)    23607 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/model/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.410387 compas_fea2-0.2.0/src/compas_fea2/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/postprocess/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/postprocess/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/postprocess/stresses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.410387 compas_fea2-0.2.0/src/compas_fea2/problem/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/combinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/loads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.414387 compas_fea2-0.2.0/src/compas_fea2/problem/steps/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/steps/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/steps/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/steps/quasistatic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/steps/static.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/steps/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/problem/steps_combinations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.414387 compas_fea2-0.2.0/src/compas_fea2/results/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/results/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/results/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/results/histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    31102 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/results/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/results/sql_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.414387 compas_fea2-0.2.0/src/compas_fea2/units/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.414387 compas_fea2-0.2.0/src/compas_fea2/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/utilities/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/src/compas_fea2/utilities/loads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.414387 compas_fea2-0.2.0/src/compas_fea2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-13 20:49:01.000000 compas_fea2-0.2.0/src/compas_fea2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-13 20:49:01.000000 compas_fea2-0.2.0/src/compas_fea2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:49:01.000000 compas_fea2-0.2.0/src/compas_fea2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 20:49:01.000000 compas_fea2-0.2.0/src/compas_fea2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:49:01.000000 compas_fea2-0.2.0/src/compas_fea2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-13 20:49:01.000000 compas_fea2-0.2.0/src/compas_fea2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 20:49:01.000000 compas_fea2-0.2.0/src/compas_fea2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:49:01.414387 compas_fea2-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 20:48:50.000000 compas_fea2-0.2.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.874486 compas_fea2-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-15 08:25:00.874486 compas_fea2-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:25:00.874486 compas_fea2-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.858486 compas_fea2-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.862486 compas_fea2-0.2.1/src/compas_fea2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.862486 compas_fea2-0.2.1/src/compas_fea2/UI/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/UI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.866486 compas_fea2-0.2.1/src/compas_fea2/UI/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/UI/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/UI/viewer/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/UI/viewer/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.866486 compas_fea2-0.2.1/src/compas_fea2/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/job/input_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.866486 compas_fea2-0.2.1/src/compas_fea2/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/bcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17204 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/ics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.866486 compas_fea2-0.2.1/src/compas_fea2/model/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/materials/concrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/materials/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/materials/steel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/materials/timber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38772 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56602 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/releases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23607 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/model/sections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.870486 compas_fea2-0.2.1/src/compas_fea2/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/postprocess/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/postprocess/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/postprocess/stresses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.870486 compas_fea2-0.2.1/src/compas_fea2/problem/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/combinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.870486 compas_fea2-0.2.1/src/compas_fea2/problem/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/steps/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/steps/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/steps/quasistatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/steps/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/problem/steps_combinations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.870486 compas_fea2-0.2.1/src/compas_fea2/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/results/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/results/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/results/histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31102 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/results/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/results/sql_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.870486 compas_fea2-0.2.1/src/compas_fea2/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.874486 compas_fea2-0.2.1/src/compas_fea2/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/utilities/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/src/compas_fea2/utilities/loads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.874486 compas_fea2-0.2.1/src/compas_fea2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-15 08:25:00.000000 compas_fea2-0.2.1/src/compas_fea2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-15 08:25:00.000000 compas_fea2-0.2.1/src/compas_fea2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:25:00.000000 compas_fea2-0.2.1/src/compas_fea2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 08:25:00.000000 compas_fea2-0.2.1/src/compas_fea2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:25:00.000000 compas_fea2-0.2.1/src/compas_fea2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-15 08:25:00.000000 compas_fea2-0.2.1/src/compas_fea2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 08:25:00.000000 compas_fea2-0.2.1/src/compas_fea2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:25:00.874486 compas_fea2-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 08:24:47.000000 compas_fea2-0.2.1/tests/test_placeholder.py
```

### Comparing `compas_fea2-0.2.0/LICENSE` & `compas_fea2-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/PKG-INFO` & `compas_fea2-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_fea2
-Version: 0.2.0
+Version: 0.2.1
 Summary: This package is the 2nd generation of Finite element Analysis tools for COMPAS.
 Author-email: Francesco Ranaudo <ranaudo@arch.ethz.ch>
 License: MIT License
         
         Copyright (c) 2018-2021 Block Research Group - ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_fea2-0.2.0/README.md` & `compas_fea2-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/pyproject.toml` & `compas_fea2-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "0.2.0"
+current_version = "0.2.1"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_fea2/__init__.py"
 search = "{current_version}"
```

### Comparing `compas_fea2-0.2.0/src/compas_fea2/UI/viewer/shapes.py` & `compas_fea2-0.2.1/src/compas_fea2/UI/viewer/shapes.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/UI/viewer/viewer.py` & `compas_fea2-0.2.1/src/compas_fea2/UI/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/__init__.py` & `compas_fea2-0.2.1/src/compas_fea2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from compas.tolerance import Tolerance  # noqa: F401
 
 
 __author__ = ["Francesco Ranaudo"]
 __copyright__ = "Block Research Group"
 __license__ = "MIT License"
 __email__ = "ranaudo@arch.ethz.ch"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 UMAT = os.path.abspath(os.path.join(DATA, "umat"))
```

### Comparing `compas_fea2-0.2.0/src/compas_fea2/base.py` & `compas_fea2-0.2.1/src/compas_fea2/base.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/cli.py` & `compas_fea2-0.2.1/src/compas_fea2/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """
 Console script for compas_fea2.
 """
 
-import json
+import importlib
 import os
 import sys
 
 import click
+import dotenv
 
 from compas_fea2 import HOME
+from compas_fea2 import VERBOSE
 
 try:
     from fea2_extension.main import init_plugin  # type: ignore
 except Exception:
-    print("WARNING: fea2_extension module not installed.")
+    if VERBOSE:
+        print("WARNING: fea2_extension module not installed.")
 
 
 # -------------------------------- MAIN ----------------------------------#
 @click.group()
 def main():
     """fea2 main.
 
@@ -42,33 +45,31 @@
         The name of the backend. This is must be lower case.
     """
     init_plugin(HOME, backend, clean)
     backend = backend.lower()
 
 
 @main.command()
-# @click.option('--clean', default='False', help='remove existing directories')
 @click.argument("backend")
 @click.argument("setting")
 @click.argument("value")
-def change_settings(backend, setting, value):
+def change_setting(backend, setting, value):
     """Change a setting for the specified backend.\n
-    backend : txt\n
-        The name of the backend.
-    setting : txt\n
-        The setting to be changed.
-    value : txt\n
-        The new value for the setting.
-    """
-    backend_settings = os.path.join(HOME, "src", "compas_fea2", "backends", backend.lower(), "settings.json")
+        backend : txt\n
+            The name of the backend.
+        setting : txt\n
+            The setting to be changed.
+        value : txt\n
+            The new value for the setting.
 
-    with open(backend_settings, "r") as f:
-        settings = json.load(f)
-
-    with open(backend_settings, "w") as f:
-        settings[setting] = value
-        json.dump(settings, f)
+    Example usage:\n
+        fea2 change-setting opensees exe "Applications/OpenSees3.5.0/bin/OpenSees"
+    """
+    m = importlib.import_module("compas_fea2_" + backend.lower())
+    env = os.path.join(m.HOME, "src", "compas_fea2_" + backend.lower(), ".env")
+    dotenv.set_key(env, setting.upper(), value)
+    print(f"{setting.upper()} set to {value} for compas_fea2_{backend.lower()}")
 
 
 # -------------------------------- DEBUG ----------------------------------#
 if __name__ == "__main__":
     sys.exit(main.init_backend())
```

### Comparing `compas_fea2-0.2.0/src/compas_fea2/job/input_file.py` & `compas_fea2-0.2.1/src/compas_fea2/job/input_file.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/__init__.py` & `compas_fea2-0.2.1/src/compas_fea2/model/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/bcs.py` & `compas_fea2-0.2.1/src/compas_fea2/model/bcs.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/connectors.py` & `compas_fea2-0.2.1/src/compas_fea2/model/connectors.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/constraints.py` & `compas_fea2-0.2.1/src/compas_fea2/model/constraints.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/elements.py` & `compas_fea2-0.2.1/src/compas_fea2/model/elements.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/groups.py` & `compas_fea2-0.2.1/src/compas_fea2/model/groups.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/ics.py` & `compas_fea2-0.2.1/src/compas_fea2/model/ics.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/materials/concrete.py` & `compas_fea2-0.2.1/src/compas_fea2/model/materials/concrete.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/materials/material.py` & `compas_fea2-0.2.1/src/compas_fea2/model/materials/material.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/materials/steel.py` & `compas_fea2-0.2.1/src/compas_fea2/model/materials/steel.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/model.py` & `compas_fea2-0.2.1/src/compas_fea2/model/model.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/nodes.py` & `compas_fea2-0.2.1/src/compas_fea2/model/nodes.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/parts.py` & `compas_fea2-0.2.1/src/compas_fea2/model/parts.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/releases.py` & `compas_fea2-0.2.1/src/compas_fea2/model/releases.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/model/sections.py` & `compas_fea2-0.2.1/src/compas_fea2/model/sections.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/postprocess/report.py` & `compas_fea2-0.2.1/src/compas_fea2/postprocess/report.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/postprocess/stresses.py` & `compas_fea2-0.2.1/src/compas_fea2/postprocess/stresses.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/__init__.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/combinations.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/combinations.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/displacements.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/displacements.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/fields.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/fields.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/loads.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/loads.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/outputs.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/outputs.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/patterns.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/patterns.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/problem.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/problem.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/steps/__init__.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/steps/perturbations.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/steps/perturbations.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/steps/quasistatic.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/steps/quasistatic.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/steps/static.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/steps/static.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/steps/step.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/steps/step.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/problem/steps_combinations.py` & `compas_fea2-0.2.1/src/compas_fea2/problem/steps_combinations.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/results/__init__.py` & `compas_fea2-0.2.1/src/compas_fea2/results/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/results/database.py` & `compas_fea2-0.2.1/src/compas_fea2/results/database.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/results/fields.py` & `compas_fea2-0.2.1/src/compas_fea2/results/fields.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/results/histories.py` & `compas_fea2-0.2.1/src/compas_fea2/results/histories.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/results/results.py` & `compas_fea2-0.2.1/src/compas_fea2/results/results.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/results/sql_wrapper.py` & `compas_fea2-0.2.1/src/compas_fea2/results/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/utilities/_utils.py` & `compas_fea2-0.2.1/src/compas_fea2/utilities/_utils.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2/utilities/loads.py` & `compas_fea2-0.2.1/src/compas_fea2/utilities/loads.py`

 * *Files identical despite different names*

### Comparing `compas_fea2-0.2.0/src/compas_fea2.egg-info/PKG-INFO` & `compas_fea2-0.2.1/src/compas_fea2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_fea2
-Version: 0.2.0
+Version: 0.2.1
 Summary: This package is the 2nd generation of Finite element Analysis tools for COMPAS.
 Author-email: Francesco Ranaudo <ranaudo@arch.ethz.ch>
 License: MIT License
         
         Copyright (c) 2018-2021 Block Research Group - ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_fea2-0.2.0/src/compas_fea2.egg-info/SOURCES.txt` & `compas_fea2-0.2.1/src/compas_fea2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

