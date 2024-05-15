# Comparing `tmp/satsure_core_test-0.1.3.tar.gz` & `tmp/satsure_core_test-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure_core_test-0.1.3.tar", last modified: Tue May 14 15:36:03 2024, max compression
+gzip compressed data, was "satsure_core_test-0.1.4.tar", last modified: Wed May 15 04:35:27 2024, max compression
```

## Comparing `satsure_core_test-0.1.3.tar` & `satsure_core_test-0.1.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.980630 satsure_core_test-0.1.3/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.1.3/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-14 15:36:03.980368 satsure_core_test-0.1.3/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.1.3/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.971602 satsure_core_test-0.1.3/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.1.3/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure_core_test-0.1.3/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.972301 satsure_core_test-0.1.3/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2479 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      733 2024-05-14 15:32:19.000000 satsure_core_test-0.1.3/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.972708 satsure_core_test-0.1.3/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure_core_test-0.1.3/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.973129 satsure_core_test-0.1.3/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.973425 satsure_core_test-0.1.3/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure_core_test-0.1.3/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.975995 satsure_core_test-0.1.3/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      448 2024-05-13 08:48:32.000000 satsure_core_test-0.1.3/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.976297 satsure_core_test-0.1.3/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2829 2024-05-13 07:51:34.000000 satsure_core_test-0.1.3/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.1.3/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure_core_test-0.1.3/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.976699 satsure_core_test-0.1.3/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4215 2024-05-13 07:51:34.000000 satsure_core_test-0.1.3/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2468 2024-05-13 10:01:38.000000 satsure_core_test-0.1.3/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure_core_test-0.1.3/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.977061 satsure_core_test-0.1.3/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.3/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure_core_test-0.1.3/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.978899 satsure_core_test-0.1.3/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.3/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure_core_test-0.1.3/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.1.3/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure_core_test-0.1.3/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure_core_test-0.1.3/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.979115 satsure_core_test-0.1.3/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure_core_test-0.1.3/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure_core_test-0.1.3/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-14 15:36:03.980141 satsure_core_test-0.1.3/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-14 15:36:03.000000 satsure_core_test-0.1.3/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1517 2024-05-14 15:36:03.000000 satsure_core_test-0.1.3/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-14 15:36:03.000000 satsure_core_test-0.1.3/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      136 2024-05-14 15:36:03.000000 satsure_core_test-0.1.3/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-14 15:36:03.000000 satsure_core_test-0.1.3/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-14 15:36:03.980677 satsure_core_test-0.1.3/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      521 2024-05-14 15:35:19.000000 satsure_core_test-0.1.3/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.146473 satsure_core_test-0.1.4/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.1.4/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 04:35:27.146205 satsure_core_test-0.1.4/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.1.4/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.137498 satsure_core_test-0.1.4/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.1.4/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure_core_test-0.1.4/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.138291 satsure_core_test-0.1.4/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2479 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      733 2024-05-14 15:32:19.000000 satsure_core_test-0.1.4/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.138844 satsure_core_test-0.1.4/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure_core_test-0.1.4/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.139250 satsure_core_test-0.1.4/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.139580 satsure_core_test-0.1.4/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure_core_test-0.1.4/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.141920 satsure_core_test-0.1.4/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      448 2024-05-13 08:48:32.000000 satsure_core_test-0.1.4/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.142640 satsure_core_test-0.1.4/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2829 2024-05-13 07:51:34.000000 satsure_core_test-0.1.4/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.1.4/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure_core_test-0.1.4/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.143013 satsure_core_test-0.1.4/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4027 2024-05-15 04:24:25.000000 satsure_core_test-0.1.4/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2468 2024-05-13 10:01:38.000000 satsure_core_test-0.1.4/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure_core_test-0.1.4/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.143310 satsure_core_test-0.1.4/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.4/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure_core_test-0.1.4/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.144843 satsure_core_test-0.1.4/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.4/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure_core_test-0.1.4/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.1.4/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure_core_test-0.1.4/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure_core_test-0.1.4/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.145124 satsure_core_test-0.1.4/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure_core_test-0.1.4/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure_core_test-0.1.4/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 04:35:27.145971 satsure_core_test-0.1.4/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 04:35:27.000000 satsure_core_test-0.1.4/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1517 2024-05-15 04:35:27.000000 satsure_core_test-0.1.4/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-15 04:35:27.000000 satsure_core_test-0.1.4/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      136 2024-05-15 04:35:27.000000 satsure_core_test-0.1.4/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-15 04:35:27.000000 satsure_core_test-0.1.4/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-15 04:35:27.146522 satsure_core_test-0.1.4/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      521 2024-05-15 04:32:11.000000 satsure_core_test-0.1.4/setup.py
```

### Comparing `satsure_core_test-0.1.3/satelite/config.py` & `satsure_core_test-0.1.4/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/core/downloader.py` & `satsure_core_test-0.1.4/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/core/uploader.py` & `satsure_core_test-0.1.4/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/gdal/gdal_commands.py` & `satsure_core_test-0.1.4/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/raster/raster.py` & `satsure_core_test-0.1.4/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure_core_test-0.1.4/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure_core_test-0.1.4/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure_core_test-0.1.4/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/sentinel2/get_tiles.py` & `satsure_core_test-0.1.4/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/sentinel2/indices/general_indices.py` & `satsure_core_test-0.1.4/satelite/sentinel2/indices/general_indices.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,41 +5,38 @@
     mask_cloud
 
 
 class GeneralIndices:
     """
      Create indices based on bands
     """
