# Comparing `tmp/apsg-1.1.4.tar.gz` & `tmp/apsg-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apsg-1.1.4.tar", last modified: Wed Dec 13 22:58:43 2023, max compression
+gzip compressed data, was "apsg-1.1.5.tar", last modified: Wed May 15 10:32:58 2024, max compression
```

## Comparing `apsg-1.1.4.tar` & `apsg-1.1.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.848875 apsg-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-13 22:58:36.000000 apsg-1.1.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-12-13 22:58:36.000000 apsg-1.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2023-12-13 22:58:36.000000 apsg-1.1.4/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-13 22:58:36.000000 apsg-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-13 22:58:36.000000 apsg-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15042 2023-12-13 22:58:43.848875 apsg-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2023-12-13 22:58:36.000000 apsg-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.840875 apsg-1.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/apsg.database.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/apsg.feature.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/apsg.helpers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/apsg.math.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/apsg.pandas.rst
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/apsg.plotting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/automodules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8787 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-13 22:58:36.000000 apsg-1.1.4/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-13 22:58:36.000000 apsg-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-13 22:58:43.848875 apsg-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-12-13 22:58:36.000000 apsg-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.836875 apsg-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.840875 apsg-1.1.4/src/apsg/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.844875 apsg-1.1.4/src/apsg/database/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18281 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/database/_alchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/database/_sdbread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.844875 apsg-1.1.4/src/apsg/decorator/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/decorator/_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.844875 apsg-1.1.4/src/apsg/feature/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56081 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/feature/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/feature/_geodata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14887 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/feature/_paleomag.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/feature/_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/feature/_tensor2.py
--rw-r--r--   0 runner    (1001) docker     (127)    27973 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/feature/_tensor3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.844875 apsg-1.1.4/src/apsg/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/helpers/_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/helpers/_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/helpers/_notation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.844875 apsg-1.1.4/src/apsg/math/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/math/_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    16476 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/math/_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.848875 apsg-1.1.4/src/apsg/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/pandas/_pandas_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.848875 apsg-1.1.4/src/apsg/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18863 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/plotting/_fabricplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/plotting/_paleomagplots.py
--rw-r--r--   0 runner    (1001) docker     (127)    21059 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/plotting/_plot_artists.py
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/plotting/_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12809 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/plotting/_roseplot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/plotting/_stereogrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    36506 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/plotting/_stereonet.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-13 22:58:36.000000 apsg-1.1.4/src/apsg/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.848875 apsg-1.1.4/src/apsg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15042 2023-12-13 22:58:43.000000 apsg-1.1.4/src/apsg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2023-12-13 22:58:43.000000 apsg-1.1.4/src/apsg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 22:58:43.000000 apsg-1.1.4/src/apsg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-13 22:58:43.000000 apsg-1.1.4/src/apsg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-13 22:58:43.000000 apsg-1.1.4/src/apsg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-13 22:58:43.000000 apsg-1.1.4/src/apsg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:43.848875 apsg-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:58:36.000000 apsg-1.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-12-13 22:58:36.000000 apsg-1.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16080 2023-12-13 22:58:36.000000 apsg-1.1.4/tests/test_apsg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-12-13 22:58:36.000000 apsg-1.1.4/tests/test_tensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.700753 apsg-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-15 10:32:50.000000 apsg-1.1.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-15 10:32:50.000000 apsg-1.1.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-05-15 10:32:50.000000 apsg-1.1.5/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-15 10:32:50.000000 apsg-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 10:32:50.000000 apsg-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-05-15 10:32:58.700753 apsg-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 10:32:50.000000 apsg-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.688753 apsg-1.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.database.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.feature.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.math.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.pandas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/automodules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-15 10:32:50.000000 apsg-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-15 10:32:58.700753 apsg-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-15 10:32:50.000000 apsg-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.684753 apsg-1.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.688753 apsg-1.1.5/src/apsg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.692753 apsg-1.1.5/src/apsg/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/database/_alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/database/_sdbread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.692753 apsg-1.1.5/src/apsg/decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/decorator/_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.692753 apsg-1.1.5/src/apsg/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56059 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_geodata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_paleomag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_tensor2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27973 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_tensor3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.692753 apsg-1.1.5/src/apsg/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/helpers/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/helpers/_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/helpers/_notation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/src/apsg/math/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/math/_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/math/_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/src/apsg/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/pandas/_pandas_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/src/apsg/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_fabricplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_paleomagplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21059 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_plot_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_roseplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_stereogrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36506 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_stereonet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/src/apsg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:50.000000 apsg-1.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-15 10:32:50.000000 apsg-1.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-05-15 10:32:50.000000 apsg-1.1.5/tests/test_apsg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-15 10:32:50.000000 apsg-1.1.5/tests/test_tensors.py
```

### Comparing `apsg-1.1.4/CONTRIBUTING.md` & `apsg-1.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/HISTORY.md` & `apsg-1.1.5/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changes
 
