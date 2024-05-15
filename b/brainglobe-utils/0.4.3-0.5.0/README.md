# Comparing `tmp/brainglobe-utils-0.4.3.tar.gz` & `tmp/brainglobe_utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-utils-0.4.3.tar", last modified: Thu Apr 11 15:26:48 2024, max compression
+gzip compressed data, was "brainglobe_utils-0.5.0.tar", last modified: Wed May 15 13:23:05 2024, max compression
```

## Comparing `brainglobe-utils-0.4.3.tar` & `brainglobe_utils-0.5.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.132340 brainglobe-utils-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.120339 brainglobe-utils-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.120339 brainglobe-utils-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-11 15:26:48.132340 brainglobe-utils-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.120339 brainglobe-utils-0.4.3/brainglobe_utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/IO/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/IO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/IO/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/IO/surfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/IO/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/brainreg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainreg/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/cells/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/cells/cells.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/citation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/bibtex_fmt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/cite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/text_fmt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/general/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/string.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/image_io/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20135 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image_io/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image_io/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/pandas/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/brainglobe.png
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/collapsible_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:26:48.132340 brainglobe-utils-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.534220 brainglobe_utils-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.522220 brainglobe_utils-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.522220 brainglobe_utils-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-15 13:23:05.534220 brainglobe_utils-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.522220 brainglobe_utils-0.5.0/brainglobe_utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.526220 brainglobe_utils-0.5.0/brainglobe_utils/IO/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/IO/cells.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.526220 brainglobe_utils-0.5.0/brainglobe_utils/IO/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/IO/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24064 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/IO/image/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/IO/image/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/IO/image/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/IO/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/IO/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.526220 brainglobe_utils-0.5.0/brainglobe_utils/brainmapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/brainmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/brainmapper/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/brainmapper/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.526220 brainglobe_utils-0.5.0/brainglobe_utils/brainreg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/brainreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/brainreg/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.526220 brainglobe_utils-0.5.0/brainglobe_utils/cells/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/cells/cells.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.526220 brainglobe_utils-0.5.0/brainglobe_utils/citation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/citation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/citation/bibtex_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/citation/cite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/citation/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/citation/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/citation/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/citation/text_fmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.530220 brainglobe_utils-0.5.0/brainglobe_utils/general/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/general/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/general/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/general/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/general/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/general/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/general/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/general/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/general/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.530220 brainglobe_utils-0.5.0/brainglobe_utils/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/image/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/image/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/image/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/image/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.530220 brainglobe_utils-0.5.0/brainglobe_utils/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/pandas/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.530220 brainglobe_utils-0.5.0/brainglobe_utils/qtpy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/qtpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/qtpy/brainglobe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/qtpy/collapsible_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/qtpy/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/qtpy/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/brainglobe_utils/qtpy/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:23:05.530220 brainglobe_utils-0.5.0/brainglobe_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-15 13:23:05.000000 brainglobe_utils-0.5.0/brainglobe_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-15 13:23:05.000000 brainglobe_utils-0.5.0/brainglobe_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:23:05.000000 brainglobe_utils-0.5.0/brainglobe_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 13:23:05.000000 brainglobe_utils-0.5.0/brainglobe_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 13:23:05.000000 brainglobe_utils-0.5.0/brainglobe_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 13:23:05.000000 brainglobe_utils-0.5.0/brainglobe_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-15 13:22:59.000000 brainglobe_utils-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:23:05.534220 brainglobe_utils-0.5.0/setup.cfg
```

### Comparing `brainglobe-utils-0.4.3/.github/workflows/test_and_deploy.yml` & `brainglobe_utils-0.5.0/.github/workflows/test_and_deploy.yml`

 * *Files 5% similar despite different names*

```diff
@@ -29,25 +29,26 @@
     strategy:
       matrix:
         # Run all supported Python versions on linux
         python-version: ["3.9", "3.10", "3.11"]
         os: [ubuntu-latest]
         # Include one windows and macos run
         include:
-        - os: macos-latest
+        - os: macos-13 # Intel Mac
+          python-version: "3.11"
+        - os: macos-latest # ARM Mac
           python-version: "3.11"
         - os: windows-latest
           python-version: "3.11"
 
     steps:
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
-
       # these libraries enable testing on Qt on linux
       - uses: pyvista/setup-headless-display-action@v2
         with:
           qt: true
       # Run tests
       - uses: neuroinformatics-unit/actions/test@v2
         with:
```

### Comparing `brainglobe-utils-0.4.3/.gitignore` & `brainglobe_utils-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/LICENSE` & `brainglobe_utils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/PKG-INFO` & `brainglobe_utils-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.4.3
+Version: 0.5.0
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT License
         
         Copyright (c) 2020 Adam Tyson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,15 @@
 License-File: LICENSE
 Requires-Dist: brainglobe-atlasapi>=2.0.1
 Requires-Dist: brainglobe-space
 Requires-Dist: configobj
 Requires-Dist: natsort
 Requires-Dist: nibabel>=2.1.0
 Requires-Dist: numpy
+Requires-Dist: dask
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: pyarrow
 Requires-Dist: pynrrd
 Requires-Dist: PyYAML
 Requires-Dist: scikit-image
 Requires-Dist: scipy
```

### Comparing `brainglobe-utils-0.4.3/README.md` & `brainglobe_utils-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/IO/cells.py` & `brainglobe_utils-0.5.0/brainglobe_utils/IO/cells.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/IO/surfaces.py` & `brainglobe_utils-0.5.0/brainglobe_utils/IO/surfaces.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/IO/yaml.py` & `brainglobe_utils-0.5.0/brainglobe_utils/IO/yaml.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/analysis.py` & `brainglobe_utils-0.5.0/brainglobe_utils/brainmapper/analysis.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/export.py` & `brainglobe_utils-0.5.0/brainglobe_utils/brainmapper/export.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/brainreg/transform.py` & `brainglobe_utils-0.5.0/brainglobe_utils/brainreg/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import brainglobe_space as bgs
 import numpy as np
 import pandas as pd
 import tifffile
 from brainglobe_atlasapi import BrainGlobeAtlas
 
