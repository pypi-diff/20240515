# Comparing `tmp/meshiphi-2.0.8.tar.gz` & `tmp/meshiphi-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshiphi-2.0.8.tar", last modified: Thu Apr 25 14:59:18 2024, max compression
+gzip compressed data, was "meshiphi-2.0.9.tar", last modified: Wed May 15 15:08:08 2024, max compression
```

## Comparing `meshiphi-2.0.8.tar` & `meshiphi-2.0.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2023-11-28 10:35:02.000000 meshiphi-2.0.8/LICENSE
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       51 2023-11-28 10:35:02.000000 meshiphi-2.0.8/MANIFEST.in
--rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5140 2024-04-25 14:59:18.947528 meshiphi-2.0.8/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3721 2024-03-06 13:55:59.000000 meshiphi-2.0.8/README.md
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.939529 meshiphi-2.0.8/meshiphi/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      722 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4566 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/cli.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.943529 meshiphi-2.0.8/meshiphi/config_validation/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7230 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/config_validation/config_validator.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1624 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/mesh_schema.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1144 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/route_schema.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      471 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/vessel_schema.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       64 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/waypoints_schema.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.943529 meshiphi-2.0.8/meshiphi/dataloaders/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1196 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/dataloader_interface.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7957 2024-03-06 13:55:59.000000 meshiphi-2.0.8/meshiphi/dataloaders/factory.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.943529 meshiphi-2.0.8/meshiphi/dataloaders/lut/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    15677 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/abstract_lut.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3031 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/density.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2174 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_csv.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2771 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_geojson.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2744 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_shapefile.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1672 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/scotland_ncmpa.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5196 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/thickness.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/dataloaders/scalar/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    39720 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/abstract_scalar.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3831 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/amsr.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1241 2024-03-14 13:28:05.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/baltic_sea_ice.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1584 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/bsose_depth.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2207 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/bsose_sea_ice.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3811 2024-02-22 16:13:29.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/ecmwf_sig_wave_height.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1854 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_max_wave_height.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1843 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_mean_wave_direction.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1855 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_sig_wave_height.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1843 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wave_period.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2053 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wind_dir.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1997 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wind_mag.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1007 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/gebco.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4479 2024-02-22 16:13:29.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/icenet.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1108 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/modis.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      934 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/scalar_csv.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5039 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/scalar_grf.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9724 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/shape.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2874 2024-03-06 13:55:59.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/visual_iced.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/dataloaders/vector/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    48488 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/abstract_vector.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1393 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/baltic_current.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1747 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/duacs_current.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2459 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/era5_wave_direction_vector.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1846 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/era5_wind.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1251 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/north_sea_current.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1331 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/oras5_current.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1271 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/sose.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      934 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/vector_csv.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3828 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/vector_grf.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/mesh_generation/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5456 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/aggregated_cellbox.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    16466 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/boundary.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    16632 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/cellbox.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      367 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/direction.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    66036 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/environment_mesh.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2724 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/jgrid_aggregated_cellbox.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7494 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/jgrid_cellbox.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5342 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/mesh.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    31997 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/mesh_builder.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2751 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/metadata.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    21832 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/neighbour_graph.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/mesh_plotting/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2024-03-06 13:55:59.000000 meshiphi-2.0.8/meshiphi/mesh_plotting/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2839 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_plotting/mesh_plotter.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/mesh_validation/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_validation/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     6913 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_validation/mesh_validator.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1565 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_validation/sampler.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9506 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/utils.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.943529 meshiphi-2.0.8/meshiphi.egg-info/
--rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5140 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3058 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/SOURCES.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/dependency_links.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      149 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/entry_points.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-11-28 10:39:12.000000 meshiphi-2.0.8/meshiphi.egg-info/not-zip-safe
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      169 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/requires.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        9 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/top_level.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       38 2024-04-25 14:59:18.951528 meshiphi-2.0.8/setup.cfg
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1676 2024-04-25 14:59:09.000000 meshiphi-2.0.8/setup.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.075840 meshiphi-2.0.9/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2023-11-28 10:35:02.000000 meshiphi-2.0.9/LICENSE
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       51 2023-11-28 10:35:02.000000 meshiphi-2.0.9/MANIFEST.in
+-rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5140 2024-05-15 15:08:08.075840 meshiphi-2.0.9/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3721 2024-03-06 13:55:59.000000 meshiphi-2.0.9/README.md
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.059840 meshiphi-2.0.9/meshiphi/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      722 2024-05-15 15:07:33.000000 meshiphi-2.0.9/meshiphi/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4566 2024-05-15 12:39:40.000000 meshiphi-2.0.9/meshiphi/cli.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.063840 meshiphi-2.0.9/meshiphi/config_validation/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/config_validation/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7234 2024-05-15 15:07:33.000000 meshiphi-2.0.9/meshiphi/config_validation/config_validator.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1624 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/config_validation/mesh_schema.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1144 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/config_validation/route_schema.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      471 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/config_validation/vessel_schema.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       64 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/config_validation/waypoints_schema.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.063840 meshiphi-2.0.9/meshiphi/dataloaders/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1196 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/dataloader_interface.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7957 2024-05-15 12:39:40.000000 meshiphi-2.0.9/meshiphi/dataloaders/factory.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.063840 meshiphi-2.0.9/meshiphi/dataloaders/lut/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/lut/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    15677 2024-04-30 12:39:04.000000 meshiphi-2.0.9/meshiphi/dataloaders/lut/abstract_lut.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3031 2024-04-30 12:39:04.000000 meshiphi-2.0.9/meshiphi/dataloaders/lut/density.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2174 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/lut/lut_csv.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2771 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/lut/lut_geojson.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2744 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/lut/lut_shapefile.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1672 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/lut/scotland_ncmpa.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5196 2024-04-25 14:57:45.000000 meshiphi-2.0.9/meshiphi/dataloaders/lut/thickness.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.067840 meshiphi-2.0.9/meshiphi/dataloaders/scalar/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    39720 2024-04-30 12:39:04.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/abstract_scalar.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3831 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/amsr.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1241 2024-03-14 13:28:05.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/baltic_sea_ice.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1584 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/bsose_depth.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2207 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/bsose_sea_ice.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3811 2024-02-22 16:13:29.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/ecmwf_sig_wave_height.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1854 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_max_wave_height.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1843 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_mean_wave_direction.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1855 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_sig_wave_height.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1843 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_wave_period.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2053 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_wind_dir.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1997 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_wind_mag.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1007 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/gebco.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4479 2024-02-22 16:13:29.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/icenet.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1108 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/modis.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      934 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/scalar_csv.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5039 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/scalar_grf.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9724 2024-05-15 12:39:40.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/shape.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2874 2024-03-06 13:55:59.000000 meshiphi-2.0.9/meshiphi/dataloaders/scalar/visual_iced.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.071840 meshiphi-2.0.9/meshiphi/dataloaders/vector/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    48488 2024-04-30 12:39:04.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/abstract_vector.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1393 2024-04-25 14:57:45.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/baltic_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1747 2024-04-30 12:39:04.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/duacs_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2459 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/era5_wave_direction_vector.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1846 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/era5_wind.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1251 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/north_sea_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1331 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/oras5_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1271 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/sose.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      934 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/vector_csv.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3828 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/dataloaders/vector/vector_grf.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.075840 meshiphi-2.0.9/meshiphi/mesh_generation/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/mesh_generation/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5456 2024-04-25 14:57:45.000000 meshiphi-2.0.9/meshiphi/mesh_generation/aggregated_cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    17393 2024-05-15 15:07:33.000000 meshiphi-2.0.9/meshiphi/mesh_generation/boundary.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    16632 2024-04-25 14:57:45.000000 meshiphi-2.0.9/meshiphi/mesh_generation/cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      367 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/mesh_generation/direction.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    66036 2024-04-30 12:39:04.000000 meshiphi-2.0.9/meshiphi/mesh_generation/environment_mesh.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2724 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/mesh_generation/jgrid_aggregated_cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7494 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/mesh_generation/jgrid_cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5342 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/mesh_generation/mesh.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    31937 2024-05-15 15:07:33.000000 meshiphi-2.0.9/meshiphi/mesh_generation/mesh_builder.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2751 2024-04-25 14:57:45.000000 meshiphi-2.0.9/meshiphi/mesh_generation/metadata.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    21832 2024-04-30 12:39:04.000000 meshiphi-2.0.9/meshiphi/mesh_generation/neighbour_graph.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.075840 meshiphi-2.0.9/meshiphi/mesh_plotting/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2024-03-06 13:55:59.000000 meshiphi-2.0.9/meshiphi/mesh_plotting/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2839 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/mesh_plotting/mesh_plotter.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.075840 meshiphi-2.0.9/meshiphi/mesh_validation/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/mesh_validation/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     6913 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/mesh_validation/mesh_validator.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1565 2023-11-28 10:35:02.000000 meshiphi-2.0.9/meshiphi/mesh_validation/sampler.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9506 2024-04-30 12:39:04.000000 meshiphi-2.0.9/meshiphi/utils.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-05-15 15:08:08.059840 meshiphi-2.0.9/meshiphi.egg-info/
+-rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5140 2024-05-15 15:08:07.000000 meshiphi-2.0.9/meshiphi.egg-info/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3058 2024-05-15 15:08:08.000000 meshiphi-2.0.9/meshiphi.egg-info/SOURCES.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2024-05-15 15:08:07.000000 meshiphi-2.0.9/meshiphi.egg-info/dependency_links.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      149 2024-05-15 15:08:07.000000 meshiphi-2.0.9/meshiphi.egg-info/entry_points.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-11-28 10:39:12.000000 meshiphi-2.0.9/meshiphi.egg-info/not-zip-safe
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      169 2024-05-15 15:08:07.000000 meshiphi-2.0.9/meshiphi.egg-info/requires.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        9 2024-05-15 15:08:07.000000 meshiphi-2.0.9/meshiphi.egg-info/top_level.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       38 2024-05-15 15:08:08.075840 meshiphi-2.0.9/setup.cfg
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1676 2024-05-15 13:32:49.000000 meshiphi-2.0.9/setup.py
```

### Comparing `meshiphi-2.0.8/LICENSE` & `meshiphi-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/PKG-INFO` & `meshiphi-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshiphi
-Version: 2.0.8
+Version: 2.0.9
 Summary: MeshiPhi: Earth's digital twin mapped on a non-uniform mesh
 Home-page: https://www.github.com/antarctica
 Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
 Author-email: amop@bas.ac.uk
 Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
 Maintainer-email: amop@bas.ac.uk
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meshiphi Version: 2.0.8 Summary: MeshiPhi: Earth's
+Metadata-Version: 2.1 Name: meshiphi Version: 2.0.9 Summary: MeshiPhi: Earth's
 digital twin mapped on a non-uniform mesh Home-page: https://www.github.com/
 antarctica Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab,
 British Antarctic Survey Author-email: amop@bas.ac.uk Maintainer: Autonomous
 Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
 Maintainer-email: amop@bas.ac.uk License: MIT Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