+### 1.1.5 (May 15 2024)
+ * paleomag Core .dd bug fixed
+ * fix round-off domain math error for acosd and asind
+
 ### 1.1.4 (Dec 13 2023)
  * Ellipsoid repr bugfix
 
 ### 1.1.3 (Oct 23 2023)
 Bugfix release
  * slip and dilatation tendency methods added to stress
  * proj alias of project for FeatureSet added
```

### Comparing `apsg-1.1.4/LICENSE` & `apsg-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/PKG-INFO` & `apsg-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsg
-Version: 1.1.4
+Version: 1.1.5
 Summary: APSG - The package for structural geologists
 Home-page: https://github.com/ondrolexa/apsg
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Project-URL: Documentation, https://apsg.readthedocs.io/
 Project-URL: Source Code, https://github.com/ondrolexa/apsg/
@@ -135,14 +135,18 @@
 ## License
 
 APSG is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changes
 
+### 1.1.5 (May 15 2024)
+ * paleomag Core .dd bug fixed
+ * fix round-off domain math error for acosd and asind
+
 ### 1.1.4 (Dec 13 2023)
  * Ellipsoid repr bugfix
 
 ### 1.1.3 (Oct 23 2023)
 Bugfix release
  * slip and dilatation tendency methods added to stress
  * proj alias of project for FeatureSet added
```

### Comparing `apsg-1.1.4/README.md` & `apsg-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/docs/Makefile` & `apsg-1.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/docs/apsg.database.rst` & `apsg-1.1.5/docs/apsg.database.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/docs/conf.py` & `apsg-1.1.5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,40 +42,40 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.autodoc",
     "nbsphinx",
     "autodocsumm",
     "sphinx_rtd_theme",
 ]
 
-autodoc_mock_imports = ['sqlalchemy']
+autodoc_mock_imports = ["sqlalchemy"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"APSG"
-copyright = u"2023, Ondrej Lexa"
+project = "APSG"
+copyright = "2023, Ondrej Lexa"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = "1.1"
 # The full version, including alpha/beta/rc tags.
-release = "1.1.4"
+release = "1.1.5"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to
 # some non-false value, then it is used:
@@ -157,15 +157,15 @@
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets)
 # here, relative to this directory. They are copied after the builtin
 # static files, so a file named "default.css" will overwrite the builtin
 # "default.css".
 
-#html_static_path = ["_static"]
+# html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page
 # bottom, using the given strftime format.
 # html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
@@ -221,15 +221,15 @@
     # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto/manual]).
 latex_documents = [
-    ("index", "apsg.tex", u"APSG Documentation", u"Ondrej Lexa", "manual"),
+    ("index", "apsg.tex", "APSG Documentation", "Ondrej Lexa", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at
 # the top of the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings
@@ -249,31 +249,31 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [("index", "apsg", u"APSG Documentation", [u"Ondrej Lexa"], 1)]
+man_pages = [("index", "apsg", "APSG Documentation", ["Ondrej Lexa"], 1)]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         "index",
         "apsg",
-        u"APSG Documentation",
-        u"Ondrej Lexa",
+        "APSG Documentation",
+        "Ondrej Lexa",
         "apsg",
         " structural geology module for Python",
         "Earth sciences",
     ),
 ]
 
 # Documents to append as an appendix to all manuals.
