# Comparing `tmp/odc_geo-0.4.4.tar.gz` & `tmp/odc_geo-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odc_geo-0.4.4.tar", last modified: Thu May  9 05:31:21 2024, max compression
+gzip compressed data, was "odc_geo-0.4.5.tar", last modified: Wed May 15 00:09:32 2024, max compression
```

## Comparing `odc_geo-0.4.4.tar` & `odc_geo-0.4.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.139427 odc_geo-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 05:31:10.000000 odc_geo-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 05:31:10.000000 odc_geo-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-09 05:31:21.139427 odc_geo-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-09 05:31:10.000000 odc_geo-0.4.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.123427 odc_geo-0.4.4/odc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.127427 odc_geo-0.4.4/odc/geo/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_interop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_rgba.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35059 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_xr_interop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.127427 odc_geo-0.4.4/odc/geo/cog/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_mpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_mpu_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17800 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_rio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    24577 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_tifffile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/crs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.131427 odc_geo-0.4.4/odc/geo/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/data/gbox.css
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/data/ocean.geojson.xz
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    49544 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/geobox.py
--rw-r--r--   0 runner    (1001) docker     (127)    46572 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/geom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    21824 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    20456 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21941 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/roi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/warp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/xr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.135427 odc_geo-0.4.4/odc_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:31:20.000000 odc_geo-0.4.4/odc_geo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 05:31:10.000000 odc_geo-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-09 05:31:21.139427 odc_geo-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:31:10.000000 odc_geo-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.135427 odc_geo-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_cog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_crs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_dask_interop.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_gbox_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_geobox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_geoboxtiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    33464 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_mpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_mpu_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_rgba.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_rioxarray_interop.py
--rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_roi.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    23073 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_xr_interop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:32.846534 odc_geo-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 00:09:21.000000 odc_geo-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 00:09:21.000000 odc_geo-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-15 00:09:32.846534 odc_geo-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-15 00:09:21.000000 odc_geo-0.4.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:32.830534 odc_geo-0.4.5/odc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:32.838534 odc_geo-0.4.5/odc/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/_interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9405 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37520 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/_xr_interop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:32.838534 odc_geo-0.4.5/odc/geo/cog/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/cog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/cog/_mpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/cog/_mpu_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17800 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/cog/_rio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/cog/_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/cog/_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24577 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/cog/_tifffile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/crs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:32.838534 odc_geo-0.4.5/odc/geo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/data/gbox.css
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/data/ocean.geojson.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49544 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/geobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46572 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21824 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20456 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21941 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/roi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/warp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-15 00:09:21.000000 odc_geo-0.4.5/odc/geo/xr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:32.846534 odc_geo-0.4.5/odc_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-15 00:09:32.000000 odc_geo-0.4.5/odc_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-15 00:09:32.000000 odc_geo-0.4.5/odc_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:09:32.000000 odc_geo-0.4.5/odc_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:09:32.000000 odc_geo-0.4.5/odc_geo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-15 00:09:32.000000 odc_geo-0.4.5/odc_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 00:09:32.000000 odc_geo-0.4.5/odc_geo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-15 00:09:21.000000 odc_geo-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-15 00:09:32.846534 odc_geo-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:09:21.000000 odc_geo-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:32.846534 odc_geo-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_cog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_dask_interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_gbox_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_geobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_geoboxtiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33464 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_mpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_mpu_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_rioxarray_interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_roi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25058 2024-05-15 00:09:21.000000 odc_geo-0.4.5/tests/test_xr_interop.py
```

### Comparing `odc_geo-0.4.4/LICENSE` & `odc_geo-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/PKG-INFO` & `odc_geo-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.4.4
+Version: 0.4.5
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc_geo-0.4.4/README.rst` & `odc_geo-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/__init__.py` & `odc_geo-0.4.5/odc/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/_blocks.py` & `odc_geo-0.4.5/odc/geo/_blocks.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/_compress.py` & `odc_geo-0.4.5/odc/geo/_compress.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/_dask.py` & `odc_geo-0.4.5/odc/geo/_dask.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/_interop.py` & `odc_geo-0.4.5/odc/geo/_interop.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/_map.py` & `odc_geo-0.4.5/odc/geo/_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-from typing import Any, Optional, Tuple, Dict
+from typing import Any, Dict, Optional, Tuple
 
 import xarray as xr
 
 from ._interop import have
 from ._rgba import colorize, is_rgb
 from .converters import map_crs
 from .gcp import GCPGeoBox
 from .geobox import GeoBox
 
 
 # pylint: disable=import-outside-toplevel, redefined-builtin, too-many-locals
-def _add_to_folium(url, bounds, map, name=None, **kw):
+def _add_to_folium(url, bounds, map, name=None, index=None, **kw):
     assert have.folium
 
     from folium.raster_layers import ImageOverlay
 
     img_overlay = ImageOverlay(url, bounds, name=name, **kw)
