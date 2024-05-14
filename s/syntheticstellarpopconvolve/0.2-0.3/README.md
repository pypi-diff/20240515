# Comparing `tmp/syntheticstellarpopconvolve-0.2.tar.gz` & `tmp/syntheticstellarpopconvolve-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntheticstellarpopconvolve-0.2.tar", last modified: Mon May 13 14:26:40 2024, max compression
+gzip compressed data, was "syntheticstellarpopconvolve-0.3.tar", last modified: Tue May 14 22:33:26 2024, max compression
```

## Comparing `syntheticstellarpopconvolve-0.2.tar` & `syntheticstellarpopconvolve-0.3.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/
--rw-rw-r--   0 david     (1002) david     (1002)    32894 2024-04-28 22:36:09.000000 syntheticstellarpopconvolve-0.2/LICENSE
--rw-rw-r--   0 david     (1002) david     (1002)      174 2024-05-13 14:22:49.000000 syntheticstellarpopconvolve-0.2/MANIFEST.in
--rw-r--r--   0 david     (1002) david     (1002)     4181 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/PKG-INFO
--rw-rw-r--   0 david     (1002) david     (1002)     2836 2024-05-05 23:07:49.000000 syntheticstellarpopconvolve-0.2/README.md
--rw-rw-r--   0 david     (1002) david     (1002)      668 2024-05-01 00:59:25.000000 syntheticstellarpopconvolve-0.2/pyproject.toml
--rw-rw-r--   0 david     (1002) david     (1002)       86 2024-05-03 12:39:25.000000 syntheticstellarpopconvolve-0.2/requirements.txt
--rw-rw-r--   0 david     (1002) david     (1002)       38 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/setup.cfg
--rw-rw-r--   0 david     (1002) david     (1002)     3336 2024-05-13 14:22:49.000000 syntheticstellarpopconvolve-0.2/setup.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.620218 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/
--rw-rw-r--   0 david     (1002) david     (1002)      869 2024-05-05 16:27:07.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/SFR_plotting_routine.py
--rw-rw-r--   0 david     (1002) david     (1002)      297 2024-05-13 14:23:10.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/__init__.py
--rw-rw-r--   0 david     (1002) david     (1002)       20 2024-05-13 14:22:49.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/_version.py
--rw-rw-r--   0 david     (1002) david     (1002)    16607 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/archive.py
--rw-rw-r--   0 david     (1002) david     (1002)     2563 2024-05-02 02:45:50.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/calculate_birth_redshift_array.py
--rw-rw-r--   0 david     (1002) david     (1002)     9660 2024-05-05 22:55:24.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/check_convolution_config.py
--rw-rw-r--   0 david     (1002) david     (1002)      978 2024-05-05 02:59:48.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/check_input_file.py
--rw-rw-r--   0 david     (1002) david     (1002)     2257 2024-05-05 03:19:16.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve.py
--rw-rw-r--   0 david     (1002) david     (1002)      868 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_custom_data.py
--rw-rw-r--   0 david     (1002) david     (1002)    46881 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_ensembles.py
--rw-rw-r--   0 david     (1002) david     (1002)     3977 2024-05-05 16:27:28.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_events.py
--rw-rw-r--   0 david     (1002) david     (1002)    16848 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_populations.py
--rw-rw-r--   0 david     (1002) david     (1002)     1508 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/cosmology_utils.py
--rw-rw-r--   0 david     (1002) david     (1002)    19995 2024-05-05 21:26:05.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/default_convolution_config.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.628218 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/
--rw-rw-r--   0 david     (1002) david     (1002)    56408 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat
--rw-rw-r--   0 david     (1002) david     (1002)  9053345 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_ensemble.json
--rw-rw-r--   0 david     (1002) david     (1002)   330384 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_population_settings.json
--rw-rw-r--   0 david     (1002) david     (1002)      730 2024-05-02 02:30:36.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/extract_population_settings.py
--rw-rw-r--   0 david     (1002) david     (1002)    16579 2024-05-01 00:21:25.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/functions_to_review.py
--rw-rw-r--   0 david     (1002) david     (1002)    14734 2024-05-05 03:08:05.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/general_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)     7060 2024-05-01 00:49:44.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/metallicity_distributions.py
--rw-rw-r--   0 david     (1002) david     (1002)      830 2024-05-05 16:23:51.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/prepare_output_file.py
--rw-rw-r--   0 david     (1002) david     (1002)     5150 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/prepare_redshift_interpolator.py
--rw-rw-r--   0 david     (1002) david     (1002)     5113 2024-05-01 00:30:47.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/starformation_rate_distributions.py
--rw-rw-r--   0 david     (1002) david     (1002)     3053 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/store_redshift_shell_info.py
--rw-rw-r--   0 david     (1002) david     (1002)     3338 2024-05-01 00:20:21.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/store_sfr_info.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/
--rw-rw-r--   0 david     (1002) david     (1002)       85 2024-05-01 00:02:02.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/generate_coverage_report.sh
--rw-rw-r--   0 david     (1002) david     (1002)     3833 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/main.py
--rw-rw-r--   0 david     (1002) david     (1002)      143 2024-04-30 23:58:15.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_SFR_plotting_routine.py
--rw-rw-r--   0 david     (1002) david     (1002)     2377 2024-05-05 16:27:45.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_calculate_birth_redshift_array.py
--rw-rw-r--   0 david     (1002) david     (1002)    13441 2024-05-05 22:55:24.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_check_convolution_config.py
--rw-rw-r--   0 david     (1002) david     (1002)     2013 2024-05-05 16:28:16.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_check_input_file.py
--rw-rw-r--   0 david     (1002) david     (1002)      307 2024-05-05 21:32:57.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_metallicity_distributions.py
--rw-rw-r--   0 david     (1002) david     (1002)     5168 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_with_ensemble.py
--rw-rw-r--   0 david     (1002) david     (1002)     4895 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_with_events.py
--rw-rw-r--   0 david     (1002) david     (1002)      254 2024-05-05 16:26:10.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve.py
--rw-rw-r--   0 david     (1002) david     (1002)      863 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_custom_data.py
--rw-rw-r--   0 david     (1002) david     (1002)    45263 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_ensembles.py
--rw-rw-r--   0 david     (1002) david     (1002)    13212 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_events.py
--rw-rw-r--   0 david     (1002) david     (1002)    16721 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_populations.py
--rw-rw-r--   0 david     (1002) david     (1002)     8293 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_cosmology_utils.py
--rw-rw-r--   0 david     (1002) david     (1002)     3389 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_default_convolution_config.py
--rw-rw-r--   0 david     (1002) david     (1002)     4272 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_extract_population_settings.py
--rw-rw-r--   0 david     (1002) david     (1002)      142 2024-04-28 23:09:56.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_functions_to_review.py
--rw-rw-r--   0 david     (1002) david     (1002)    23145 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_general_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)     1600 2024-05-05 16:25:46.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_prepare_output_file.py
--rw-rw-r--   0 david     (1002) david     (1002)     6042 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_prepare_redshift_interpolator.py
--rw-rw-r--   0 david     (1002) david     (1002)      318 2024-05-05 16:31:51.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_starformation_rate_distributions.py
--rw-rw-r--   0 david     (1002) david     (1002)     4976 2024-05-05 16:28:50.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_store_redshift_shell_info.py
--rw-rw-r--   0 david     (1002) david     (1002)      272 2024-05-05 16:28:42.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_store_sfr_info.py
--rw-rw-r--   0 david     (1002) david     (1002)      126 2024-05-01 00:49:14.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_tmp.py
--rw-rw-r--   0 david     (1002) david     (1002)     2118 2024-05-05 16:26:15.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_update_convolution_config.py
--rw-rw-r--   0 david     (1002) david     (1002)      691 2024-04-28 23:05:37.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tmp.py
--rw-rw-r--   0 david     (1002) david     (1002)      566 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/update_convolution_config.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/
--rw-r--r--   0 david     (1002) david     (1002)     4181 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1002) david     (1002)     3443 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1002) david     (1002)        1 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1002) david     (1002)       86 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/requires.txt
--rw-rw-r--   0 david     (1002) david     (1002)       28 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-14 22:33:26.115777 syntheticstellarpopconvolve-0.3/
+-rw-rw-r--   0 david     (1002) david     (1002)    32894 2024-04-28 22:36:09.000000 syntheticstellarpopconvolve-0.3/LICENSE
+-rw-rw-r--   0 david     (1002) david     (1002)      228 2024-05-14 22:13:18.000000 syntheticstellarpopconvolve-0.3/MANIFEST.in
+-rw-r--r--   0 david     (1002) david     (1002)     7536 2024-05-14 22:33:26.115777 syntheticstellarpopconvolve-0.3/PKG-INFO
+-rw-rw-r--   0 david     (1002) david     (1002)     6191 2024-05-14 13:59:42.000000 syntheticstellarpopconvolve-0.3/README.md
+-rw-rw-r--   0 david     (1002) david     (1002)      668 2024-05-01 00:59:25.000000 syntheticstellarpopconvolve-0.3/pyproject.toml
+-rw-rw-r--   0 david     (1002) david     (1002)       86 2024-05-03 12:39:25.000000 syntheticstellarpopconvolve-0.3/requirements.txt
+-rw-rw-r--   0 david     (1002) david     (1002)       38 2024-05-14 22:33:26.115777 syntheticstellarpopconvolve-0.3/setup.cfg
+-rw-rw-r--   0 david     (1002) david     (1002)     3336 2024-05-13 14:22:49.000000 syntheticstellarpopconvolve-0.3/setup.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-14 22:33:26.099778 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/
+-rw-rw-r--   0 david     (1002) david     (1002)      869 2024-05-05 16:27:07.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/SFR_plotting_routine.py
+-rw-rw-r--   0 david     (1002) david     (1002)      297 2024-05-13 14:23:10.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/__init__.py
+-rw-rw-r--   0 david     (1002) david     (1002)       20 2024-05-14 22:32:09.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/_version.py
+-rw-rw-r--   0 david     (1002) david     (1002)    16607 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/archive.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2563 2024-05-02 02:45:50.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/calculate_birth_redshift_array.py
+-rw-rw-r--   0 david     (1002) david     (1002)     9660 2024-05-14 22:28:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/check_convolution_config.py
+-rw-rw-r--   0 david     (1002) david     (1002)      978 2024-05-05 02:59:48.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/check_input_file.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2257 2024-05-05 03:19:16.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve.py
+-rw-rw-r--   0 david     (1002) david     (1002)      868 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve_custom_data.py
+-rw-rw-r--   0 david     (1002) david     (1002)    46881 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve_ensembles.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3977 2024-05-05 16:27:28.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve_events.py
+-rw-rw-r--   0 david     (1002) david     (1002)    16848 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve_populations.py
+-rw-rw-r--   0 david     (1002) david     (1002)     1508 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/cosmology_utils.py
+-rw-rw-r--   0 david     (1002) david     (1002)    19995 2024-05-05 21:26:05.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/default_convolution_config.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-14 22:33:26.111777 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/example_data/
+-rw-rw-r--   0 david     (1002) david     (1002)  1072680 2024-05-14 21:55:35.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/example_data/example_BinCodex.h5
+-rw-rw-r--   0 david     (1002) david     (1002)    56408 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat
+-rw-rw-r--   0 david     (1002) david     (1002)  9053345 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/example_data/example_ensemble.json
+-rw-rw-r--   0 david     (1002) david     (1002)   330384 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/example_data/example_population_settings.json
+-rw-rw-r--   0 david     (1002) david     (1002)      730 2024-05-02 02:30:36.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/extract_population_settings.py
+-rw-rw-r--   0 david     (1002) david     (1002)    16579 2024-05-01 00:21:25.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/functions_to_review.py
+-rw-rw-r--   0 david     (1002) david     (1002)    14734 2024-05-05 03:08:05.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/general_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     7060 2024-05-01 00:49:44.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/metallicity_distributions.py
+-rw-rw-r--   0 david     (1002) david     (1002)      830 2024-05-05 16:23:51.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/prepare_output_file.py
+-rw-rw-r--   0 david     (1002) david     (1002)     5150 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/prepare_redshift_interpolator.py
+-rw-rw-r--   0 david     (1002) david     (1002)     5113 2024-05-01 00:30:47.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/starformation_rate_distributions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3053 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/store_redshift_shell_info.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3338 2024-05-01 00:20:21.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/store_sfr_info.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-14 22:33:26.115777 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/
+-rw-rw-r--   0 david     (1002) david     (1002)       85 2024-05-01 00:02:02.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/generate_coverage_report.sh
+-rw-rw-r--   0 david     (1002) david     (1002)     3833 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/main.py
+-rw-rw-r--   0 david     (1002) david     (1002)      143 2024-04-30 23:58:15.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_SFR_plotting_routine.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2377 2024-05-05 16:27:45.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_calculate_birth_redshift_array.py
+-rw-rw-r--   0 david     (1002) david     (1002)    13441 2024-05-05 22:55:24.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_check_convolution_config.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2013 2024-05-05 16:28:16.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_check_input_file.py
+-rw-rw-r--   0 david     (1002) david     (1002)      307 2024-05-05 21:32:57.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolution_metallicity_distributions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     5168 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolution_with_ensemble.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4895 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolution_with_events.py
+-rw-rw-r--   0 david     (1002) david     (1002)      254 2024-05-05 16:26:10.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolve.py
+-rw-rw-r--   0 david     (1002) david     (1002)      863 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolve_custom_data.py
+-rw-rw-r--   0 david     (1002) david     (1002)    45263 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolve_ensembles.py
+-rw-rw-r--   0 david     (1002) david     (1002)    13212 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolve_events.py
+-rw-rw-r--   0 david     (1002) david     (1002)    16721 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolve_populations.py
+-rw-rw-r--   0 david     (1002) david     (1002)     8293 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_cosmology_utils.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3389 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_default_convolution_config.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4272 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_extract_population_settings.py
+-rw-rw-r--   0 david     (1002) david     (1002)      142 2024-04-28 23:09:56.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_functions_to_review.py
+-rw-rw-r--   0 david     (1002) david     (1002)    23145 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_general_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     1600 2024-05-05 16:25:46.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_prepare_output_file.py
+-rw-rw-r--   0 david     (1002) david     (1002)     6042 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_prepare_redshift_interpolator.py
+-rw-rw-r--   0 david     (1002) david     (1002)      318 2024-05-05 16:31:51.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_starformation_rate_distributions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4976 2024-05-05 16:28:50.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_store_redshift_shell_info.py
+-rw-rw-r--   0 david     (1002) david     (1002)      272 2024-05-05 16:28:42.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_store_sfr_info.py
+-rw-rw-r--   0 david     (1002) david     (1002)      126 2024-05-01 00:49:14.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_tmp.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2118 2024-05-05 16:26:15.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_update_convolution_config.py
+-rw-rw-r--   0 david     (1002) david     (1002)      691 2024-04-28 23:05:37.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tmp.py
+-rw-rw-r--   0 david     (1002) david     (1002)      566 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/update_convolution_config.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-14 22:33:26.115777 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve.egg-info/
+-rw-r--r--   0 david     (1002) david     (1002)     7536 2024-05-14 22:33:26.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1002) david     (1002)     3504 2024-05-14 22:33:26.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1002) david     (1002)        1 2024-05-14 22:33:26.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1002) david     (1002)       86 2024-05-14 22:33:26.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve.egg-info/requires.txt
+-rw-rw-r--   0 david     (1002) david     (1002)       28 2024-05-14 22:33:26.000000 syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve.egg-info/top_level.txt
```

### Comparing `syntheticstellarpopconvolve-0.2/LICENSE` & `syntheticstellarpopconvolve-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/pyproject.toml` & `syntheticstellarpopconvolve-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/setup.py` & `syntheticstellarpopconvolve-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/SFR_plotting_routine.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/SFR_plotting_routine.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/archive.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/archive.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/calculate_birth_redshift_array.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/calculate_birth_redshift_array.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/check_convolution_config.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/check_convolution_config.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/check_input_file.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/check_input_file.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_custom_data.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve_custom_data.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_ensembles.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve_ensembles.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_events.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve_events.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_populations.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/convolve_populations.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/cosmology_utils.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/cosmology_utils.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/default_convolution_config.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/default_convolution_config.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_ensemble.json` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/example_data/example_ensemble.json`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_population_settings.json` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/example_data/example_population_settings.json`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/extract_population_settings.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/extract_population_settings.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/functions_to_review.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/functions_to_review.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/general_functions.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/general_functions.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/metallicity_distributions.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/metallicity_distributions.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/prepare_output_file.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/prepare_output_file.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/prepare_redshift_interpolator.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/prepare_redshift_interpolator.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/starformation_rate_distributions.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/starformation_rate_distributions.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/store_redshift_shell_info.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/store_redshift_shell_info.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/store_sfr_info.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/store_sfr_info.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/main.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/main.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_calculate_birth_redshift_array.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_calculate_birth_redshift_array.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_check_convolution_config.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_check_convolution_config.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_check_input_file.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_check_input_file.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_with_ensemble.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolution_with_ensemble.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_with_events.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolution_with_events.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_custom_data.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolve_custom_data.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_ensembles.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolve_ensembles.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_events.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolve_events.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_populations.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_convolve_populations.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_cosmology_utils.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_cosmology_utils.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_default_convolution_config.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_default_convolution_config.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_extract_population_settings.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_extract_population_settings.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_general_functions.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_general_functions.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_prepare_output_file.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_prepare_output_file.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_prepare_redshift_interpolator.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_prepare_redshift_interpolator.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_store_redshift_shell_info.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_store_redshift_shell_info.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_update_convolution_config.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tests/test_update_convolution_config.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tmp.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/tmp.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/update_convolution_config.py` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve/update_convolution_config.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/SOURCES.txt` & `syntheticstellarpopconvolve-0.3/syntheticstellarpopconvolve.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 syntheticstellarpopconvolve/tmp.py
 syntheticstellarpopconvolve/update_convolution_config.py
 syntheticstellarpopconvolve.egg-info/PKG-INFO
 syntheticstellarpopconvolve.egg-info/SOURCES.txt
 syntheticstellarpopconvolve.egg-info/dependency_links.txt
 syntheticstellarpopconvolve.egg-info/requires.txt
 syntheticstellarpopconvolve.egg-info/top_level.txt
+syntheticstellarpopconvolve/example_data/example_BinCodex.h5
 syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat
 syntheticstellarpopconvolve/example_data/example_ensemble.json
 syntheticstellarpopconvolve/example_data/example_population_settings.json
 syntheticstellarpopconvolve/tests/generate_coverage_report.sh
 syntheticstellarpopconvolve/tests/main.py
 syntheticstellarpopconvolve/tests/test_SFR_plotting_routine.py
 syntheticstellarpopconvolve/tests/test_calculate_birth_redshift_array.py
```