@@ -285,9 +285,9 @@
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 # texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 # Sort members by type
-#autodoc_member_order = "groupwise"
-autodoc_member_order = 'bysource'
+# autodoc_member_order = "groupwise"
+autodoc_member_order = "bysource"
```

### Comparing `apsg-1.1.4/docs/contributing.rst` & `apsg-1.1.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/docs/index.rst` & `apsg-1.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/docs/installation.rst` & `apsg-1.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/docs/make.bat` & `apsg-1.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/setup.py` & `apsg-1.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open(path.join(CURRENT_PATH, "HISTORY.md")) as file:
     history = file.read()
 
 setup(
     name="apsg",
-    version="1.1.4",
+    version="1.1.5",
     description="APSG - The package for structural geologists",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     author="Ondrej Lexa",
     author_email="lexa.ondrej@gmail.com",
     url="https://github.com/ondrolexa/apsg",
     license="MIT",
```

### Comparing `apsg-1.1.4/src/apsg/__init__.py` & `apsg-1.1.5/src/apsg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     "VollmerPlot",
     "RamsayPlot",
     "FlinnPlot",
     "HsuPlot",
     "quicknet",
 )
 
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 __author__ = "Ondrej Lexa"
 __email__ = "lexa.ondrej@gmail.com"
```

### Comparing `apsg-1.1.4/src/apsg/config.py` & `apsg-1.1.5/src/apsg/config.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/database/_alchemy.py` & `apsg-1.1.5/src/apsg/database/_alchemy.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/database/_sdbread.py` & `apsg-1.1.5/src/apsg/database/_sdbread.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/decorator/_decorator.py` & `apsg-1.1.5/src/apsg/decorator/_decorator.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/feature/__init__.py` & `apsg-1.1.5/src/apsg/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/feature/_container.py` & `apsg-1.1.5/src/apsg/feature/_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,26 +138,26 @@
 
     @property
     def direction(self):
         """Return array of direction angles"""
         return np.asarray([e.direction for e in self]).T
 
     def proj(self, vec):
-        """Return projections of all features in ``FeatureSet`` onto vector."""
+        """Return projections of all features in ``Vector2Set`` onto vector."""
         return type(self)([e.project() for e in self], name=self.name)
 
     def dot(self, vec):
-        """Return array of dot products of all features in ``FeatureSet`` with vector."""
+        """Return array of dot products of all features in ``Vector2Set`` with vector."""
         return np.array([e.dot(vec) for e in self])
 
     def cross(self, other=None):
-        """Return cross products of all features in ``FeatureSet``
+        """Return cross products of all features in ``Vector2Set``
 
         Without arguments it returns cross product of all pairs in dataset.
-        If argument is ``FeatureSet`` of same length or single data object
+        If argument is ``Vector2Set`` of same length or single data object
         element-wise cross-products are calculated.
         """
         res = []
         if other is None:
             res = [e.cross(f) for e, f in combinations(self.data, 2)]
         elif issubclass(type(other), FeatureSet):
             res = [e.cross(f) for e, f in zip(self, other)]
@@ -166,56 +166,56 @@
         else:
             raise TypeError("Wrong argument type!")
         return np.asarray(res)
 
     __pow__ = cross
 
     def angle(self, other=None):
-        """Return angles of all data in ``FeatureSet`` object
+        """Return angles of all data in ``Vector2Set`` object
 
         Without arguments it returns angles of all pairs in dataset.
-        If argument is ``FeatureSet`` of same length or single data object
+        If argument is ``Vector2Set`` of same length or single data object
         element-wise angles are calculated.
         """
         res = []
         if other is None:
             res = [e.angle(f) for e, f in combinations(self.data, 2)]
         elif issubclass(type(other), FeatureSet):
             res = [e.angle(f) for e, f in zip(self, other)]
         elif issubclass(type(other), Vector3):
             res = [e.angle(other) for e in self]
         else:
             raise TypeError("Wrong argument type!")
         return np.asarray(res)
 
     def normalized(self):
