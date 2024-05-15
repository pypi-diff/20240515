# Comparing `tmp/satsure_core_test-0.1.7.tar.gz` & `tmp/satsure_core_test-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure_core_test-0.1.7.tar", last modified: Wed May 15 10:42:16 2024, max compression
+gzip compressed data, was "satsure_core_test-0.1.8.tar", last modified: Wed May 15 14:32:44 2024, max compression
```

## Comparing `satsure_core_test-0.1.7.tar` & `satsure_core_test-0.1.8.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.984828 satsure_core_test-0.1.7/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.1.7/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 10:42:16.984584 satsure_core_test-0.1.7/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.1.7/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.977098 satsure_core_test-0.1.7/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.1.7/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure_core_test-0.1.7/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.977670 satsure_core_test-0.1.7/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2479 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      733 2024-05-14 15:32:19.000000 satsure_core_test-0.1.7/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.978143 satsure_core_test-0.1.7/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure_core_test-0.1.7/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.978460 satsure_core_test-0.1.7/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.978820 satsure_core_test-0.1.7/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.980829 satsure_core_test-0.1.7/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      448 2024-05-13 08:48:32.000000 satsure_core_test-0.1.7/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.981129 satsure_core_test-0.1.7/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2829 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.1.7/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure_core_test-0.1.7/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.981449 satsure_core_test-0.1.7/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3979 2024-05-15 10:42:04.000000 satsure_core_test-0.1.7/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2399 2024-05-15 09:34:30.000000 satsure_core_test-0.1.7/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.981747 satsure_core_test-0.1.7/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.7/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure_core_test-0.1.7/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.983378 satsure_core_test-0.1.7/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1020 2024-05-15 10:11:28.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure_core_test-0.1.7/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.983607 satsure_core_test-0.1.7/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure_core_test-0.1.7/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 10:42:16.984357 satsure_core_test-0.1.7/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1566 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      136 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-15 10:42:16.000000 satsure_core_test-0.1.7/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-15 10:42:16.984869 satsure_core_test-0.1.7/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      521 2024-05-15 10:42:15.000000 satsure_core_test-0.1.7/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.081534 satsure_core_test-0.1.8/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.1.8/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 14:32:44.081232 satsure_core_test-0.1.8/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.1.8/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.071508 satsure_core_test-0.1.8/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.1.8/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure_core_test-0.1.8/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.072074 satsure_core_test-0.1.8/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4982 2024-05-15 14:05:41.000000 satsure_core_test-0.1.8/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      733 2024-05-14 15:32:19.000000 satsure_core_test-0.1.8/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.072552 satsure_core_test-0.1.8/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure_core_test-0.1.8/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.072924 satsure_core_test-0.1.8/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.073365 satsure_core_test-0.1.8/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure_core_test-0.1.8/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.075813 satsure_core_test-0.1.8/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      448 2024-05-13 08:48:32.000000 satsure_core_test-0.1.8/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.076135 satsure_core_test-0.1.8/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-15 12:28:03.000000 satsure_core_test-0.1.8/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.1.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure_core_test-0.1.8/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.076499 satsure_core_test-0.1.8/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-15 12:01:41.000000 satsure_core_test-0.1.8/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-15 14:22:44.000000 satsure_core_test-0.1.8/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2362 2024-05-15 14:15:25.000000 satsure_core_test-0.1.8/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure_core_test-0.1.8/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.076817 satsure_core_test-0.1.8/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.8/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure_core_test-0.1.8/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.079446 satsure_core_test-0.1.8/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-15 12:53:42.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1305 2024-05-15 12:55:00.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure_core_test-0.1.8/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.079687 satsure_core_test-0.1.8/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure_core_test-0.1.8/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure_core_test-0.1.8/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 14:32:44.080894 satsure_core_test-0.1.8/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 14:32:44.000000 satsure_core_test-0.1.8/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1661 2024-05-15 14:32:44.000000 satsure_core_test-0.1.8/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-15 14:32:44.000000 satsure_core_test-0.1.8/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      136 2024-05-15 14:32:44.000000 satsure_core_test-0.1.8/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-15 14:32:44.000000 satsure_core_test-0.1.8/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-15 14:32:44.081599 satsure_core_test-0.1.8/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      521 2024-05-15 14:31:09.000000 satsure_core_test-0.1.8/setup.py
```

### Comparing `satsure_core_test-0.1.7/satelite/config.py` & `satsure_core_test-0.1.8/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/core/uploader.py` & `satsure_core_test-0.1.8/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/gdal/gdal_commands.py` & `satsure_core_test-0.1.8/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/raster/raster.py` & `satsure_core_test-0.1.8/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure_core_test-0.1.8/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             files = []
             for band in self.bands:
                 files += list(input_folder.glob(
                     f"*{unique_tile}*{band}*.{input_file_format}"))
             if files:
                 date = files[0].stem.split(file_name_delimiter)[
                            date_identifier_position][:8]
