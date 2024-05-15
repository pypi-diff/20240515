# Comparing `tmp/basil_core-0.3.0.tar.gz` & `tmp/basil_core-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basil_core-0.3.0.tar", last modified: Fri Jan  5 17:52:18 2024, max compression
+gzip compressed data, was "basil_core-0.3.2.tar", last modified: Wed May 15 16:44:58 2024, max compression
```

## Comparing `basil_core-0.3.0.tar` & `basil_core-0.3.2.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.973860 basil_core-0.3.0/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      602 2024-01-05 17:51:45.000000 basil_core-0.3.0/MANIFEST.in
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1061 2024-01-05 17:52:18.973556 basil_core-0.3.0/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1321 2023-03-06 22:29:34.000000 basil_core-0.3.0/README.md
--rw-r--r--   0 vdelfave (669582709) staff       (20)      107 2023-08-16 18:47:21.000000 basil_core-0.3.0/REQUIREMENTS.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)       20 2024-01-05 17:52:11.000000 basil_core-0.3.0/__version__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      166 2023-08-16 18:47:25.000000 basil_core-0.3.0/pyproject.toml
--rw-r--r--   0 vdelfave (669582709) staff       (20)       38 2024-01-05 17:52:18.973915 basil_core-0.3.0/setup.cfg
--rw-r--r--   0 vdelfave (669582709) staff       (20)     8046 2024-01-05 13:56:37.000000 basil_core-0.3.0/setup.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.923998 basil_core-0.3.0/src/
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.937512 basil_core-0.3.0/src/basil_core/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2023-03-02 18:49:51.000000 basil_core-0.3.0/src/basil_core/__init__.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.940956 basil_core-0.3.0/src/basil_core/array_tools/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       45 2024-01-05 13:47:21.000000 basil_core-0.3.0/src/basil_core/array_tools/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    20457 2024-01-05 17:39:11.000000 basil_core-0.3.0/src/basil_core/array_tools/_indexer.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2812 2024-01-05 17:51:27.000000 basil_core-0.3.0/src/basil_core/array_tools/indexer.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.941371 basil_core-0.3.0/src/basil_core/astro/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2023-03-05 17:15:29.000000 basil_core-0.3.0/src/basil_core/astro/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      269 2023-03-07 01:24:09.000000 basil_core-0.3.0/src/basil_core/astro/_basil_core_astro_const.h
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.943683 basil_core-0.3.0/src/basil_core/astro/coordinates/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       27 2022-10-17 15:31:15.000000 basil_core-0.3.0/src/basil_core/astro/coordinates/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    32592 2023-03-16 17:05:49.000000 basil_core-0.3.0/src/basil_core/astro/coordinates/_coordinates.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    27272 2023-03-16 17:05:49.000000 basil_core-0.3.0/src/basil_core/astro/coordinates/_spin.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    27645 2023-03-16 17:05:49.000000 basil_core-0.3.0/src/basil_core/astro/coordinates/_tides.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    15423 2023-03-02 18:52:16.000000 basil_core-0.3.0/src/basil_core/astro/coordinates/coordinates.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.945407 basil_core-0.3.0/src/basil_core/astro/orbit/
--rw-r--r--   0 vdelfave (669582709) staff       (20)    12168 2023-03-16 17:05:49.000000 basil_core-0.3.0/src/basil_core/astro/orbit/_DWD_RLOF.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    19237 2023-03-16 17:05:49.000000 basil_core-0.3.0/src/basil_core/astro/orbit/_GW.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)       21 2023-03-06 21:58:48.000000 basil_core-0.3.0/src/basil_core/astro/orbit/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4823 2023-03-16 17:05:49.000000 basil_core-0.3.0/src/basil_core/astro/orbit/_kepler.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    15606 2023-03-06 23:32:16.000000 basil_core-0.3.0/src/basil_core/astro/orbit/orbit.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.957933 basil_core-0.3.0/src/basil_core/astro/priors/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2023-05-16 14:57:11.000000 basil_core-0.3.0/src/basil_core/astro/priors/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    12628 2023-05-16 18:57:25.000000 basil_core-0.3.0/src/basil_core/astro/priors/callister_priors.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.958419 basil_core-0.3.0/src/basil_core/c_utils/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1236 2023-01-30 17:47:08.000000 basil_core-0.3.0/src/basil_core/c_utils/dbg.h
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.960042 basil_core-0.3.0/src/basil_core/plots/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2023-08-11 00:12:48.000000 basil_core-0.3.0/src/basil_core/plots/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    12670 2023-08-13 23:27:49.000000 basil_core-0.3.0/src/basil_core/plots/axis.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    27113 2023-09-27 21:38:19.000000 basil_core-0.3.0/src/basil_core/plots/corner.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1905 2023-08-11 02:08:10.000000 basil_core-0.3.0/src/basil_core/plots/utils.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.962526 basil_core-0.3.0/src/basil_core/stats/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       24 2023-03-02 20:57:03.000000 basil_core-0.3.0/src/basil_core/stats/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     7284 2023-03-16 17:05:49.000000 basil_core-0.3.0/src/basil_core/stats/_distance.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11703 2023-03-16 17:05:49.000000 basil_core-0.3.0/src/basil_core/stats/_relative_entropy.c
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.963626 basil_core-0.3.0/src/basil_core/stats/density/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2023-07-29 12:59:43.000000 basil_core-0.3.0/src/basil_core/stats/density/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3099 2023-08-11 13:07:17.000000 basil_core-0.3.0/src/basil_core/stats/density/density_utils.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    37149 2023-09-27 19:01:34.000000 basil_core-0.3.0/src/basil_core/stats/density/histogram_overhang.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     9168 2023-08-20 22:09:56.000000 basil_core-0.3.0/src/basil_core/stats/distance.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1283 2023-07-30 13:55:33.000000 basil_core-0.3.0/src/basil_core/stats/hypercube.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1921 2023-03-21 14:23:25.000000 basil_core-0.3.0/src/basil_core/stats/random.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.973156 basil_core-0.3.0/src/basil_core.egg-info/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1061 2024-01-05 17:52:18.000000 basil_core-0.3.0/src/basil_core.egg-info/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1700 2024-01-05 17:52:18.000000 basil_core-0.3.0/src/basil_core.egg-info/SOURCES.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2024-01-05 17:52:18.000000 basil_core-0.3.0/src/basil_core.egg-info/dependency_links.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)      122 2024-01-05 17:52:18.000000 basil_core-0.3.0/src/basil_core.egg-info/requires.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)       11 2024-01-05 17:52:18.000000 basil_core-0.3.0/src/basil_core.egg-info/top_level.txt
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-01-05 17:52:18.972713 basil_core-0.3.0/tests/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     6642 2023-05-16 18:50:35.000000 basil_core-0.3.0/tests/test_callister_priors.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    26159 2023-10-23 22:43:15.000000 basil_core-0.3.0/tests/test_coordinates.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3385 2023-08-11 17:08:55.000000 basil_core-0.3.0/tests/test_corner.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    15248 2023-03-21 15:21:16.000000 basil_core-0.3.0/tests/test_distance.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11746 2023-08-12 00:22:40.000000 basil_core-0.3.0/tests/test_histogram_overhang.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1217 2023-03-20 19:34:43.000000 basil_core-0.3.0/tests/test_hypercube.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4215 2024-01-05 17:51:23.000000 basil_core-0.3.0/tests/test_indexer.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     9698 2023-03-07 01:36:11.000000 basil_core-0.3.0/tests/test_orbit.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2842 2023-03-21 14:49:44.000000 basil_core-0.3.0/tests/test_random.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.131539 basil_core-0.3.2/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      644 2024-05-15 16:11:29.000000 basil_core-0.3.2/MANIFEST.in
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1061 2024-05-15 16:44:58.131217 basil_core-0.3.2/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1321 2023-03-06 22:29:34.000000 basil_core-0.3.2/README.md
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      107 2023-08-16 18:47:21.000000 basil_core-0.3.2/REQUIREMENTS.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       22 2024-05-15 16:44:48.000000 basil_core-0.3.2/__version__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      166 2023-08-16 18:47:25.000000 basil_core-0.3.2/pyproject.toml
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       38 2024-05-15 16:44:58.131605 basil_core-0.3.2/setup.cfg
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     8324 2024-05-15 14:41:49.000000 basil_core-0.3.2/setup.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.078684 basil_core-0.3.2/src/
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.100112 basil_core-0.3.2/src/basil_core/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       47 2024-05-15 14:42:44.000000 basil_core-0.3.2/src/basil_core/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       22 2024-05-15 16:44:48.000000 basil_core-0.3.2/src/basil_core/__version__.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.108695 basil_core-0.3.2/src/basil_core/array_tools/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       45 2024-01-05 13:47:21.000000 basil_core-0.3.2/src/basil_core/array_tools/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    20457 2024-01-05 17:39:11.000000 basil_core-0.3.2/src/basil_core/array_tools/_indexer.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2812 2024-01-05 17:51:27.000000 basil_core-0.3.2/src/basil_core/array_tools/indexer.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.109452 basil_core-0.3.2/src/basil_core/astro/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2023-03-05 17:15:29.000000 basil_core-0.3.2/src/basil_core/astro/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      269 2023-03-07 01:24:09.000000 basil_core-0.3.2/src/basil_core/astro/_basil_core_astro_const.h
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.112219 basil_core-0.3.2/src/basil_core/astro/coordinates/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       27 2022-10-17 15:31:15.000000 basil_core-0.3.2/src/basil_core/astro/coordinates/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    32592 2023-03-16 17:05:49.000000 basil_core-0.3.2/src/basil_core/astro/coordinates/_coordinates.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    27272 2023-03-16 17:05:49.000000 basil_core-0.3.2/src/basil_core/astro/coordinates/_spin.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    27645 2023-03-16 17:05:49.000000 basil_core-0.3.2/src/basil_core/astro/coordinates/_tides.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    15423 2023-03-02 18:52:16.000000 basil_core-0.3.2/src/basil_core/astro/coordinates/coordinates.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.115501 basil_core-0.3.2/src/basil_core/astro/orbit/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    12168 2023-03-16 17:05:49.000000 basil_core-0.3.2/src/basil_core/astro/orbit/_DWD_RLOF.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    19237 2023-03-16 17:05:49.000000 basil_core-0.3.2/src/basil_core/astro/orbit/_GW.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       21 2023-03-06 21:58:48.000000 basil_core-0.3.2/src/basil_core/astro/orbit/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4823 2023-03-16 17:05:49.000000 basil_core-0.3.2/src/basil_core/astro/orbit/_kepler.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    15606 2023-03-06 23:32:16.000000 basil_core-0.3.2/src/basil_core/astro/orbit/orbit.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.117958 basil_core-0.3.2/src/basil_core/astro/priors/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2023-05-16 14:57:11.000000 basil_core-0.3.2/src/basil_core/astro/priors/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    12628 2023-05-16 18:57:25.000000 basil_core-0.3.2/src/basil_core/astro/priors/callister_priors.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.118619 basil_core-0.3.2/src/basil_core/c_utils/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1236 2023-01-30 17:47:08.000000 basil_core-0.3.2/src/basil_core/c_utils/dbg.h
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.120123 basil_core-0.3.2/src/basil_core/plots/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2023-08-11 00:12:48.000000 basil_core-0.3.2/src/basil_core/plots/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13985 2024-02-25 17:33:08.000000 basil_core-0.3.2/src/basil_core/plots/axis.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    31452 2024-02-25 17:33:08.000000 basil_core-0.3.2/src/basil_core/plots/corner.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1905 2023-08-11 02:08:10.000000 basil_core-0.3.2/src/basil_core/plots/utils.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.123792 basil_core-0.3.2/src/basil_core/stats/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       57 2024-05-15 16:11:08.000000 basil_core-0.3.2/src/basil_core/stats/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     7284 2023-03-16 17:05:49.000000 basil_core-0.3.2/src/basil_core/stats/_distance.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11703 2023-03-16 17:05:49.000000 basil_core-0.3.2/src/basil_core/stats/_relative_entropy.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     9041 2024-05-15 16:31:30.000000 basil_core-0.3.2/src/basil_core/stats/_schechter.c
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.125115 basil_core-0.3.2/src/basil_core/stats/density/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2023-07-29 12:59:43.000000 basil_core-0.3.2/src/basil_core/stats/density/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3099 2023-08-11 13:07:17.000000 basil_core-0.3.2/src/basil_core/stats/density/density_utils.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    37149 2023-09-27 19:01:34.000000 basil_core-0.3.2/src/basil_core/stats/density/histogram_overhang.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     9168 2023-08-20 22:09:56.000000 basil_core-0.3.2/src/basil_core/stats/distance.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1283 2023-07-30 13:55:33.000000 basil_core-0.3.2/src/basil_core/stats/hypercube.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1921 2023-03-21 14:23:25.000000 basil_core-0.3.2/src/basil_core/stats/random.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3336 2024-05-15 16:29:48.000000 basil_core-0.3.2/src/basil_core/stats/schechter.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.130834 basil_core-0.3.2/src/basil_core.egg-info/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1061 2024-05-15 16:44:58.000000 basil_core-0.3.2/src/basil_core.egg-info/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1822 2024-05-15 16:44:58.000000 basil_core-0.3.2/src/basil_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2024-05-15 16:44:58.000000 basil_core-0.3.2/src/basil_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      122 2024-05-15 16:44:58.000000 basil_core-0.3.2/src/basil_core.egg-info/requires.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       11 2024-05-15 16:44:58.000000 basil_core-0.3.2/src/basil_core.egg-info/top_level.txt
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-05-15 16:44:58.130390 basil_core-0.3.2/tests/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     6642 2023-05-16 18:50:35.000000 basil_core-0.3.2/tests/test_callister_priors.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    26159 2023-10-23 22:43:15.000000 basil_core-0.3.2/tests/test_coordinates.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3580 2024-02-25 17:33:08.000000 basil_core-0.3.2/tests/test_corner.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    15248 2023-03-21 15:21:16.000000 basil_core-0.3.2/tests/test_distance.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11746 2023-08-12 00:22:40.000000 basil_core-0.3.2/tests/test_histogram_overhang.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1217 2023-03-20 19:34:43.000000 basil_core-0.3.2/tests/test_hypercube.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4215 2024-01-05 17:51:23.000000 basil_core-0.3.2/tests/test_indexer.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     9698 2023-03-07 01:36:11.000000 basil_core-0.3.2/tests/test_orbit.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2842 2023-03-21 14:49:44.000000 basil_core-0.3.2/tests/test_random.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     6473 2024-05-15 16:44:05.000000 basil_core-0.3.2/tests/test_schechter.py
```

### Comparing `basil_core-0.3.0/MANIFEST.in` & `basil_core-0.3.2/MANIFEST.in`

 * *Files 22% similar despite different names*

```diff
@@ -4,12 +4,13 @@
 include README.md
 include src/basil_core/array_tools/_indexer.c
 include src/basil_core/astro/coordinates/_coordinates.c
 include src/basil_core/astro/coordinates/_tides.c
 include src/basil_core/astro/coordinates/_spin.c
 include src/basil_core/stats/_distance.c
 include src/basil_core/stats/_relative_entropy.c