-from brainglobe_utils.image_io import get_size_image_from_file_paths
+from brainglobe_utils.IO.image import get_size_image_from_file_paths
 
 
 def transform_points_from_downsampled_to_atlas_space(
     downsampled_points: np.ndarray,
     atlas: BrainGlobeAtlas,
     deformation_field_paths: List[os.PathLike],
     output_filename: Optional[os.PathLike] = None,
```

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/cells/cells.py` & `brainglobe_utils-0.5.0/brainglobe_utils/cells/cells.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/citation/bibtex_fmt.py` & `brainglobe_utils-0.5.0/brainglobe_utils/citation/bibtex_fmt.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/citation/cite.py` & `brainglobe_utils-0.5.0/brainglobe_utils/citation/cite.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/citation/fetch.py` & `brainglobe_utils-0.5.0/brainglobe_utils/citation/fetch.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/citation/format.py` & `brainglobe_utils-0.5.0/brainglobe_utils/citation/format.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/citation/repositories.py` & `brainglobe_utils-0.5.0/brainglobe_utils/citation/repositories.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/citation/text_fmt.py` & `brainglobe_utils-0.5.0/brainglobe_utils/citation/text_fmt.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/general/list.py` & `brainglobe_utils-0.5.0/brainglobe_utils/general/list.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/general/numerical.py` & `brainglobe_utils-0.5.0/brainglobe_utils/general/numerical.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/general/string.py` & `brainglobe_utils-0.5.0/brainglobe_utils/general/string.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/general/system.py` & `brainglobe_utils-0.5.0/brainglobe_utils/general/system.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/image/binning.py` & `brainglobe_utils-0.5.0/brainglobe_utils/image/binning.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/image/heatmap.py` & `brainglobe_utils-0.5.0/brainglobe_utils/image/heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from scipy.ndimage import zoom
 from skimage.filters import gaussian
 
 from brainglobe_utils.general.system import ensure_directory_exists
 from brainglobe_utils.image.binning import get_bins
 from brainglobe_utils.image.masking import mask_image_threshold
 from brainglobe_utils.image.scale import scale_and_convert_to_16_bits
-from brainglobe_utils.image_io import to_tiff
+from brainglobe_utils.IO.image import to_tiff
 
 
 def rescale_array(source_array, target_array, order=1):
     """
     Rescale a source array to the size of a target array.
 
     Parameters
```

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/image/masking.py` & `brainglobe_utils-0.5.0/brainglobe_utils/image/masking.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/image/scale.py` & `brainglobe_utils-0.5.0/brainglobe_utils/image/scale.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/image_io/load.py` & `brainglobe_utils-0.5.0/brainglobe_utils/IO/image/load.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+import glob
 import logging
 import math
+import os
 import warnings
 from concurrent.futures import ProcessPoolExecutor
 from pathlib import Path
+from typing import Tuple
 
 import nrrd
 import numpy as np
 import tifffile
+from dask import array as da
+from dask import delayed
 from natsort import natsorted
 from skimage import transform
 from tqdm import tqdm
 
 from brainglobe_utils.general.system import (
     get_num_processes,
     get_sorted_file_paths,
 )
-from brainglobe_utils.image_io.utils import ImageIOLoadException
+from brainglobe_utils.IO.image.utils import ImageIOLoadException
 
 from .utils import check_mem, scale_z
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import nibabel as nib
 
@@ -86,19 +91,19 @@
     -------
     np.ndarray
         The loaded brain.
 
     Raises
     ------
     ImageIOLoadException
-        If there was an issue loading the image with image_io.
+        If there was an issue loading the image with image.
 
     See Also
     ------
-    image_io.utils.ImageIOLoadException
+    image.utils.ImageIOLoadException
     """
     src_path = Path(src_path)
 
     if src_path.is_dir():
         logging.debug("Data type is: directory of files")
         img = load_from_folder(
             src_path,
@@ -661,37 +666,149 @@
             raise ImageIOLoadException("sequence_shape")
         volume[:, :, i] = img
     return volume
 
 
 def get_size_image_from_file_paths(file_path, file_extension="tif"):
     """
-    Returns the size of an image (which is a list of 2D tiff files),
-    without loading the whole image.
+    Returns the size of an image (which is a list of 2D tiff files or a
+    single-file tif stack), without loading the whole image.
 
     Parameters
     ----------
     file_path : str or pathlib.Path
-        Filepath of text file containing paths of all 2D files, or
-        filepath of a directory containing all 2D files.
+        Filepath of text file containing paths of all 2D files, a
+        filepath of a directory containing all 2D files, or a single
+        tiff file z-stack.
 
     file_extension : str, optional
         Optional file extension (if a directory is passed).
 
     Returns
     -------
     dict
         Dict of image sizes.
     """
     file_path = Path(file_path)
+    if file_path.suffix in [".tif", ".tiff"]:
+        # read just the metadata
+        with tifffile.TiffFile(file_path) as tiff:
+            if not len(tiff.series):
+                raise ValueError(
+                    f"Attempted to load {file_path} but didn't find a z-stack"
+                )
+            if len(tiff.series) != 1:
+                raise ValueError(
+                    f"Attempted to load {file_path} but found multiple stacks"
+                )
+
+            shape = tiff.series[0].shape
+            axes = tiff.series[0].axes.lower()
+
+            if len(shape) != 3:
+                raise ValueError(
+                    f"Attempted to load {file_path} but didn't find a "
+                    f"3-dimensional stack. Found {axes} axes "
+                    f"with shape {shape}"
+                )
+            # axes is e.g. "zxy"
+            if set(axes) == {"x", "y", "z"}:
+                image_shape = {ax: n for ax, n in zip(axes, shape)}
+                return image_shape
+            else:  # metadata does not specify axes as expected,
+                logging.debug(
+                    f"Axis metadata is {axes}, "
+                    "which is not the expected set of x,y,z in any order. "
+                    "Assume z,y,x"
+                )
+                image_shape = {
+                    ax: n
+                    for ax, n in zip(["z", "y", "x"], tiff.series[0].shape)
+                }
+                return image_shape
 
     img_paths = get_sorted_file_paths(file_path, file_extension=file_extension)
     z_shape = len(img_paths)
 
     logging.debug(
         "Loading file: {} to check raw image size" "".format(img_paths[0])
     )
     image_0 = tifffile.imread(img_paths[0])
     y_shape, x_shape = image_0.shape
 
     image_shape = {"x": x_shape, "y": y_shape, "z": z_shape}
     return image_shape
+
+
+def get_tiff_meta(
+    path: str,
+) -> Tuple[Tuple[int, int], np.dtype]:
+    with tifffile.TiffFile(path) as tfile:
+        nz = len(tfile.pages)
+        if not nz:
+            raise ValueError(f"tiff file {path} has no pages!")
+        first_page = tfile.pages[0]
+
+    return tfile.pages[0].shape, first_page.dtype
+
+
+lazy_imread = delayed(tifffile.imread)  # lazy reader
+
+
+def read_z_stack(path):
+    """
+    Reads z-stack, lazily, if possible.
+
+    If it's a text file or folder with 2D tiff files use dask to read lazily,
+    otherwise it's a single file tiff stack and is read into memory.
+
+    :param path: Filename of text file listing 2D tiffs, folder of 2D tiffs,
+        or single file tiff z-stack.
+    :return: The data as a dask/numpy array.
+    """
+    if path.endswith(".tiff") or path.endswith(".tif"):
+        with tifffile.TiffFile(path) as tiff:
+            if not len(tiff.series):
+                raise ValueError(
+                    f"Attempted to load {path} but couldn't read a z-stack"
+                )
+            if len(tiff.series) != 1:
+                raise ValueError(
+                    f"Attempted to load {path} but found multiple stacks"
+                )
+
+            axes = tiff.series[0].axes.lower()
+            if set(axes) != {"x", "y", "z"}:
+                # log that metadata does not specify expected axes
+                logging.debug(
+                    f"Axis metadata is {axes}, "
+                    "which is not the expected set of x,y,z in any order. "
+                    "Assume z,y,x"
+                )
+
+        return tifffile.imread(path)
+
+    return read_with_dask(path)
+
+
+def read_with_dask(path):
+    """
+    Based on https://github.com/tlambert03/napari-ndtiffs
+    :param path:
+    :return:
+    """
+    path = str(path)
+    if path.endswith(".txt"):
+        with open(path, "r") as f:
+            filenames = [line.rstrip() for line in f.readlines()]
+
+    else:
+        filenames = glob.glob(os.path.join(path, "*.tif"))
+
+    shape, dtype = get_tiff_meta(filenames[0])
+    lazy_arrays = [lazy_imread(fn) for fn in get_sorted_file_paths(filenames)]
+    dask_arrays = [
+        da.from_delayed(delayed_reader, shape=shape, dtype=dtype)
+        for delayed_reader in lazy_arrays
+    ]
+    stack = da.stack(dask_arrays, axis=0)
+    return stack
```

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/image_io/save.py` & `brainglobe_utils-0.5.0/brainglobe_utils/IO/image/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,20 @@
         The file path where to save the tiff stack.
 
     photometric: str
         Color space of image (to pass to tifffile.imwrite)
         Use 'minisblack' (default) for grayscale and 'rgb' for rgb
     """
     dest_path = Path(dest_path)
-    tifffile.imwrite(dest_path, img_volume, photometric=photometric)
+    tifffile.imwrite(
+        dest_path,
+        img_volume,
+        photometric=photometric,
+        metadata={"axes": "ZYX"},
+    )
 
 
 def to_tiffs(img_volume, path_prefix, path_suffix="", extension=".tif"):
     """
     Save the image volume (numpy array) as a sequence of tiff planes.
     Each plane will have a filepath of the following format:
     {path_prefix}_{zeroPaddedIndex}{path_suffix}{extension}
```

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/image_io/utils.py` & `brainglobe_utils-0.5.0/brainglobe_utils/IO/image/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import psutil
 from scipy.ndimage import zoom
 
 
 class ImageIOLoadException(Exception):
     """
     Custom exception class for errors found loading images with
-    image_io.load.
+    brainglobe_utils.IO.image.load
 
     Alerts the user of: loading a directory containing only a single .tiff,
     loading a single 2D .tiff, loading an image sequence where all 2D images
     don't have the same shape, lack of memory to complete loading.
 
     Set the error message to self.message to read during testing.
     """
@@ -41,17 +41,15 @@
             )
             if total_size is not None and free_mem is not None:
                 self.message += (
                     f" Needed {total_size}, only {free_mem} " f"available."
                 )
 
         else:
-            self.message = (
-                "File failed to load with brainglobe_utils.image_io."
-            )
+            self.message = "File failed to load with brainglobe_utils.image."
 
         super().__init__(self.message)
 
 
 def check_mem(img_byte_size, n_imgs):
     """
     Checks how much memory is available on the system and compares it to the
```

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/pandas/misc.py` & `brainglobe_utils-0.5.0/brainglobe_utils/pandas/misc.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/qtpy/brainglobe.png` & `brainglobe_utils-0.5.0/brainglobe_utils/qtpy/brainglobe.png`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/qtpy/collapsible_widget.py` & `brainglobe_utils-0.5.0/brainglobe_utils/qtpy/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/qtpy/dialog.py` & `brainglobe_utils-0.5.0/brainglobe_utils/qtpy/dialog.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/qtpy/interaction.py` & `brainglobe_utils-0.5.0/brainglobe_utils/qtpy/interaction.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils/qtpy/logo.py` & `brainglobe_utils-0.5.0/brainglobe_utils/qtpy/logo.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils.egg-info/PKG-INFO` & `brainglobe_utils-0.5.0/brainglobe_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.4.3
+Version: 0.5.0
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT License
         
         Copyright (c) 2020 Adam Tyson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,15 @@
 License-File: LICENSE
 Requires-Dist: brainglobe-atlasapi>=2.0.1
 Requires-Dist: brainglobe-space
 Requires-Dist: configobj
 Requires-Dist: natsort
 Requires-Dist: nibabel>=2.1.0
 Requires-Dist: numpy
+Requires-Dist: dask
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: pyarrow
 Requires-Dist: pynrrd
 Requires-Dist: PyYAML
 Requires-Dist: scikit-image
 Requires-Dist: scipy
```

### Comparing `brainglobe-utils-0.4.3/brainglobe_utils.egg-info/SOURCES.txt` & `brainglobe_utils-0.5.0/brainglobe_utils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 brainglobe_utils.egg-info/entry_points.txt
 brainglobe_utils.egg-info/requires.txt
 brainglobe_utils.egg-info/top_level.txt
 brainglobe_utils/IO/__init__.py
 brainglobe_utils/IO/cells.py
 brainglobe_utils/IO/surfaces.py
 brainglobe_utils/IO/yaml.py
+brainglobe_utils/IO/image/__init__.py
+brainglobe_utils/IO/image/load.py
+brainglobe_utils/IO/image/save.py
+brainglobe_utils/IO/image/utils.py
 brainglobe_utils/brainmapper/__init__.py
 brainglobe_utils/brainmapper/analysis.py
 brainglobe_utils/brainmapper/export.py
 brainglobe_utils/brainreg/__init__.py
 brainglobe_utils/brainreg/transform.py
 brainglobe_utils/cells/__init__.py
 brainglobe_utils/cells/cells.py
@@ -40,18 +44,14 @@
 brainglobe_utils/general/string.py
 brainglobe_utils/general/system.py
 brainglobe_utils/image/__init__.py
 brainglobe_utils/image/binning.py
 brainglobe_utils/image/heatmap.py
 brainglobe_utils/image/masking.py
 brainglobe_utils/image/scale.py
-brainglobe_utils/image_io/__init__.py
-brainglobe_utils/image_io/load.py
-brainglobe_utils/image_io/save.py
-brainglobe_utils/image_io/utils.py
 brainglobe_utils/pandas/__init__.py
 brainglobe_utils/pandas/misc.py
 brainglobe_utils/qtpy/__init__.py
 brainglobe_utils/qtpy/brainglobe.png
 brainglobe_utils/qtpy/collapsible_widget.py
 brainglobe_utils/qtpy/dialog.py
 brainglobe_utils/qtpy/interaction.py
```

### Comparing `brainglobe-utils-0.4.3/pyproject.toml` & `brainglobe_utils-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 dependencies = [
     "brainglobe-atlasapi >= 2.0.1",
     "brainglobe-space",
     "configobj",
     "natsort",
     "nibabel >= 2.1.0",
     "numpy",
+    "dask",
     "pandas",
     "psutil",
     "pyarrow",
     "pynrrd",
     "PyYAML",
     "scikit-image",
     "scipy",
```

