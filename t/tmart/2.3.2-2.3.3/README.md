# Comparing `tmp/tmart-2.3.2.tar.gz` & `tmp/tmart-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmart-2.3.2.tar", last modified: Fri Apr 26 02:50:50 2024, max compression
+gzip compressed data, was "tmart-2.3.3.tar", last modified: Wed May 15 14:58:02 2024, max compression
```

## Comparing `tmart-2.3.2.tar` & `tmart-2.3.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.427745 tmart-2.3.2/
--rw-r--r--   0 yw         (501) staff       (20)       51 2023-10-19 15:57:58.000000 tmart-2.3.2/MANIFEST.in
--rw-r--r--   0 yw         (501) staff       (20)     5181 2024-04-26 02:50:50.427512 tmart-2.3.2/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     4334 2024-04-11 20:04:30.000000 tmart-2.3.2/README.md
--rw-r--r--   0 yw         (501) staff       (20)       38 2024-04-26 02:50:50.427799 tmart-2.3.2/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)     2045 2024-04-26 02:49:16.000000 tmart-2.3.2/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.408933 tmart-2.3.2/tests/
--rwxrwxrwx   0 yw         (501) staff       (20)      413 2023-10-19 16:51:10.000000 tmart-2.3.2/tests/test_AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     2960 2023-05-23 22:19:27.000000 tmart-2.3.2/tests/test_AE_modelling.py
--rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-2.3.2/tests/test_E_diffuse.py
--rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-2.3.2/tests/test_L_sky.py
--rw-r--r--   0 yw         (501) staff       (20)     2569 2024-01-30 23:00:00.000000 tmart-2.3.2/tests/test_basic.py
--rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-2.3.2/tests/test_basic_import.py
--rw-r--r--   0 yw         (501) staff       (20)      824 2023-05-26 03:52:15.000000 tmart-2.3.2/tests/test_calc_rho.py
--rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-2.3.2/tests/test_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     1172 2023-05-26 22:25:30.000000 tmart-2.3.2/tests/test_fresnel.py
--rwxrwxrwx   0 yw         (501) staff       (20)     1489 2023-10-19 16:51:11.000000 tmart-2.3.2/tests/test_modelling.py
--rw-r--r--   0 yw         (501) staff       (20)     2047 2024-04-11 14:38:23.000000 tmart-2.3.2/tests/test_plot.py
--rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-2.3.2/tests/test_quickstart.py
--rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-2.3.2/tests/test_specular_contribution.py
--rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-2.3.2/tests/test_typical_ocean.py
--rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-2.3.2/tests/test_whales_SR.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.411898 tmart-2.3.2/tmart/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.418206 tmart-2.3.2/tmart/AEC/
--rw-r--r--   0 yw         (501) staff       (20)     9444 2024-03-28 18:17:03.000000 tmart-2.3.2/tmart/AEC/AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     1016 2024-03-28 20:07:38.000000 tmart-2.3.2/tmart/AEC/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     1758 2023-10-20 19:50:31.000000 tmart-2.3.2/tmart/AEC/anci_download.py
--rw-r--r--   0 yw         (501) staff       (20)     3546 2024-03-10 16:18:02.000000 tmart-2.3.2/tmart/AEC/anci_get_AER.py
--rw-r--r--   0 yw         (501) staff       (20)     2383 2024-03-10 16:16:52.000000 tmart-2.3.2/tmart/AEC/anci_get_OWV.py
--rw-r--r--   0 yw         (501) staff       (20)     1788 2024-03-10 16:16:09.000000 tmart-2.3.2/tmart/AEC/anci_list_files.py
--rw-r--r--   0 yw         (501) staff       (20)     1628 2024-03-10 16:14:25.000000 tmart-2.3.2/tmart/AEC/compute_gas_transmittance.py
--rw-r--r--   0 yw         (501) staff       (20)     9844 2024-03-28 18:15:37.000000 tmart-2.3.2/tmart/AEC/compute_masks.py
--rw-r--r--   0 yw         (501) staff       (20)      648 2023-10-18 00:57:41.000000 tmart-2.3.2/tmart/AEC/fillnan.py
--rw-r--r--   0 yw         (501) staff       (20)     9982 2024-03-10 16:15:20.000000 tmart-2.3.2/tmart/AEC/get_AOT.py
--rw-r--r--   0 yw         (501) staff       (20)     1579 2023-12-14 02:45:52.000000 tmart-2.3.2/tmart/AEC/get_ancillary.py
--rw-r--r--   0 yw         (501) staff       (20)     6588 2024-03-10 16:17:43.000000 tmart-2.3.2/tmart/AEC/get_parameters.py
--rw-r--r--   0 yw         (501) staff       (20)      995 2024-03-10 16:16:22.000000 tmart-2.3.2/tmart/AEC/identify_sensor.py
--rw-r--r--   0 yw         (501) staff       (20)     4553 2024-03-10 16:14:57.000000 tmart-2.3.2/tmart/AEC/irradiance_correction.py
--rw-r--r--   0 yw         (501) staff       (20)     1184 2024-01-11 18:18:13.000000 tmart-2.3.2/tmart/AEC/read_PRISMA_north.py
--rw-r--r--   0 yw         (501) staff       (20)     2886 2023-10-18 01:13:05.000000 tmart-2.3.2/tmart/AEC/read_PRISMA_vaa.py
--rw-r--r--   0 yw         (501) staff       (20)     1060 2024-03-10 16:17:04.000000 tmart-2.3.2/tmart/AEC/read_config.py
--rw-r--r--   0 yw         (501) staff       (20)    11907 2024-03-28 21:59:35.000000 tmart-2.3.2/tmart/AEC/read_metadata_Landsat.py
--rw-r--r--   0 yw         (501) staff       (20)     6684 2024-03-10 16:17:00.000000 tmart-2.3.2/tmart/AEC/read_metadata_S2.py
--rw-r--r--   0 yw         (501) staff       (20)     2036 2023-10-18 01:15:47.000000 tmart-2.3.2/tmart/AEC/read_xml_S2.py
--rw-r--r--   0 yw         (501) staff       (20)     1331 2023-10-18 01:14:23.000000 tmart-2.3.2/tmart/AEC/read_xml_S2_scene.py
--rw-r--r--   0 yw         (501) staff       (20)     4979 2024-04-26 02:46:10.000000 tmart-2.3.2/tmart/AEC/run.py
--rw-r--r--   0 yw         (501) staff       (20)    12107 2024-04-26 02:47:20.000000 tmart-2.3.2/tmart/AEC/run_acoliteL1R.py
--rw-r--r--   0 yw         (501) staff       (20)     2780 2024-04-26 02:47:20.000000 tmart-2.3.2/tmart/AEC/run_regular.py
--rw-r--r--   0 yw         (501) staff       (20)     1144 2024-01-11 21:20:16.000000 tmart-2.3.2/tmart/AEC/write_atm_info.py
--rw-r--r--   0 yw         (501) staff       (20)     1811 2024-01-18 16:28:44.000000 tmart-2.3.2/tmart/Aerosol.py
--rw-r--r--   0 yw         (501) staff       (20)    11377 2024-03-10 16:08:40.000000 tmart-2.3.2/tmart/Atmosphere.py
--rw-r--r--   0 yw         (501) staff       (20)     9961 2024-01-18 16:27:41.000000 tmart-2.3.2/tmart/Surface.py
--rw-r--r--   0 yw         (501) staff       (20)    13680 2024-01-18 16:35:11.000000 tmart-2.3.2/tmart/Tmart.py
--rw-r--r--   0 yw         (501) staff       (20)    38594 2024-04-11 14:37:47.000000 tmart-2.3.2/tmart/Tmart2.py
--rw-r--r--   0 yw         (501) staff       (20)      550 2023-12-28 20:42:03.000000 tmart-2.3.2/tmart/__init__.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.420518 tmart-2.3.2/tmart/ancillary/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.425917 tmart-2.3.2/tmart/ancillary/aerosolSPF/
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/BiomassBurning.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Continental.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Desert.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Maritime.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Stratospheric.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-2.3.2/tmart/ancillary/aerosolSPF/Urban.csv
--rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-2.3.2/tmart/ancillary/conifer_forest.csv
--rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-2.3.2/tmart/ancillary/dry_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-2.3.2/tmart/ancillary/lawn_grass.csv
--rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-2.3.2/tmart/ancillary/soil.csv
--rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-2.3.2/tmart/ancillary/vegetation.csv
--rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-2.3.2/tmart/ancillary/water.csv
--rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-2.3.2/tmart/ancillary/water_chl1.csv
--rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-2.3.2/tmart/ancillary/wet_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-2.3.2/tmart/ancillary/whitecap_factor.csv
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.426659 tmart-2.3.2/tmart/config/
--rw-r--r--   0 yw         (501) staff       (20)     1303 2024-03-28 18:02:22.000000 tmart-2.3.2/tmart/config/config.txt
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.427163 tmart-2.3.2/tmart/surface_rho/
--rw-r--r--   0 yw         (501) staff       (20)      341 2023-05-23 22:27:30.000000 tmart-2.3.2/tmart/surface_rho/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     5038 2023-05-26 07:42:38.000000 tmart-2.3.2/tmart/surface_rho/calculate.py
--rw-r--r--   0 yw         (501) staff       (20)     2003 2024-03-10 16:10:22.000000 tmart-2.3.2/tmart/tm_OT.py
--rw-r--r--   0 yw         (501) staff       (20)     3195 2024-01-18 16:28:32.000000 tmart-2.3.2/tmart/tm_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     3976 2024-03-10 16:09:31.000000 tmart-2.3.2/tmart/tm_geometry.py
--rw-r--r--   0 yw         (501) staff       (20)    12883 2024-03-10 16:09:57.000000 tmart-2.3.2/tmart/tm_intersect.py
--rw-r--r--   0 yw         (501) staff       (20)    11243 2024-03-10 16:10:06.000000 tmart-2.3.2/tmart/tm_move.py
--rw-r--r--   0 yw         (501) staff       (20)     6748 2024-01-18 16:33:59.000000 tmart-2.3.2/tmart/tm_sampling.py
--rw-r--r--   0 yw         (501) staff       (20)    12104 2024-04-11 14:31:53.000000 tmart-2.3.2/tmart/tm_water.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 02:50:50.412685 tmart-2.3.2/tmart.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)     5181 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     2067 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       70 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)        6 2024-04-26 02:50:50.000000 tmart-2.3.2/tmart.egg-info/top_level.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-15 14:58:02.318033 tmart-2.3.3/
+-rw-r--r--   0 yw         (501) staff       (20)       51 2023-10-19 15:57:58.000000 tmart-2.3.3/MANIFEST.in
+-rw-r--r--   0 yw         (501) staff       (20)     5181 2024-05-15 14:58:02.317736 tmart-2.3.3/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     4334 2024-04-11 20:04:30.000000 tmart-2.3.3/README.md
+-rw-r--r--   0 yw         (501) staff       (20)       38 2024-05-15 14:58:02.318098 tmart-2.3.3/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)     2045 2024-05-15 14:56:32.000000 tmart-2.3.3/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-15 14:58:02.292050 tmart-2.3.3/tests/
+-rwxrwxrwx   0 yw         (501) staff       (20)      413 2023-10-19 16:51:10.000000 tmart-2.3.3/tests/test_AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     2960 2023-05-23 22:19:27.000000 tmart-2.3.3/tests/test_AE_modelling.py
+-rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-2.3.3/tests/test_E_diffuse.py
+-rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-2.3.3/tests/test_L_sky.py
+-rw-r--r--   0 yw         (501) staff       (20)     2569 2024-01-30 23:00:00.000000 tmart-2.3.3/tests/test_basic.py
+-rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-2.3.3/tests/test_basic_import.py
+-rw-r--r--   0 yw         (501) staff       (20)      824 2023-05-26 03:52:15.000000 tmart-2.3.3/tests/test_calc_rho.py
+-rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-2.3.3/tests/test_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     1172 2023-05-26 22:25:30.000000 tmart-2.3.3/tests/test_fresnel.py
+-rwxrwxrwx   0 yw         (501) staff       (20)     1489 2023-10-19 16:51:11.000000 tmart-2.3.3/tests/test_modelling.py
+-rw-r--r--   0 yw         (501) staff       (20)     2047 2024-04-11 14:38:23.000000 tmart-2.3.3/tests/test_plot.py
+-rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-2.3.3/tests/test_quickstart.py
+-rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-2.3.3/tests/test_specular_contribution.py
+-rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-2.3.3/tests/test_typical_ocean.py
+-rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-2.3.3/tests/test_whales_SR.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-15 14:58:02.296508 tmart-2.3.3/tmart/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-15 14:58:02.306956 tmart-2.3.3/tmart/AEC/
+-rw-r--r--   0 yw         (501) staff       (20)     9500 2024-05-15 14:54:57.000000 tmart-2.3.3/tmart/AEC/AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     1016 2024-03-28 20:07:38.000000 tmart-2.3.3/tmart/AEC/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     1758 2023-10-20 19:50:31.000000 tmart-2.3.3/tmart/AEC/anci_download.py
+-rw-r--r--   0 yw         (501) staff       (20)     3546 2024-03-10 16:18:02.000000 tmart-2.3.3/tmart/AEC/anci_get_AER.py
+-rw-r--r--   0 yw         (501) staff       (20)     2383 2024-03-10 16:16:52.000000 tmart-2.3.3/tmart/AEC/anci_get_OWV.py
+-rw-r--r--   0 yw         (501) staff       (20)     1788 2024-03-10 16:16:09.000000 tmart-2.3.3/tmart/AEC/anci_list_files.py
+-rw-r--r--   0 yw         (501) staff       (20)     1628 2024-03-10 16:14:25.000000 tmart-2.3.3/tmart/AEC/compute_gas_transmittance.py
+-rw-r--r--   0 yw         (501) staff       (20)     9844 2024-03-28 18:15:37.000000 tmart-2.3.3/tmart/AEC/compute_masks.py
+-rw-r--r--   0 yw         (501) staff       (20)      648 2023-10-18 00:57:41.000000 tmart-2.3.3/tmart/AEC/fillnan.py
+-rw-r--r--   0 yw         (501) staff       (20)     9982 2024-03-10 16:15:20.000000 tmart-2.3.3/tmart/AEC/get_AOT.py
+-rw-r--r--   0 yw         (501) staff       (20)     1579 2023-12-14 02:45:52.000000 tmart-2.3.3/tmart/AEC/get_ancillary.py
+-rw-r--r--   0 yw         (501) staff       (20)     6588 2024-03-10 16:17:43.000000 tmart-2.3.3/tmart/AEC/get_parameters.py
+-rw-r--r--   0 yw         (501) staff       (20)      995 2024-03-10 16:16:22.000000 tmart-2.3.3/tmart/AEC/identify_sensor.py
+-rw-r--r--   0 yw         (501) staff       (20)     4553 2024-03-10 16:14:57.000000 tmart-2.3.3/tmart/AEC/irradiance_correction.py
+-rw-r--r--   0 yw         (501) staff       (20)     1184 2024-01-11 18:18:13.000000 tmart-2.3.3/tmart/AEC/read_PRISMA_north.py
+-rw-r--r--   0 yw         (501) staff       (20)     2886 2023-10-18 01:13:05.000000 tmart-2.3.3/tmart/AEC/read_PRISMA_vaa.py
+-rw-r--r--   0 yw         (501) staff       (20)     1060 2024-03-10 16:17:04.000000 tmart-2.3.3/tmart/AEC/read_config.py
+-rw-r--r--   0 yw         (501) staff       (20)    11907 2024-03-28 21:59:35.000000 tmart-2.3.3/tmart/AEC/read_metadata_Landsat.py
+-rw-r--r--   0 yw         (501) staff       (20)     6684 2024-03-10 16:17:00.000000 tmart-2.3.3/tmart/AEC/read_metadata_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)     2036 2023-10-18 01:15:47.000000 tmart-2.3.3/tmart/AEC/read_xml_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)     1331 2023-10-18 01:14:23.000000 tmart-2.3.3/tmart/AEC/read_xml_S2_scene.py
+-rw-r--r--   0 yw         (501) staff       (20)     4979 2024-04-26 02:46:10.000000 tmart-2.3.3/tmart/AEC/run.py
+-rw-r--r--   0 yw         (501) staff       (20)    12107 2024-04-26 02:47:20.000000 tmart-2.3.3/tmart/AEC/run_acoliteL1R.py
+-rw-r--r--   0 yw         (501) staff       (20)     2780 2024-04-26 02:47:20.000000 tmart-2.3.3/tmart/AEC/run_regular.py
+-rw-r--r--   0 yw         (501) staff       (20)     1144 2024-01-11 21:20:16.000000 tmart-2.3.3/tmart/AEC/write_atm_info.py
+-rw-r--r--   0 yw         (501) staff       (20)     1811 2024-01-18 16:28:44.000000 tmart-2.3.3/tmart/Aerosol.py
+-rw-r--r--   0 yw         (501) staff       (20)    11377 2024-03-10 16:08:40.000000 tmart-2.3.3/tmart/Atmosphere.py
+-rw-r--r--   0 yw         (501) staff       (20)     9961 2024-01-18 16:27:41.000000 tmart-2.3.3/tmart/Surface.py
+-rw-r--r--   0 yw         (501) staff       (20)    13680 2024-01-18 16:35:11.000000 tmart-2.3.3/tmart/Tmart.py
+-rw-r--r--   0 yw         (501) staff       (20)    38594 2024-04-11 14:37:47.000000 tmart-2.3.3/tmart/Tmart2.py
+-rw-r--r--   0 yw         (501) staff       (20)      550 2023-12-28 20:42:03.000000 tmart-2.3.3/tmart/__init__.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-15 14:58:02.309355 tmart-2.3.3/tmart/ancillary/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-15 14:58:02.315360 tmart-2.3.3/tmart/ancillary/aerosolSPF/
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-2.3.3/tmart/ancillary/aerosolSPF/BiomassBurning.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-2.3.3/tmart/ancillary/aerosolSPF/Continental.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-2.3.3/tmart/ancillary/aerosolSPF/Desert.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-2.3.3/tmart/ancillary/aerosolSPF/Maritime.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-2.3.3/tmart/ancillary/aerosolSPF/Stratospheric.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-2.3.3/tmart/ancillary/aerosolSPF/Urban.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-2.3.3/tmart/ancillary/conifer_forest.csv
+-rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-2.3.3/tmart/ancillary/dry_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-2.3.3/tmart/ancillary/lawn_grass.csv
+-rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-2.3.3/tmart/ancillary/soil.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-2.3.3/tmart/ancillary/vegetation.csv
+-rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-2.3.3/tmart/ancillary/water.csv
+-rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-2.3.3/tmart/ancillary/water_chl1.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-2.3.3/tmart/ancillary/wet_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-2.3.3/tmart/ancillary/whitecap_factor.csv
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-15 14:58:02.316058 tmart-2.3.3/tmart/config/
+-rw-r--r--   0 yw         (501) staff       (20)     1303 2024-03-28 18:02:22.000000 tmart-2.3.3/tmart/config/config.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-15 14:58:02.317038 tmart-2.3.3/tmart/surface_rho/
+-rw-r--r--   0 yw         (501) staff       (20)      341 2023-05-23 22:27:30.000000 tmart-2.3.3/tmart/surface_rho/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     5038 2023-05-26 07:42:38.000000 tmart-2.3.3/tmart/surface_rho/calculate.py
+-rw-r--r--   0 yw         (501) staff       (20)     2003 2024-03-10 16:10:22.000000 tmart-2.3.3/tmart/tm_OT.py
+-rw-r--r--   0 yw         (501) staff       (20)     3195 2024-01-18 16:28:32.000000 tmart-2.3.3/tmart/tm_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     3976 2024-03-10 16:09:31.000000 tmart-2.3.3/tmart/tm_geometry.py
+-rw-r--r--   0 yw         (501) staff       (20)    12883 2024-03-10 16:09:57.000000 tmart-2.3.3/tmart/tm_intersect.py
+-rw-r--r--   0 yw         (501) staff       (20)    11243 2024-03-10 16:10:06.000000 tmart-2.3.3/tmart/tm_move.py
+-rw-r--r--   0 yw         (501) staff       (20)     6748 2024-01-18 16:33:59.000000 tmart-2.3.3/tmart/tm_sampling.py
+-rw-r--r--   0 yw         (501) staff       (20)    12104 2024-04-11 14:31:53.000000 tmart-2.3.3/tmart/tm_water.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-15 14:58:02.297413 tmart-2.3.3/tmart.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)     5181 2024-05-15 14:58:02.000000 tmart-2.3.3/tmart.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     2067 2024-05-15 14:58:02.000000 tmart-2.3.3/tmart.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2024-05-15 14:58:02.000000 tmart-2.3.3/tmart.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       70 2024-05-15 14:58:02.000000 tmart-2.3.3/tmart.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)        6 2024-05-15 14:58:02.000000 tmart-2.3.3/tmart.egg-info/top_level.txt
```

### Comparing `tmart-2.3.2/PKG-INFO` & `tmart-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 2.3.2
+Version: 2.3.3
 Summary: Modelling and correcting for the adjacency effect in aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tmart-2.3.2/README.md` & `tmart-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/setup.py` & `tmart-2.3.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tmart",                     # This is the name of the package