+include src/basil_core/stats/_schechter.c
 include src/basil_core/astro/orbit/_GW.c
 include src/basil_core/astro/orbit/_DWD_RLOF.c
 include src/basil_core/astro/orbit/_kepler.c
 include src/basil_core/astro/_basil_core_astro_const.h
 include src/basil_core/c_utils/dbg.h
```

### Comparing `basil_core-0.3.0/PKG-INFO` & `basil_core-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basil_core
-Version: 0.3.0
+Version: 0.3.2
 Summary: basil_core for postprocessing and inference with core simulations
 Home-page: https://gitlab.com/xevra/basil-core
 Author: Vera Delfavero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Delfavero
 Maintainer-email: xevra86@gmail.com
 License: MIT License
```

### Comparing `basil_core-0.3.0/README.md` & `basil_core-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/setup.py` & `basil_core-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 #-------------------------------------------------------------------------------
 #   Version
 #-------------------------------------------------------------------------------
 VERSIONFILE="__version__.py"
 with open(VERSIONFILE, 'r') as F:
     _line = F.read()
-__version__  = _line.split("=")[-1].lstrip(" ").rstrip(" ")
+__version__  = _line.split("=")[-1].lstrip(" '").rstrip(" '\n")
 
 #-------------------------------------------------------------------------------
 #   GENERAL
 #-------------------------------------------------------------------------------
 __name__        = "basil_core"
