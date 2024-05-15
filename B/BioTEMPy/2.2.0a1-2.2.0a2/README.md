# Comparing `tmp/BioTEMPy-2.2.0a1.tar.gz` & `tmp/BioTEMPy-2.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BioTEMPy-2.2.0a1.tar", last modified: Mon Apr 15 13:10:10 2024, max compression
+gzip compressed data, was "dist/BioTEMPy-2.2.0a2.tar", last modified: Wed May 15 13:37:11 2024, max compression
```

## Comparing `BioTEMPy-2.2.0a1.tar` & `BioTEMPy-2.2.0a2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/BioTEMPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/BioTEMPy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1723 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/BioTEMPy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/BioTEMPy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      209 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/BioTEMPy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/BioTEMPy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/BioTEMPy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3329 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/
--rw-rw-rw-   0 root         (0) root         (0)       52 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/assembly/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/assembly/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    13073 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/assembly/assembly.py
--rw-rw-rw-   0 root         (0) root         (0)    46773 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/assembly/gamma.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14142 2024-04-15 12:35:53.000000 BioTEMPy-2.2.0a1/TEMPy/cli/arg_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    11044 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/cli/class_arg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/core/data/
--rw-rw-rw-   0 root         (0) root         (0)       82 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/core/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1778 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/core/data/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/core/errors/
--rw-rw-rw-   0 root         (0) root         (0)       86 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/core/errors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/core/errors/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/core/warn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/graphics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/graphics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20832 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/graphics/show_plot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/map_process/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/map_process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21815 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/map_process/map_filters.py
--rw-rw-rw-   0 root         (0) root         (0)    31367 2023-04-26 10:48:58.000000 BioTEMPy-2.2.0a1/TEMPy/map_process/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/maps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/maps/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    95871 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/maps/em_map.py
--rwxrwxrwx   0 root         (0) root         (0)    17392 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/maps/map_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4070 2022-11-18 16:17:02.000000 BioTEMPy-2.2.0a1/TEMPy/maps/map_transform_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29185 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/math/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)    25634 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/math/consensus.py
--rw-rw-rw-   0 root         (0) root         (0)    11869 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/math/fourier.py
--rw-rw-rw-   0 root         (0) root         (0)     5064 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/math/quaternion.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/math/transform_parser.py
--rwxrwxrwx   0 root         (0) root         (0)    16705 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/math/vector.py
--rwxrwxrwx   0 root         (0) root         (0)     4746 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/math/vq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/optimisation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/optimisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10371 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/optimisation/ensemble_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/protein/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/protein/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/protein/blur.py
--rw-rw-rw-   0 root         (0) root         (0)    12573 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/protein/density_calculator.py
--rw-rw-rw-   0 root         (0) root         (0)    14647 2023-04-26 14:26:52.000000 BioTEMPy-2.2.0a1/TEMPy/protein/mmcif.py
--rw-rw-rw-   0 root         (0) root         (0)    68320 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/protein/prot_rep_biopy.py
--rw-rw-rw-   0 root         (0) root         (0)    11687 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/protein/rigid_body_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/protein/scores/
--rw-rw-rw-   0 root         (0) root         (0)     1000 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/protein/scores/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6888 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/protein/scores/base_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    31507 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/protein/scores/glob.py
--rw-rw-rw-   0 root         (0) root         (0)    17213 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/protein/scores/local.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/protein/scores/segmented.py
--rw-rw-rw-   0 root         (0) root         (0)   145324 2024-04-15 12:35:53.000000 BioTEMPy-2.2.0a1/TEMPy/protein/scoring_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    54468 2024-03-25 16:02:14.000000 BioTEMPy-2.2.0a1/TEMPy/protein/structure_blurrer.py
--rw-rw-rw-   0 root         (0) root         (0)    19018 2024-03-26 11:36:45.000000 BioTEMPy-2.2.0a1/TEMPy/protein/structure_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/script/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 13:26:42.000000 BioTEMPy-2.2.0a1/TEMPy/script/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10663 2023-04-26 14:26:52.000000 BioTEMPy-2.2.0a1/TEMPy/script/gamma.py
--rw-rw-rw-   0 root         (0) root         (0)     5045 2023-04-26 14:26:52.000000 BioTEMPy-2.2.0a1/TEMPy/script/loqfit.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2023-04-26 14:26:52.000000 BioTEMPy-2.2.0a1/TEMPy/script/mi.py
--rw-rw-rw-   0 root         (0) root         (0)    11963 2023-04-26 14:26:52.000000 BioTEMPy-2.2.0a1/TEMPy/script/output.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-04-26 14:26:52.000000 BioTEMPy-2.2.0a1/TEMPy/script/sccc.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-15 12:35:53.000000 BioTEMPy-2.2.0a1/TEMPy/script/scores.py
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-04-26 14:26:52.000000 BioTEMPy-2.2.0a1/TEMPy/script/smoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/TEMPy/tempy_data/
--rw-rw-rw-   0 root         (0) root         (0)   523370 2022-07-12 12:03:45.000000 BioTEMPy-2.2.0a1/TEMPy/tempy_data/quaternion_vectors_5000.pk
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 13:10:10.000000 BioTEMPy-2.2.0a1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-04-15 12:46:52.000000 BioTEMPy-2.2.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/BioTEMPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/BioTEMPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1723 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/BioTEMPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/BioTEMPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      209 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/BioTEMPy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/BioTEMPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/BioTEMPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3329 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/assembly/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/assembly/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13073 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/assembly/assembly.py
+-rw-rw-rw-   0 root         (0) root         (0)    46773 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/assembly/gamma.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14142 2024-04-15 12:40:14.000000 BioTEMPy-2.2.0a2/TEMPy/cli/arg_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    11044 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/cli/class_arg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/core/data/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/core/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/core/data/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/core/errors/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/core/errors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/core/errors/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/core/warn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/graphics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/graphics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20832 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/graphics/show_plot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/map_process/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/map_process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21815 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/map_process/map_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    31367 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/map_process/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/maps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/maps/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    95871 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/maps/em_map.py
+-rwxrwxrwx   0 root         (0) root         (0)    17392 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/maps/map_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4070 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/maps/map_transform_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/math/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/math/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29185 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/math/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)    25634 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/math/consensus.py
+-rw-rw-rw-   0 root         (0) root         (0)    11869 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/math/fourier.py
+-rw-rw-rw-   0 root         (0) root         (0)     5064 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/math/quaternion.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/math/transform_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)    16705 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/math/vector.py
+-rwxrwxrwx   0 root         (0) root         (0)     4746 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/math/vq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/optimisation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/optimisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10371 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/optimisation/ensemble_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/protein/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/protein/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/blur.py
+-rw-rw-rw-   0 root         (0) root         (0)    12573 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/density_calculator.py
+-rw-rw-rw-   0 root         (0) root         (0)    14647 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/mmcif.py
+-rw-rw-rw-   0 root         (0) root         (0)    68320 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/prot_rep_biopy.py
+-rw-rw-rw-   0 root         (0) root         (0)    11687 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/rigid_body_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/protein/scores/
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/scores/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6888 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/scores/base_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    31507 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/scores/glob.py
+-rw-rw-rw-   0 root         (0) root         (0)    17213 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/scores/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/scores/segmented.py
+-rw-rw-rw-   0 root         (0) root         (0)   145324 2024-04-15 12:40:14.000000 BioTEMPy-2.2.0a2/TEMPy/protein/scoring_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    54468 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/structure_blurrer.py
+-rw-rw-rw-   0 root         (0) root         (0)    19018 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/protein/structure_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/script/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 13:36:58.000000 BioTEMPy-2.2.0a2/TEMPy/script/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10682 2024-05-15 13:34:17.000000 BioTEMPy-2.2.0a2/TEMPy/script/gamma.py
+-rw-rw-rw-   0 root         (0) root         (0)     5045 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/script/loqfit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/script/mi.py
+-rw-rw-rw-   0 root         (0) root         (0)    11963 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/script/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/script/sccc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-15 12:40:14.000000 BioTEMPy-2.2.0a2/TEMPy/script/scores.py
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/script/smoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/TEMPy/tempy_data/
+-rw-rw-rw-   0 root         (0) root         (0)   523370 2024-03-26 15:05:49.000000 BioTEMPy-2.2.0a2/TEMPy/tempy_data/quaternion_vectors_5000.pk
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 13:37:11.000000 BioTEMPy-2.2.0a2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-15 13:36:08.000000 BioTEMPy-2.2.0a2/setup.py
```

### Comparing `BioTEMPy-2.2.0a1/BioTEMPy.egg-info/SOURCES.txt` & `BioTEMPy-2.2.0a2/BioTEMPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/README.md` & `BioTEMPy-2.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/assembly/assembly.py` & `BioTEMPy-2.2.0a2/TEMPy/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/assembly/gamma.py` & `BioTEMPy-2.2.0a2/TEMPy/assembly/gamma.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/cli/arg_parser.py` & `BioTEMPy-2.2.0a2/TEMPy/cli/arg_parser.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/cli/class_arg.py` & `BioTEMPy-2.2.0a2/TEMPy/cli/class_arg.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/core/data/download.py` & `BioTEMPy-2.2.0a2/TEMPy/core/data/download.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/core/warn.py` & `BioTEMPy-2.2.0a2/TEMPy/core/warn.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/graphics/show_plot.py` & `BioTEMPy-2.2.0a2/TEMPy/graphics/show_plot.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/map_process/map_filters.py` & `BioTEMPy-2.2.0a2/TEMPy/map_process/map_filters.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/map_process/process.py` & `BioTEMPy-2.2.0a2/TEMPy/map_process/process.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/maps/em_map.py` & `BioTEMPy-2.2.0a2/TEMPy/maps/em_map.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/maps/map_parser.py` & `BioTEMPy-2.2.0a2/TEMPy/maps/map_parser.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/maps/map_transform_score.py` & `BioTEMPy-2.2.0a2/TEMPy/maps/map_transform_score.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/math/cluster.py` & `BioTEMPy-2.2.0a2/TEMPy/math/cluster.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/math/consensus.py` & `BioTEMPy-2.2.0a2/TEMPy/math/consensus.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/math/fourier.py` & `BioTEMPy-2.2.0a2/TEMPy/math/fourier.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/math/quaternion.py` & `BioTEMPy-2.2.0a2/TEMPy/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/math/transform_parser.py` & `BioTEMPy-2.2.0a2/TEMPy/math/transform_parser.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/math/vector.py` & `BioTEMPy-2.2.0a2/TEMPy/math/vector.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/math/vq.py` & `BioTEMPy-2.2.0a2/TEMPy/math/vq.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/optimisation/ensemble_generation.py` & `BioTEMPy-2.2.0a2/TEMPy/optimisation/ensemble_generation.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/blur.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/blur.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/density_calculator.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/density_calculator.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/mmcif.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/mmcif.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/prot_rep_biopy.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/prot_rep_biopy.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/rigid_body_parser.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/rigid_body_parser.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/scores/__init__.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/scores/__init__.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/scores/base_classes.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/scores/base_classes.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/scores/glob.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/scores/glob.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/scores/local.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/scores/local.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/scores/segmented.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/scores/segmented.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/scoring_functions.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/scoring_functions.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/structure_blurrer.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/structure_blurrer.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/protein/structure_parser.py` & `BioTEMPy-2.2.0a2/TEMPy/protein/structure_parser.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/script/gamma.py` & `BioTEMPy-2.2.0a2/TEMPy/script/gamma.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         "the VQ point distances). This is a advanced setting "
         "for expert user",
     )
 
     return parser.parser
 
 