-    version="2.3.2",                       
+    version="2.3.3",                       
     author="Yulun Wu",                     # Full name of the author
     description="Modelling and correcting for the adjacency effect in aquatic remote sensing",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),    # List of all python modules to be installed
     packages = ['tmart','tmart.surface_rho','tmart.AEC','tmart.ancillary','tmart.ancillary.aerosolSPF','tmart.config'],
     include_package_data=True,
```

### Comparing `tmart-2.3.2/tests/test_AE_modelling.py` & `tmart-2.3.3/tests/test_AE_modelling.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_E_diffuse.py` & `tmart-2.3.3/tests/test_E_diffuse.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_L_sky.py` & `tmart-2.3.3/tests/test_L_sky.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_basic.py` & `tmart-2.3.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_basic_import.py` & `tmart-2.3.3/tests/test_basic_import.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_calc_rho.py` & `tmart-2.3.3/tests/test_calc_rho.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_calcref.py` & `tmart-2.3.3/tests/test_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_fresnel.py` & `tmart-2.3.3/tests/test_fresnel.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_modelling.py` & `tmart-2.3.3/tests/test_modelling.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_plot.py` & `tmart-2.3.3/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_quickstart.py` & `tmart-2.3.3/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_specular_contribution.py` & `tmart-2.3.3/tests/test_specular_contribution.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_typical_ocean.py` & `tmart-2.3.3/tests/test_typical_ocean.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tests/test_whales_SR.py` & `tmart-2.3.3/tests/test_whales_SR.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/AEC.py` & `tmart-2.3.3/tmart/AEC/AEC.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,17 +167,17 @@
         # Negative to 0, this ensures the lowest TOA reflectance is no lower than R_atm
         # temp_out[temp_out<0] = 0
         
         # Scaling
         temp_out = temp_out + R_atm # TOA reflectance
         
         if sensor =='L8' or sensor == 'L9':