-__date__        = date(2024, 1, 5)
+__date__        = date(2024, 5, 15)
 __keywords__    = [
     "astronomy",
     "information analysis",
     "machine learning",
     "physics",
 ]
 __status__      = "Alpha"
@@ -140,14 +140,19 @@
                          include_dirs = INCLUDE,
                         ),
                Extension("basil_core.array_tools._indexer",
                          sources = [os.path.join("src","basil_core","array_tools", "_indexer.c")],
                          py_limited_api=True,
                          include_dirs = INCLUDE,
                         ),
+               Extension("basil_core.stats._schechter",
+                         sources = [os.path.join("src","basil_core","stats", "_schechter.c")],
+                         py_limited_api=True,
+                         include_dirs = INCLUDE,
+                        ),
               ]
 #PACKAGE_DATA = {
 #    "": [],
 #}
 
 DOCLINES = __doc__.split("\n")
```

### Comparing `basil_core-0.3.0/src/basil_core/array_tools/_indexer.c` & `basil_core-0.3.2/src/basil_core/array_tools/_indexer.c`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/array_tools/indexer.py` & `basil_core-0.3.2/src/basil_core/array_tools/indexer.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/astro/coordinates/_coordinates.c` & `basil_core-0.3.2/src/basil_core/astro/coordinates/_coordinates.c`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/astro/coordinates/_spin.c` & `basil_core-0.3.2/src/basil_core/astro/coordinates/_spin.c`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/astro/coordinates/_tides.c` & `basil_core-0.3.2/src/basil_core/astro/coordinates/_tides.c`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/astro/coordinates/coordinates.py` & `basil_core-0.3.2/src/basil_core/astro/coordinates/coordinates.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/astro/orbit/_DWD_RLOF.c` & `basil_core-0.3.2/src/basil_core/astro/orbit/_DWD_RLOF.c`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/astro/orbit/_GW.c` & `basil_core-0.3.2/src/basil_core/astro/orbit/_GW.c`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/astro/orbit/_kepler.c` & `basil_core-0.3.2/src/basil_core/astro/orbit/_kepler.c`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/astro/orbit/orbit.py` & `basil_core-0.3.2/src/basil_core/astro/orbit/orbit.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/astro/priors/callister_priors.py` & `basil_core-0.3.2/src/basil_core/astro/priors/callister_priors.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/c_utils/dbg.h` & `basil_core-0.3.2/src/basil_core/c_utils/dbg.h`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/plots/axis.py` & `basil_core-0.3.2/src/basil_core/plots/axis.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     # Show data
     im = ax.imshow(
                    rho.T,
                    extent = [limits[0,0], limits[0,1], limits[1,0], limits[1,1]],
                    origin='lower',
                    aspect = 'auto',
                    cmap = cmap,
+                   zorder=0,
                   )
 
     if set_limits:
         ax.set_xlim(limits[0])
         ax.set_ylim(limits[1])
     return im
 
