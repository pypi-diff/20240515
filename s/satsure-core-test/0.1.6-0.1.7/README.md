# Comparing `tmp/satsure_core_test-0.1.6.tar.gz` & `tmp/satsure_core_test-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure_core_test-0.1.6.tar", last modified: Wed May 15 10:13:31 2024, max compression
+gzip compressed data, was "satsure_core_test-0.1.7.tar", last modified: Wed May 15 10:42:16 2024, max compression
```

## Comparing `satsure_core_test-0.1.6.tar` & `satsure_core_test-0.1.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.965645 satsure_core_test-0.1.6/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.1.6/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 10:13:31.965386 satsure_core_test-0.1.6/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.1.6/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.957699 satsure_core_test-0.1.6/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.1.6/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure_core_test-0.1.6/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.958354 satsure_core_test-0.1.6/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2479 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      733 2024-05-14 15:32:19.000000 satsure_core_test-0.1.6/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.958812 satsure_core_test-0.1.6/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure_core_test-0.1.6/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.959126 satsure_core_test-0.1.6/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.959436 satsure_core_test-0.1.6/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure_core_test-0.1.6/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.961364 satsure_core_test-0.1.6/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      448 2024-05-13 08:48:32.000000 satsure_core_test-0.1.6/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.961658 satsure_core_test-0.1.6/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2829 2024-05-13 07:51:34.000000 satsure_core_test-0.1.6/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.1.6/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure_core_test-0.1.6/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.961967 satsure_core_test-0.1.6/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4041 2024-05-15 10:00:38.000000 satsure_core_test-0.1.6/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2399 2024-05-15 09:34:30.000000 satsure_core_test-0.1.6/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure_core_test-0.1.6/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.962267 satsure_core_test-0.1.6/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.6/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure_core_test-0.1.6/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.964143 satsure_core_test-0.1.6/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.6/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure_core_test-0.1.6/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.1.6/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1020 2024-05-15 10:11:28.000000 satsure_core_test-0.1.6/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure_core_test-0.1.6/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure_core_test-0.1.6/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.964368 satsure_core_test-0.1.6/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure_core_test-0.1.6/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure_core_test-0.1.6/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:13:31.965152 satsure_core_test-0.1.6/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 10:13:31.000000 satsure_core_test-0.1.6/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1566 2024-05-15 10:13:31.000000 satsure_core_test-0.1.6/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-15 10:13:31.000000 satsure_core_test-0.1.6/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      136 2024-05-15 10:13:31.000000 satsure_core_test-0.1.6/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-15 10:13:31.000000 satsure_core_test-0.1.6/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-15 10:13:31.965694 satsure_core_test-0.1.6/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      521 2024-05-15 10:12:39.000000 satsure_core_test-0.1.6/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.984828 satsure_core_test-0.1.7/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.1.7/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 10:42:16.984584 satsure_core_test-0.1.7/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.1.7/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.977098 satsure_core_test-0.1.7/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.1.7/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure_core_test-0.1.7/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.977670 satsure_core_test-0.1.7/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2479 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      733 2024-05-14 15:32:19.000000 satsure_core_test-0.1.7/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.978143 satsure_core_test-0.1.7/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure_core_test-0.1.7/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.978460 satsure_core_test-0.1.7/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.978820 satsure_core_test-0.1.7/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.980829 satsure_core_test-0.1.7/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      448 2024-05-13 08:48:32.000000 satsure_core_test-0.1.7/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.981129 satsure_core_test-0.1.7/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2829 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.1.7/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure_core_test-0.1.7/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.981449 satsure_core_test-0.1.7/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3979 2024-05-15 10:42:04.000000 satsure_core_test-0.1.7/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2399 2024-05-15 09:34:30.000000 satsure_core_test-0.1.7/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.981747 satsure_core_test-0.1.7/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.7/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure_core_test-0.1.7/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.983378 satsure_core_test-0.1.7/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1020 2024-05-15 10:11:28.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.983607 satsure_core_test-0.1.7/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.984357 satsure_core_test-0.1.7/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1566 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      136 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-15 10:42:16.984869 satsure_core_test-0.1.7/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      521 2024-05-15 10:42:15.000000 satsure_core_test-0.1.7/setup.py
```

### Comparing `satsure_core_test-0.1.6/satelite/config.py` & `satsure_core_test-0.1.7/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/core/downloader.py` & `satsure_core_test-0.1.7/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/core/uploader.py` & `satsure_core_test-0.1.7/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/gdal/gdal_commands.py` & `satsure_core_test-0.1.7/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/raster/raster.py` & `satsure_core_test-0.1.7/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure_core_test-0.1.7/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure_core_test-0.1.7/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure_core_test-0.1.7/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/sentinel2/get_tiles.py` & `satsure_core_test-0.1.7/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/sentinel2/indices/general_indices.py` & `satsure_core_test-0.1.7/satelite/sentinel2/indices/general_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,15 @@
 
             date = filename_band_A[0].stem.split(file_name_delimiter)[
                        date_identifier_position][:8]
             index_path = create_normalised_difference_index(
                 filename_band_A[0],
                 filename_band_B[0],
                 output_folder,
-                output_name=f"{date}_{unique_tile}_IS1{band_combination_id}01{file_version}.tif",
-                creation_option="COMPRESS=LZW",
-            )
+                output_name=f"{date}_{unique_tile}_IS1{band_combination_id}01{file_version}.tif")
             if not create_cloud_mask or not index_path:
                 continue
 
             cloud_mask_bands_path = []
             for cloud_mask_band in cloud_mask_bands:
                 cloud_mask_bands_path += list(input_folder.glob(
                     f"*{unique_tile}*{cloud_mask_band}.{input_file_format}"))
```

### Comparing `satsure_core_test-0.1.6/satelite/sentinel2/mosaic_same_bands.py` & `satsure_core_test-0.1.7/satelite/sentinel2/mosaic_same_bands.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/sentinel2/path_row_from_shp.py` & `satsure_core_test-0.1.7/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/sentinel2/s2_l1c_urls.py` & `satsure_core_test-0.1.7/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/sentinel2/s2_l2a_urls.py` & `satsure_core_test-0.1.7/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/tests/conftest.py` & `satsure_core_test-0.1.7/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/tests/sentinel2/test_general_indices.py` & `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/tests/sentinel2/test_get_tile.py` & `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/tests/sentinel2/test_validate.py` & `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satelite/validators/check_shape_of_rid.py` & `satsure_core_test-0.1.7/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/satsure_core_test.egg-info/SOURCES.txt` & `satsure_core_test-0.1.7/satsure_core_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.6/setup.py` & `satsure_core_test-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='satsure-core-test',
-    version='0.1.6',
+    version='0.1.7',
     description='satsure core package',
     author='Satsure',
     author_email='kmstpm@email.com',
     packages=find_packages(),
     install_requires=['awscli', 'fiona','gdal==3.6.2', 'google-cloud-storage', 'pandas',
                       'pyproj',
                       'pystac', 'python-dotenv', 'rasterstats', 'rasterio',
```