-    BANDS = ("B02", "B03", "B04", "B05", "B08", "B12",)
 
     def __init__(self, input_folder: PosixPath,
                  output_folder: PosixPath,
-                 bands: Tuple[str] = None,
-                 tile_identifier_position: int = 1, ):
+                 level: str = "L1C"):
 
         self.input_folder = input_folder
         self.output_folder = output_folder
-        self.bands = bands
-        self.tile_identifier_position = tile_identifier_position
+        self.level = level
 
     def create_s2_normalised_index(self,
                                    band_A_identifier: str,
                                    band_B_identifier: str,
+                                   tile_identifier_position: int = 1,
                                    file_name_delimiter: str = "_",
                                    date_identifier_position: int = 0,
                                    band_combination_id: str = "8",
+                                   input_file_format: str = "jp2",
                                    create_cloud_mask: bool = True,
                                    cloud_mask_bands: Tuple[str] = (
                                            "B02", "B03"),
                                    cloud_mask_threshold: Tuple[int] = (
                                            3200, 3000),
                                    cloud_mask_output_folder: PosixPath = None,
-                                   input_file_format: str = "jp2",
-                                   file_version: str = "0",
-                                   level: str = "L1C"
+                                   file_version: str = "0"
                                    ):
         """
             Create indices based on bands
 
         :param band_A_identifier:
         :param band_B_identifier:
         :param file_name_delimiter:
@@ -47,24 +44,23 @@
         :param band_combination_id:
         :param create_cloud_mask:
         :param cloud_mask_bands:
         :param cloud_mask_threshold:
         :param cloud_mask_output_folder:
         :param input_file_format:
         :param file_version:
-        :param level:
         :return:
         """
         input_folder = Path(self.input_folder)
         files = input_folder.glob(f"*.{input_file_format}")
         unique_tiles = set()
         for file in files:
             unique_tiles.add(
                 file.stem.split(file_name_delimiter)[
-                    self.tile_identifier_position])
+                    tile_identifier_position])
 
         for unique_tile in unique_tiles:
             filename_band_A = list(input_folder.glob(
                 f"*{unique_tile}*{band_A_identifier}*.{input_file_format}"))
             filename_band_B = list(input_folder.glob(
                 f"*{unique_tile}*{band_B_identifier}*.{input_file_format}"))
 
@@ -97,9 +93,9 @@
 
             mask_cloud(
                 index_path,
                 cloud_mask_output_folder,
                 output_name=f"{date}_{unique_tile}_IS1{band_combination_id}02{file_version}.tif",
                 cloud_mask_bands=cloud_mask_bands_path,
                 cloud_mask_threshold=cloud_mask_threshold,
-                level=level
+                level=self.level
             )
```

### Comparing `satsure_core_test-0.1.3/satelite/sentinel2/mosaic_same_bands.py` & `satsure_core_test-0.1.4/satelite/sentinel2/mosaic_same_bands.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/sentinel2/path_row_from_shp.py` & `satsure_core_test-0.1.4/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/sentinel2/s2_l1c_urls.py` & `satsure_core_test-0.1.4/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/sentinel2/s2_l2a_urls.py` & `satsure_core_test-0.1.4/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/tests/conftest.py` & `satsure_core_test-0.1.4/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/tests/sentinel2/test_get_tile.py` & `satsure_core_test-0.1.4/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure_core_test-0.1.4/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure_core_test-0.1.4/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/tests/sentinel2/test_validate.py` & `satsure_core_test-0.1.4/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satelite/validators/check_shape_of_rid.py` & `satsure_core_test-0.1.4/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/satsure_core_test.egg-info/SOURCES.txt` & `satsure_core_test-0.1.4/satsure_core_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.3/setup.py` & `satsure_core_test-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='satsure-core-test',
-    version='0.1.3',
+    version='0.1.4',
     description='satsure core package',
     author='Satsure',
     author_email='kmstpm@email.com',
     packages=find_packages(),
     install_requires=['awscli', 'fiona','gdal==3.6.2', 'google-cloud-storage', 'pandas',
                       'pyproj',
                       'pystac', 'python-dotenv', 'rasterstats', 'rasterio',
```