@@ -147,14 +148,15 @@
     ct = ax.contour(
                     xgrid,
                     ygrid,
                     rho.T,
                     levels=percentiles,
                     extent = [limits[0,0], limits[0,1], limits[1,0], limits[1,1]],
                     origin='lower',
+                    aspect = 'auto',
                     vmin=0.,
                     vmax=np.max(rho),
                     cmap = cmap,
                     **kwargs
                     )
 
     # Set limits
@@ -245,18 +247,20 @@
     # Show data
     ct = ax.contour(
                     xgrid,
                     ygrid,
                     rho,
                     levels=percentiles,
                     extent = [limits[0,0], limits[0,1], limits[1,0], limits[1,1]],
+                    aspect = 'auto',
                     origin='lower',
                     cmap = cmap,
                     vmin=0.,
                     vmax=np.max(rho),
+                    zorder=0,
                     **kwargs
                     )
 
     # Set limits
     if set_limits:
         ax.set_xlim(limits[0])
         ax.set_ylim(limits[1])
@@ -319,14 +323,15 @@
                    extent = [limits[0,0], limits[0,1], limits[1,0], limits[1,1]],
                    origin='lower',
                    aspect = 'auto',
                    cmap = cmap,
                    norm=colornorm,
                    vmin = vmin,
                    vmax = np.max(rho),