-            temp_out = ((temp_out * math.cos(metadata['sza']/180*math.pi) - scale_add) / scale_mult).astype(int)
+            temp_out = np.maximum(((temp_out * math.cos(metadata['sza']/180*math.pi) - scale_add) / scale_mult),1).astype(int)
         else:
-            temp_out = ((temp_out - scale_add) / scale_mult).astype(int)
+            temp_out = np.maximum(((temp_out - scale_add) / scale_mult),1).astype(int)
     
     # If only water correction 
     else:
         # Negative to 0
         # temp_SR_water[temp_SR_water<0] = 0
         
         temp_out = temp_SR_water + R_atm # TOA reflectance
@@ -189,17 +189,17 @@
             temp_mask = temp_mask[:-pad_rows_tmp]
         if pad_columns_tmp>0: 
             temp_out = temp_out[:, :-pad_columns_tmp]
             temp_mask = temp_mask[:, :-pad_columns_tmp]
         
         # Scaling
         if sensor =='L8' or sensor == 'L9':
-            temp_out = np.where(temp_mask,    band_ds.read(1),  ((temp_out * math.cos(metadata['sza']/180*math.pi) - scale_add) / scale_mult).astype(int) )
+            temp_out = np.where(temp_mask,    band_ds.read(1),  np.maximum(((temp_out * math.cos(metadata['sza']/180*math.pi) - scale_add) / scale_mult),1).astype(int) )
         else:
-            temp_out = np.where(temp_mask,    band_ds.read(1),  ((temp_out - scale_add) / scale_mult).astype(int) )
+            temp_out = np.where(temp_mask,    band_ds.read(1),  np.maximum(((temp_out - scale_add) / scale_mult),1).astype(int) )
 
     # Convert nan back to 0
     temp_is_nan = is_nan
     if pad_rows_tmp>0: temp_is_nan = temp_is_nan[:-pad_rows_tmp]
     if pad_columns_tmp>0: temp_is_nan = temp_is_nan[:, :-pad_columns_tmp]
     
     temp_out[temp_is_nan] = 0
```

### Comparing `tmart-2.3.2/tmart/AEC/__init__.py` & `tmart-2.3.3/tmart/AEC/__init__.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/anci_download.py` & `tmart-2.3.3/tmart/AEC/anci_download.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/anci_get_AER.py` & `tmart-2.3.3/tmart/AEC/anci_get_AER.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/anci_get_OWV.py` & `tmart-2.3.3/tmart/AEC/anci_get_OWV.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/anci_list_files.py` & `tmart-2.3.3/tmart/AEC/anci_list_files.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/compute_gas_transmittance.py` & `tmart-2.3.3/tmart/AEC/compute_gas_transmittance.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/compute_masks.py` & `tmart-2.3.3/tmart/AEC/compute_masks.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/fillnan.py` & `tmart-2.3.3/tmart/AEC/fillnan.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/get_AOT.py` & `tmart-2.3.3/tmart/AEC/get_AOT.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/get_ancillary.py` & `tmart-2.3.3/tmart/AEC/get_ancillary.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/get_parameters.py` & `tmart-2.3.3/tmart/AEC/get_parameters.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/identify_sensor.py` & `tmart-2.3.3/tmart/AEC/identify_sensor.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/irradiance_correction.py` & `tmart-2.3.3/tmart/AEC/irradiance_correction.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/read_PRISMA_north.py` & `tmart-2.3.3/tmart/AEC/read_PRISMA_north.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/read_PRISMA_vaa.py` & `tmart-2.3.3/tmart/AEC/read_PRISMA_vaa.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/read_config.py` & `tmart-2.3.3/tmart/AEC/read_config.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/read_metadata_Landsat.py` & `tmart-2.3.3/tmart/AEC/read_metadata_Landsat.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/read_metadata_S2.py` & `tmart-2.3.3/tmart/AEC/read_metadata_S2.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/read_xml_S2.py` & `tmart-2.3.3/tmart/AEC/read_xml_S2.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/read_xml_S2_scene.py` & `tmart-2.3.3/tmart/AEC/read_xml_S2_scene.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/run.py` & `tmart-2.3.3/tmart/AEC/run.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/run_acoliteL1R.py` & `tmart-2.3.3/tmart/AEC/run_acoliteL1R.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/run_regular.py` & `tmart-2.3.3/tmart/AEC/run_regular.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/AEC/write_atm_info.py` & `tmart-2.3.3/tmart/AEC/write_atm_info.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/Aerosol.py` & `tmart-2.3.3/tmart/Aerosol.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/Atmosphere.py` & `tmart-2.3.3/tmart/Atmosphere.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/Surface.py` & `tmart-2.3.3/tmart/Surface.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/Tmart.py` & `tmart-2.3.3/tmart/Tmart.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/Tmart2.py` & `tmart-2.3.3/tmart/Tmart2.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/__init__.py` & `tmart-2.3.3/tmart/__init__.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/aerosolSPF/BiomassBurning.csv` & `tmart-2.3.3/tmart/ancillary/aerosolSPF/BiomassBurning.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/aerosolSPF/Continental.csv` & `tmart-2.3.3/tmart/ancillary/aerosolSPF/Continental.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/aerosolSPF/Desert.csv` & `tmart-2.3.3/tmart/ancillary/aerosolSPF/Desert.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/aerosolSPF/Maritime.csv` & `tmart-2.3.3/tmart/ancillary/aerosolSPF/Maritime.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/aerosolSPF/Stratospheric.csv` & `tmart-2.3.3/tmart/ancillary/aerosolSPF/Stratospheric.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/aerosolSPF/Urban.csv` & `tmart-2.3.3/tmart/ancillary/aerosolSPF/Urban.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/conifer_forest.csv` & `tmart-2.3.3/tmart/ancillary/conifer_forest.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/dry_beach_sand.csv` & `tmart-2.3.3/tmart/ancillary/dry_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/lawn_grass.csv` & `tmart-2.3.3/tmart/ancillary/lawn_grass.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/soil.csv` & `tmart-2.3.3/tmart/ancillary/soil.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/vegetation.csv` & `tmart-2.3.3/tmart/ancillary/vegetation.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/water_chl1.csv` & `tmart-2.3.3/tmart/ancillary/water_chl1.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/ancillary/wet_beach_sand.csv` & `tmart-2.3.3/tmart/ancillary/wet_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/config/config.txt` & `tmart-2.3.3/tmart/config/config.txt`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/surface_rho/calculate.py` & `tmart-2.3.3/tmart/surface_rho/calculate.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/tm_OT.py` & `tmart-2.3.3/tmart/tm_OT.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/tm_calcref.py` & `tmart-2.3.3/tmart/tm_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/tm_geometry.py` & `tmart-2.3.3/tmart/tm_geometry.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/tm_intersect.py` & `tmart-2.3.3/tmart/tm_intersect.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/tm_move.py` & `tmart-2.3.3/tmart/tm_move.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/tm_sampling.py` & `tmart-2.3.3/tmart/tm_sampling.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart/tm_water.py` & `tmart-2.3.3/tmart/tm_water.py`

 * *Files identical despite different names*

### Comparing `tmart-2.3.2/tmart.egg-info/PKG-INFO` & `tmart-2.3.3/tmart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 2.3.2
+Version: 2.3.3
 Summary: Modelling and correcting for the adjacency effect in aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tmart-2.3.2/tmart.egg-info/SOURCES.txt` & `tmart-2.3.3/tmart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