-                output_folder = Path(self.output_folder / unique_tile)
+                output_folder = Path(f"{self.output_folder}/{unique_tile}")
                 fcc_path = merge(
                     files,
                     output_folder=output_folder,
                     output_name=f"{date}_{unique_tile}_IS{len(files)}{band_combination_id}01{file_version}.tif",
                     output_nodata_value=0,
                     keep_separate=True,
                     output_format="COG",
```

### Comparing `satsure_core_test-0.1.7/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure_core_test-0.1.8/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure_core_test-0.1.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/sentinel2/get_tiles.py` & `satsure_core_test-0.1.8/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/sentinel2/indices/general_indices.py` & `satsure_core_test-0.1.8/satelite/sentinel2/indices/general_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,18 @@
                 f"*{unique_tile}*{band_A_identifier}*.{input_file_format}"))
             filename_band_B = list(input_folder.glob(
                 f"*{unique_tile}*{band_B_identifier}*.{input_file_format}"))
 
             if not filename_band_A or not filename_band_B:
                 continue
 
-            output_folder = Path(f"{self.output_folder} / {unique_tile}")
+            output_folder = Path(f"{self.output_folder}/{unique_tile}")
             if cloud_mask_output_folder:
                 cloud_mask_output_folder = Path(
-                    f"{cloud_mask_output_folder} / {unique_tile}")
+                    f"{cloud_mask_output_folder}/{unique_tile}")
 
             date = filename_band_A[0].stem.split(file_name_delimiter)[
                        date_identifier_position][:8]
             index_path = create_normalised_difference_index(
                 filename_band_A[0],
                 filename_band_B[0],
                 output_folder,
```

### Comparing `satsure_core_test-0.1.7/satelite/sentinel2/mosaic_same_bands.py` & `satsure_core_test-0.1.8/satelite/sentinel2/mosaic_same_bands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from collections.abc import Iterable
 from pathlib import Path, PosixPath
+from typing import List
 
 from satelite.raster.raster import merge
-from typing import  List
+
 
 class MosaicSameBands:
     """
     Stack similar bands on same date
     """
     BANDS = ("B02", "B03", "B04", "B05", "B08", "B12",)
```

### Comparing `satsure_core_test-0.1.7/satelite/sentinel2/path_row_from_shp.py` & `satsure_core_test-0.1.8/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/sentinel2/s2_l1c_urls.py` & `satsure_core_test-0.1.8/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/sentinel2/s2_l2a_urls.py` & `satsure_core_test-0.1.8/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/tests/conftest.py` & `satsure_core_test-0.1.8/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_general_indices.py` & `satsure_core_test-0.1.8/satelite/tests/sentinel2/test_general_indices.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,39 @@
+import glob
+import os
 from pathlib import Path
 
-from satelite.sentinel2.indices.general_indices import GeneralIndices
-
 import pytest
 
+from satelite.sentinel2.indices.general_indices import GeneralIndices
+
 
-@pytest.skip("need to rewrite")
+@pytest.mark.skip("need to add tiff files")
 class TestGeneralIndices:
+    """Testcase for General Indices """
 
     def test_general_indices(self):
-        base_path = "/home/ubuntu/"
-        date = "2024-03-29"
-        level = "L2A"
-        input_folder = Path(base_path, level, date.replace("-", ""))
+        """ test
+
+        :return:
+        """
+        base_path = "/Users/meenakshisundaram/Documents/airflow-dags-file"
+        input_folder = Path(base_path)
         product_code = "IS18021"
         params = {'band_A_identifier': 'B04', 'band_B_identifier': 'B08',
                   'tile_identifier_position': 1, 'file_name_delimiter': '_',
                   'date_identifier_position': 0, 'band_combination_id': '8',
                   'input_file_format': 'tif',
                   'cloud_mask_bands': ('B02', 'B03'),
                   'cloud_mask_threshold': (3600, 3800),
                   'cloud_mask_output_folder': 'IS18021', 'file_version': '1'}
 
-        obj = GeneralIndices(input_folder, f"{base_path} / {product_code}",
-                             "L2a")
+        obj = GeneralIndices(input_folder, f"{base_path}/{product_code}",
+                             "L2A")
         obj.create_s2_normalised_index(**params)
+
+        pattern = os.path.join(
+            '/Users/meenakshisundaram/Documents/airflow-dags-file/IS18021/T43PCT/',
+            "*.tif")
+        result = glob.glob(pattern)
+
+        assert len(result) == 1
```

### Comparing `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_get_tile.py` & `satsure_core_test-0.1.8/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure_core_test-0.1.8/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure_core_test-0.1.8/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/tests/sentinel2/test_validate.py` & `satsure_core_test-0.1.8/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satelite/validators/check_shape_of_rid.py` & `satsure_core_test-0.1.8/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.1.7/satsure_core_test.egg-info/SOURCES.txt` & `satsure_core_test-0.1.8/satsure_core_test.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,29 @@
 satelite/models/s2_enum.py
 satelite/raster/__init__.py
 satelite/raster/raster.py
 satelite/sentinel2/__init__.py
 satelite/sentinel2/fetch_unique_tile_date.py
 satelite/sentinel2/fetch_unique_tile_date_pystac.py
 satelite/sentinel2/get_tiles.py
+satelite/sentinel2/mosaic_custom_bands.py
 satelite/sentinel2/mosaic_same_bands.py
 satelite/sentinel2/path_row_from_shp.py
 satelite/sentinel2/s2_l1c_urls.py
 satelite/sentinel2/s2_l2a_urls.py
 satelite/sentinel2/band_stack/__init__.py
 satelite/sentinel2/band_stack/generate_band_stack.py
 satelite/sentinel2/indices/__init__.py
 satelite/sentinel2/indices/general_indices.py
 satelite/tests/__init__.py
 satelite/tests/conftest.py
 satelite/tests/sentinel2/__init__.py
 satelite/tests/sentinel2/test_fetch_unique_tile_date.py
 satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+satelite/tests/sentinel2/test_genarate_band_stack.py
 satelite/tests/sentinel2/test_general_indices.py
 satelite/tests/sentinel2/test_get_tile.py
 satelite/tests/sentinel2/test_mosaic_same_bands.py
 satelite/tests/sentinel2/test_s2_l1c_urls.py
 satelite/tests/sentinel2/test_s2_l2a_urls.py
 satelite/tests/sentinel2/test_validate.py
 satelite/validators/__init__.py
```

### Comparing `satsure_core_test-0.1.7/setup.py` & `satsure_core_test-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='satsure-core-test',
-    version='0.1.7',
+    version='0.1.8',
     description='satsure core package',
     author='Satsure',
     author_email='kmstpm@email.com',
     packages=find_packages(),
     install_requires=['awscli', 'fiona','gdal==3.6.2', 'google-cloud-storage', 'pandas',
                       'pyproj',
                       'pystac', 'python-dotenv', 'rasterstats', 'rasterio',
```