+                   zorder=0,
                    **kwargs
                   )
 
     # Set limits
     if set_limits:
         ax.set_xlim(limits[0])
         ax.set_ylim(limits[1])
@@ -400,38 +405,40 @@
     # Show data
     ct = ax.contour(
                     x,
                     y,
                     z,
                     levels=percentiles,
                     extent = [limits[0,0], limits[0,1], limits[1,0], limits[1,1]],
+                    aspect = 'auto',
                     origin='lower',
                     cmap = cmap,
                     vmin=0.,
                     vmax=np.max(z),
+                    zorder=0,
                     **kwargs
                     )
 
     # Set limits
     if set_limits:
         ax.set_xlim(limits[0])
         ax.set_ylim(limits[1])
     return ct
 
-def ax_scatter2d(
-                 ax,
-                 x, y, z,
-                 limits=None,
-                 set_limits=False,
-                 cmap="terrain_r",
-                 density=False,
-                 log_scale=False,
-                 log_offset=0.,
-                 **kwargs
-                ):
+def ax_scatter2d_density(
+                         ax,
+                         x, y, z,
+                         limits=None,
+                         set_limits=False,
+                         cmap="terrain_r",
+                         density=False,
+                         log_scale=False,
+                         log_offset=0.,
+                         **kwargs
+                        ):
     '''Quickly make some contours using histograms'''
     import numpy as np
     # Update limits
     if limits is None:
         limits = np.asarray([[np.min(x), np.max(x)],[np.min(y), np.max(y)]])
 
     # log scale
@@ -462,7 +469,43 @@
 
     # Set limits
     if set_limits:
         ax.set_xlim(limits[0])
         ax.set_ylim(limits[1])
     return im
 
+def ax_scatter2d_error(
+                       ax,
+                       x, y,
+                       dx,dy,
+                       limits=None,
+                       set_limits=False,
+                       ecolor=None,
+                       elinewidth=None,
+                       **kwargs
+                      ):
+    '''Quickly make some contours using histograms'''
+    import numpy as np
+    # Update limits
+    if limits is None:
+        limits = np.asarray([[np.min(x), np.max(x)],[np.min(y), np.max(y)]])
+
+    # Show data
+    ax.scatter(
+               x,y,
+               **kwargs
+              )
+    if (not ecolor is None) and (not elinewidth is None):
+        # Show error bars
+        ax.errorbar(
+                    x,y,
+                    dy,dx,
+                    fmt='none',
+                    ecolor=ecolor,
+                    elinewidth=elinewidth,
+                   )
+
+    # Set limits
+    if set_limits:
+        ax.set_xlim(limits[0])
+        ax.set_ylim(limits[1])
+
```

### Comparing `basil_core-0.3.0/src/basil_core/plots/corner.py` & `basil_core-0.3.2/src/basil_core/plots/corner.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ######## Imports ########
 import numpy as np
 
 from basil_core.plots.axis import ax_histogram1d, ax_histogram2d
 from basil_core.plots.axis import ax_histogram_contour2d
 from basil_core.plots.axis import ax_function1d, ax_function2d
 from basil_core.plots.axis import ax_function_contour2d