-        """Return ``FeatureSet`` object with normalized (unit length) elements."""
+        """Return ``Vector2Set`` object with normalized (unit length) elements."""
         return type(self)([e.normalized() for e in self], name=self.name)
 
     uv = normalized
 
     def transform(self, F, **kwargs):
-        """Return affine transformation of all features ``FeatureSet`` by matrix 'F'.
+        """Return affine transformation of all features ``Vector2Set`` by matrix 'F'.
 
         Args:
           F: Transformation matrix. Array-like value e.g. ``DeformationGradient3``
 
         Keyword Args:
           norm: normalize transformed features. True or False. Default False
 
         """
         return type(self)([e.transform(F, **kwargs) for e in self], name=self.name)
 
     def R(self, mean=False):
-        """Return resultant of data in ``FeatureSet`` object.
+        """Return resultant of data in ``Vector2Set`` object.
 
-        Resultant is of same type as features in ``FeatureSet``. Note
-        that ``Foliation`` and ``Lineation`` are axial in nature so
-        resultant can give other result than expected. Anyway for axial
-        data orientation tensor analysis will give you right answer.
+        Resultant is of same type as features in ``Vector2Set``. Note
+        that ``Axial2`` is axial in nature so resultant can give
+        other result than expected. Anyway for axial data orientation
+        tensor analysis will give you right answer.
 
         Args:
             mean: if True returns mean resultant. Default False
         """
         R = sum(self)
         if mean:
             R = R / len(self)
@@ -250,15 +250,15 @@
 
         For enough large sample it approach angular standard deviation (csd)
         of Fisher statistics
         """
         return acosd(abs(self.R(mean=True)))
 
     def rdegree(self):
-        """Degree of preffered orientation of vectors in ``FeatureSet``.
+        """Degree of preffered orientation of vectors in ``Vector2Set``.
 
         D = 100 * (2 * abs(R) - n) / n
         """
         N = len(self)
         return 100 * (2 * abs(self.normalized().R()) - N) / N
 
     def ortensor(self):
@@ -275,15 +275,15 @@
     @property
     def _svd(self):
         if "svd" not in self._cache:
             self._cache["svd"] = np.linalg.svd(self._ortensor)
         return self._cache["svd"]
 
     def halfspace(self):
-        """Change orientation of vectors in ``FeatureSet``, so all have angle<=90 with
+        """Change orientation of vectors in ``Vector2Set``, so all have angle<=90 with
         resultant.
 
         """
         dtype_cls = getattr(sys.modules[__name__], type(self).__feature_type__)
         v = Vector3Set(self)
         v_data = list(v)
         alldone = np.all(v.angle(v.R()) <= 90)
@@ -294,49 +294,49 @@
                     v_data[ix] = -v_data[ix]
                 v = Vector3Set(v_data)
                 alldone = np.all(v.angle(v.R()) <= 90)
         return type(self)([dtype_cls(vec) for vec in v], name=self.name)
 
     @classmethod
     def from_direction(cls, angles, name="Default"):
-        """Create ``FeatureSet`` object from arrays of direction angles
+        """Create ``Vector2Set`` object from arrays of direction angles
 
         Args:
           angles: list or angles
 
         Keyword Args:
-          name: name of ``FeatureSet`` object. Default is 'Default'
+          name: name of ``Vector2Set`` object. Default is 'Default'
 
         Example:
           >>> f = vec2set.from_angles([120,130,140,125, 132. 131])
         """
         dtype_cls = getattr(sys.modules[__name__], cls.__feature_type__)
         return cls([dtype_cls(a) for a in angles], name=name)
 
     @classmethod
     def from_xy(cls, x, y, name="Default"):