```

### Comparing `meshiphi-2.0.8/README.md` & `meshiphi-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/__init__.py` & `meshiphi-2.0.9/meshiphi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 __description__ = "MeshiPhi: Earth's digital twin mapped on a non-uniform mesh"
 __license__ = "MIT"
 __author__ = "Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey"
 __email__ = "amop@bas.ac.uk"
 __copyright__ = "2021-, BAS AI Lab"
 
 # Wrapped in try-except so that setup.py can import meshiphi without crashing due to dependency errors
```

### Comparing `meshiphi-2.0.8/meshiphi/cli.py` & `meshiphi-2.0.9/meshiphi/cli.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/config_validation/config_validator.py` & `meshiphi-2.0.9/meshiphi/config_validation/config_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         boundary.
 
         Args:
             bound_min (float): Minimum value of boundary in one axis
             bound_max (float): Maximum value of boundary in the same axis
             cell_size (float): Initial cellbox size in the same axis
         """
-        assert(((bound_max - bound_min)/cell_size)%1 == 0), \
+        assert(((bound_max - bound_min)%360/cell_size)%1 == 0), \
             f"{bound_max}-{bound_min}={bound_max-bound_min} is not evenly "+\
             f"divided by {cell_size}"
         
         
     # Deals with flexible input
     config_json = flexi_json_input(config)
     # Validate against the schema to check syntax is correct
```

### Comparing `meshiphi-2.0.8/meshiphi/config_validation/mesh_schema.py` & `meshiphi-2.0.9/meshiphi/config_validation/mesh_schema.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/config_validation/route_schema.py` & `meshiphi-2.0.9/meshiphi/config_validation/route_schema.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/dataloader_interface.py` & `meshiphi-2.0.9/meshiphi/dataloaders/dataloader_interface.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/factory.py` & `meshiphi-2.0.9/meshiphi/dataloaders/factory.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/lut/abstract_lut.py` & `meshiphi-2.0.9/meshiphi/dataloaders/lut/abstract_lut.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/lut/density.py` & `meshiphi-2.0.9/meshiphi/dataloaders/lut/density.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_csv.py` & `meshiphi-2.0.9/meshiphi/dataloaders/lut/lut_csv.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_geojson.py` & `meshiphi-2.0.9/meshiphi/dataloaders/lut/lut_geojson.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_shapefile.py` & `meshiphi-2.0.9/meshiphi/dataloaders/lut/lut_shapefile.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/lut/scotland_ncmpa.py` & `meshiphi-2.0.9/meshiphi/dataloaders/lut/scotland_ncmpa.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/lut/thickness.py` & `meshiphi-2.0.9/meshiphi/dataloaders/lut/thickness.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/abstract_scalar.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/abstract_scalar.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/amsr.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/amsr.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/baltic_sea_ice.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/baltic_sea_ice.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/bsose_depth.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/bsose_depth.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/bsose_sea_ice.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/bsose_sea_ice.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/ecmwf_sig_wave_height.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/ecmwf_sig_wave_height.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_max_wave_height.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_max_wave_height.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_mean_wave_direction.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_mean_wave_direction.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_sig_wave_height.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_sig_wave_height.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wave_period.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_wave_period.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wind_dir.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_wind_dir.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wind_mag.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/era5_wind_mag.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/gebco.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/gebco.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/icenet.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/icenet.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/modis.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/modis.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/scalar_csv.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/scalar_csv.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/scalar_grf.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/scalar_grf.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/shape.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/shape.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/scalar/visual_iced.py` & `meshiphi-2.0.9/meshiphi/dataloaders/scalar/visual_iced.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/abstract_vector.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/abstract_vector.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/baltic_current.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/baltic_current.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/duacs_current.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/duacs_current.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/era5_wave_direction_vector.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/era5_wave_direction_vector.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/era5_wind.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/era5_wind.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/north_sea_current.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/north_sea_current.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/oras5_current.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/oras5_current.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/sose.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/sose.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/vector_csv.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/vector_csv.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/dataloaders/vector/vector_grf.py` & `meshiphi-2.0.9/meshiphi/dataloaders/vector/vector_grf.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/aggregated_cellbox.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/aggregated_cellbox.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/boundary.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/boundary.py`

 * *Files 9% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             returns the min longtitude
         """
         return self.long_range[0]
     def get_long_max(self):
         """
             returns the max longtitude
         """