-from basil_core.plots.axis import ax_plot1d, ax_scatter2d, ax_scatter_contour2d
+from basil_core.plots.axis import ax_plot1d, ax_scatter2d_density, ax_scatter_contour2d, ax_scatter2d_error
 
 
 ######## Information ########
 
 EXTENSIONS = ["png", "pdf"]
 
 ######## Corner object ########
@@ -32,14 +32,15 @@
                  fontscale=1.,
                  style='bmh',
                  log_scale=True,
                  density=True,
                  legend_loc=1,
                  title=None,
                  log_offset=0.,
+                 diag_ticklabels=False,
                 ):
         '''Initialize corner plot config
 
         Parameters
         ----------
         ndim: int
             Number of dimensions for corner plot
@@ -59,16 +60,17 @@
             Log offset for colors of imshow
         density: bool
             Normalize everything under integration?
         legend_loc: matplotlib legend loc
             Location for a legend, if present
         title: string
             Title for fgure
-
-
+        diag_ticklabels: bool
+            Show diagonal ticklabels?
+ 
         Returns
         -------
         self: Corner object
             The corner plot configuration object
         '''
         # Assign ndim
         assert isinstance(ndim, int)
@@ -89,19 +91,19 @@
         if labels is None:
             self.labels = None
         else:
             assert len(labels) == ndim
             self.labels = labels
 
         # Check size
-        assert isinstance(figsize, float)
+        assert (isinstance(figsize, float)) or (isinstance(figsize, int))
         self.figsize = figsize
 
         # Assign fontscale
-        assert isinstance(fontscale, float)
+        assert (isinstance(fontscale, float)) or (isinstance(fontscale, int))
         self.fontscale = (self.figsize / 3.375) * fontscale
 
         # Assign log_scale
         self.log_scale = log_scale
         self.log_offset = log_offset
 
         # Assign density
@@ -109,18 +111,23 @@
 
         # Assign style
         self.style = style
 
         # Assign title
         self.title = title
 
+        # Assign diag ticklabels
+        self.diag_ticklabels = diag_ticklabels
+
         # Initialize histogram layers
         self.histogram_layers = []
         # Initialize HOGPEN layers
         self.HOGPEN_layers = []
+        # Initialize scatter2d layers
+        self.scatter2d_layers = []
 
         # Initialize colorbar
         self._colorbar = None
         # Initialize legend toggle
         self._legend = False
         self.legend_loc = legend_loc
 
@@ -180,22 +187,76 @@
                  "npts"     : npts,
                  "data"     : data,
                  "bins"     : bins,
                  "label"    : label,
                  "cmap"     : cmap,
                  "imshow"   : imshow,
                  "contour"  : contour,
-                 "colorbar" : colorbar,
                  "weights"  : weights,
                  "levels"   : levels,
                  "linestyle": linestyle,
                 }
         # Append layer to histogram layers
         self.histogram_layers.append(layer)
 