-        """Create ``FeatureSet`` object from arrays of x and y components
+        """Create ``Vector2Set`` object from arrays of x and y components
 
         Args:
           x: list or array of x components
           y: list or array of y components
 
         Keyword Args:
-          name: name of ``FeatureSet`` object. Default is 'Default'
+          name: name of ``Vector2Set`` object. Default is 'Default'
 
         Example:
           >>> v = vec2set.from_xy([-0.4330127, -0.4330127, -0.66793414],
                                   [0.75, 0.25, 0.60141061])
         """
         dtype_cls = getattr(sys.modules[__name__], cls.__feature_type__)
         return cls([dtype_cls(xx, yy) for xx, yy in zip(x, y)], name=name)
 
     @classmethod
     def random(cls, n=100, name="Default"):
-        """Method to create ``FeatureSet`` of features with uniformly distributed
+        """Method to create ``Vector2Set`` of features with uniformly distributed
         random orientation.
 
         Keyword Args:
           n: number of objects to be generated
           name: name of dataset. Default is 'Default'
 
         Example:
@@ -345,15 +345,15 @@
 
         """
         dtype_cls = getattr(sys.modules[__name__], cls.__feature_type__)
         return cls([dtype_cls.random() for i in range(n)], name=name)
 
     @classmethod
     def random_vonmises(cls, n=100, position=0, kappa=5, name="Default"):
-        """Return ``FeatureSet`` of random vectors sampled from von Mises distribution
+        """Return ``Vector2Set`` of random vectors sampled from von Mises distribution
         around center position with concentration kappa.
 
         Args:
           n: number of objects to be generated
           position: mean orientation given as angle. Default 0
           kappa: precision parameter of the distribution. Default 20
           name: name of dataset. Default is 'Default'
```

### Comparing `apsg-1.1.4/src/apsg/feature/_geodata.py` & `apsg-1.1.5/src/apsg/feature/_geodata.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/feature/_paleomag.py` & `apsg-1.1.5/src/apsg/feature/_paleomag.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,18 +152,18 @@
         if filename is None:
             filename = self.filename
         ff = os.path.splitext(os.path.basename(filename))[0][:8]
         dt = self.date.strftime("%m-%d-%Y %H:%M")
         infoln = "{:<8}  a={:5.1f}   b={:5.1f}   s={:5.1f}   d={:5.1f}   v={}m3  {}"
         ln0 = infoln.format(
             ff,
-            self.gref.lin.dd[0],
-            self.gref.lin.dd[1],
-            self.bedding.dd[0],
-            self.bedding.dd[1],
+            self.gref.lin.geo[0],
+            self.gref.lin.geo[1],
+            self.bedding.geo[0],
+            self.bedding.geo[1],
             eformat(self.volume, 2),
             dt,
         )
         headln = (
             "STEP  Xc [Am2]  Yc [Am2]  Zc [Am2]  MAG[A/m]   Dg    Ig    Ds    Is   a95 "
         )
         with open(filename, "w") as pmdfile:
@@ -270,15 +270,15 @@
         data["date"] = datetime.now()
         ix = body.iloc[:, 0].apply(lambda x: x not in exclude)
         data["steps"] = body[ix].iloc[:, 1].astype(int).to_list()
         data["comments"] = body[ix]["Note"].to_list()
         data["a95"] = body[ix]["Prec"].to_list()
         data["vectors"] = []
         for n, r in body[ix].iterrows():