-if __name__ == "__main__":
+def main():
     args = get_parser().parse_args()
 
     prot = args.model
     nchains = prot.no_of_chains()
 
     emmap = args.map
     emmap.normalise()
@@ -292,15 +292,15 @@
         f.write("Map vector quantisation file  : " + output_filename + "_vq.pdb" + "\n")
     else:
         f.write("Map vector quantisation file  : " + args.seed_file + "\n")
     f.close()
 
     print("Starting gamma tempy run...")
     # Run GA assembly fitting
-    results = ga.run(
+    _ = ga.run(
         grun,
         ngen,
         total_popsize,
         selection_method,
         gof,
         w_gof,
         w_clash,
@@ -321,7 +321,11 @@
     f.write(
         "------------------------------------------------------------------------------------------\n"
     )
     f.write("Execution time (sec): " + str(time.time() - start_time) + "\n")
     f.close()
     print("Finished gamma tempy run!")
     exit(0)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `BioTEMPy-2.2.0a1/TEMPy/script/loqfit.py` & `BioTEMPy-2.2.0a2/TEMPy/script/loqfit.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/script/mi.py` & `BioTEMPy-2.2.0a2/TEMPy/script/mi.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/script/output.py` & `BioTEMPy-2.2.0a2/TEMPy/script/output.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/script/sccc.py` & `BioTEMPy-2.2.0a2/TEMPy/script/sccc.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/script/scores.py` & `BioTEMPy-2.2.0a2/TEMPy/script/scores.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/script/smoc.py` & `BioTEMPy-2.2.0a2/TEMPy/script/smoc.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/TEMPy/tempy_data/quaternion_vectors_5000.pk` & `BioTEMPy-2.2.0a2/TEMPy/tempy_data/quaternion_vectors_5000.pk`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.2.0a1/setup.py` & `BioTEMPy-2.2.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 if os.path.exists('build') is True:
     print('build exists')
     shutil.rmtree('./build')
 
 setup(
     name='BioTEMPy',
-    version='2.2.0a1',
+    version='2.2.0a2',
     author='Maya Topf, Daven Vasishtan, Arun Prasad Pandurangan, Irene Farabella, Agnel-Praveen Joseph, Harpal Sahota',
     author_email='tempy-help@cryst.bbk.ac.uk',
     packages=setuptools.find_packages(),
     url='http://tempy.ismb.lon.ac.uk/',
     description='TEMPy: a Python Library for Assessment of 3D Electron Microscopy Density Fits',
     package_dir={'TEMPy': 'TEMPy'},
     python_requires='>=3.7',
```