-    img_overlay.add_to(map)
+    if map is not None:
+        img_overlay.add_to(map, name=name, index=index)
     return img_overlay
 
 
-def _add_to_ipyleaflet(url, bounds, map, name=None, **kw):
+def _add_to_ipyleaflet(url, bounds, map, name=None, index=None, **kw):
     assert have.ipyleaflet
 
     from ipyleaflet import ImageOverlay, Map
 
     assert isinstance(map, Map)
 
     if name is not None:
         kw.update(name=name)
 
     img_overlay = ImageOverlay(url=url, bounds=bounds, **kw)
-    map.add(img_overlay)
+    if map is not None:
+        map.add(img_overlay, index=index)
 
     return img_overlay
 
 
 def _get_add_to_method(map):
     if map is None:
         return None
@@ -52,14 +54,15 @@
 
 
 def add_to(
     xx: Any,
     map: Any,
     *,
     name: Optional[str] = None,
+    index: Optional[int] = None,
     fmt: str = "png",
     max_size: int = 4096,
     resampling: str = "nearest",
     # jpeg options:
     transparent_pixel: Optional[Tuple[int, int, int]] = None,
     # RGB conversion parameters
     cmap: Optional[Any] = None,
@@ -163,20 +166,21 @@
     url = xx.odc.compress(
         *compress_opts, as_data_url=True, transparent=transparent_pixel
     )
     bounds = gbox.map_bounds()
     if _add_to is None:
         return url, bounds
 
-    return _add_to(url, bounds, map, name=name, **kw)
+    return _add_to(url, bounds, map, name=name, index=index, **kw)
 
 
 def explore(
     xx: Any,
     map: Optional[Any] = None,
+    *,
     bands: Optional[Tuple[str, str, str]] = None,
     vmin: Optional[float] = None,
     vmax: Optional[float] = None,
     cmap: Optional[Any] = None,
     robust: bool = False,
     tiles: Any = "OpenStreetMap",
     attr: Optional[str] = None,
@@ -241,44 +245,48 @@
 
     if not have.folium:
         raise ModuleNotFoundError(
             "'folium' is required but not installed. "
             "Please install it before using `.explore()`."
         )
 
-    from folium import Map, LayerControl
+    from folium import LayerControl, Map
 
-    # Update any supplied kwargs with custom params
     map_kwds = {} if map_kwds is None else map_kwds
-    kwargs.update(cmap=cmap, vmin=vmin, vmax=vmax, robust=robust, resampling=resampling)
-    map_kwds.update(tiles=tiles, attr=attr)
+    new_map = map is None
 
     # If input is a dataset, convert to an RGBA array
     if isinstance(xx, xr.Dataset):
         xx = xx.odc.to_rgba(bands=bands, vmin=vmin, vmax=vmax)
 
     # Create folium Map if required
     if map is None:
-        map = Map(**map_kwds)
+        map = Map(tiles=tiles, attr=attr, **map_kwds)
 
     # Add to map and raise a friendly error if data has unsuitable dims
     try:
-        xx.odc.add_to(map, **kwargs)
+        xx.odc.add_to(
+            map,
+            cmap=cmap,
+            vmin=vmin,
+            vmax=vmax,
+            robust=robust,
+            resampling=resampling,
+            **kwargs,
+        )
     except ValueError as e:
         raise ValueError(
             "Only 2D single-band (x, y) or 3D multi-band (x, y, band) "
             "arrays are supported by `.explore()`. Please reduce the "
             "dimensions in your array, for example by using `.isel()` "
             "or `.sel()`: `da.isel(time=0).odc.explore()`."
         ) from e
 
-    # Zoom map to extent of data
-    map.fit_bounds(xx.odc.map_bounds())
-
-    # Add a layer control if requested and not already added
-    layer_control_added = any(
-        isinstance(child, LayerControl) for child in map._children.values()
-    )
-    if layer_control and not layer_control_added:
-        LayerControl().add_to(map)
+    if new_map:
+        # Zoom map to extent of data
+        map.fit_bounds(xx.odc.map_bounds())
+
+        # Add a layer control if requested
+        if layer_control:
+            LayerControl().add_to(map)
 
     return map
```

### Comparing `odc_geo-0.4.4/odc/geo/_rgba.py` & `odc_geo-0.4.5/odc/geo/_rgba.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/_xr_interop.py` & `odc_geo-0.4.5/odc/geo/_xr_interop.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from .crs import CRS, CRSError, SomeCRS, norm_crs_or_error
 from .gcp import GCPGeoBox, GCPMapping
 from .geobox import Coordinate, GeoBox, GeoboxAnchor
 from .geom import Geometry
 from .math import (
     affine_from_axis,
     approx_equal_affine,
+    is_affine_st,
     maybe_int,
     resolution_from_affine,
 )
 from .overlap import compute_output_geobox
 from .roi import roi_is_empty
 from .types import Resolution, SomeResolution, SomeShape, xy_
 
@@ -59,14 +60,22 @@
 SomeGeoBox = Union[GeoBox, GCPGeoBox]
 
 _DEFAULT_CRS_COORD_NAME = "spatial_ref"
 
 # these attributes are pruned during reproject
 SPATIAL_ATTRIBUTES = ("crs", "crs_wkt", "grid_mapping", "gcps", "epsg")
 
+# dimensions with these names are considered spatial
+STANDARD_SPATIAL_DIMS = [
+    ("y", "x"),
+    ("yc", "xc"),
+    ("latitude", "longitude"),
+    ("lat", "lon"),
+]
+
 
 @dataclass
 class GeoState:
     """
     Geospatial information for xarray object.
     """
 
@@ -147,22 +156,38 @@
 
     If ``relaxed=True`` and none of the above dimension names are found,
     assume that last two dimensions are spatial dimensions.
 
     :returns: ``None`` if no dimensions with expected names are found
     :returns: ``('y', 'x') | ('latitude', 'longitude') | ('lat', 'lon')``
     """
-    guesses = [("y", "x"), ("latitude", "longitude"), ("lat", "lon")]
+
+    def skip_dim(dim: str) -> bool:
+        if dim in ("time", "band", "bands", "wavelength", "wavelengths"):
+            return True
+
+        # skip dimensions without coord of the same name
+        if dim not in xx.coords:
+            return True
+
+        coord = xx.coords[dim]
+        # Primary coordinate for spatial dimension must have floating point type
+        if coord.dtype.kind != "f":
+            return True
+
+        return False
 
     _dims = [str(dim) for dim in xx.dims]
     dims = set(_dims)
-    for guess in guesses:
+    for guess in STANDARD_SPATIAL_DIMS:
         if dims.issuperset(guess):
             return guess
 
+    _dims = [dim for dim in _dims if not skip_dim(str(dim))]
+
     if relaxed and len(_dims) >= 2:
         return _dims[-2], _dims[-1]
 
     return None
 
 
 def _mk_crs_coord(
@@ -331,101 +356,125 @@
 
     :return:
         A :py:class:`~xarray.Dataset` or :py:class:`~xarray.DataArray`
         cropped and optionally masked to the spatial extent of ``poly``.
 
     .. seealso:: :py:meth:`odc.geo.xr.mask`
     """
+    meta: ODCExtension = xx.odc
+    sdims = meta.spatial_dims
+    gbox = meta.geobox
+
+    if sdims is None or gbox is None:
+        raise ValueError("Can't locate spatial dimensions")
+
+    if not isinstance(gbox, GeoBox):
+        raise ValueError("Can't crop GCPGeoBox")
+
     # Create new geobox with pixel grid of `xx` but enclosing `poly`.
-    poly_geobox = xx.odc.geobox.enclosing(poly)
+    poly_geobox = gbox.enclosing(poly)
 
     # Calculate ROI slices into `xx` for intersection between both geoboxes.
-    roi = xx.odc.geobox.overlap_roi(poly_geobox)
+    roi = gbox.overlap_roi(poly_geobox)
 
     # Verify that `poly` overlaps with `xx` by checking if the returned
     # ROI is empty
     if roi_is_empty(roi):
         raise ValueError(
             "The supplied `poly` must overlap spatially with the extent of `xx`."
         )
 
     # Crop spatial dims of `xx` using ROI
-    sdims = spatial_dims(xx)
-    if sdims is None:
-        raise ValueError("Can't locate spatial dimensions")
     xx_cropped = xx.isel({sdims[0]: roi[0], sdims[1]: roi[1]})
 
     # Optionally mask data outside rasterized `poly`
     if apply_mask:
         xx_cropped = mask(xx_cropped, poly, all_touched=all_touched)
 
     return xx_cropped
 
 
 def xr_coords(
-    gbox: SomeGeoBox, crs_coord_name: Optional[str] = _DEFAULT_CRS_COORD_NAME
+    gbox: SomeGeoBox,
+    crs_coord_name: Optional[str] = _DEFAULT_CRS_COORD_NAME,
+    always_yx: bool = False,
+    dims: Optional[Tuple[str, str]] = None,
 ) -> Dict[Hashable, xarray.DataArray]:
     """
     Dictionary of Coordinates in xarray format.
 
+    :param gbox:
+      :py:class:`~odc.geo.geobox.GeoBox` or :py:class:`~odc.geo.gcp.GCPGeoBox`
+
     :param crs_coord_name:
-       Use custom name for CRS coordinate, default is "spatial_ref". Set to ``None`` to not generate
-       CRS coordinate at all.
+       Use custom name for CRS coordinate, default is "spatial_ref". Set to
+       ``None`` to not generate CRS coordinate at all.
+
+    :param always_yx:
+       If True, always use names ``y,x`` for spatial coordinates even for
+       geographic geoboxes.
+
+    :param dims:
+       Use custom names for spatial dimensions, default is to use ``y,x`` or
+       ``latitude, longitude`` based on projection used. Dimensions are supplied
+       in "array" order, i.e. ``('y', 'x')``.
 
     :returns:
-       Dictionary ``name:str -> xr.DataArray``. Where names are either ``y,x`` for projected or
+       Dictionary ``name:str -> xr.DataArray``. Where names are either as
+       supplied by ``dims=`` or otherwise ``y,x`` for projected or
        ``latitude, longitude`` for geographic.
 
     """
+    if dims is None:
+        if always_yx:
+            dims = ("y", "x")
+        else:
+            dims = gbox.dimensions
+
     attrs = {}
     crs = gbox.crs
     if crs is not None:
         attrs["crs"] = str(crs)
 
     gcps = None
     transform: Optional[Affine] = None
 
     if isinstance(gbox, GCPGeoBox):
         coords: Dict[Hashable, xarray.DataArray] = {
-            name: _mk_pixel_coord(name, sz, None)
-            for name, sz in zip(gbox.dimensions, gbox.shape)
+            name: _mk_pixel_coord(name, sz) for name, sz in zip(dims, gbox.shape)
         }
         gcps = gbox.gcps()
     else:
         transform = gbox.transform
         if gbox.axis_aligned:
             coords = {
                 name: _coord_to_xr(name, coord, **attrs)
-                for name, coord in gbox.coordinates.items()
+                for name, coord in zip(dims, gbox.coordinates.values())
             }
         else:
             coords = {
-                name: _mk_pixel_coord(name, sz, transform)
-                for name, sz in zip(gbox.dimensions, gbox.shape)
+                name: _mk_pixel_coord(name, sz) for name, sz in zip(dims, gbox.shape)
             }
 
     if crs_coord_name is not None and crs is not None:
         coords[crs_coord_name] = _mk_crs_coord(
             crs, crs_coord_name, gcps=gcps, transform=transform
         )
 
     return coords
 
 
 def _mk_pixel_coord(
     name: str,
     sz: int,
-    transform: Optional[Affine],
 ) -> xarray.DataArray:
     data = numpy.arange(0.5, sz, dtype="float32")
     xx = xarray.DataArray(
         data, coords={name: data}, dims=(name,), attrs={"units": "pixel"}
     )
-    if transform is not None:
-        xx.encoding["_transform"] = transform[:6]
     return xx
 
 
 def _is_spatial_ref(coord) -> bool:
     return coord.ndim == 0 and (
         "spatial_ref" in coord.attrs or "crs_wkt" in coord.attrs
     )
@@ -527,29 +576,32 @@
                 _xx.values,
                 _yy.values,
                 resolution_from_affine(original_transform),
             )
         except ValueError:
             return None
 
-    if original_transform is not None and approx_equal_affine(
-        transform, original_transform
-    ):
-        transform = original_transform
-
-    if not gcp and (_pix2world := _xx.encoding.get("_transform", None)) is not None:
-        # non-axis aligned geobox detected
-        # adjust transform
-        #  world <- pix' <- pix
-        transform = Affine(*_pix2world) * transform
+    if original_transform is not None:
+        if not is_affine_st(original_transform):
+            # non-axis aligned geobox detected
+            # adjust transform
+            #  world <- pix' <- pix
+            transform = original_transform * transform
+
+        if approx_equal_affine(transform, original_transform):
+            transform = original_transform
+
     return transform
 
 
 def _locate_geo_info(src: XarrayObject) -> GeoState:
     # pylint: disable=too-many-locals
+    if len(src.dims) < 2:
+        return GeoState()
+
     sdims = spatial_dims(src, relaxed=True)
     if sdims is None:
         return GeoState()
 
     crs_coord: Optional[xarray.DataArray] = None
     crs: Optional[CRS] = None
     geobox: Optional[SomeGeoBox] = None
@@ -1007,55 +1059,94 @@
 def wrap_xr(
     im: Any,
     gbox: SomeGeoBox,
     *,
     time=None,
     nodata=None,
     crs_coord_name: Optional[str] = _DEFAULT_CRS_COORD_NAME,
+    always_yx: bool = False,
+    dims: Optional[Tuple[str, ...]] = None,
     axis: Optional[int] = None,
     **attrs,
 ) -> xarray.DataArray:
     """
     Wrap xarray around numpy array with CRS and x,y coords.
 
     :param im: numpy array to wrap, last two axes are Y,X
     :param gbox: Geobox, must same shape as last two axis of ``im``
     :param time: optional time axis value(s), defaults to None
     :param nodata: optional `nodata` value, defaults to None
+    :param crs_coord_name: allows to change name of the crs coordinate variable
+    :param always_yx: If True, always use names ``y,x`` for spatial coordinates
+    :param dims: Custom names for spatial dimensions
+    :param axis: Which axis of the input array corresponds to Y,X
     :param attrs: Any other attributes to set on the result
     :return: xarray DataArray
     """
+    # pylint: disable=too-many-locals,too-many-arguments
+    assert dims is None or len(dims) == im.ndim
+
     if axis is None:
         axis = 1 if time is not None else 0
+    elif axis < 0:  # handle numpy style negative axis
+        axis = int(im.ndim) + axis
 
     if im.ndim == 2 and axis == 1:
         im = im[numpy.newaxis, ...]
 
-    assert axis in (0, 1)  # upto 1 extra dimension on the left only
-    assert im.ndim - axis - 2 in (0, 1)  # upto 1 extra dimension on the right only
+    assert axis >= 0
+    assert im.ndim - axis - 2 >= 0
     assert im.shape[axis : axis + 2] == gbox.shape
 
-    prefix_dims: Tuple[str, ...] = ("time",) if axis == 1 else ()
-    postfix_dims: Tuple[str, ...] = ("band",) if im.ndim - axis > 2 else ()
+    def _prefix_dims(n):
+        if n == 0:
+            return ()
+        if n == 1:
+            return ("time",)
+        return ("time", *[f"dim_{i}" for i in range(n - 1)])
+
+    def _postfix_dims(n):
+        if n == 0:
+            return ()
+        if n == 1:
+            return ("band",)
+        return (f"b_{i}" for i in range(n))
+
+    sdims: Optional[Tuple[str, str]] = None
+    if dims is None:
+        sdims = ("y", "x") if always_yx else gbox.dimensions
+        dims = (*_prefix_dims(axis), *sdims, *_postfix_dims(im.ndim - axis - 2))
+    else:
+        sdims = dims[axis], dims[axis + 1]
 
-    dims = (*prefix_dims, *gbox.dimensions, *postfix_dims)
-    coords = xr_coords(gbox, crs_coord_name=crs_coord_name)
+    prefix_dims = dims[:axis]
+    postfix_dims = dims[axis + 2 :]
+
+    coords = xr_coords(
+        gbox,
+        crs_coord_name=crs_coord_name,
+        always_yx=always_yx,
+        dims=sdims,
+    )
 
     if time is not None:
         if not isinstance(time, xarray.DataArray):
             if len(prefix_dims) > 0 and isinstance(time, (str, datetime)):
                 time = [time]
 
-            time = xarray.DataArray(time, dims=prefix_dims).astype("datetime64[ns]")
+            time = xarray.DataArray(time, dims=prefix_dims[:1]).astype("datetime64[ns]")
 
         coords["time"] = time
+
     if postfix_dims:
-        coords["band"] = xarray.DataArray(
-            [f"b{i}" for i in range(im.shape[-1])], dims=postfix_dims
-        )
+        for a, dim in enumerate(postfix_dims):
+            nb = im.shape[axis + 2 + a]
+            coords[dim] = xarray.DataArray(
+                [f"b{i}" for i in range(nb)], dims=(dim,), name=dim
+            )
 
     if nodata is not None:
         attrs = {"nodata": nodata, **attrs}
 
     out = xarray.DataArray(im, coords=coords, dims=dims, attrs=attrs)
     if crs_coord_name is not None:
         out.encoding["grid_mapping"] = crs_coord_name
@@ -1077,14 +1168,17 @@
     :param gbox: Desired footprint and resolution
     :param dtype: Pixel data type
     :param chunks: Create a dask array instead of numpy array
     :param time: When set adds time dimension
     :param crs_coord_name: allows to change name of the crs coordinate variable
 
     :return: :py:class:`xarray.DataArray` filled with zeros (numpy or dask)
+
+    .. seealso:: :py:meth:`odc.geo.xr.wrap_xr`
+
     """
     if time is not None:
         _shape: Tuple[int, ...] = (len(time), *geobox.shape.yx)
     else:
         _shape = geobox.shape.yx
 
     if chunks is not None:
```

### Comparing `odc_geo-0.4.4/odc/geo/cog/_mpu.py` & `odc_geo-0.4.5/odc/geo/cog/_mpu.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/cog/_mpu_fs.py` & `odc_geo-0.4.5/odc/geo/cog/_mpu_fs.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/cog/_rio.py` & `odc_geo-0.4.5/odc/geo/cog/_rio.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/cog/_s3.py` & `odc_geo-0.4.5/odc/geo/cog/_s3.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/cog/_shared.py` & `odc_geo-0.4.5/odc/geo/cog/_shared.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/cog/_tifffile.py` & `odc_geo-0.4.5/odc/geo/cog/_tifffile.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/converters.py` & `odc_geo-0.4.5/odc/geo/converters.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/crs.py` & `odc_geo-0.4.5/odc/geo/crs.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/data/__init__.py` & `odc_geo-0.4.5/odc/geo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/data/gbox.css` & `odc_geo-0.4.5/odc/geo/data/gbox.css`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/data/ocean.geojson.xz` & `odc_geo-0.4.5/odc/geo/data/ocean.geojson.xz`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/gcp.py` & `odc_geo-0.4.5/odc/geo/gcp.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/geobox.py` & `odc_geo-0.4.5/odc/geo/geobox.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/geom.py` & `odc_geo-0.4.5/odc/geo/geom.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/gridspec.py` & `odc_geo-0.4.5/odc/geo/gridspec.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/math.py` & `odc_geo-0.4.5/odc/geo/math.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/overlap.py` & `odc_geo-0.4.5/odc/geo/overlap.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/roi.py` & `odc_geo-0.4.5/odc/geo/roi.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/testutils.py` & `odc_geo-0.4.5/odc/geo/testutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,14 @@
 def purge_crs_info(xx: xr.DataArray) -> xr.DataArray:
     attributes_to_clear = ["crs", "wkt", "crs_wkt", "transform", "epsg", "resolution"]
 
     def _purge_attributes(_x: xr.DataArray) -> xr.DataArray:
         for attr in attributes_to_clear:
             _x.attrs.pop(attr, None)
         _x.encoding.pop("grid_mapping", None)
-        _x.encoding.pop("_transform", None)
         return _x
 
     # remove non-dimensional coordinate, which is CRS in our case
     to_drop = [name for name in xx.coords if name not in xx.dims]
     xx = xx.drop_vars(to_drop)
     xx.encoding.pop("grid_spatial", None)
```

### Comparing `odc_geo-0.4.4/odc/geo/types.py` & `odc_geo-0.4.5/odc/geo/types.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/ui.py` & `odc_geo-0.4.5/odc/geo/ui.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/warp.py` & `odc_geo-0.4.5/odc/geo/warp.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc/geo/xr.py` & `odc_geo-0.4.5/odc/geo/xr.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/odc_geo.egg-info/PKG-INFO` & `odc_geo-0.4.5/odc_geo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.4.4
+Version: 0.4.5
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc_geo-0.4.4/odc_geo.egg-info/SOURCES.txt` & `odc_geo-0.4.5/odc_geo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/pyproject.toml` & `odc_geo-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/setup.cfg` & `odc_geo-0.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_bbox.py` & `odc_geo-0.4.5/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_blocks.py` & `odc_geo-0.4.5/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_cog.py` & `odc_geo-0.4.5/tests/test_cog.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_converters.py` & `odc_geo-0.4.5/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_crs.py` & `odc_geo-0.4.5/tests/test_crs.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_dask_interop.py` & `odc_geo-0.4.5/tests/test_dask_interop.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_datasets.py` & `odc_geo-0.4.5/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_gbox_ops.py` & `odc_geo-0.4.5/tests/test_gbox_ops.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_gcp.py` & `odc_geo-0.4.5/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_geobox.py` & `odc_geo-0.4.5/tests/test_geobox.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_geoboxtiles.py` & `odc_geo-0.4.5/tests/test_geoboxtiles.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_geom.py` & `odc_geo-0.4.5/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_gridspec.py` & `odc_geo-0.4.5/tests/test_gridspec.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_map.py` & `odc_geo-0.4.5/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_math.py` & `odc_geo-0.4.5/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_mpu.py` & `odc_geo-0.4.5/tests/test_mpu.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_mpu_fs.py` & `odc_geo-0.4.5/tests/test_mpu_fs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 import pickle
 from pathlib import Path
 from uuid import uuid4
 
 import pytest
 
+_ = pytest.importorskip("odc.geo.cog")
+
 from odc.geo.cog._mpu_fs import MPUFileSink
 
 # pylint: disable=protected-access
 
 
 def slurp(path: Path) -> bytes:
     with path.open("rb") as f:
         return f.read()
 
 
-@pytest.mark.parametrize("parts_base", [f"parts-{uuid4().hex[:8]}", None])
+@pytest.mark.parametrize("parts_base", [f"parts-3782781", None])
 @pytest.mark.parametrize("num_parts", [1, 2, 3, 10])
 def test_filesink(tmp_path: Path, parts_base: str | None, num_parts: int):
     dst = Path(tmp_path / f"{uuid4().hex}.bin")
     assert dst.exists() is False
     if parts_base is not None:
         parts_base = str(tmp_path / parts_base)
```

### Comparing `odc_geo-0.4.4/tests/test_overlap.py` & `odc_geo-0.4.5/tests/test_overlap.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_rgba.py` & `odc_geo-0.4.5/tests/test_rgba.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_rioxarray_interop.py` & `odc_geo-0.4.5/tests/test_rioxarray_interop.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_roi.py` & `odc_geo-0.4.5/tests/test_roi.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_types.py` & `odc_geo-0.4.5/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_ui.py` & `odc_geo-0.4.5/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `odc_geo-0.4.4/tests/test_xr_interop.py` & `odc_geo-0.4.5/tests/test_xr_interop.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,27 @@
 from odc.geo.testutils import approx_equal_geobox, epsg3577, mkA, purge_crs_info
 from odc.geo.types import ROI, resxy_
 from odc.geo.xr import (
     ODCExtensionDa,
     ODCExtensionDs,
     rasterize,
     register_geobox,
+    spatial_dims,
     wrap_xr,
     xr_coords,
     xr_reproject,
     xr_zeros,
 )
 
 # pylint: disable=redefined-outer-name,import-outside-toplevel,protected-access
+TEST_GEOBOXES_SMALL_AXIS_ALIGNED = [
+    GeoBox.from_bbox((-10, -2, 5, 4), "epsg:4326", tight=True, resolution=0.2),
+    GeoBox.from_bbox((-10, -2, 5, 4), "epsg:3857", tight=True, resolution=1),
+    GeoBox.from_bbox((-10, -2, 5, 4), "epsg:3857", tight=True, resolution=resxy_(1, 2)),
+]
 
 
 @pytest.fixture
 def geobox_epsg4326():
     _box = geom.box(-20, -10, 20, 10, "epsg:4326")
     yield GeoBox.from_geopolygon(_box, 5)
 
@@ -83,16 +89,15 @@
     assert _gbox.axis_aligned is False
     cc = xr_coords(_gbox)
     assert list(cc) == ["y", "x", "spatial_ref"]
     assert cc["spatial_ref"].shape == ()
     assert cc["spatial_ref"].attrs["spatial_ref"] == gbox.crs.wkt
     assert isinstance(cc["spatial_ref"].attrs["grid_mapping_name"], str)
     assert isinstance(cc["spatial_ref"].attrs["GeoTransform"], str)
-    assert cc["x"].encoding["_transform"] == _gbox.affine[:6]
-    assert cc["y"].encoding["_transform"] == _gbox.affine[:6]
+    assert xr_zeros(_gbox, dtype="uint16").odc.geobox == _gbox
 
     # geographic CRS
     A = mkA(0, scale=(0.1, -0.1), translation=(10, 30))
     gbox = GeoBox(_shape, A, "epsg:4326")
 
     cc = xr_coords(gbox)
     assert list(cc) == ["latitude", "longitude", "spatial_ref"]
@@ -172,14 +177,15 @@
     assert xx.odc.spatial_dims == ("latitude", "longitude")
     assert xx.spatial_ref.attrs["spatial_ref"] == gbox.crs.wkt
     assert xx.spatial_ref.attrs["grid_mapping_name"] == "latitude_longitude"
     assert xx.odc.uncached.transform == xx.odc.transform
     assert xx.odc.output_geobox("epsg:3857").crs == "epsg:3857"
     assert xx.odc.map_bounds() == gbox.map_bounds()
     assert xx.odc.output_geobox("utm").crs.epsg is not None
+    assert xx.odc.aspect == gbox.aspect
 
     # this drops encoding/attributes, but crs/geobox should remain the same
     _xx = xx * 10.0
     assert _xx.encoding == {}
     assert _xx.odc.crs == xx.odc.crs
     assert _xx.odc.geobox == xx.odc.geobox
 
@@ -348,14 +354,17 @@
 
     xx = wrap_xr(data, gbox)
     assert xx.shape == gbox.shape
     assert xx.odc.geobox == gbox
     assert xx.dims == gbox.dims
     assert xx.attrs == {}
 
+    assert wrap_xr(data, gbox, always_yx=True).dims == ("y", "x")
+    assert wrap_xr(data, gbox, dims=("Y", "X")).dims == ("Y", "X")
+
     xx = wrap_xr(data, gbox, nodata=None)
     assert xx.attrs == {}
 
     xx = wrap_xr(data, gbox, nodata=10, some_flag=3)
     assert xx.attrs == dict(nodata=10, some_flag=3)
 
     xx = wrap_xr(data, gbox, time="2022-02-02T22:22:22.222222")
@@ -373,14 +382,39 @@
     assert xx.time.dt.month.values[0] == 2
 
     xx = wrap_xr(data[..., np.newaxis], gbox)
     assert xx.shape == (*gbox.shape, 1)
     assert xx.band.data.tolist() == ["b0"]
 
 
+@pytest.mark.parametrize("gbox", TEST_GEOBOXES_SMALL_AXIS_ALIGNED)
+@pytest.mark.parametrize("nprefix", [0, 1, 2])
+@pytest.mark.parametrize("npostfix", [0, 1, 2])
+def test_wrap_xr_nd(gbox: GeoBox, nprefix: int, npostfix: int):
+    shape = (1,) * nprefix + gbox.shape + (3,) * npostfix
+    data = np.zeros(shape, dtype="uint16")
+    xx = wrap_xr(data, gbox, axis=nprefix)
+    assert xx.odc.geobox == gbox
+    assert xx.odc.ydim == nprefix
+    assert xx.dims[:nprefix] == ("time", "dim_0", "dim_1", "dim_2", "dim_3")[:nprefix]
+
+    if npostfix == 1:
+        assert xx.dims[-1] == "band"
+    if npostfix > 1:
+        assert xx.dims[nprefix + 2 :] == tuple(f"b_{i}" for i in range(npostfix))
+
+    _dims = tuple(f"custom_{dim}" for dim in xx.dims)
+    _dims = _dims[:nprefix] + ("y", "x") + _dims[nprefix + 2 :]
+
+    yy = wrap_xr(data, gbox, axis=nprefix, dims=_dims)
+    assert yy.dims == _dims
+    assert yy.odc.geobox == gbox
+    assert yy.odc.spatial_dims == _dims[nprefix : nprefix + 2]
+
+
 @pytest.mark.parametrize("xx_time", [None, ["2020-01-30"]])
 @pytest.mark.parametrize("xx_chunks", [None, (-1, -1), (4, 4)])
 def test_xr_reproject(xx_epsg4326: xr.DataArray):
     assert isinstance(xx_epsg4326.odc, ODCExtensionDa)
     xx0 = xx_epsg4326
     xx0.attrs["crs"] = "epsg:4326"
     # smoke-test only
@@ -477,21 +511,14 @@
 
     import odc.geo._interop
 
     assert "is_dask_collection" in dir(odc.geo._interop)
     assert is_dask_collection is dask.is_dask_collection
 
 
-TEST_GEOBOXES_SMALL_AXIS_ALIGNED = [
-    GeoBox.from_bbox((-10, -2, 5, 4), "epsg:4326", tight=True, resolution=0.2),
-    GeoBox.from_bbox((-10, -2, 5, 4), "epsg:3857", tight=True, resolution=1),
-    GeoBox.from_bbox((-10, -2, 5, 4), "epsg:3857", tight=True, resolution=resxy_(1, 2)),
-]
-
-
 @pytest.mark.parametrize("geobox", TEST_GEOBOXES_SMALL_AXIS_ALIGNED)
 @pytest.mark.parametrize(
     "bad_geo_transform",
     [
         "some random string",
         "1 2 3 4 5 not-a-float",
     ],
@@ -699,7 +726,37 @@
     assert xx_notouched.notnull().sum() < xx_masked.notnull().sum()
 
     # Verify that masking also works on datasets
     xx_ds = xx.to_dataset(name="test")
     xx_ds_masked = xx_ds.odc.mask(poly=poly)
     assert xx_ds_masked.odc.geobox == xx_ds.odc.geobox
     assert xx_ds_masked.test.isnull().any()
+
+
+def test_spatial_dims():
+    gbox = GeoBox.from_bbox([0, -10, 100, 20], "epsg:4326", tight=True, shape=(13, 29))
+    xx0 = xr_zeros(gbox, "int16", always_yx=True, time=["2020-01-01", "2020-01-02"])
+    assert spatial_dims(xx0) == ("y", "x")
+
+    assert wrap_xr(
+        xx0.data,
+        gbox,
+        dims=("T", "Y", "X"),
+        axis=1,
+    ).odc.spatial_dims == ("Y", "X")
+    assert wrap_xr(
+        xx0.data[..., np.newaxis],
+        gbox,
+        dims=("time", "Y", "X", "wavelength"),
+        axis=1,
+    ).odc.spatial_dims == ("Y", "X")
+
+    xx = wrap_xr(
+        np.zeros((2, 3, *gbox.shape.yx, 2, 3), dtype="int16"),
+        gbox,
+        axis=2,
+        dims=("A", "B", "Y", "X", "C", "D"),
+    )
+    assert "X" in xx.coords and "Y" in xx.coords
+    assert xx.odc.geobox == gbox
+    assert xx.odc.ydim == 2
+    assert xx.odc.spatial_dims == xx.dims[2:4]
```