-            data["vectors"].append(r[2] * Vector3(r["Dsp"], r["Isp"]))
+            data["vectors"].append(r.iloc[2] * Vector3(r["Dsp"], r["Isp"]))
         return cls(**data)
 
     def write_rs3(self, filename=None):
         """Save ``Core`` instance to RS3 file.
 
         Args:
           filename: RS3 file
@@ -291,22 +291,22 @@
         step_lbl = f"Step[{self.demag_units}]"
         module_lbl = f"M[{self.module_units}]"
         susceptibility_lbl = f"K[{self.susceptibility_units}]"
         subhead = f"ID {step_lbl:<10} {module_lbl:>12}   Dsp   Isp   Dge   Ige   Dtc   Itc   Dfc   Ifc   Prec {susceptibility_lbl:>13} Limit1    Limit2    Note      "
         latitude = self.latitude if self.latitude is not None else ""
         longitude = self.longitude if self.longitude is not None else ""
         height = self.height if self.height is not None else ""
-        sdec, sinc = (round(self.gref.fol.dd[0]), round(self.gref.fol.dd[1]))
+        sdec, sinc = (round(self.gref.fol.geo[0]), round(self.gref.fol.geo[1]))
         bdec, binc = (
-            (round(self.bedding.dd[0]), round(self.bedding.dd[1]))
+            (round(self.bedding.geo[0]), round(self.bedding.geo[1]))
             if self.bedding is not None
             else ("", "")
         )
         fdec, finc = (
-            (round(self.foldaxis.dd[0]), round(self.foldaxis.dd[1]))
+            (round(self.foldaxis.geo[0]), round(self.foldaxis.geo[1]))
             if self.foldaxis is not None
             else ("", "")
         )
         hline = f"{self.specimen:9} {self.site:9} {latitude:<9} {longitude:<10} {height:<9} {self.rock:14} {self.age:<7} {sdec:<5} {sinc:<5} {bdec:<5} {binc:<5} {fdec:<5} {finc:<5} 12 0  6  0      "
         prefix = "T" if self.demag_units == "°C" else "M"
         with open(filename, "w", encoding="windows-1250") as res3file:
             print(head, file=res3file, end="\r\n")
@@ -320,15 +320,15 @@
                 self.MAG,
                 self.V,
                 self.geo,
                 self.tilt,
                 self.a95,
                 self.comments,
             ):
-                ln = f"{id:2} {step:<10} {MAG:>13g} {V.dd[0]:>5.1f} {V.dd[1]:> 5.1f} {geo.dd[0]:>5.1f} {geo.dd[1]:> 5.1f} {tilt.dd[0]:>5.1f} {tilt.dd[1]:> 5.1f}             {a95:>5.1f}                                   {comment:10}"
+                ln = f"{id:2} {step:<10} {MAG:>13g} {V.geo[0]:>5.1f} {V.geo[1]:> 5.1f} {geo.geo[0]:>5.1f} {geo.geo[1]:> 5.1f} {tilt.geo[0]:>5.1f} {tilt.geo[1]:> 5.1f}             {a95:>5.1f}                                   {comment:10}"
                 print(ln, file=res3file, end="\r\n")
 
     @property
     def datatable(self):
         """Return data list of strings"""
         tb = []
         for step, MAG, V, geo, tilt, a95, comment in zip(
@@ -338,22 +338,22 @@
             self.geo,
             self.tilt,
             self.a95,
             self.comments,
         ):
             ln = "{:<4} {: 9.2E} {: 9.2E} {: 9.2E} {: 9.2E} {:5.1f} {:5.1f} {:5.1f} {:5.1f} {:4.1f} {}".format(
                 step,
-                V[0],
-                V[1],
-                V[2],
+                V.x,
+                V.y,
+                V.z,
                 MAG,
-                geo.dd[0],
-                geo.dd[1],
-                tilt.dd[0],
-                tilt.dd[1],
+                geo.geo[0],
+                geo.geo[1],
+                tilt.geo[0],
+                tilt.geo[1],
                 a95,
                 comment,
             )
             tb.append(ln)
         return tb
 
     def show(self):
@@ -395,15 +395,15 @@
         H = DeformationGradient3.from_two_pairs(self.sref, self.gref)
         return self.V.transform(H)
 
     @property
     def tilt(self):
         """Returns ``Vector3Set`` of vectors in tilt‐corrected coordinates system"""
         return self.geo.rotate(
-            Lineation(self.bedding.dd[0] - 90, 0), -self.bedding.dd[1]
+            Lineation(self.bedding.geo[0] - 90, 0), -self.bedding.geo[1]
         )
 
     def pca(self, kind="geo", origin=False):
         """
         PCA analysis to calculate principal component and MAD
 
         Keyword Args:
```

### Comparing `apsg-1.1.4/src/apsg/feature/_statistics.py` & `apsg-1.1.5/src/apsg/feature/_statistics.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/feature/_tensor2.py` & `apsg-1.1.5/src/apsg/feature/_tensor2.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/feature/_tensor3.py` & `apsg-1.1.5/src/apsg/feature/_tensor3.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/helpers/__init__.py` & `apsg-1.1.5/src/apsg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/helpers/_math.py` & `apsg-1.1.5/src/apsg/helpers/_math.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 def tand(x):
     """Calculate tangent of angle in degrees"""
     return math.tan(math.radians(x))
 
 
 def asind(x):
     """Calculate arc sine in degrees"""
-    return math.degrees(math.asin(x))
+    return math.degrees(math.asin(max(min(x, 1), -1)))
 
 
 def acosd(x):
     """Calculate arc cosine in degrees"""
-    return math.degrees(math.acos(x))
+    return math.degrees(math.acos(max(min(x, 1), -1)))
 
 
 def atand(x):
     """Calculate arc tangent in degrees"""
     return math.degrees(math.atan(x))
```

### Comparing `apsg-1.1.4/src/apsg/helpers/_notation.py` & `apsg-1.1.5/src/apsg/helpers/_notation.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/math/_matrix.py` & `apsg-1.1.5/src/apsg/math/_matrix.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/math/_vector.py` & `apsg-1.1.5/src/apsg/math/_vector.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/pandas/_pandas_api.py` & `apsg-1.1.5/src/apsg/pandas/_pandas_api.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/plotting/__init__.py` & `apsg-1.1.5/src/apsg/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/plotting/_fabricplot.py` & `apsg-1.1.5/src/apsg/plotting/_fabricplot.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/plotting/_paleomagplots.py` & `apsg-1.1.5/src/apsg/plotting/_paleomagplots.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/plotting/_plot_artists.py` & `apsg-1.1.5/src/apsg/plotting/_plot_artists.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/plotting/_projection.py` & `apsg-1.1.5/src/apsg/plotting/_projection.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/plotting/_roseplot.py` & `apsg-1.1.5/src/apsg/plotting/_roseplot.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/plotting/_stereogrid.py` & `apsg-1.1.5/src/apsg/plotting/_stereogrid.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/plotting/_stereonet.py` & `apsg-1.1.5/src/apsg/plotting/_stereonet.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg/shell.py` & `apsg-1.1.5/src/apsg/shell.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/src/apsg.egg-info/PKG-INFO` & `apsg-1.1.5/src/apsg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsg
-Version: 1.1.4
+Version: 1.1.5
 Summary: APSG - The package for structural geologists
 Home-page: https://github.com/ondrolexa/apsg
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Project-URL: Documentation, https://apsg.readthedocs.io/
 Project-URL: Source Code, https://github.com/ondrolexa/apsg/
@@ -135,14 +135,18 @@
 ## License
 
 APSG is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changes
 
+### 1.1.5 (May 15 2024)
+ * paleomag Core .dd bug fixed
+ * fix round-off domain math error for acosd and asind
+
 ### 1.1.4 (Dec 13 2023)
  * Ellipsoid repr bugfix
 
 ### 1.1.3 (Oct 23 2023)
 Bugfix release
  * slip and dilatation tendency methods added to stress
  * proj alias of project for FeatureSet added
```

### Comparing `apsg-1.1.4/src/apsg.egg-info/SOURCES.txt` & `apsg-1.1.5/src/apsg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/tests/conftest.py` & `apsg-1.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/tests/test_apsg.py` & `apsg-1.1.5/tests/test_apsg.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.4/tests/test_tensors.py` & `apsg-1.1.5/tests/test_tensors.py`

 * *Files identical despite different names*