-        return self.long_range[1]  
+        return self.long_range[1]
     def get_time_min(self):
         """
             returns the min of time range
         """
         return self.time_range[0]
     def get_time_max(self):
         """
@@ -330,24 +330,40 @@
         rectangle in mercator projection.
         
         Returns:
             (shapely.geometry.polygon.Polygon):
                 Shapely polygon with corners at the min/max lat/long 
                 values of this boundary
         """
-        # If not going over the antimeridian
+        # If boundary not going over the antimeridian
         if self.get_long_min() < self.get_long_max():
             # Create a polygon of boundary
             polygon = wkt.loads(
                         f'POLYGON(({self.get_long_min()} {self.get_lat_min()},' + \
                                 f'{self.get_long_min()} {self.get_lat_max()},' + \
                                 f'{self.get_long_max()} {self.get_lat_max()},' + \
                                 f'{self.get_long_max()} {self.get_lat_min()},' + \
                                 f'{self.get_long_min()} {self.get_lat_min()}))'
                 )
+        elif self.get_long_min() == 180:
+            polygon = wkt.loads(
+                        f'POLYGON((-180 {self.get_lat_min()},' + \
+                                f'-180 {self.get_lat_max()},' + \
+                                f'{self.get_long_max()} {self.get_lat_max()},' + \
+                                f'{self.get_long_max()} {self.get_lat_min()},' + \
+                                f'-180 {self.get_lat_min()}))'
+                )
+        elif self.get_long_max() == -180:
+            polygon = wkt.loads(
+                        f'POLYGON(({self.get_long_min()} {self.get_lat_min()},' + \
+                                f'{self.get_long_min()} {self.get_lat_max()},' + \
+                                f'180 {self.get_lat_max()},' + \
+                                f'180 {self.get_lat_min()},' + \
+                                f'{self.get_long_min()} {self.get_lat_min()}))'
+            )
         else:
             # Create a multipolygon of boundary
             polygon_1 = wkt.loads(
                         f'POLYGON(({self.get_long_min()} {self.get_lat_min()},' + \
                                 f'{self.get_long_min()} {self.get_lat_max()},' + \
                                 f'180 {self.get_lat_max()},' + \
                                 f'180 {self.get_lat_min()},' + \
```

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/cellbox.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/cellbox.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/environment_mesh.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/environment_mesh.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/jgrid_aggregated_cellbox.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/jgrid_aggregated_cellbox.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/jgrid_cellbox.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/jgrid_cellbox.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/mesh.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/mesh.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/mesh_builder.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/mesh_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,16 @@
 
         logging.info("Initialising mesh...")
         logging.info("Initialising cellboxes...")
      
         cellboxes = []
         cellboxes = self.initialize_cellboxes(bounds, cell_width, cell_height)
         
-        # Account for going over the antimeridian with longitude_distance        
-        grid_width = np.divide(bounds.get_long_max() - bounds.get_long_min(),
-                               cell_width)
+        # Calculate width of mesh in cell-coordinates rather than degrees
+        grid_width = np.divide(bounds.get_width(), cell_width)
         
         min_datapoints = 5
         if 'splitting' in self.config:
             min_datapoints = self.config['splitting']['minimum_datapoints']
         meta_data_list = self.initialize_meta_data(bounds, min_datapoints)
 
         # Initialise the metadata for each cellbox, including subsets of each
@@ -333,15 +332,15 @@
                 cellbox.set_data_source(
                     cellbox.get_data_source() + [meta_data_obj]
                 )
 
         
 
     def validate_bounds(self, bounds, cell_width, cell_height):
-        assert (bounds.get_long_max() - bounds.get_long_min()) % cell_width == 0, \
+        assert (bounds.get_long_max() - bounds.get_long_min()) % 360 % cell_width == 0, \
             f"""The defined longitude region <{bounds.get_long_min()} :{bounds.get_long_max()}>
             is not divisable by the initial cell width <{cell_width}>"""
 
         assert (bounds.get_lat_max() - bounds.get_lat_min()) % cell_height == 0, \
             f"""The defined longitude region <{bounds.get_lat_min()} :{bounds.get_lat_max()}>
             is not divisable by the initial cell width <{cell_height}>"""
```

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/metadata.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/metadata.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_generation/neighbour_graph.py` & `meshiphi-2.0.9/meshiphi/mesh_generation/neighbour_graph.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_plotting/mesh_plotter.py` & `meshiphi-2.0.9/meshiphi/mesh_plotting/mesh_plotter.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_validation/mesh_validator.py` & `meshiphi-2.0.9/meshiphi/mesh_validation/mesh_validator.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/mesh_validation/sampler.py` & `meshiphi-2.0.9/meshiphi/mesh_validation/sampler.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi/utils.py` & `meshiphi-2.0.9/meshiphi/utils.py`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/meshiphi.egg-info/PKG-INFO` & `meshiphi-2.0.9/meshiphi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshiphi
-Version: 2.0.8
+Version: 2.0.9
 Summary: MeshiPhi: Earth's digital twin mapped on a non-uniform mesh
 Home-page: https://www.github.com/antarctica
 Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
 Author-email: amop@bas.ac.uk
 Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
 Maintainer-email: amop@bas.ac.uk
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meshiphi Version: 2.0.8 Summary: MeshiPhi: Earth's
+Metadata-Version: 2.1 Name: meshiphi Version: 2.0.9 Summary: MeshiPhi: Earth's
 digital twin mapped on a non-uniform mesh Home-page: https://www.github.com/
 antarctica Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab,
 British Antarctic Survey Author-email: amop@bas.ac.uk Maintainer: Autonomous
 Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
 Maintainer-email: amop@bas.ac.uk License: MIT Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
```

### Comparing `meshiphi-2.0.8/meshiphi.egg-info/SOURCES.txt` & `meshiphi-2.0.9/meshiphi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshiphi-2.0.8/setup.py` & `meshiphi-2.0.9/setup.py`

 * *Files identical despite different names*