+    def add_scatter2d_layer(
+                            self,
+                            data,
+                            sig,
+                            label=None,
+                            s=10.,
+                            color='black',
+                            marker='d',
+                            ecolor='black',
+                            elinewidth=0.5,
+                           ):
+        '''Add a scatter 2d layer to the corner plot
+
+        Parameters
+        ----------
+        data: array like, shape=(npts, ndim)
+            Samples for histograming
+        label: str
+            label for legend
+        s: float
+            Maker size
+        color: str
+            matplotlib color choices
+        elinewidth: float
+            error bar line width
+        ecolor: str
+            erorr bar color
+        '''
+        # Check the data
+        assert len(data.shape) == 2
+        assert data.shape[1] == self.ndim
+        npts = data.shape[0]
+        # Check sig
+        if np.asarray(sig).size == self.ndim:
+            sig = np.tile(sig, (npts,1))
+        else:
+            assert np.asarray(sig).shape[0] == npts
+            assert np.asarray(sig).shape[1] == self.ndim
+        # Check s
+        s = s * self.fontscale
+        # Define layer dictionary
+        layer = {
+                 "npts"         : npts,
+                 "data"         : data,
+                 "sig"          : sig,
+                 "label"        : label,
+                 's'            : s,
+                 "color"        : color,
+                 "marker"       : marker,
+                 "ecolor"       : ecolor,
+                 "elinewidth"   : elinewidth,
+                }
+        # Append layer to histogram layers
+        self.scatter2d_layers.append(layer)
+
     def add_HOGPEN_layer(
                          self,
                          marginals,
                          res=100,
                          label=None,
                          cmap="terrain_r",
                          imshow=False,
@@ -367,15 +428,18 @@
             The axes for the plot
         '''
         # Loop the dimensions
         for i in range(self.ndim):
             # Update the tick params
             axes[i,i].tick_params(axis="both", which="both", labelsize=6*self.fontscale, labelleft=False)
             # Remove the y ticklabels
-            axes[i,i].set_yticklabels([])
+            if self.diag_ticklabels:
+                pass
+            else:
+                axes[i,i].set_yticklabels([])
             # Update axis label ticks
             if not (self.labels is None):
                 # Set the xlabels
                 axes[-1,i].set_xlabel(self.labels[i], size=10*self.fontscale)
                 # Set the y lables
                 if not i==0:
                     axes[i,0].set_ylabel(self.labels[i], size=10*self.fontscale)
@@ -505,14 +569,66 @@
                                            bins=np.asarray([layer["bins"][j], layer["bins"][i]]),
                                            cmap=layer["cmap"],
                                            w=layer["weights"],
                                            linestyles=layer["linestyle"],
                                            levels=layer["levels"],
                                           )
 
+    def _make_scatter2d_layer(self, axes, layer):
+        ''' Make the Scatter2d layer
+        
+        Parameters
+        ----------
+        axes: matplotlib axes
+            The axes for the corner plot
+        layer: dict
+            dictionary created by add_scatter2d_layer
+        
+        # Define layer dictionary
+        layer = {
+                 "npts"         : npts,
+                 "data"         : data,
+                 "sig"          : sig,
+                 "label"        : label,
+                 's'            : s,
+                 "color"        : color,
+                 "marker"       : marker,
+                 "ecolor"       : ecolor,
+                 "elinewidth"   : elinewidth,
+                }
+        '''
+        ## No 1-D plots ##
+        ### 2D plots ###
+        for i in range(self.ndim):
+            for j in range(i):
+                # Set label
+                if (i == 0) & (j == 0) & (not (layer["label"] is None)):
+                    layer_label = layer["label"]
+                    self._legend = True
+                else:
+                    layer_label = None
+
+                # Make the scatter plot 
+                ax_scatter2d_error(
+                                   axes[i,j], 
+                                   layer["data"][:,j],
+                                   layer["data"][:,i],
+                                   layer["sig"][:,j],
+                                   layer["sig"][:,i],
+                                   limits=np.asarray([self.limits[j], self.limits[i]]),
+                                   set_limits=True,
+                                   label=layer_label,
+                                   s=layer["s"],
+                                   color=layer["color"],
+                                   marker=layer["marker"],
+                                   ecolor=layer["ecolor"],
+                                   elinewidth=layer["elinewidth"],
+                                   zorder=1,
+                                  )
+
     def _make_HOGPEN_layer(self, axes, layer):
         ''' Make the HOGPEN layer
 
         Parameters
         ----------
         axes: matplotlib axes
             The axes for the corner plot
@@ -618,15 +734,15 @@
                                              cmap=layer["cmap"],
                                              limits=np.asarray([self.limits[j], self.limits[i]]),
                                              set_limits=True,
                                              levels=layer["levels"],
                                             )
                                              
                     else:
-                        ax_scatter2d(
+                        ax_scatter2d_density(
                                      axes[i,j], 
                                      layer["2d_%d_%d_x_train"%(i,j)][:hist_bins,1],
                                      layer["2d_%d_%d_x_train"%(i,j)][:hist_bins,0],
                                      layer["2d_%d_%d_y_train"%(i,j)][:hist_bins],
                                      cmap=layer["cmap"],
                                      limits=np.asarray([self.limits[j], self.limits[i]]),
                                      set_limits=True,
@@ -646,15 +762,15 @@
                                              cmap=layer["cmap"],
                                              limits=np.asarray([self.limits[j], self.limits[i]]),
                                              set_limits=True,
                                              levels=layer["levels"],
                                             )
                                              
                     else:
-                        ax_scatter2d(
+                        ax_scatter2d_density(
                                      axes[i,j], 
                                      layer["2d_%d_%d_x_train"%(i,j)][hist_bins:,1],
                                      layer["2d_%d_%d_x_train"%(i,j)][hist_bins:,0],
                                      layer["2d_%d_%d_y_train"%(i,j)][hist_bins:],
                                      cmap=layer["cmap"],
                                      limits=np.asarray([self.limits[j], self.limits[i]]),
                                      set_limits=True,
@@ -723,14 +839,17 @@
         self._get_limits()
         # Make the HOGPEN layers
         for layer in self.HOGPEN_layers:
             self._make_HOGPEN_layer(axes, layer)
         # Make the histogram layers
         for layer in self.histogram_layers:
             self._make_histogram_layer(axes, layer)
+        # Make the scatter layers
+        for layer in self.scatter2d_layers:
+            self._make_scatter2d_layer(axes, layer)
         # Fix tick params
         self._fix_tick_params(axes)
         # Add legend
         self._add_legend(fig)
         # Add title
         self._add_title(fig)
         return fig, axes
```

### Comparing `basil_core-0.3.0/src/basil_core/plots/utils.py` & `basil_core-0.3.2/src/basil_core/plots/utils.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/stats/_distance.c` & `basil_core-0.3.2/src/basil_core/stats/_distance.c`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/stats/_relative_entropy.c` & `basil_core-0.3.2/src/basil_core/stats/_relative_entropy.c`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/stats/density/density_utils.py` & `basil_core-0.3.2/src/basil_core/stats/density/density_utils.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/stats/density/histogram_overhang.py` & `basil_core-0.3.2/src/basil_core/stats/density/histogram_overhang.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/stats/distance.py` & `basil_core-0.3.2/src/basil_core/stats/distance.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/stats/hypercube.py` & `basil_core-0.3.2/src/basil_core/stats/hypercube.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core/stats/random.py` & `basil_core-0.3.2/src/basil_core/stats/random.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/src/basil_core.egg-info/PKG-INFO` & `basil_core-0.3.2/src/basil_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basil_core
-Version: 0.3.0
+Version: 0.3.2
 Summary: basil_core for postprocessing and inference with core simulations
 Home-page: https://gitlab.com/xevra/basil-core
 Author: Vera Delfavero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Delfavero
 Maintainer-email: xevra86@gmail.com
 License: MIT License
```

### Comparing `basil_core-0.3.0/src/basil_core.egg-info/SOURCES.txt` & `basil_core-0.3.2/src/basil_core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.md
 REQUIREMENTS.txt
 __version__.py
 pyproject.toml
 setup.py
 src/basil_core/__init__.py
+src/basil_core/__version__.py
 src/basil_core.egg-info/PKG-INFO
 src/basil_core.egg-info/SOURCES.txt
 src/basil_core.egg-info/dependency_links.txt
 src/basil_core.egg-info/requires.txt
 src/basil_core.egg-info/top_level.txt
 src/basil_core/array_tools/__init__.py
 src/basil_core/array_tools/_indexer.c
@@ -31,22 +32,25 @@
 src/basil_core/plots/__init__.py
 src/basil_core/plots/axis.py
 src/basil_core/plots/corner.py
 src/basil_core/plots/utils.py
 src/basil_core/stats/__init__.py
 src/basil_core/stats/_distance.c
 src/basil_core/stats/_relative_entropy.c
+src/basil_core/stats/_schechter.c
 src/basil_core/stats/distance.py
 src/basil_core/stats/hypercube.py
 src/basil_core/stats/random.py
+src/basil_core/stats/schechter.py
 src/basil_core/stats/density/__init__.py
 src/basil_core/stats/density/density_utils.py
 src/basil_core/stats/density/histogram_overhang.py
 tests/test_callister_priors.py
 tests/test_coordinates.py
 tests/test_corner.py
 tests/test_distance.py
 tests/test_histogram_overhang.py
 tests/test_hypercube.py
 tests/test_indexer.py
 tests/test_orbit.py
-tests/test_random.py
+tests/test_random.py
+tests/test_schechter.py
```

### Comparing `basil_core-0.3.0/tests/test_callister_priors.py` & `basil_core-0.3.2/tests/test_callister_priors.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/tests/test_coordinates.py` & `basil_core-0.3.2/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/tests/test_corner.py` & `basil_core-0.3.2/tests/test_corner.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,19 @@
                                  samples2,
                                  bins=bins,
                                  imshow=False,
                                  contour=True,
                                  linestyle="dotted",
                                  label="samples2",
                                 )
+    # Create a scatter layer
+    mycorner.add_scatter2d_layer(
+                               samples[:10],
+                               np.std(samples,axis=0),
+                              )
     # Show it to me
     #mycorner.show()
     # Save it
     mycorner.save("data/test_corner.png")
 
 ######## All Tests ########
```

### Comparing `basil_core-0.3.0/tests/test_distance.py` & `basil_core-0.3.2/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/tests/test_histogram_overhang.py` & `basil_core-0.3.2/tests/test_histogram_overhang.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/tests/test_hypercube.py` & `basil_core-0.3.2/tests/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/tests/test_indexer.py` & `basil_core-0.3.2/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/tests/test_orbit.py` & `basil_core-0.3.2/tests/test_orbit.py`

 * *Files identical despite different names*

### Comparing `basil_core-0.3.0/tests/test_random.py` & `basil_core-0.3.2/tests/test_random.py`

 * *Files identical despite different names*

