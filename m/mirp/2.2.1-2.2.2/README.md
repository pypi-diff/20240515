# Comparing `tmp/mirp-2.2.1.tar.gz` & `tmp/mirp-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirp-2.2.1.tar", last modified: Fri Apr 19 14:44:44 2024, max compression
+gzip compressed data, was "mirp-2.2.2.tar", last modified: Wed May 15 14:40:16 2024, max compression
```

## Comparing `mirp-2.2.1.tar` & `mirp-2.2.2.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.538627 mirp-2.2.1/
--rw-rw-rw-   0        0        0     1375 2024-04-04 14:37:05.000000 mirp-2.2.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    14139 2020-10-01 17:38:34.000000 mirp-2.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0       33 2023-10-27 15:27:23.000000 mirp-2.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0    12992 2024-04-19 14:41:38.000000 mirp-2.2.1/NEWS.md
--rw-rw-rw-   0        0        0    26846 2024-04-19 14:44:44.537627 mirp-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     8958 2024-04-09 11:53:59.000000 mirp-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.443542 mirp-2.2.1/mirp/
--rw-rw-rw-   0        0        0      927 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.467563 mirp-2.2.1/mirp/_data_import/
--rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/__init__.py
--rw-rw-rw-   0        0        0    24825 2024-04-19 07:42:34.000000 mirp-2.2.1/mirp/_data_import/dicom_file.py
--rw-rw-rw-   0        0        0     4595 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/dicom_file_ct.py
--rw-rw-rw-   0        0        0     6577 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/dicom_file_mr.py
--rw-rw-rw-   0        0        0    36854 2024-04-17 11:02:29.000000 mirp-2.2.1/mirp/_data_import/dicom_file_pet.py
--rw-rw-rw-   0        0        0     7289 2024-04-18 15:42:31.000000 mirp-2.2.1/mirp/_data_import/dicom_file_rtdose.py
--rw-rw-rw-   0        0        0    31324 2024-04-18 15:43:46.000000 mirp-2.2.1/mirp/_data_import/dicom_file_rtstruct.py
--rw-rw-rw-   0        0        0    21406 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/dicom_file_seg.py
--rw-rw-rw-   0        0        0    10873 2024-04-17 15:11:01.000000 mirp-2.2.1/mirp/_data_import/dicom_file_stack.py
--rw-rw-rw-   0        0        0    22746 2024-04-18 15:11:10.000000 mirp-2.2.1/mirp/_data_import/directory.py
--rw-rw-rw-   0        0        0    45837 2024-04-17 14:40:58.000000 mirp-2.2.1/mirp/_data_import/generic_file.py
--rw-rw-rw-   0        0        0    11185 2024-04-17 14:40:58.000000 mirp-2.2.1/mirp/_data_import/generic_file_stack.py
--rw-rw-rw-   0        0        0     6508 2024-04-18 14:55:20.000000 mirp-2.2.1/mirp/_data_import/itk_file.py
--rw-rw-rw-   0        0        0     7141 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/itk_file_stack.py
--rw-rw-rw-   0        0        0    13474 2024-04-10 14:03:09.000000 mirp-2.2.1/mirp/_data_import/mask_contour.py
--rw-rw-rw-   0        0        0     5845 2024-04-18 14:55:20.000000 mirp-2.2.1/mirp/_data_import/numpy_file.py
--rw-rw-rw-   0        0        0     2944 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/numpy_file_stack.py
--rw-rw-rw-   0        0        0     1308 2024-04-19 06:51:53.000000 mirp-2.2.1/mirp/_data_import/read_data.py
--rw-rw-rw-   0        0        0    22434 2024-04-12 11:31:49.000000 mirp-2.2.1/mirp/_data_import/suv.py
--rw-rw-rw-   0        0        0    17570 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.479574 mirp-2.2.1/mirp/_featuresets/
--rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/__init__.py
--rw-rw-rw-   0        0        0    21581 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/cm.py
--rw-rw-rw-   0        0        0    11525 2024-04-05 11:27:52.000000 mirp-2.2.1/mirp/_featuresets/dzm.py
--rw-rw-rw-   0        0        0     6917 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/intensity_histogram.py
--rw-rw-rw-   0        0        0    10922 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/intensity_volume_histogram.py
--rw-rw-rw-   0        0        0     6275 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/local_intensity.py
--rw-rw-rw-   0        0        0    32584 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/morphology_3d.py
--rw-rw-rw-   0        0        0    13752 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/ngldm.py
--rw-rw-rw-   0        0        0    12853 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/ngtdm.py
--rw-rw-rw-   0        0        0    18910 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/rlm.py
--rw-rw-rw-   0        0        0     4278 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/statistics.py
--rw-rw-rw-   0        0        0    10900 2024-04-05 11:27:52.000000 mirp-2.2.1/mirp/_featuresets/szm.py
--rw-rw-rw-   0        0        0     3185 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.488582 mirp-2.2.1/mirp/_image_processing/
--rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/__init__.py
--rw-rw-rw-   0        0        0     2808 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/alter_mask.py
--rw-rw-rw-   0        0        0     1223 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/anti_aliasing.py
--rw-rw-rw-   0        0        0     4256 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/cropping.py
--rw-rw-rw-   0        0        0     5128 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/discretise_image.py
--rw-rw-rw-   0        0        0     2004 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/randomise_mask.py
--rw-rw-rw-   0        0        0     1597 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/split_mask.py
--rw-rw-rw-   0        0        0     2696 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/tissue_mask.py
--rw-rw-rw-   0        0        0     2656 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.501595 mirp-2.2.1/mirp/_imagefilters/
--rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/__init__.py
--rw-rw-rw-   0        0        0     1454 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/exponential_transform.py
--rw-rw-rw-   0        0        0     9339 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/gabor.py
--rw-rw-rw-   0        0        0     6436 2024-04-04 13:44:39.000000 mirp-2.2.1/mirp/_imagefilters/gaussian.py
--rw-rw-rw-   0        0        0      562 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/generic.py
--rw-rw-rw-   0        0        0     7495 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/laplacian_of_gaussian.py
--rw-rw-rw-   0        0        0     7321 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/laws.py
--rw-rw-rw-   0        0        0     1496 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/log_transform.py
--rw-rw-rw-   0        0        0     2546 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/mean.py
--rw-rw-rw-   0        0        0     9798 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/nonseparable_wavelet.py
--rw-rw-rw-   0        0        0     7484 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/separable_wavelet.py
--rw-rw-rw-   0        0        0     1261 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/square_root_transform.py
--rw-rw-rw-   0        0        0     1230 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/square_transform.py
--rw-rw-rw-   0        0        0    23965 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.511604 mirp-2.2.1/mirp/_images/
--rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/__init__.py
--rw-rw-rw-   0        0        0     9143 2024-04-05 10:37:51.000000 mirp-2.2.1/mirp/_images/base_image.py
--rw-rw-rw-   0        0        0     2115 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/ct_image.py
--rw-rw-rw-   0        0        0    51861 2024-04-10 15:17:41.000000 mirp-2.2.1/mirp/_images/generic_image.py
--rw-rw-rw-   0        0        0    22184 2024-04-05 10:39:33.000000 mirp-2.2.1/mirp/_images/mask_image.py
--rw-rw-rw-   0        0        0     1939 2024-04-09 08:50:40.000000 mirp-2.2.1/mirp/_images/mr_image.py
--rw-rw-rw-   0        0        0     2204 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/pet_image.py
--rw-rw-rw-   0        0        0     1908 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/rtdose_image.py
--rw-rw-rw-   0        0        0    26540 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/transformed_image.py
--rw-rw-rw-   0        0        0     4098 2024-04-09 05:58:15.000000 mirp-2.2.1/mirp/_images/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.513604 mirp-2.2.1/mirp/_masks/
--rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_masks/__init__.py
--rw-rw-rw-   0        0        0    28747 2024-04-10 11:46:45.000000 mirp-2.2.1/mirp/_masks/base_mask.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.515606 mirp-2.2.1/mirp/_workflows/
--rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_workflows/__init__.py
--rw-rw-rw-   0        0        0      328 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_workflows/baseWorkflow.py
--rw-rw-rw-   0        0        0    35003 2024-04-16 15:05:09.000000 mirp-2.2.1/mirp/_workflows/standardWorkflow.py
--rw-rw-rw-   0        0        0     3379 2023-10-27 15:27:23.000000 mirp-2.2.1/mirp/config_data.xml
--rw-rw-rw-   0        0        0    21251 2024-04-12 06:00:24.000000 mirp-2.2.1/mirp/config_settings.xml
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.519610 mirp-2.2.1/mirp/data_import/
--rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/data_import/__init__.py
--rw-rw-rw-   0        0        0     8904 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/data_import/import_image.py
--rw-rw-rw-   0        0        0    16692 2024-04-17 12:57:14.000000 mirp-2.2.1/mirp/data_import/import_image_and_mask.py
--rw-rw-rw-   0        0        0     5072 2024-04-05 08:18:29.000000 mirp-2.2.1/mirp/data_import/import_mask.py
--rw-rw-rw-   0        0        0    17516 2024-04-03 12:22:01.000000 mirp-2.2.1/mirp/deep_learning_preprocessing.py
--rw-rw-rw-   0        0        0     1417 2024-04-03 12:34:47.000000 mirp-2.2.1/mirp/deprecated.py
--rw-rw-rw-   0        0        0    21617 2024-04-09 05:58:15.000000 mirp-2.2.1/mirp/extract_features_and_images.py
--rw-rw-rw-   0        0        0     4422 2024-04-05 14:31:39.000000 mirp-2.2.1/mirp/extract_image_parameters.py
--rw-rw-rw-   0        0        0     4363 2024-04-05 14:31:39.000000 mirp-2.2.1/mirp/extract_mask_labels.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.530621 mirp-2.2.1/mirp/settings/
--rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.1/mirp/settings/__init__.py
--rw-rw-rw-   0        0        0    34723 2024-04-03 13:34:07.000000 mirp-2.2.1/mirp/settings/feature_parameters.py
--rw-rw-rw-   0        0        0     3811 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/general_parameters.py
--rw-rw-rw-   0        0        0     8382 2024-03-27 09:37:42.000000 mirp-2.2.1/mirp/settings/generic.py
--rw-rw-rw-   0        0        0    22952 2024-04-16 14:53:14.000000 mirp-2.2.1/mirp/settings/image_processing_parameters.py
--rw-rw-rw-   0        0        0     6596 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/import_config_parameters.py
--rw-rw-rw-   0        0        0     5665 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/import_data_parameters.py
--rw-rw-rw-   0        0        0    10008 2024-04-03 14:06:25.000000 mirp-2.2.1/mirp/settings/interpolation_parameters.py
--rw-rw-rw-   0        0        0    13717 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/perturbation_parameters.py
--rw-rw-rw-   0        0        0     4149 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/resegmentation_parameters.py
--rw-rw-rw-   0        0        0    66066 2024-04-03 13:49:05.000000 mirp-2.2.1/mirp/settings/transformation_parameters.py
--rw-rw-rw-   0        0        0     6872 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.534623 mirp-2.2.1/mirp/utilities/
--rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.1/mirp/utilities/__init__.py
--rw-rw-rw-   0        0        0     2551 2024-04-04 15:10:05.000000 mirp-2.2.1/mirp/utilities/config_utilities.py
--rw-rw-rw-   0        0        0     2533 2024-03-27 10:48:43.000000 mirp-2.2.1/mirp/utilities/parallel.py
--rw-rw-rw-   0        0        0      862 2024-01-25 14:55:38.000000 mirp-2.2.1/mirp/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.535625 mirp-2.2.1/mirp.egg-info/
--rw-rw-rw-   0        0        0    26846 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3473 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      291 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1749 2024-04-09 10:25:45.000000 mirp-2.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 14:44:44.538627 mirp-2.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.263760 mirp-2.2.2/
+-rw-rw-rw-   0        0        0     1375 2024-04-19 15:02:24.000000 mirp-2.2.2/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    14139 2020-10-01 17:38:34.000000 mirp-2.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       33 2023-10-27 15:27:23.000000 mirp-2.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    13914 2024-05-15 14:08:30.000000 mirp-2.2.2/NEWS.md
+-rw-rw-rw-   0        0        0    26846 2024-05-15 14:40:16.263760 mirp-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8958 2024-04-19 15:02:24.000000 mirp-2.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.191250 mirp-2.2.2/mirp/
+-rw-rw-rw-   0        0        0      927 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.206876 mirp-2.2.2/mirp/_data_import/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_data_import/__init__.py
+-rw-rw-rw-   0        0        0    26667 2024-05-15 13:36:58.000000 mirp-2.2.2/mirp/_data_import/dicom_file.py
+-rw-rw-rw-   0        0        0     4595 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_data_import/dicom_file_ct.py
+-rw-rw-rw-   0        0        0     6577 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_data_import/dicom_file_mr.py
+-rw-rw-rw-   0        0        0    37948 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/dicom_file_pet.py
+-rw-rw-rw-   0        0        0     7411 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/dicom_file_rtdose.py
+-rw-rw-rw-   0        0        0    31477 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/dicom_file_rtstruct.py
+-rw-rw-rw-   0        0        0    21685 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/dicom_file_seg.py
+-rw-rw-rw-   0        0        0    10946 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/dicom_file_stack.py
+-rw-rw-rw-   0        0        0    22746 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_data_import/directory.py
+-rw-rw-rw-   0        0        0    47568 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/generic_file.py
+-rw-rw-rw-   0        0        0    11427 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/generic_file_stack.py
+-rw-rw-rw-   0        0        0     6742 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/itk_file.py
+-rw-rw-rw-   0        0        0     7260 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/itk_file_stack.py
+-rw-rw-rw-   0        0        0    13474 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_data_import/mask_contour.py
+-rw-rw-rw-   0        0        0     6211 2024-04-26 05:56:18.000000 mirp-2.2.2/mirp/_data_import/numpy_file.py
+-rw-rw-rw-   0        0        0     2944 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_data_import/numpy_file_stack.py
+-rw-rw-rw-   0        0        0     1308 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_data_import/read_data.py
+-rw-rw-rw-   0        0        0    22434 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_data_import/suv.py
+-rw-rw-rw-   0        0        0    17570 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_data_import/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.216879 mirp-2.2.2/mirp/_featuresets/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/__init__.py
+-rw-rw-rw-   0        0        0    21581 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/cm.py
+-rw-rw-rw-   0        0        0    11525 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_featuresets/dzm.py
+-rw-rw-rw-   0        0        0     6917 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/intensity_histogram.py
+-rw-rw-rw-   0        0        0    10922 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/intensity_volume_histogram.py
+-rw-rw-rw-   0        0        0     6275 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/local_intensity.py
+-rw-rw-rw-   0        0        0    32515 2024-04-24 13:17:42.000000 mirp-2.2.2/mirp/_featuresets/morphology_3d.py
+-rw-rw-rw-   0        0        0    13752 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/ngldm.py
+-rw-rw-rw-   0        0        0    12853 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/ngtdm.py
+-rw-rw-rw-   0        0        0    18910 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/rlm.py
+-rw-rw-rw-   0        0        0     4278 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/statistics.py
+-rw-rw-rw-   0        0        0    10900 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_featuresets/szm.py
+-rw-rw-rw-   0        0        0     3185 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_featuresets/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.216879 mirp-2.2.2/mirp/_image_processing/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_image_processing/__init__.py
+-rw-rw-rw-   0        0        0     2808 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_image_processing/alter_mask.py
+-rw-rw-rw-   0        0        0     1223 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_image_processing/anti_aliasing.py
+-rw-rw-rw-   0        0        0     4256 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_image_processing/cropping.py
+-rw-rw-rw-   0        0        0     5128 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_image_processing/discretise_image.py
+-rw-rw-rw-   0        0        0     2004 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_image_processing/randomise_mask.py
+-rw-rw-rw-   0        0        0     1597 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_image_processing/split_mask.py
+-rw-rw-rw-   0        0        0     2696 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_image_processing/tissue_mask.py
+-rw-rw-rw-   0        0        0     2656 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_image_processing/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.232508 mirp-2.2.2/mirp/_imagefilters/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/__init__.py
+-rw-rw-rw-   0        0        0     1454 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/exponential_transform.py
+-rw-rw-rw-   0        0        0     9339 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/gabor.py
+-rw-rw-rw-   0        0        0     6436 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_imagefilters/gaussian.py
+-rw-rw-rw-   0        0        0      562 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/generic.py
+-rw-rw-rw-   0        0        0     7495 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/laplacian_of_gaussian.py
+-rw-rw-rw-   0        0        0     7321 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/laws.py
+-rw-rw-rw-   0        0        0     1496 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/log_transform.py
+-rw-rw-rw-   0        0        0     2546 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/mean.py
+-rw-rw-rw-   0        0        0     9798 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/nonseparable_wavelet.py
+-rw-rw-rw-   0        0        0     7484 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/separable_wavelet.py
+-rw-rw-rw-   0        0        0     1261 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/square_root_transform.py
+-rw-rw-rw-   0        0        0     1230 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/square_transform.py
+-rw-rw-rw-   0        0        0    23965 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_imagefilters/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.248134 mirp-2.2.2/mirp/_images/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_images/__init__.py
+-rw-rw-rw-   0        0        0     9143 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_images/base_image.py
+-rw-rw-rw-   0        0        0     2115 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_images/ct_image.py
+-rw-rw-rw-   0        0        0    51861 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_images/generic_image.py
+-rw-rw-rw-   0        0        0    22184 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_images/mask_image.py
+-rw-rw-rw-   0        0        0     1939 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_images/mr_image.py
+-rw-rw-rw-   0        0        0     2204 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_images/pet_image.py
+-rw-rw-rw-   0        0        0     1908 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_images/rtdose_image.py
+-rw-rw-rw-   0        0        0    26540 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_images/transformed_image.py
+-rw-rw-rw-   0        0        0     4644 2024-04-23 06:26:31.000000 mirp-2.2.2/mirp/_images/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.248134 mirp-2.2.2/mirp/_masks/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_masks/__init__.py
+-rw-rw-rw-   0        0        0    28747 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_masks/base_mask.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.248134 mirp-2.2.2/mirp/_workflows/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_workflows/__init__.py
+-rw-rw-rw-   0        0        0      328 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/_workflows/baseWorkflow.py
+-rw-rw-rw-   0        0        0    35003 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/_workflows/standardWorkflow.py
+-rw-rw-rw-   0        0        0     3379 2023-10-27 15:27:23.000000 mirp-2.2.2/mirp/config_data.xml
+-rw-rw-rw-   0        0        0    21398 2024-04-23 14:07:10.000000 mirp-2.2.2/mirp/config_settings.xml
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.248134 mirp-2.2.2/mirp/data_import/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/data_import/__init__.py
+-rw-rw-rw-   0        0        0     8904 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/data_import/import_image.py
+-rw-rw-rw-   0        0        0    16692 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/data_import/import_image_and_mask.py
+-rw-rw-rw-   0        0        0     5072 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/data_import/import_mask.py
+-rw-rw-rw-   0        0        0    17512 2024-04-23 10:30:50.000000 mirp-2.2.2/mirp/deep_learning_preprocessing.py
+-rw-rw-rw-   0        0        0     1417 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/deprecated.py
+-rw-rw-rw-   0        0        0    30395 2024-04-24 11:59:18.000000 mirp-2.2.2/mirp/extract_features_and_images.py
+-rw-rw-rw-   0        0        0     4422 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/extract_image_parameters.py
+-rw-rw-rw-   0        0        0     4363 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/extract_mask_labels.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.263760 mirp-2.2.2/mirp/settings/
+-rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.2/mirp/settings/__init__.py
+-rw-rw-rw-   0        0        0    34723 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/settings/feature_parameters.py
+-rw-rw-rw-   0        0        0     3811 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/settings/general_parameters.py
+-rw-rw-rw-   0        0        0     8382 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/settings/generic.py
+-rw-rw-rw-   0        0        0    23034 2024-04-23 13:55:18.000000 mirp-2.2.2/mirp/settings/image_processing_parameters.py
+-rw-rw-rw-   0        0        0     6844 2024-04-23 13:36:47.000000 mirp-2.2.2/mirp/settings/import_config_parameters.py
+-rw-rw-rw-   0        0        0     5665 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/settings/import_data_parameters.py
+-rw-rw-rw-   0        0        0    10008 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/settings/interpolation_parameters.py
+-rw-rw-rw-   0        0        0    13717 2024-03-18 16:02:31.000000 mirp-2.2.2/mirp/settings/perturbation_parameters.py
+-rw-rw-rw-   0        0        0     4074 2024-04-23 10:29:09.000000 mirp-2.2.2/mirp/settings/resegmentation_parameters.py
+-rw-rw-rw-   0        0        0    66066 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/settings/transformation_parameters.py
+-rw-rw-rw-   0        0        0     7288 2024-04-23 13:15:03.000000 mirp-2.2.2/mirp/settings/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.263760 mirp-2.2.2/mirp/utilities/
+-rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.2/mirp/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2551 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/utilities/config_utilities.py
+-rw-rw-rw-   0        0        0     2533 2024-04-19 15:02:24.000000 mirp-2.2.2/mirp/utilities/parallel.py
+-rw-rw-rw-   0        0        0      862 2024-01-25 14:55:38.000000 mirp-2.2.2/mirp/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:40:16.263760 mirp-2.2.2/mirp.egg-info/
+-rw-rw-rw-   0        0        0    26846 2024-05-15 14:40:16.000000 mirp-2.2.2/mirp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3473 2024-05-15 14:40:16.000000 mirp-2.2.2/mirp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:40:16.000000 mirp-2.2.2/mirp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      291 2024-05-15 14:40:16.000000 mirp-2.2.2/mirp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 14:40:16.000000 mirp-2.2.2/mirp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1810 2024-05-15 13:55:54.000000 mirp-2.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:40:16.263760 mirp-2.2.2/setup.cfg
```

### Comparing `mirp-2.2.1/CONTRIBUTING.md` & `mirp-2.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/LICENSE.txt` & `mirp-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/NEWS.md` & `mirp-2.2.2/NEWS.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+# Version 2.2.2
+
+## Minor changes
+
+- `show` method of `GenericImage` and subclasses now indicate if a user-provided `slice_id` is out-of-volume and 
+  select the nearest slice instead.
+
+- Naming of branches in the settings `xml` file now matches that of their respective settings classes. `xml` files 
+  with the previous branch names still function.
+
+- Errors encountered during file import and handling are now more descriptive.
+- `extract_mask_labels` and `extract_image_parameters` now export extra information from DICOM metadata, e.g. series 
+  UID.
+
+## Documentation
+
+- Added a new tutorial on applying image filters to images.
+- Added documentation on the feature naming system.
+- Added documentation on the design of MIRP.
+
+## Fixes
+
+- Computing features related to the minimum volume enclosing ellipsoid no longer produces warnings due to the use of 
+  deprecated `numpy.matrix` class.
+
 # Version 2.2.1
 
 ## Minor changes
 
 - If mask-related parameters are not provided for computing features or processing of images for deep learning, a 
   mask is generated that covers the entire image.
```

### Comparing `mirp-2.2.1/PKG-INFO` & `mirp-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirp
-Version: 2.2.1
+Version: 2.2.2
 Summary: A package for standardised processing of medical imaging and computation of quantitative features.
 Author-email: Alex Zwanenburg <alexander.zwanenburg@nct-dresden.de>
 License: European Union Public Licence
         V. 1.2
         
         EUPL © the European Union 2007, 2016
```

### Comparing `mirp-2.2.1/README.md` & `mirp-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/__init__.py` & `mirp-2.2.2/mirp/__init__.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_data_import/dicom_file.py` & `mirp-2.2.2/mirp/_data_import/dicom_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,16 +103,18 @@
 
     def _check_modality(self, raise_error: bool) -> bool:
         dicom_modality = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0060), tag_type="str")
         support_modalities = supported_image_modalities(self.modality)
         if dicom_modality.lower() not in support_modalities:
             if raise_error:
                 raise ValueError(
-                    f"The current DICOM file {self.file_path} does not have the expected modality. "
-                    f"Found: {dicom_modality.lower()}. Expected: {', '.join(support_modalities)}")
+                    f"The current DICOM file does not have the expected modality. "
+                    f"Found: {dicom_modality.lower()}. Expected: one of {', '.join(support_modalities)}. "
+                    f"[{self.describe_self()}]"
+                )
 
             return False
 
         return True
 
     def _check_sample_name(self, raise_error: bool) -> bool:
         if self.sample_name is not None:
@@ -136,17 +138,18 @@
             ]
 
             if len(dicom_sample_name) > 0:
                 matching_sample_name = set(dicom_sample_name).intersection(set(allowed_sample_name))
                 if len(matching_sample_name) == 0:
                     if raise_error:
                         raise ValueError(
-                            f"The current DICOM file {self.file_path} does not have a matching sample name among "
-                            f"potential identifiers. Potential identifiers: {', '.join(dicom_sample_name)}; "
-                            f"Expected identifiers: {', '.join(allowed_sample_name)}."
+                            f"The current DICOM file does not have a matching sample name among potential identifiers. "
+                            f"Potential identifiers: {', '.join(dicom_sample_name)}; "
+                            f"Expected identifiers: {', '.join(allowed_sample_name)}. "
+                            f"[{self.describe_self()}]"
                         )
                     else:
                         return False
 
                 return True
         else:
             return True
@@ -165,15 +168,15 @@
         from mirp._data_import.dicom_file_rtdose import ImageDicomFileRTDose
 
         # Load metadata so that the modality tag can be read.
         self.load_metadata(limited=True)
         modality = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0060), tag_type="str").lower()
 
         if modality is None:
-            raise TypeError(f"Modality attribute could not be obtained from DICOM file ({self.file_path})")
+            raise TypeError(f"Modality attribute could not be obtained from DICOM file. [{self.describe_self()}]")
 
         if modality == "ct":
             file_class = ImageDicomFileCT
         elif modality == "pt":
             file_class = ImageDicomFilePT
         elif modality == "mr":
             file_class = ImageDicomFileMR
@@ -208,34 +211,42 @@
 
         # complete loads metadata.
         super().complete(remove_metadata=False, force=force)
 
         # Set SOP instance UID.
         if self.sop_instance_uid is None:
             self.load_metadata(limited=True)
-            self.sop_instance_uid = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0018), tag_type="str")
+            self.sop_instance_uid = get_pydicom_meta_tag(
+                dcm_seq=self.image_metadata,
+                tag=(0x0008, 0x0018),
+                tag_type="str"
+            )
 
         # Set Frame of Reference UID (if any)
         self._complete_frame_of_reference_uid()
 
         # Set series UID
         if self.series_instance_uid is None:
             self.load_metadata(limited=True)
-            self.series_instance_uid = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0020, 0x000E), tag_type="str")
+            self.series_instance_uid = get_pydicom_meta_tag(
+                dcm_seq=self.image_metadata,
+                tag=(0x0020, 0x000E),
+                tag_type="str"
+            )
 
         if remove_metadata:
             self.remove_metadata()
 
     def _complete_modality(self):
         if self.modality is None:
             self.load_metadata(limited=True)
             self.modality = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0060), tag_type="str")
 
         if self.modality is None:
-            warn(f"Could not ascertain the modality from the DICOM file ({self.file_path}).", UserWarning)
+            warn(f"Could not ascertain the modality from the DICOM file. [{self.describe_self()}]", UserWarning)
 
             self.modality = "generic"
         else:
             self.modality = self.modality.lower()
 
     def _complete_sample_name(self):
         # Set sample name -- note that if sample_name is a (single) string, it is neither replaced nor updated.
@@ -381,15 +392,16 @@
 
         # A full image metadata set exists.
         if self.image_metadata is not None and not self.is_limited_metadata:
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
-                f"The image file could not be found at the expected location: {self.file_path}")
+                f"The image file could not be found at the expected location: {self.file_path}. "
+                f"[{self.describe_self()}]")
 
         if limited:
             dcm = dcmread(
                 self.file_path,
                 stop_before_pixels=True,
                 force=True,
                 specific_tags=self._get_limited_metadata_tags()
@@ -416,19 +428,19 @@
         :return:
         """
         if self.image_data is not None:
             return self.image_data
 
         if self.file_path is not None and not os.path.exists(self.file_path):
             raise FileNotFoundError(
-                f"The image file could not be found at the expected location: {self.file_path}"
+                f"The image file could not be found at the expected location: {self.file_path}. [{self.describe_self()}]"
             )
 
         if self.file_path is None:
-            raise ValueError(f"A path to a file was expected, but not present.")
+            raise ValueError(f"A path to a file was expected, but not present. [{self.describe_self()}]")
 
         # Load metadata.
         self.load_metadata(include_image=True)
         image_data = self.image_metadata.pixel_array.astype(np.float32)
 
         # Update data with scale and intercept. These may change per slice.
         rescale_intercept = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x1052), tag_type="float", default=0.0)
@@ -512,31 +524,66 @@
             acquisition_ref_time = convert_dicom_time(
                 date_str=acquisition_start_date,
                 time_str=acquisition_start_time
             )
 
         # Final check.
         if acquisition_ref_time is None:
-            raise ValueError(f"Acquisition start time cannot be determined from DICOM metadata in {self.file_path}.")
+            raise ValueError(
+                f"Acquisition start time cannot be determined from DICOM metadata."
+            )
 
         return acquisition_ref_time
 
+    def _get_export_attributes(self) -> dict[str, Any]:
+        attributes = []
+        self.load_metadata()
+
+        study_description = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x1030), tag_type="str")
+        if study_description is not None and study_description != "":
+            attributes += [("study_description", study_description)]
+
+        series_description = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x103E), tag_type="str")
+        if series_description is not None and series_description != "":
+            attributes += [("series_description", series_description)]
+
+        # Try to find the acquisition time (which may be equal to series time).
+        try:
+            acquisition_time = self._get_acquisition_start_time()
+        except ValueError:
+            acquisition_time = None
+        if acquisition_time is not None:
+            attributes += [("acquisition_time", acquisition_time)]
+
+        if self.series_instance_uid is not None:
+            attributes += [("series_instance_uid", self.series_instance_uid)]
+        if self.frame_of_reference_uid is not None:
+            attributes += [("frame_of_reference_uid", self.frame_of_reference_uid)]
+
+        parent_attributes = super()._get_export_attributes()
+        parent_attributes.update(dict(attributes))
+
+        return parent_attributes
+
 
 class MaskDicomFile(ImageDicomFile, MaskFile):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def _check_modality(self, raise_error: bool) -> bool:
         dicom_modality = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0060), tag_type="str")
         support_modalities = supported_mask_modalities(self.modality)
         if dicom_modality.lower() not in support_modalities:
             if raise_error:
                 raise ValueError(
-                    f"The current DICOM file {self.file_path} does not have the expected modality. "
-                    f"Found: {dicom_modality.lower()}. Expected: {', '.join(support_modalities)}")
+                    f"The current DICOM file does not have the expected modality. "
+                    f"Found: {dicom_modality.lower()}. "
+                    f"Expected: {', '.join(support_modalities)}. "
+                    f"[{self.describe_self()}]"
+                )
 
             return False
 
         return True
 
     def load_data(self, **kwargs):
         raise NotImplementedError(
@@ -557,15 +604,15 @@
 
         # Load metadata so that the modality tag can be read.
         self.load_metadata(limited=True)
 
         modality = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0060), tag_type="str").lower()
 
         if modality is None:
-            raise TypeError(f"Modality attribute could not be obtained from DICOM file ({self.file_path})")
+            raise TypeError(f"Modality attribute could not be obtained from the DICOM file. [{self.describe_self()}]")
 
         if modality == "rtstruct":
             file_class = MaskDicomFileRTSTRUCT
         elif modality == "seg":
             file_class = MaskDicomFileSEG
         else:
             return None
```

### Comparing `mirp-2.2.1/mirp/_data_import/dicom_file_ct.py` & `mirp-2.2.2/mirp/_data_import/dicom_file_ct.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_data_import/dicom_file_mr.py` & `mirp-2.2.2/mirp/_data_import/dicom_file_mr.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_data_import/dicom_file_pet.py` & `mirp-2.2.2/mirp/_data_import/dicom_file_pet.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,36 +49,52 @@
     def load_data(
             self,
             pet_suv_conversion: str = "body_weight",
             **kwargs
     ):
         image_data = self.load_data_generic()
 
+        conversion_possible = True
         # Get decay correction factor
         try:
             decay_factor = self._get_administration_decay_factor()
         except ValueError as err:
             warnings.warn(
-                f"Decay correction factor could not be determined. {str(err)}",
+                f"SUV cannot be computed as decay correction factor could not be determined. {str(err)}",
                 UserWarning
             )
+            conversion_possible = False
             decay_factor = 1.0
 
         # Get conversion factor to BQML
         try:
             bqml_factor = self._get_pet_unit_conversion_factor()
         except ValueError as err:
-            warnings.warn(
-                f"BQML conversion factor could not be determined. {str(err)}",
-                UserWarning
-            )
+            if pet_suv_conversion != "none":
+                warnings.warn(
+                    f"SUV cannot be computed. BQML conversion factor could not be determined. {str(err)}",
+                    UserWarning
+                )
+            conversion_possible = False
+            bqml_factor = 1.0
+
+        except NotImplementedError as err:
+            if pet_suv_conversion != "none":
+                warnings.warn(
+                    f"SUV cannot be computed. BQML conversion factor could not be determined. {str(err)}",
+                    UserWarning
+                )
+            conversion_possible = False
             bqml_factor = 1.0
 
         # Get SUV conversion factor.
-        suv_factor = self._get_suv_conversion_factor(new_suv_type=pet_suv_conversion)
+        if conversion_possible:
+            suv_factor = self._get_suv_conversion_factor(new_suv_type=pet_suv_conversion)
+        else:
+            suv_factor = 1.0
 
         # Update image_data
         image_data *= decay_factor * bqml_factor * suv_factor
 
         # Set image data.
         self.image_data = image_data
 
@@ -457,15 +473,15 @@
                 tag_type="str"
             )
             admin_ref_time = convert_dicom_time(datetime_str=admin_ref_time)
 
         # Final check.
         if admin_ref_time is None:
             raise ValueError(
-                f"Radiopharmaceutical start time cannot be determined from DICOM metadata in {self.file_path}."
+                f"Radiopharmaceutical start time cannot be determined from DICOM metadata. [{self.describe_self()}]"
             )
 
         return admin_ref_time
 
     def _get_administration_decay_factor(self) -> float:
         self.load_metadata()
 
@@ -477,41 +493,41 @@
             default="NONE"
         )
         if decay_correction == "ADMIN":
             return 1.0
 
         elif decay_correction not in ["NONE", "START"]:
             raise ValueError(
-                f"Decay correction DICOM tag in {self.file_path} was not recognised: {decay_correction}. One of ",
-                f"NONE, START or ADMIN was expected."
+                f"Decay correction DICOM tag was not recognised: {decay_correction}. One of ",
+                f"NONE, START or ADMIN was expected. [{self.describe_self()}]"
             )
 
         # Get acquisition start time and tracer administration time.
         acquisition_start_time = self._get_acquisition_start_time()
         tracer_administration_time = self._get_tracer_administration_time()
 
         # Get frame duration in seconds.
         frame_duration = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0018, 0x1242), tag_type="float")
         if frame_duration is None:
-            raise ValueError(f"Frame duration cannot be determined from DICOM metadata in {self.file_path}.")
+            raise ValueError(f"Frame duration cannot be determined from DICOM metadata. [{self.describe_self()}]")
         frame_duration /= 1000.0  # From milliseconds to seconds.
 
         # Radionuclide total dose and radionuclide half-life
         half_life = None
         if get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0054, 0x0016), test_tag=True):
             half_life = get_pydicom_meta_tag(
                 dcm_seq=self.image_metadata[0x0054, 0x0016][0],
                 tag=(0x0018, 0x1075),
                 tag_type="float"
             )
 
         if half_life is None:
             raise ValueError(
                 f"Radionuclide half-life (0x0018, 0x1075) was missing in the Radiopharmaceutical "
-                f"information sequence (0x0054, 0x0016) of {self.file_path}."
+                f"information sequence (0x0054, 0x0016). [{self.describe_self()}]"
             )
 
         # Decay constant.
         _lambda = np.log(2.0) / half_life
 
         # Process for different decay corrections
         if decay_correction == "NONE":
@@ -528,56 +544,66 @@
 
         elif decay_correction == "START":
             # Decay correction of pixel values for the period from pixel acquisition up to scan start
             # Additionally correct for decay between administration and acquisition start. Based on QIBA SUV
             # vendorneutral pseudocode.
 
             # Get frame_reference_time in seconds.
-            frame_reference_time = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0054, 0x1300), tag_type="float")
+            frame_reference_time = get_pydicom_meta_tag(
+                dcm_seq=self.image_metadata,
+                tag=(0x0054, 0x1300),
+                tag_type="float"
+            )
             if frame_reference_time is None:
-                raise ValueError(f"Frame reference time (0x0054, 0x1300) was missing in {self.file_path}.")
+                raise ValueError(f"Frame reference time (0x0054, 0x1300) was missing. [{self.describe_self()}]")
             frame_reference_time /= 1000.0
 
             # Time at which the average count rate is found, relative to acquisition start time.
-            time_count_average = 1.0 / _lambda * np.log(_lambda * frame_duration / (1.0 - np.exp(-_lambda * frame_duration)))
+            time_count_average = 1.0 / _lambda * np.log(
+                _lambda * frame_duration / (1.0 - np.exp(-_lambda * frame_duration))
+            )
 
             # Set reference start time (this may coincide with the acquisition start time).
-            reference_start_time = acquisition_start_time + datetime.timedelta(seconds=time_count_average - frame_reference_time)
+            reference_start_time = acquisition_start_time + datetime.timedelta(
+                seconds=time_count_average - frame_reference_time
+            )
             time_to_reference_start = reference_start_time - tracer_administration_time
             time_to_reference_start = (
                     time_to_reference_start.days * 86400.0 +
                     time_to_reference_start.seconds +
                     time_to_reference_start.microseconds / 1000000.0
             )
             decay_factor = np.exp(_lambda * time_to_reference_start)
 
         else:
             raise ValueError(
-                f"Decay correction DICOM tag in {self.file_path} was not recognised: {decay_correction}. One of ",
-                f"NONE, START or ADMIN was expected."
+                f"Decay correction DICOM tag was not recognised: {decay_correction}. One of NONE, START or ADMIN "
+                f"was expected. [{self.describe_self()}]"
             )
 
         return decay_factor
 
     def _get_pet_unit_conversion_factor(self) -> float:
         """To compute SUV, PET units need to be converted to BQML."""
         self.load_metadata()
 
         pet_unit = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0054, 0x1001), tag_type="str")
         if pet_unit is None:
-            raise ValueError(f"PET Units (0x0054, 0x1001) was missing in {self.file_path}.")
+            raise ValueError(f"PET Units (0x0054, 0x1001) was missing. [{self.describe_self()}]")
 
         if pet_unit in ["CNTS", "CPS"]:
             conversion_factor = self._pet_unit_cnt_to_bqml()
         elif pet_unit in ["BQML"]:
             conversion_factor = 1.0
         elif pet_unit in ["GML", "CM2ML"]:
             conversion_factor = 1.0
         else:
-            raise NotImplementedError(f"Conversion factor for converting {pet_unit} to BQML is not implemented")
+            raise NotImplementedError(
+                f"Conversion factor for converting {pet_unit} to BQML is not implemented. [{self.describe_self()}]"
+            )
 
         return conversion_factor
 
     def _pet_unit_cnt_to_bqml(self) -> float:
         self.load_metadata()
 
         pet_unit = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0054, 0x1001), tag_type="str")
@@ -591,42 +617,47 @@
             if pet_unit == "CNTS":
                 frame_duration = get_pydicom_meta_tag(
                     dcm_seq=self.image_metadata,
                     tag=(0x0018, 0x1242),
                     tag_type="float"
                 )
                 if frame_duration is None:
-                    raise ValueError(f"Frame duration cannot be determined from DICOM metadata in {self.file_path}.")
+                    raise ValueError(
+                        f"Frame duration cannot be determined from DICOM metadata. [{self.describe_self()}]"
+                    )
                 frame_duration /= 1000.0  # From milliseconds to seconds.
                 conversion_factor = 1.0 / frame_duration
 
             # Radiopharmaceutical volume should come from the Radiopharmaceutical Information Sequence (0x0054, 0x0016).
             if get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0054, 0x0016), test_tag=True):
                 administered_volume = get_pydicom_meta_tag(
                     dcm_seq=self.image_metadata[0x0054, 0x0016][0],
                     tag=(0x0018, 0x1071),
                     tag_type="float"
                 )
                 if administered_volume is None:
                     raise ValueError(
-                        f"Radiopharmaceutical volume cannot be determined from DICOM metadata in {self.file_path}"
+                        f"Radiopharmaceutical volume cannot be determined from DICOM metadata. [{self.describe_self()}]"
                     )
 
                 # Divide by administered volume (in cubic cm == milliliter)
                 conversion_factor /= administered_volume
 
             else:
                 raise ValueError(
-                    f"Radiopharmaceutical Information Sequence (0x0054, 0x0016) is missing in DICOM metadata in "
-                    f"{self.file_path}."
+                    f"Radiopharmaceutical Information Sequence (0x0054, 0x0016) is missing in DICOM metadata. "
+                    f"[{self.describe_self()}]"
                 )
 
         # Final check
         if conversion_factor is None:
-            raise ValueError(f"Conversion factor for converting {pet_unit} to BQML could not be established")
+            raise ValueError(
+                f"Conversion factor for converting {pet_unit} to BQML could not be established. "
+                f"[{self.describe_self()}]"
+            )
 
         return conversion_factor
 
     def _get_suv_conversion_factor(self, new_suv_type: str) -> float:
         self.load_metadata()
 
         current_suv_type = get_pydicom_meta_tag(
@@ -635,15 +666,15 @@
             tag_type="str"
         )
 
         # Set SUV type based on PET unit.
         if current_suv_type is None:
             pet_unit = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0054, 0x1001), tag_type="str")
             if pet_unit is None:
-                raise ValueError(f"PET Units (0x0054, 0x1001) was missing in {self.file_path}.")
+                raise ValueError(f"PET Units (0x0054, 0x1001) was missing. [{self.describe_self()}]")
 
             if pet_unit == "GML":
                 # If absent, and the Units (0054,1001) are GML, then the type of SUV shall be assumed to be BW.
                 current_suv_type = "BW"
             elif pet_unit == "CM2ML":
                 current_suv_type = "BSA"
 
@@ -683,20 +714,21 @@
         if suv_type == "none":
             return 1.0
 
         # Require body weight and administered dose.
         patient_weight = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0010, 0x1030), tag_type="float")
         if patient_weight is None:
             raise ValueError(
-                f"Patient weight (0x0010, 0x1030) was missing in {self.file_path}. SUV normalisation is not possible."
+                f"Patient weight (0x0010, 0x1030) was missing. SUV normalisation is not possible. "
+                f"[{self.describe_self()}]"
             )
         elif patient_weight <= 0.0:
             raise ValueError(
-                f"Patient weight (0x0010, 0x1030) was not positive ({patient_weight}) in {self.file_path}. SUV "
-                f"normalisation is not possible."
+                f"Patient weight (0x0010, 0x1030) was not positive ({patient_weight}). SUV normalisation is not "
+                f"possible. [{self.describe_self()}]"
             )
         elif patient_weight >= 1000.0:
             # Weight is likely provide in grams, not kilograms. Convert to kg.
             patient_weight /= 1000.0
 
         # Administered dose should come from the Radiopharmaceutical Information Sequence (0x0054, 0x0016).
         administered_dose = None
@@ -706,38 +738,38 @@
                 dcm_seq=self.image_metadata[0x0054, 0x0016][0],
                 tag=(0x0018, 0x1074),
                 tag_type="float"
             )
 
         if administered_dose is None:
             raise ValueError(
-                f"Radionuclide Total Dose (0x0018, 0x1074) was missing in {self.file_path}. SUV normalisation is not "
-                f"possible."
+                f"Radionuclide Total Dose (0x0018, 0x1074) was missing. SUV normalisation is not possible. "
+                f"[{self.describe_self()}]"
             )
         elif administered_dose <= 0.0:
             raise ValueError(
-                f"Radionuclide Total Dose (0x0018, 0x1074) was not positive ({administered_dose}) in "
-                f"{self.file_path}. SUV normalisation is not possible."
+                f"Radionuclide Total Dose (0x0018, 0x1074) was not positive ({administered_dose}). "
+                f"SUV normalisation is not possible. [{self.describe_self()}]"
             )
 
         # Body weight-corrected SUV ------------------------------------------------------------------------------------
         if suv_type == "body_weight":
             return patient_weight * 1000.0 / administered_dose
 
         # Require patient height.
         patient_height = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0010, 0x1020), tag_type="float")
         if patient_height is None:
             raise ValueError(
-                f"Patient Size (0x0010, 0x1020) was missing in {self.file_path}. SUV normalisation ({suv_type}) is not "
-                f"possible."
+                f"Patient Size (0x0010, 0x1020) was missing. SUV normalisation ({suv_type}) is not possible. "
+                f"[{self.describe_self()}]"
             )
         elif patient_height <= 0.0:
             raise ValueError(
-                f"Patient Size (0x0010, 0x1020) was not positive ({patient_height}) in {self.file_path}. SUV "
-                f"normalisation ({suv_type}) is not possible."
+                f"Patient Size (0x0010, 0x1020) was not positive ({patient_height}). SUV normalisation ({suv_type}) "
+                f"is not possible. [{self.describe_self()}]"
             )
         elif patient_height > 3.0:
             # Interpret patient height as cm and convert to meter.
             patient_height /= 100.0
 
         # Body surface area-corrected SUV ------------------------------------------------------------------------------
         if suv_type == "body_surface_area":
@@ -746,16 +778,16 @@
 
         # Require patient biological sex.
         patient_biological_sex = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0010, 0x0040), tag_type="str")
         if patient_biological_sex is None:
             patient_biological_sex = "O"
         if patient_biological_sex.lower() not in ["m", "f", "w", "o", "d", "u"]:
             raise ValueError(
-                f"Patient Sex (0x0010, 0x0040) was not recognised ({patient_biological_sex} in {self.file_path}. SUV "
-                f"normalisation ({suv_type}) is not possible."
+                f"Patient Sex (0x0010, 0x0040) was not recognised ({patient_biological_sex}. SUV normalisation "
+                f"({suv_type}) is not possible. [{self.describe_self()}]"
             )
 
         # Erroneous lean body mass-corrected SUV -----------------------------------------------------------------------
         if suv_type == "lean_body_mass_error":
             if patient_biological_sex.lower() == "m":
                 norm_factor = 1.10 * patient_weight - 120.0 * (patient_weight ** 2.0 / (patient_height * 100.0) ** 2.0)
             elif patient_biological_sex.lower() in ["f", "w"]:
```

### Comparing `mirp-2.2.1/mirp/_data_import/dicom_file_rtdose.py` & `mirp-2.2.2/mirp/_data_import/dicom_file_rtdose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import warnings
 import os
 
 import numpy as np
 
 from typing import Any
-from pydicom import dcmread
 from mirp._data_import.dicom_file import ImageDicomFile
 from mirp._data_import.utilities import get_pydicom_meta_tag
 
 
 class ImageDicomFileRTDose(ImageDicomFile):
     def __init__(
             self,
@@ -58,15 +57,14 @@
                 dcm_seq=self.image_metadata,
                 tag=(0x0020, 0x0037),
                 tag_type="mult_float"
             )
 
             # First compute z-orientation.
             orientation += list(np.cross(orientation[0:3], orientation[3:6]))
-
             self.image_orientation = np.reshape(orientation[::-1], [3, 3], order="F")
 
     def _complete_image_spacing(self, force=False):
         if self.image_spacing is None:
 
             # Load relevant metadata.
             self.load_metadata(limited=True)
@@ -82,23 +80,24 @@
             )
 
             if len(z_spacing) > 1:
                 # DICOM file contains multiple frames.
                 z_spacing = np.unique(np.diff(z_spacing))
                 if len(z_spacing) > 1:
                     raise ValueError(
-                        f"Spacing of radiation dose grid in {self.file_path} is inconsistent: {', '.join(z_spacing)}"
+                        f"Spacing of radiation dose grid is inconsistent: {', '.join(z_spacing)}. "
+                        f"[{self.describe_self()}]"
                     )
                 z_spacing = z_spacing[0]
             else:
                 # DICOM file contains only a single frame. Use a default 1.0 mm value.
                 z_spacing = 1.0
                 warnings.warn(
-                    f"Radiation dose grid in {self.file_path} only contains a single frame (slice). A default frame "
-                    f"spacing of 1.0 mm is assumed. Within-plane spacing is not affected."
+                    f"Radiation dose grid only contains a single frame (slice). A default frame spacing of 1.0 mm is "
+                    f"assumed. Within-plane spacing is not affected. [{self.describe_self()}]"
                 )
 
             if z_spacing < 0.0:
                 self.image_orientation = np.matmul(
                     self.image_orientation, [[-1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
                 )
                 z_spacing = np.abs(z_spacing)
@@ -123,26 +122,31 @@
 
     def load_data(self, **kwargs):
         if self.image_data is not None:
             return self.image_data
 
         if self.file_path is not None and not os.path.exists(self.file_path):
             raise FileNotFoundError(
-                f"The image file could not be found at the expected location: {self.file_path}"
+                f"The image file could not be found at the expected location: {self.file_path} [{self.describe_self()}]"
             )
 
         if self.file_path is None:
-            raise ValueError(f"A path to a file was expected, but not present.")
+            raise ValueError(f"A path to a file was expected, but not present. [{self.describe_self()}]")
 
         # Load metadata.
         self.load_metadata(include_image=True)
         image_data = self.image_metadata.pixel_array.astype(np.float32)
 
         # Update data with dose grid scaling
-        dose_grid_scaling = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x3004, 0x000E), tag_type="float", default=1.0)
+        dose_grid_scaling = get_pydicom_meta_tag(
+            dcm_seq=self.image_metadata,
+            tag=(0x3004, 0x000E),
+            tag_type="float",
+            default=1.0
+        )
         image_data = image_data * dose_grid_scaling
 
         self.image_data = image_data
 
     def export_metadata(self, self_only: bool = False, **kwargs) -> None | dict[str, Any]:
         if not self_only:
             metadata = super().export_metadata()
```

### Comparing `mirp-2.2.1/mirp/_data_import/dicom_file_rtstruct.py` & `mirp-2.2.2/mirp/_data_import/dicom_file_rtstruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,55 +46,57 @@
 
             # Try to obtain a frame of reference UID
             if has_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0020, 0x0052)):
                 if get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0020, 0x0052), tag_type="str") is not None:
                     self.frame_of_reference_uid = get_pydicom_meta_tag(
                         dcm_seq=self.image_metadata,
                         tag=(0x0020, 0x0052),
-                        tag_type="str")
+                        tag_type="str"
+                    )
 
             # For RT structure sets, the FOR UID may be tucked away in the Structure Set ROI Sequence
             if self.frame_of_reference_uid is None and \
                     has_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x3006, 0x0020)):
                 structure_set_roi_sequence = self.image_metadata[(0x3006, 0x0020)]
 
                 for structure_set_roi_element in structure_set_roi_sequence:
                     if has_pydicom_meta_tag(dcm_seq=structure_set_roi_element, tag=(0x3006, 0x0024)):
                         self.frame_of_reference_uid = get_pydicom_meta_tag(
                             dcm_seq=structure_set_roi_element,
                             tag=(0x3006, 0x0024),
-                            tag_type="str")
+                            tag_type="str"
+                        )
                         break
 
     def check_mask(self, raise_error=True):
         if self.image_metadata is None:
             raise TypeError("DEV: the image_meta_data attribute has not been set.")
 
         if not get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x3006, 0x0020), test_tag=True):
             if raise_error:
                 warnings.warn(
-                    f"The RT-structure set ({self.file_path}) did not contain any ROI sequences.",
+                    f"The current RT-structure set did not contain any ROI sequences. [{self.describe_self()}]",
                 )
             return False
 
         roi_name_present = [
             get_pydicom_meta_tag(
                 dcm_seq=current_structure_set_roi_sequence, tag=(0x3006, 0x0026), tag_type="str", default=None)
             for current_structure_set_roi_sequence in self.image_metadata[(0x3006, 0x0020)]
         ]
 
         if len(roi_name_present) == 0 and raise_error:
             warnings.warn(
-                f"The current RT-structure set ({self.file_path}) does not contain any ROI contours."
+                f"The current RT-structure set does not contain any ROI contours. [{self.describe_self()}]"
             )
             return False
 
         if any(x is None for x in roi_name_present) and raise_error:
             warnings.warn(
-                f"The current RT-structure set ({self.file_path}) lacks one or more ROI names."
+                f"The current RT-structure set lacks one or more ROI names. [{self.describe_self()}]"
             )
             return False
 
         return True
 
     def load_data(self, **kwargs):
         pass
@@ -104,15 +106,15 @@
             image: None | ImageFile,
             **kwargs
     ) -> list[BaseMask] | None:
 
         if image is None:
             raise TypeError(
                 f"Converting an RT-structure to a segmentation mask requires that the corresponding image is set. "
-                f"No image was provided ({self.file_path})."
+                f"No image was provided. [{self.describe_self()}]"
             )
         else:
             image.complete()
 
         self.load_metadata()
         if not self.check_mask():
             return None
@@ -688,27 +690,27 @@
                     merging_contours += [contour_objects[ii]]
 
             merged_contour_list += [
                 parent_contour.merge(other_contours=merging_contours, slice_id=slice_id)]
 
         return merged_contour_list
 
-    @staticmethod
-    def _match_slice_position(slice_position, known_position, image_spacing_z):
-        # Match slice position of mask with any known slice position.
-        img_slice_position = slice_position * image_spacing_z
-        position_difference = np.around(np.abs(img_slice_position - known_position), 3)
-
-        # Check if there is any matching position.
-        if np.any(position_difference == 0.0):
-            int_slice_position = int(np.argwhere(position_difference == 0.0))
-        else:
-            int_slice_position = None
-
-        return int_slice_position
+    # @staticmethod
+    # def _match_slice_position(slice_position, known_position, image_spacing_z):
+    #     # Match slice position of mask with any known slice position.
+    #     img_slice_position = slice_position * image_spacing_z
+    #     position_difference = np.around(np.abs(img_slice_position - known_position), 3)
+    #
+    #     # Check if there is any matching position.
+    #     if np.any(position_difference == 0.0):
+    #         int_slice_position = int(np.argwhere(position_difference == 0.0))
+    #     else:
+    #         int_slice_position = None
+    #
+    #     return int_slice_position
 
     def export_roi_labels(self):
 
         self.load_metadata()
 
         # Find which roi numbers (3006,0022) are associated with which roi names (3004,0024).
         labels = [
@@ -718,13 +720,15 @@
         ]
 
         n_labels = max([1, len(labels)])
 
         if len(labels) == 0:
             labels = [None]
 
-        return {
-            "sample_name": [self.sample_name] * n_labels,
-            "dir_path": [self.dir_path] * n_labels,
-            "file_path": [self.file_name] * n_labels,
-            "roi_label": labels
-        }
+        # Get general attributes.
+        parent_attributes = self._get_export_attributes()
+
+        # Add roi labels as attribute.
+        attributes = [("roi_label", labels)]
+        parent_attributes.update(dict(attributes))
+
+        return parent_attributes
```

### Comparing `mirp-2.2.1/mirp/_data_import/dicom_file_seg.py` & `mirp-2.2.2/mirp/_data_import/dicom_file_seg.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,33 +36,33 @@
     def check_mask(self, raise_error=True):
         if self.image_metadata is None:
             raise TypeError("DEV: the image_meta_data attribute has not been set.")
 
         if not get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0062, 0x0002), test_tag=True):
             if raise_error:
                 warnings.warn(
-                    f"The SEG set ({self.file_path}) did not contain any segment sequences.",
+                    f"The current SEG set did not contain any segment sequences. [{self.describe_self()}]",
                 )
             return False
 
         roi_name_present = [
             get_pydicom_meta_tag(
                 dcm_seq=current_segment_sequence, tag=(0x0062, 0x0005), tag_type="str", default=None)
             for current_segment_sequence in self.image_metadata[(0x0062, 0x0002)]
         ]
 
         if len(roi_name_present) == 0 and raise_error:
             warnings.warn(
-                f"The current SEG set ({self.file_path}) does not contain any segmentations."
+                f"The current SEG set does not contain any segmentations. [{self.describe_self()}]"
             )
             return False
 
         if any(x is None for x in roi_name_present) and raise_error:
             warnings.warn(
-                f"The current SEG set ({self.file_path}) does not contain any labels."
+                f"The current SEG set does not contain any labels. [{self.describe_self()}]"
             )
             return False
 
         return True
 
     def load_data(self, **kwargs):
         pass
@@ -187,15 +187,17 @@
                     dcm_seq=self.image_metadata[(0x5200, 0x9230)][ii][(0x0062, 0x000A)][0],
                     tag=(0x0062, 0x000B),
                     tag_type="int",
                     default=None
                 )
 
             if current_roi_number is None:
-                raise ValueError(f"The current frame ({ii + 1}) has no associated segment number.")
+                raise ValueError(
+                    f"The current frame ({ii + 1}) has no associated segment number. [{self.describe_self()}]"
+                )
 
             if roi_index == current_roi_number:
                 yield ii
 
     def _get_mask_origin(self, frames: list[int]) -> tuple[float, ...]:
         mask_origin = None
 
@@ -211,16 +213,16 @@
 
         if mask_origin is not None:
             return tuple(mask_origin[::-1])
 
         # Check that the Per-Frame Functional Groups Sequence exists.
         if not has_pydicom_meta_tag(self.image_metadata, tag=(0x5200, 0x9230)):
             raise ValueError(
-                f"The DICOM SEG file ({self.file_path}) lacks a Per-Frame Functions Groups Sequence that is required ",
-                f"to set the spatial origin of the mask."
+                f"The DICOM SEG file lacks a Per-Frame Functions Groups Sequence that is required ",
+                f"to set the spatial origin of the mask. [{self.describe_self()}]"
             )
 
         mask_position = self._get_origin_position_table(frames=frames)
         mask_position = mask_position.iloc[0]
 
         return tuple([mask_position.position_z, mask_position.position_y, mask_position.position_x])
 
@@ -255,27 +257,27 @@
             frame_functional_group
             for ii, frame_functional_group in enumerate(self.image_metadata[(0x5200, 0x9230)])
             if ii in frames
         ]
 
         if not len(frame_functional_groups) == len(frames):
             raise ValueError(
-                f"The DICOM SEG file ({self.file_path}) does not have the same number of per-frame functional group "
+                f"The DICOM SEG file does not have the same number of per-frame functional group "
                 f"sequences ({len(frame_functional_groups)}) as the expected number of frames containing a part of "
-                f"the segmentation ({len(frames)}."
+                f"the segmentation ({len(frames)}. [{self.describe_self()}]"
             )
 
         mask_spacing_x = None
         mask_spacing_y = None
         mask_spacing_z = None
         for ii, frame_functional_group in enumerate(frame_functional_groups):
             if not has_pydicom_meta_tag(frame_functional_group, tag=(0x0028, 0x9110)):
                 raise ValueError(
-                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file ({self.file_path}) lack "
-                    f"a Pixel Measure Sequence (0028, 9110) to determine the mask spacing."
+                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file lack a Pixel Measure "
+                    f"Sequence (0028, 9110) to determine the mask spacing. [{self.describe_self()}]"
                 )
 
             pixel_spacing = get_pydicom_meta_tag(
                 dcm_seq=frame_functional_group[(0x0028, 0x9110)][0],
                 tag=(0x0028, 0x0030),
                 tag_type="mult_float",
                 default=None
@@ -286,27 +288,28 @@
                 tag=(0x0018, 0x0088),
                 tag_type="float",
                 default=None
             )
 
             if pixel_spacing is None or slice_spacing is None:
                 raise ValueError(
-                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file ({self.file_path}) lack "
-                    f"a complete Pixel Measure Sequence (0028, 9110) to determine the mask spacing."
+                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file lack a complete Pixel "
+                    f"Measure Sequence (0028, 9110) to determine the mask spacing. [{self.describe_self()}]"
                 )
 
             if mask_spacing_x is None or mask_spacing_y is None or mask_spacing_z is None:
                 mask_spacing_x = pixel_spacing[0]
                 mask_spacing_y = pixel_spacing[1]
                 mask_spacing_z = slice_spacing
 
             elif not (mask_spacing_x == pixel_spacing[0] and mask_spacing_y == pixel_spacing[1] and mask_spacing_z ==
                       slice_spacing):
                 raise ValueError(
-                    f"Inconsistent spacing detected for one or more frames of the DICOM SEG file ({self.file_path})."
+                    f"Inconsistent spacing detected for one or more frames of the DICOM SEG file. "
+                    f"[{self.describe_self()}]"
                 )
             else:
                 pass
 
         return tuple([mask_spacing_z, mask_spacing_y, mask_spacing_x])
 
     def _get_mask_orientation(self, frames: list[int], spacing: tuple[float, ...]) -> np.array:
@@ -331,46 +334,47 @@
             frame_functional_group
             for ii, frame_functional_group in enumerate(self.image_metadata[(0x5200, 0x9230)])
             if ii in frames
         ]
 
         if not len(frame_functional_groups) == len(frames):
             raise ValueError(
-                f"The DICOM SEG file ({self.file_path}) does not have the same number of per-frame functional group "
+                f"The DICOM SEG file does not have the same number of per-frame functional group "
                 f"sequences ({len(frame_functional_groups)}) as the expected number of frames containing a part of "
-                f"the segmentation ({len(frames)}."
+                f"the segmentation ({len(frames)}. [{self.describe_self()}]"
             )
 
         for ii, frame_functional_group in enumerate(frame_functional_groups):
             if not has_pydicom_meta_tag(frame_functional_group, tag=(0x0020, 0x9116)):
                 raise ValueError(
-                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file ({self.file_path}) lack "
-                    f"a Pixel Measure Sequence (0020, 9110) to determine the mask spacing."
+                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file lack "
+                    f"a Pixel Measure Sequence (0020, 9110) to determine the mask spacing. [{self.describe_self()}]"
                 )
 
             frame_mask_orientation = get_pydicom_meta_tag(
                 dcm_seq=frame_functional_group[(0x0020, 0x9116)][0],
                 tag=(0x0020, 0x0037),
                 tag_type="mult_float",
                 default=None
             )
 
             if frame_mask_orientation is None:
                 raise ValueError(
-                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file ({self.file_path}) lack "
-                    f"a complete Pixel Orientation Sequence (0020, 9116) to determine the mask orientation."
+                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file lack "
+                    f"a complete Pixel Orientation Sequence (0020, 9116) to determine the mask orientation. "
+                    f"[{self.describe_self()}]"
                 )
 
             if mask_orientation is None:
                 mask_orientation = frame_mask_orientation
 
             elif not (mask_orientation == frame_mask_orientation):
                 raise ValueError(
-                    f"Inconsistent orientation detected for one or more frames of the DICOM SEG file "
-                    f"({self.file_path})."
+                    f"Inconsistent orientation detected for one or more frames of the DICOM SEG file. "
+                    f"[{self.describe_self()}]"
                 )
             else:
                 pass
 
         mask_orientation += list(np.cross(mask_orientation[0:3], mask_orientation[3:6]))
         return np.reshape(mask_orientation[::-1], [3, 3], order="F")
 
@@ -422,37 +426,38 @@
             frame_functional_group
             for ii, frame_functional_group in enumerate(self.image_metadata[(0x5200, 0x9230)])
             if ii in frames
         ]
 
         if not len(frame_functional_groups) == len(frames):
             raise ValueError(
-                f"The DICOM SEG file ({self.file_path}) does not have the same number of per-frame functional group "
+                f"The DICOM SEG file does not have the same number of per-frame functional group "
                 f"sequences ({len(frame_functional_groups)}) as the expected number of frames containing a part of "
-                f"the segmentation ({len(frames)}."
+                f"the segmentation ({len(frames)}. [{self.describe_self()}]"
             )
 
         for ii, frame_functional_group in enumerate(frame_functional_groups):
             if not has_pydicom_meta_tag(frame_functional_group, tag=(0x0020, 0x9113)):
                 raise ValueError(
-                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file ({self.file_path}) lack "
-                    f"a Plane Position Sequence (0020, 9113) to determine the mask origin."
+                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file lack "
+                    f"a Plane Position Sequence (0020, 9113) to determine the mask origin. [{self.describe_self()}]"
                 )
 
             slice_origin = get_pydicom_meta_tag(
                 dcm_seq=frame_functional_group[(0x0020, 0x9113)][0],
                 tag=(0x0020, 0x0032),
                 tag_type="mult_float",
                 default=None
             )
 
             if slice_origin is None:
                 raise ValueError(
-                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file ({self.file_path}) lack "
-                    f"a complete Plane Position Sequence (0020, 9113) to determine the mask origin."
+                    f"One or more Per-Frame Functional Group Sequences of the DICOM SEG file lack "
+                    f"a complete Plane Position Sequence (0020, 9113) to determine the mask origin. "
+                    f"[{self.describe_self()}]"
                 )
             slice_origin = slice_origin[::-1]
 
             mask_position_z[ii] = slice_origin[0]
             mask_position_y[ii] = slice_origin[1]
             mask_position_x[ii] = slice_origin[2]
 
@@ -497,13 +502,15 @@
         ]
 
         n_labels = max([1, len(labels)])
 
         if len(labels) == 0:
             labels = [None]
 
-        return {
-            "sample_name": [self.sample_name] * n_labels,
-            "dir_path": [self.dir_path] * n_labels,
-            "file_path": [self.file_name] * n_labels,
-            "roi_label": labels
-        }
+        # Get general attributes.
+        parent_attributes = self._get_export_attributes()
+
+        # Add roi labels as attribute.
+        attributes = [("roi_label", labels)]
+        parent_attributes.update(dict(attributes))
+
+        return parent_attributes
```

### Comparing `mirp-2.2.1/mirp/_data_import/dicom_file_stack.py` & `mirp-2.2.2/mirp/_data_import/dicom_file_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,31 +129,32 @@
 
         # Find how much other slices differ.
         image_slice_spacing_multiplier = image_slice_spacing / min_slice_spacing
 
         if np.any(image_slice_spacing_multiplier > 1.2):
             warnings.warn(
                 f"Inconsistent distance between slice origins of subsequent slices: {np.unique(image_slice_spacing)}. "
-                "Slices cannot be aligned correctly. This is likely due to missing slices. "
-                "MIRP will attempt to interpolate the missing slices and their ROI masks for volumetric analysis.",
+                f"Slices cannot be aligned correctly. This is likely due to missing slices. "
+                f"MIRP will attempt to interpolate the missing slices and their ROI masks for volumetric analysis. "
+                f"[{self.describe_self()}]",
                 UserWarning)
 
         # Determine image slice spacing.
         image_slice_spacing = np.around(np.mean(image_slice_spacing[image_slice_spacing_multiplier <= 1.2]), 5)
 
         # Warn the user if there is a mismatch between slice thickness and the actual slice spacing.
         image_slice_thickness = get_pydicom_meta_tag(
             dcm_seq=self.image_file_objects[0].image_metadata,
             tag=(0x0018, 0x0050),
             tag_type="float")
 
         if not np.around(image_slice_thickness - image_slice_spacing, decimals=3) == 0.0:
             warnings.warn(
-                f"Mismatch between slice thickness ({image_slice_thickness}) and actual slice spacing"
-                f" ({image_slice_spacing}). The actual slice spacing will be used.",
+                f"Mismatch between slice thickness ({image_slice_thickness}) and actual slice spacing "
+                f"({image_slice_spacing}). The actual slice spacing will be used. [{self.describe_self()}]",
                 UserWarning)
 
         image_pixel_spacing = get_pydicom_meta_tag(
             dcm_seq=self.image_file_objects[0].image_metadata,
             tag=(0x0028, 0x0030),
             tag_type="mult_float")
```

### Comparing `mirp-2.2.1/mirp/_data_import/directory.py` & `mirp-2.2.2/mirp/_data_import/directory.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_data_import/generic_file.py` & `mirp-2.2.2/mirp/_data_import/generic_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -214,18 +214,18 @@
 
     def set_modality(self, modality: None | str):
         from mirp._data_import.utilities import supported_image_modalities
         if modality is None:
             return
 
         if not isinstance(modality, str):
-            raise ValueError(f"modality is expected to be a character string. Found: {modality}")
+            raise ValueError(f"modality is expected to be a character string. Found: {modality} [{self.describe_self()}]")
 
         if modality == "generic":
-            raise ValueError(f"modality cannot be 'generic'")
+            raise ValueError(f"modality cannot be 'generic' [{self.describe_self()}]")
 
         modality = supported_image_modalities(modality)
         if self.modality is None or self.modality == "generic":
             self.modality = modality[0]
 
     def create(self):
         # Import locally to avoid potential circular references.
@@ -255,15 +255,17 @@
         elif any(self.file_path.lower().endswith(ii) for ii in file_extensions) and\
                 any(self.file_path.lower().endswith(ii) for ii in supported_file_types("numpy")):
 
             file_class = ImageNumpyFile
             file_type = "numpy"
 
         else:
-            raise NotImplementedError(f"The provided image type is not implemented: {self.file_type}")
+            raise NotImplementedError(
+                f"The provided image type is not implemented: {self.file_type} [{self.describe_self()}]"
+            )
 
         image_file = file_class(
             file_path=self.file_path,
             dir_path=self.dir_path,
             sample_name=self.sample_name,
             file_name=self.file_name,
             image_name=self.image_name,
@@ -292,33 +294,38 @@
         # Dispatch to subclass based on file_path.
         allowed_file_extensions = supported_file_types(self.file_type)
 
         # Check that the file type is correct.
         if not self.file_path.lower().endswith(tuple(allowed_file_extensions)):
             if raise_error:
                 raise ValueError(
-                    f"The file type does not correspond to a known, implemented image type: {self.file_type}.")
+                    f"The file type does not correspond to a known, implemented image type: {self.file_type}. "
+                    f"[{self.describe_self()}]"
+                )
 
             return False
 
         # Check that the file exists.
         if not os.path.exists(self.file_path):
             if raise_error:
                 raise FileNotFoundError(
-                    f"The image file could not be found at the expected location: {self.file_path}")
+                    f"The image file could not be found at the expected location: {self.file_path} "
+                    f"[{self.describe_self()}]"
+                )
 
             return False
 
         # Check that the file name contains image_name.
         if self.image_name is not None:
             if not match_file_name(self.file_path, pattern=self.image_name, file_extension=allowed_file_extensions):
                 if raise_error:
                     raise ValueError(
                         f"The file name of the image file {os.path.basename(self.file_path)} does not match "
-                        f"the expected pattern: {self.image_name}")
+                        f"the expected pattern: {self.image_name} [{self.describe_self()}]"
+                    )
 
             return False
 
         # Check modality.
         modality_check = self._check_modality(raise_error=raise_error)
         if not modality_check:
             return False
@@ -335,103 +342,108 @@
             return True
 
         # Check that image_data has the expected type.
         if not isinstance(self.image_data, np.ndarray):
             if raise_error:
                 raise TypeError(
                     f"The image_data argument expects None or a numpy ndarray. Found object with class "
-                    f"{type(self.image_data).name}"
+                    f"{type(self.image_data).name} [{self.describe_self()}]"
                 )
             else:
                 return False
 
         # Check that image_data has up to 3 dimensions.
         data_shape = self.image_data.shape
         if not 1 <= len(data_shape) <= 3:
             if raise_error:
                 raise ValueError(
                     f"MIRP supports image data up to 3 dimensions. The current numpy array has a dimension of "
-                    f"{len(data_shape)} ({data_shape})."
+                    f"{len(data_shape)} ({data_shape}). [{self.describe_self()}]"
                 )
             else:
                 return False
 
         # Check that the shape of image_data matches that of image_dimensions.
         if self.image_dimension is not None and not np.array_equal(self.image_dimension, data_shape):
             if raise_error:
                 raise ValueError(
                     f"The shape of the image data itself and the purported shape (image_dimensions) are different. The "
                     f"current numpy array has dimensions ({data_shape}), where ({self.image_dimension}) is expected."
+                    f"[{self.describe_self()}]"
                 )
             else:
                 return False
 
         # Check that image_origin has the correct number of dimensions.
         if self.image_origin is not None and not len(data_shape) == len(self.image_origin):
             if raise_error:
                 raise ValueError(
                     f"The dimensions of the image data itself ({len(data_shape)} and the dimensions of the origin ("
-                    f"image_origin; {len(self.image_origin)}) are different."
+                    f"image_origin; {len(self.image_origin)}) are different. [{self.describe_self()}]"
                 )
             else:
                 return False
 
         # Check that image_orientation has the correct number of dimensions, and is correctly formatted.
         if self.image_orientation is not None:
             if not np.all(np.equal(self.image_orientation.shape, len(data_shape))):
                 if raise_error:
                     raise ValueError(
                         f"The orientation matrix should be square, with a dimension equal to the dimensions "
                         f"the image data itself ({len(data_shape)}. Found: {self.image_orientation.shape}."
+                        f"[{self.describe_self()}]"
                     )
                 else:
                     return False
 
         # Check that image orientation has a l2-norm of 1.0.
         if self.image_orientation is not None:
             l2_norm = np.around(np.linalg.norm(self.image_orientation, ord=2), decimals=3)
             if not l2_norm == 1.0:
                 if raise_error:
                     raise ValueError(
                         f"The orientation matrix should be square with an l2-norm of 1.0. Found: {l2_norm}."
+                        f"[{self.describe_self()}]"
                     )
                 else:
                     return False
 
         # Check that spacing has the correct number of dimensions.
         if self.image_spacing is not None:
             if not len(self.image_spacing) == len(data_shape):
                 if raise_error:
                     raise ValueError(
                         f"The dimensions of the image data itself ({len(data_shape)}) and the dimensions of the voxel "
-                        f"spacing (image_spacing; {len(self.image_spacing)}) are different."
+                        f"spacing (image_spacing; {len(self.image_spacing)}) are different. [{self.describe_self()}]"
                     )
                 else:
                     return False
 
         # Check that spacing contains strictly positive values.
         if self.image_spacing is not None:
             if np.any(np.array(self.image_spacing) <= 0.0):
                 if raise_error:
                     raise ValueError(
-                        f"Image spacing should be strictly positive. Found: {self.image_spacing}."
+                        f"Image spacing should be strictly positive. Found: {self.image_spacing}. "
+                        f"[{self.describe_self()}]"
                     )
                 else:
                     return False
 
     def _check_sample_name(self, raise_error: bool) -> bool:
         # Check that image file contains a sample name, if multiple sample names are present. To assess the filename,
         # we first strip the extension. Optionally we split the filename on the image name pattern, reducing the
         # filename into parts that should contain the sample name.
         if isinstance(self.sample_name, list) and len(self.sample_name) > 1:
             if self.get_sample_name_from_file() is None:
                 if raise_error:
                     raise ValueError(
                         f"The file name of the image file {os.path.basename(self.file_path)} does not contain "
-                        f"any of the expected patterns: {', '.join(self.sample_name)}")
+                        f"any of the expected patterns: {', '.join(self.sample_name)} [{self.describe_self()}]"
+                    )
                 else:
                     return False
 
         return True
 
     def _check_modality(self, raise_error: bool) -> bool:
         return True
@@ -560,15 +572,18 @@
 
         if len(file_name_parts) == 0:
             return None
 
         # Remove sample name.
         if self.sample_name is not None:
             if isinstance(self.sample_name, list):
-                raise TypeError("The sample_name attribute cannot be a list for extracting numeric sequences.")
+                raise TypeError(
+                    f"The sample_name attribute cannot be a list for extracting numeric sequences. "
+                    f"[{self.describe_self()}]"
+                )
 
             file_name_parts = [
                 current_file_name_part.split(sep=self.sample_name)
                 for current_file_name_part in file_name_parts
             ]
 
             # Flatten list
@@ -684,25 +699,25 @@
     def update_image_data(self):
         if self.image_data is None:
             return
 
         if not isinstance(self.image_data, np.ndarray):
             raise TypeError(
                 f"The image_data argument expects None or a numpy ndarray. Found object with class "
-                f"{type(self.image_data).name}"
+                f"{type(self.image_data).name}. [{self.describe_self()}]"
             )
 
         # If the image is already 3D, we forgo adding dimensions.
         if len(self.image_data.shape) == 3:
             return
 
         if not 1 <= len(self.image_data.shape) <= 3:
             raise ValueError(
                 f"MIRP supports image data up to 3 dimensions. The current numpy array has a dimension of "
-                f"{len(self.image_data.shape)} ({self.image_data.shape})."
+                f"{len(self.image_data.shape)} ({self.image_data.shape}). [{self.describe_self()}]"
             )
 
         dims_to_add = 3 - len(self.image_data.shape)
 
         # Add new dimensions to image.
         if dims_to_add == 2:
             self.image_data = self.image_data[np.newaxis, np.newaxis, :]
@@ -766,27 +781,44 @@
             image_spacing=self.image_spacing,
             image_origin=self.image_origin,
             image_orientation=self.image_orientation,
             image_dimensions=self.image_dimension
         )
 
     def export_metadata(self, **kwargs) -> None | dict[str, Any]:
+        # Get general attributes.
+        parent_attributes = self._get_export_attributes()
+
+        # Add metadata.
         metadata = []
-        if self.sample_name is not None:
-            metadata += [("sample_name", self.sample_name)]
-        if self.modality is not None:
-            metadata += [("modality", self.modality)]
         if self.image_spacing is not None:
             metadata += [
                 ("spacing_z", self.image_spacing[0]),
                 ("spacing_y", self.image_spacing[1]),
                 ("spacing_x", self.image_spacing[2])
             ]
+        parent_attributes.update(dict(metadata))
 
-        return dict(metadata)
+        return parent_attributes
+
+    def _get_export_attributes(self) -> dict[str, Any]:
+        attributes = []
+        if self.sample_name is not None:
+            attributes += [("sample_name", self.sample_name)]
+        if self.modality is not None:
+            attributes += [("modality", self.modality)]
+        if self.dir_path is not None:
+            attributes += [("dir_path", self.dir_path)]
+        if self.file_name is not None:
+            attributes += [("file_name", self.file_name)]
+
+        return dict(attributes)
+
+    def describe_self(self):
+        return f"{self._get_export_attributes()}"
 
 
 class MaskFile(ImageFile):
 
     def __init__(
             self,
             roi_name: None | str | list[str] | dict[str, str] = None,
@@ -799,15 +831,15 @@
             (isinstance(roi_name, list) and all(isinstance(x, str) for x in roi_name)) or \
                 (isinstance(roi_name, dict) and all(isinstance(x, str) for x in roi_name.values()) and all(
                     isinstance(x, str) for x in roi_name.keys())):
             self.roi_name = roi_name
         else:
             raise TypeError(
                 f"ROI names are expected to be a string, a list of strings, or a dictionary of strings. Found:"
-                f" {roi_name} with type {type(roi_name)}.")
+                f" {roi_name} with type {type(roi_name)}. [{self.describe_self()}]")
 
     def is_stackable(self, stack_images: str):
         raise NotImplementedError(
             f"DEV: There is (intentionally) no generic implementation of is_stackable. Please specify "
             f"implementation for subclasses."
         )
 
@@ -854,18 +886,20 @@
 
     def set_modality(self, modality: None | str):
         from mirp._data_import.utilities import supported_mask_modalities
         if modality is None:
             return
 
         if not isinstance(modality, str):
-            raise ValueError(f"modality is expected to be a character string. Found: {modality}")
+            raise ValueError(
+                f"modality is expected to be a character string. Found: {modality}. [{self.describe_self()}]"
+            )
 
         if modality == "generic_mask":
-            raise ValueError(f"modality cannot be 'generic_mask'")
+            raise ValueError(f"modality cannot be 'generic_mask'. [{self.describe_self()}]")
 
         modality = supported_mask_modalities(modality)
         if self.modality is None or self.modality == "generic_mask":
             self.modality = modality[0]
 
     def create(self):
         # Import locally to avoid potential circular references.
@@ -895,15 +929,17 @@
         elif any(self.file_path.lower().endswith(ii) for ii in file_extensions) and\
                 any(self.file_path.lower().endswith(ii) for ii in supported_file_types("numpy")):
 
             file_class = MaskNumpyFile
             file_type = "numpy"
 
         else:
-            raise NotImplementedError(f"The provided mask type is not implemented: {self.file_type}")
+            raise NotImplementedError(
+                f"The provided mask type is not implemented: {self.file_type}. [{self.describe_self()}]"
+            )
 
         image_file = file_class(
             file_path=self.file_path,
             dir_path=self.dir_path,
             sample_name=self.sample_name,
             file_name=self.file_name,
             image_name=self.image_name,
@@ -917,50 +953,52 @@
             roi_name=self.roi_name
         ).create()
 
         return image_file
 
     def check_mask(self, raise_error=True):
         if self.image_data is None:
-            raise TypeError("DEV: the image_data attribute has not been set.")
+            raise TypeError(f"DEV: the image_data attribute has not been set. [{self.describe_self()}]")
 
         if np.issubdtype(self.image_data.dtype, bool):
 
             if not np.any(self.image_data):
                 if raise_error:
                     warnings.warn(
-                        f"No regions of interest were formed ({self.file_path}. "
+                        f"No regions of interest were formed. "
                         f"The mask object only contains background values (False). "
-                        f"No voxels were found with True values to identify segmentation masks.",
+                        f"No voxels were found with True values to identify segmentation masks. "
+                        f"[{self.describe_self()}]",
                         UserWarning
                     )
             return True
 
         if np.issubdtype(self.image_data.dtype, np.integer):
             if np.any(self.image_data < 0):
                 if raise_error:
                     raise ValueError(
-                        f"Labels in a mask should be 0 or positive integers. Negative values were found in "
-                        f"{self.file_path}. Note that 0 is interpreted as background."
+                        f"Labels in a mask should be 0 or positive integers. Negative values were found. "
+                        f"Note that 0 is interpreted as background. [{self.describe_self()}]"
                     )
                 return False
 
             if len(np.unique(self.image_data)) > 10:
                 if raise_error:
                     warnings.warn(
-                        f"More than 10 labels were found ({self.file_path}). Please check that this is correct.",
+                        f"More than 10 labels were found. Please check that this is correct. "
+                        f"[{self.describe_self()}]",
                         UserWarning
                     )
 
             if np.all(self.image_data == 0):
                 if raise_error:
                     warnings.warn(
-                        f"No regions of interest were formed ({self.file_path}. The mask object only contains "
+                        f"No regions of interest were formed. The mask object only contains "
                         f"background values (0). No voxels were found with positive integers to identify segmentation "
-                        f"masks.",
+                        f"masks. [{self.describe_self()}]",
                         UserWarning
                     )
 
         else:
             raise TypeError(f"DEV: the image_data contains non-integer data ({self.image_data.dtype})")
 
         return True
@@ -981,28 +1019,28 @@
             if isinstance(self.roi_name, str):
                 roi_name = self.roi_name
             elif isinstance(self.roi_name, list):
                 if len(self.roi_name) == 1:
                     roi_name = self.roi_name[0]
                 else:
                     warnings.warn(
-                        f"The name of the region of interest could not be unambiguously determined ("
-                        f"{self.file_path}). One of the following should be used, but it is not clear which: "
-                        f"{self.roi_name}",
+                        f"The name of the region of interest could not be unambiguously determined. "
+                        f"One of the following should be used, but it is not clear which: {self.roi_name}. "
+                        f"[{self.describe_self()}]",
                         UserWarning
                     )
                     roi_name = "region_1"
             elif isinstance(self.roi_name, dict):
                 if len(self.roi_name) == 1:
                     roi_name = list(self.roi_name.values())[0]
                 else:
                     warnings.warn(
-                        f"The name of the region of interest could not be unambiguously determined ("
-                        f"{self.file_path}). One of the following should be used, but it is not clear which: "
-                        f"{self.roi_name}",
+                        f"The name of the region of interest could not be unambiguously determined. "
+                        f"One of the following should be used, but it is not clear which: {self.roi_name}. "
+                        f"[{self.describe_self()}]",
                         UserWarning
                     )
                     roi_name = "region_1"
             else:
                 roi_name = "region_1"
 
             mask_list += [
@@ -1039,17 +1077,18 @@
                         filtered_labels += [current_label]
                 elif isinstance(self.roi_name, dict):
                     if str(current_label) in self.roi_name.keys() or "region_" + str(current_label) in self.roi_name.keys():
                         filtered_labels += [current_label]
 
             if len(filtered_labels) == 0:
                 warnings.warn(
-                    f"No regions of interest were formed ({self.file_path}). "
+                    f"No regions of interest were formed. "
                     f"The available labels ({', '.join([str(x) for x in labels])}) likely did not match "
-                    f"any of the expected labels ({self.roi_name}).",
+                    f"any of the expected labels ({self.roi_name}). "
+                    f"[{self.describe_self()}]",
                     UserWarning
                 )
 
                 return None
 
             for current_label in filtered_labels:
 
@@ -1093,20 +1132,22 @@
         # Identify available labels that are non-background.
         labels = list(set(np.unique(self.image_data)) - {0})
         n_labels = max([1, len(labels)])
 
         if len(labels) == 0:
             labels = [None]
 
-        return {
-            "sample_name": [self.sample_name] * n_labels,
-            "dir_path": [self.dir_path] * n_labels,
-            "file_path": [self.file_name] * n_labels,
-            "roi_label": labels
-        }
+        # Get general attributes.
+        parent_attributes = self._get_export_attributes()
+
+        # Add roi labels as attribute.
+        attributes = [("roi_label", labels)]
+        parent_attributes.update(dict(attributes))
+
+        return parent_attributes
 
 
 class MaskFullImage(MaskFile):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.roi_name = "full_image_mask"
 
@@ -1114,15 +1155,15 @@
             self,
             image: None | ImageFile,
             **kwargs
     ) -> None | list[BaseMask]:
         if image is None:
             raise TypeError(
                 f"Creation of a full image mask requires that the corresponding image is set. "
-                f"No image was provided ({self.file_path})."
+                f"No image was provided. [{self.describe_self()}]"
             )
         else:
             image.complete()
 
         self._complete_modality()
 
         return [BaseMask(
```

### Comparing `mirp-2.2.1/mirp/_data_import/generic_file_stack.py` & `mirp-2.2.2/mirp/_data_import/generic_file_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,17 @@
             file_type = self.image_file_objects[0].file_type
 
         elif all(isinstance(image_file_object, ImageNumpyFile) for image_file_object in self.image_file_objects):
             file_stack_class = ImageNumpyFileStack
             file_type = "numpy"
 
         else:
-            raise TypeError(f"The list of image objects does not consist of a known object type.")
+            raise TypeError(
+                f"The list of image objects does not consist of a known object type. [{self.describe_self()}]"
+            )
 
         image_file_stack = file_stack_class(
             image_file_objects=self.image_file_objects,
             dir_path=self.dir_path,
             sample_name=self.sample_name,
             image_name=self.image_name,
             image_modality=self.modality,
@@ -136,38 +138,40 @@
         :return: nothing, changes are made in-place.
         """
 
         file_name_numeric = [image_object._get_numeric_sequence_from_file() for image_object in self.image_file_objects]
         if any(current_file_name_numeric is None for current_file_name_numeric in file_name_numeric):
             warnings.warn(
                 f"Cannot form stacks from numpy slices based on the file name as numeric values are missing "
-                "from one or more files. The original file order is used.", UserWarning
+                f"from one or more files. The original file order is used. [{self.describe_self()}]", UserWarning
             )
             return
 
         if any(len(current_file_name_numeric) > 1 for current_file_name_numeric in file_name_numeric):
             warnings.warn(
                 f"Cannot form stacks from numpy slices based on the file name as more than one sequence of numeric "
                 f"values are present in the name of one or more files. This excludes the sample name (if known) and "
-                f"any identifiers for image data. The original file order is used.", UserWarning
+                f"any identifiers for image data. The original file order is used. [{self.describe_self()}]",
+                UserWarning
             )
             return
 
         # Flatten array and convert to integer values.
         file_name_numeric = list(itertools.chain.from_iterable(file_name_numeric))
         file_name_numeric = [int(current_file_name_numeric) for current_file_name_numeric in file_name_numeric]
 
         if len(file_name_numeric) == 1:
             return
 
         # Check that all numbers are sequential.
         if not np.all(np.diff(np.sort(np.array(file_name_numeric))) == 1):
             warnings.warn(
                 f"Cannot form stacks from numpy slices based on the file name as numbers are not fully sequential for"
-                f" all files. The original file order is used.", UserWarning
+                f" all files. The original file order is used. [{self.describe_self()}]",
+                UserWarning
             )
             return
 
         position_table = pd.DataFrame({
             "original_object_order": list(range(len(self.image_file_objects))),
             "order_id": file_name_numeric,
         }).sort_values(by=["order_id"])
@@ -237,15 +241,17 @@
             file_type = self.image_file_objects[0].file_type
 
         elif all(isinstance(image_file_object, MaskNumpyFile) for image_file_object in self.image_file_objects):
             file_stack_class = MaskNumpyFileStack
             file_type = "numpy"
 
         else:
-            raise TypeError(f"The list of image objects does not consist of a known object type.")
+            raise TypeError(
+                f"The list of image objects does not consist of a known object type. [{self.describe_self()}]"
+            )
 
         image_file_stack = file_stack_class(
             image_file_objects=self.image_file_objects,
             dir_path=self.dir_path,
             sample_name=self.sample_name,
             image_name=self.image_name,
             image_modality=self.modality,
@@ -259,11 +265,12 @@
         if self.image_data is not None:
             return
 
         image = np.zeros(self.image_dimension, dtype=int)
         for ii, image_file in enumerate(self.image_file_objects):
             if image_file.image_data is None:
                 raise ValueError(
-                    "DEV: the image_data attribute of underlying mask files are not set. Please call load_data first.")
+                    "DEV: the image_data attribute of underlying mask files are not set. Please call load_data first."
+                )
             image[ii, :, :] = image_file.image_data.astype(int)
 
         self.image_data = image
```

### Comparing `mirp-2.2.1/mirp/_data_import/itk_file.py` & `mirp-2.2.2/mirp/_data_import/itk_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,29 +47,30 @@
         :return: boolean value
         """
         if stack_images == "auto":
             return False
         elif stack_images == "yes":
             if self.image_dimension is None:
                 raise ValueError(
-                    "The image_dimension argument is expected to be set. Call load_metadata to set this attribute."
+                    "DEV: The image_dimension argument is expected to be set. Call load_metadata to set this attribute."
                 )
 
             if len(self.image_dimension) < 3:
                 return True
             elif self.image_dimension[0] == 1:
                 return True
             else:
                 return False
 
         elif stack_images == "no":
             return False
         else:
             raise ValueError(
-                f"The stack_images argument is expected to be one of yes, auto, or no. Found: {stack_images}."
+                f"The stack_images argument is expected to be one of yes, auto, or no. Found: {stack_images}. "
+                f"[{self.describe_self()}]"
             )
 
     def _complete_image_origin(self, force=False):
         if self.image_origin is None:
             self.load_metadata()
 
             # Get dimensions, as this determines what can be meaningfully read.
@@ -132,30 +133,34 @@
 
     def load_metadata(self, **kwargs):
         if self.image_metadata is not None:
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
-                f"The image file could not be found at the expected location: {self.file_path}")
+                f"The image file could not be found at the expected location: {self.file_path}. "
+                f"[{self.describe_self()}]"
+            )
 
         # Generate reader.
         reader = itk.ImageIOFactory.CreateImageIO(self.file_path, itk.CommonEnums.IOFileMode_ReadMode)
         reader.SetFileName(self.file_path)
         reader.ReadImageInformation()
 
         self.image_metadata = reader
 
     def load_data(self, **kwargs):
         if self.image_data is not None:
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
-                f"The image file could not be found at the expected location: {self.file_path}")
+                f"The image file could not be found at the expected location: {self.file_path}. "
+                f"[{self.describe_self()}]"
+            )
 
         # Load the image
         itk_img = itk.imread(os.path.join(self.file_path))
         self.image_data = itk.GetArrayFromImage(itk_img).astype(np.float32)
 
 
 class MaskITKFile(ImageITKFile, MaskFile):
@@ -165,12 +170,14 @@
 
     def load_data(self, **kwargs):
         if self.image_data is not None:
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
-                f"The mask file could not be found at the expected location: {self.file_path}")
+                f"The mask file could not be found at the expected location: {self.file_path}. "
+                f"[{self.describe_self()}]"
+            )
 
         # Load the image
         itk_img = itk.imread(os.path.join(self.file_path))
         self.image_data = itk.GetArrayFromImage(itk_img).astype(int)
```

### Comparing `mirp-2.2.1/mirp/_data_import/itk_file_stack.py` & `mirp-2.2.2/mirp/_data_import/itk_file_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,17 @@
             np.power(np.diff(position_table.position_z.values), 2.0))
 
         # Find the smallest slice spacing.
         min_slice_spacing = np.min(image_slice_spacing)
         if min_slice_spacing == 0.0:
             warnings.warn(
                 "Images files contain overlapping origins. Attempting to sort image files by numeric name "
-                "patterns.", UserWarning)
+                f"patterns. [{self.describe_self()}]",
+                UserWarning
+            )
             self.sort_image_objects_by_file()
 
             image_object = copy.deepcopy(self.image_file_objects[0])
             image_object.complete()
 
             if self.image_origin is None:
                 self.image_origin = image_object.image_origin
@@ -99,17 +101,19 @@
 
         # Find how much other slices differ.
         image_slice_spacing_multiplier = image_slice_spacing / min_slice_spacing
 
         if np.any(image_slice_spacing_multiplier > 1.2):
             warnings.warn(
                 f"Inconsistent distance between slice origins of subsequent slices: {np.unique(image_slice_spacing)}. "
-                "Slices cannot be aligned correctly. This is likely due to missing slices. "
-                "MIRP will attempt to interpolate the missing slices and their ROI masks for volumetric analysis.",
-                UserWarning)
+                f"Slices cannot be aligned correctly. This is likely due to missing slices. "
+                f"MIRP will attempt to interpolate the missing slices and their ROI masks for volumetric analysis. "
+                f"[{self.describe_self()}]",
+                UserWarning
+            )
 
             # Update slice positions.
             self.slice_positions = list(np.cumsum(np.insert(np.around(image_slice_spacing, 5), 0, 0.0)))
 
         # Determine image slice spacing.
         image_slice_spacing = np.around(np.mean(image_slice_spacing[image_slice_spacing_multiplier <= 1.2]), 5)
```

### Comparing `mirp-2.2.1/mirp/_data_import/mask_contour.py` & `mirp-2.2.2/mirp/_data_import/mask_contour.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_data_import/numpy_file.py` & `mirp-2.2.2/mirp/_data_import/numpy_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,53 +45,59 @@
         :param stack_images: One of auto, yes or no. By default (auto), images are stackable if an image object
         represents a single slice.
         :return: boolean value.
         """
         if stack_images in ["auto", "yes"]:
             if self.image_dimension is None:
                 raise ValueError(
-                    "The image_dimension argument is expected to be set. Call load_metadata to set this attribute."
+                    f"The image_dimension argument is expected to be set. Call load_metadata to set this attribute. "
+                    f"[{self.describe_self()}]"
                 )
 
             if len(self.image_dimension) < 3:
                 return True
             elif self.image_dimension[0] == 1:
                 return True
             else:
                 return False
 
         elif stack_images == "no":
             return False
         else:
             raise ValueError(
-                f"The stack_images argument is expected to be one of yes, auto, or no. Found: {stack_images}."
+                f"The stack_images argument is expected to be one of yes, auto, or no. Found: {stack_images}. "
+                f"[{self.describe_self()}]"
             )
 
     def check(self, raise_error=False, remove_metadata=True) -> bool:
 
         # Perform general checks.
         if not super().check(raise_error=raise_error):
             return False
 
         # Read Numpy file.
         image_data = np.load(file=self.file_path, mmap_mode="r")
 
         # Check that the contents are in fact a ndarray.
         if not isinstance(image_data, np.ndarray):
             if raise_error:
-                raise TypeError(f"The current numpy dataset {self.file_path} does not have the expected content. "
-                                f"Found: {type(image_data)}. Expected: numpy.ndarray")
+                raise TypeError(
+                    f"The current numpy dataset {self.file_path} does not have the expected content. "
+                    f"Found: {type(image_data)}. Expected: numpy.ndarray. [{self.describe_self()}]"
+                )
 
             return False
 
         # Check dimensions.
         if not 0 < image_data.ndim <= 3:
             if raise_error:
-                raise ValueError(f"The current numpy dataset has as an unexpected number of dimensions: "
-                                 f"Found: {image_data.ndim}. Expected: 1, 2, or 3 dimensions")
+                raise ValueError(
+                    f"The current numpy dataset has as an unexpected number of dimensions: "
+                    f"Found: {image_data.ndim}. Expected: 1, 2, or 3 dimensions. [{self.describe_self()}]"
+                )
 
             return False
 
         return True
 
     def _complete_image_origin(self, force=False):
         if self.image_origin is None:
@@ -121,27 +127,31 @@
 
     def load_metadata(self, **kwargs):
         if self.image_metadata is not None:
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
-                f"The image file could not be found at the expected location: {self.file_path}")
+                f"The image file could not be found at the expected location: {self.file_path}. "
+                f"[{self.describe_self()}]"
+            )
 
         # `Lazy load the data
         self.image_metadata = np.load(file=self.file_path, mmap_mode="r")
 
     def load_data(self, **kwargs):
         if self.image_data is not None:
             self.update_image_data()
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
-                f"The image file could not be found at the expected location: {self.file_path}")
+                f"The image file could not be found at the expected location: {self.file_path}. "
+                f"[{self.describe_self()}]"
+            )
 
         self.image_data = np.load(self.file_path).astype(np.float32)
         self.update_image_data()
 
 
 class MaskNumpyFile(ImageNumpyFile, MaskFile):
     def __init__(self, **kwargs):
@@ -150,11 +160,12 @@
     def load_data(self, **kwargs):
         if self.image_data is not None:
             self.update_image_data()
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
-                f"The mask file could not be found at the expected location: {self.file_path}")
+                f"The mask file could not be found at the expected location: {self.file_path}. [{self.describe_self()}]"
+            )
 
         self.image_data = np.load(self.file_path).astype(int)
         self.update_image_data()
```

### Comparing `mirp-2.2.1/mirp/_data_import/numpy_file_stack.py` & `mirp-2.2.2/mirp/_data_import/numpy_file_stack.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_data_import/read_data.py` & `mirp-2.2.2/mirp/_data_import/read_data.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_data_import/suv.py` & `mirp-2.2.2/mirp/_data_import/suv.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_data_import/utilities.py` & `mirp-2.2.2/mirp/_data_import/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/cm.py` & `mirp-2.2.2/mirp/_featuresets/cm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/dzm.py` & `mirp-2.2.2/mirp/_featuresets/dzm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/intensity_histogram.py` & `mirp-2.2.2/mirp/_featuresets/intensity_histogram.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/intensity_volume_histogram.py` & `mirp-2.2.2/mirp/_featuresets/intensity_volume_histogram.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/local_intensity.py` & `mirp-2.2.2/mirp/_featuresets/local_intensity.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/morphology_3d.py` & `mirp-2.2.2/mirp/_featuresets/morphology_3d.py`

 * *Files 5% similar despite different names*

```diff
@@ -566,15 +566,14 @@
 
     import copy
     import numpy.linalg as npla
 
     # Cast to np.matrix
     mat_p = copy.deepcopy(pos_mat)
     mat_p = np.transpose(mat_p)
-    mat_p = np.asmatrix(mat_p)
 
     # Dimension of the point set
     ndim = np.shape(mat_p)[0]
 
     # Number of points in the point set
     npoint = np.shape(mat_p)[1]
 
@@ -589,19 +588,19 @@
     vec_u = 1.0 * np.ones(shape=npoint) / npoint
 
     # Khachiyan algorithm
     while err > tolerance:
         # Matrix multiplication:
         # np.diag(u) : if u is a vector, places the elements of u
         # in the diagonal of an NxN matrix of zeros
-        mat_x = mat_q * np.diag(vec_u) * np.transpose(mat_q)
+        mat_x = np.matmul(mat_q, np.matmul(np.diag(vec_u), np.transpose(mat_q)))
 
         # npla.inv(mat_x) returns the matrix inverse of mat_x
         # np.diag(mat_M) when mat_M is a matrix returns the diagonal vector of mat_M
-        vec_m = np.diag(np.transpose(mat_q) * npla.inv(mat_x) * mat_q)
+        vec_m = np.diag(np.matmul(np.transpose(mat_q), np.matmul(npla.inv(mat_x), mat_q)))
 
         # Find the value and location of the maximum element in the vector M
         max_m = np.max(vec_m)
         ind_j = np.argmax(vec_m)
 
         # Calculate the step size for the ascent
         step_size = (max_m - ndim - 1.0) / ((ndim + 1.0) * (max_m - 1.0))
@@ -620,22 +619,21 @@
 
         # Increment iter_count and replace vec_u
         iter_count += 1
         vec_u = vec_new_u
 
     # Put the elements of the vector u into the diagonal of a matrix
     # U with the rest of the elements as 0
-    mat_u = np.asmatrix(np.diag(vec_u))
+    mat_u = np.diag(vec_u)
 
     # Compute the A-matrix
-    vec_u = np.transpose(np.asmatrix(vec_u))
-    mat_a = (1.0 / ndim) * npla.inv(mat_p * mat_u * np.transpose(mat_p) - (mat_p * vec_u) * np.transpose(mat_p * vec_u))
-
-    # Compute the center - This is not required as output.
-    # mat_c = mat_p * vec_u
+    mat_a = (1.0 / ndim) * npla.inv(
+        np.matmul(mat_p, np.matmul(mat_u, np.transpose(mat_p)))
+        - np.matmul(np.matmul(mat_p, vec_u), np.transpose(np.matmul(mat_p, vec_u)))
+    )
 
     # Perform singular value decomposition
     s = npla.svd(mat_a, compute_uv=False)
 
     # The semi-axis lengths are the inverse square root of the singular values
     semi_axes_length = np.sort(1.0/np.sqrt(s))
```

### Comparing `mirp-2.2.1/mirp/_featuresets/ngldm.py` & `mirp-2.2.2/mirp/_featuresets/ngldm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/ngtdm.py` & `mirp-2.2.2/mirp/_featuresets/ngtdm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/rlm.py` & `mirp-2.2.2/mirp/_featuresets/rlm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/statistics.py` & `mirp-2.2.2/mirp/_featuresets/statistics.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/szm.py` & `mirp-2.2.2/mirp/_featuresets/szm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_featuresets/utilities.py` & `mirp-2.2.2/mirp/_featuresets/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_image_processing/alter_mask.py` & `mirp-2.2.2/mirp/_image_processing/alter_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_image_processing/anti_aliasing.py` & `mirp-2.2.2/mirp/_image_processing/anti_aliasing.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_image_processing/cropping.py` & `mirp-2.2.2/mirp/_image_processing/cropping.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_image_processing/discretise_image.py` & `mirp-2.2.2/mirp/_image_processing/discretise_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_image_processing/randomise_mask.py` & `mirp-2.2.2/mirp/_image_processing/randomise_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_image_processing/split_mask.py` & `mirp-2.2.2/mirp/_image_processing/split_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_image_processing/tissue_mask.py` & `mirp-2.2.2/mirp/_image_processing/tissue_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_image_processing/utilities.py` & `mirp-2.2.2/mirp/_image_processing/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/exponential_transform.py` & `mirp-2.2.2/mirp/_imagefilters/exponential_transform.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/gabor.py` & `mirp-2.2.2/mirp/_imagefilters/gabor.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/gaussian.py` & `mirp-2.2.2/mirp/_imagefilters/gaussian.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/generic.py` & `mirp-2.2.2/mirp/_imagefilters/generic.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/laplacian_of_gaussian.py` & `mirp-2.2.2/mirp/_imagefilters/laplacian_of_gaussian.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/laws.py` & `mirp-2.2.2/mirp/_imagefilters/laws.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/log_transform.py` & `mirp-2.2.2/mirp/_imagefilters/log_transform.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/mean.py` & `mirp-2.2.2/mirp/_imagefilters/mean.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/nonseparable_wavelet.py` & `mirp-2.2.2/mirp/_imagefilters/nonseparable_wavelet.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/separable_wavelet.py` & `mirp-2.2.2/mirp/_imagefilters/separable_wavelet.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/square_root_transform.py` & `mirp-2.2.2/mirp/_imagefilters/square_root_transform.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/square_transform.py` & `mirp-2.2.2/mirp/_imagefilters/square_transform.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_imagefilters/utilities.py` & `mirp-2.2.2/mirp/_imagefilters/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_images/base_image.py` & `mirp-2.2.2/mirp/_images/base_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_images/ct_image.py` & `mirp-2.2.2/mirp/_images/ct_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_images/generic_image.py` & `mirp-2.2.2/mirp/_images/generic_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_images/mask_image.py` & `mirp-2.2.2/mirp/_images/mask_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_images/mr_image.py` & `mirp-2.2.2/mirp/_images/mr_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_images/pet_image.py` & `mirp-2.2.2/mirp/_images/pet_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_images/rtdose_image.py` & `mirp-2.2.2/mirp/_images/rtdose_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_images/transformed_image.py` & `mirp-2.2.2/mirp/_images/transformed_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_images/utilities.py` & `mirp-2.2.2/mirp/_images/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.colors import LinearSegmentedColormap
 
 from mirp._images.generic_image import GenericImage
 from mirp._images.mask_image import MaskImage
 from mirp._masks.base_mask import BaseMask
@@ -36,16 +38,27 @@
         self.image_data = image.get_voxel_grid()
 
         self.mask_data = None
         if show_mask:
             self.mask_data = mask.get_voxel_grid()
 
         self.n_slices, _, _ = image.image_dimension
-        if slice_id is None or slice_id < 1 or slice_id > self.n_slices:
+        if slice_id is None:
             self.slice_index = int(np.floor(self.n_slices / 2.0))
+        elif not isinstance(slice_id, int):
+            raise TypeError(f"slice_id should be an integer (int). Found: {type(slice_id)}")
+        elif slice_id < 1:
+            self.slice_index = 0
+            warnings.warn(f"slice_id cannot be smaller than 1. Found: {slice_id}", UserWarning)
+        elif slice_id > self.n_slices:
+            self.slice_index = self.n_slices - 1
+            warnings.warn(
+                f"slice_id cannot be greater than the number of slices ({self.n_slices}). Found: {slice_id}",
+                UserWarning
+            )
         else:
             self.slice_index = slice_id - 1
 
         # Set plotting options
         colour_map = image.get_colour_map()
         min_intensity = image.get_default_lowest_intensity() if image.get_default_lowest_intensity() is not None else (
             np.min(self.image_data))
```

### Comparing `mirp-2.2.1/mirp/_masks/base_mask.py` & `mirp-2.2.2/mirp/_masks/base_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/_workflows/standardWorkflow.py` & `mirp-2.2.2/mirp/_workflows/standardWorkflow.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/config_data.xml` & `mirp-2.2.2/mirp/config_data.xml`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/config_settings.xml` & `mirp-2.2.2/mirp/config_settings.xml`

 * *Files 3% similar despite different names*

#### Comparing `mirp-2.2.1/mirp/config_settings.xml` & `mirp-2.2.2/mirp/config_settings.xml`

```diff
@@ -19,37 +19,37 @@
       <mask_select_largest_region/>
       <!-- Defines whether the largest slice within a mask object should be selected. Default: False -->
       <mask_select_largest_slice/>
       <!-- Defines whether any approximation can be made to speed up image processing and feature processing.
             Default: True -->
       <no_approximation/>
     </general>
-    <img_interpolate>
+    <image_interpolation>
       <!-- Voxel spacing after interpolation. Units are defined by the headers of the image files. Every
             value represents the spacing that will be applied in all directions. Non-uniform voxel spacing may also
             be provided, but requires 3 values for z, y, and x directions (if by_slice = False) or 2 values for y and
             x directions (otherwise). -->
       <new_spacing/>
       <!-- Sets the order of the interpolation spline. It can be 0 (nearest neighbour), 1 (linear), 2, 3
             (cubic), 4, 5 -->
       <spline_order/>
       <!-- Anti-aliasing filter to reduce aliasing artefacts when down-sampling. Enabled by default (True). -->
       <anti_aliasing/>
       <!-- Smoothing parameter beta for antialiasing filter. Must be in range (0.0, 1.0]. At 1.0 no
             antialiasing is performed. Default is 0.98. -->
       <smoothing_beta/>
-    </img_interpolate>
-    <roi_interpolate>
+    </image_interpolation>
+    <mask_interpolation>
       <!-- Sets the order of the interpolation spline. It can be 0 (nearest neighbour), 1 (linear), 2 (cubic),
             3, 4, 5. Nearest neighbour or linear interpolation (default) are recommended. -->
       <spline_order/>
       <!-- Threshold for ROIS with partial volumes after interpolation. Default: 0.5 -->
       <incl_threshold/>
-    </roi_interpolate>
-    <post_processing>
+    </mask_interpolation>
+    <image_processing>
       <!-- Type of algorithm used to produce an approximate mask of the tissue. Can be none, range (requires
             intensity values), relative_range (default; requires fractions). -->
       <tissue_mask_type/>
       <!-- Range values for creating an approximate mask of the tissue. Required for range and relative range
             options. Default: 0.02, 1.0 (relative_range); 0.0, nan (range; effectively none) -->
       <tissue_mask_range/>
       <!-- Whether N4 bias field correction should be performed. Disabled by default (False); only applicable
@@ -60,15 +60,15 @@
       <!-- Max number of iterations for each of the fitting levels for N4 bias field correction, e.g. 100, 100
             if two fitting levels are used. Default: 50 -->
       <n_max_iterations/>
       <!-- Convergence threshold for N4 bias field correction. Default: 0.001 -->
       <convergence_threshold/>
       <!-- Intensities in PET imaging are often stored as detected radiotracer activity. To make detected activity more
             comparable between patients, these are converted to standardised uptake values. The following are possible:
-            body_weight, none. -->
+            body_weight, body_surface_area, lean_body_mass, lean_body_mass_bmi, ideal_body_weight, none -->
       <pet_suv_conversion/>
       <!-- Algorithm used to normalise intensities in the image. Will use only intensities in voxels masked by
             the  tissue mask. Can be none (default), range (maps to an intensity range), relative_range (maps to a
             range  of relative intensities), quantile_range (maps to a range of relative intensities based on
             intensity percentiles), standardisation (performs z-normalisation). -->
       <intensity_normalisation/>
       <!-- Intensity range for range, relative_range and quantile_range normalisation. -->
@@ -77,16 +77,16 @@
              You may define two values for lower and upper boundary respectively. Default: [np.nan, np.nan] (no
              saturation). -->
       <intensity_normalisation_saturation/>
       <!-- Defines scaling parameter to linearly scale intensities with. The scaling parameter is applied after
             normalisation (if any). For example, intensity_scaling = 1000.0, combined with intensity_normalisation =
             "range" results in intensities being mapped to a [0.0, 1000.0] range instead of [0.0, 1.0]. -->
       <intensity_scaling/>
-    </post_processing>
-    <vol_adapt>
+    </image_processing>
+    <image_perturbation>
       <!-- Whether the image may be cut to only maintain the interesting parts. Default: False. Setting this to
              True speeds up calculations and saves memory. -->
       <crop_around_roi/>
       <!-- Distance (in mm) around the ROI mask that should be maintained when cropping. Default: 150 mm. -->
       <crop_distance/>
       <!-- Number of times noise is randomly added to the image. Used in noise addition image perturbations.
             Default: 0 -->
@@ -115,24 +115,24 @@
       <!-- Width of the rim used for splitting the mask into bulk and rim masks, in physical dimensions. Multiple values
             can be provided to generate rims of different widths. -->
       <roi_boundary_size/>
       <!-- Determines the minimum volume of the bulk mask when splitting the original mask into bulk and rim sections.
             Fraction of the original volume, e.g. 0.6 means that the bulk contains at least 60% of the original mask.
              -->
       <roi_split_max_erosion/>
-    </vol_adapt>
-    <roi_resegment>
+    </image_perturbation>
+    <mask_resegmentation>
       <!-- Intensity threshold for threshold-based re-segmentation (threshold and range). If set, requires two
              values for lower and upper range respectively. The upper range value can also be nan for half-open
              ranges. -->
       <intensity_range/>
       <!-- Number of standard deviations for outlier-based intensity re-segmentation. 3 is a common setting. -->
       <sigma/>
-    </roi_resegment>
-    <feature_extr>
+    </mask_resegmentation>
+    <feature_computation>
       <!-- Set of feature families to be computed from the image. Default is all. -->
       <feature_families/>
       <!-- Discretisation algorithm. Can be none, fixed_bin_number and/or fixed_bin_size. Combinations are
             possible. No default. -->
       <discretisation_method/>
       <!-- Bin width (in intensity units) for the fixed_bin_size algorithm. Multiple values are possible. -->
       <discretisation_bin_width/>
@@ -163,16 +163,16 @@
       <ngtdm_spatial_method/>
       <!-- Distance (in voxels) for NGLDM for determining the neighbourhood. -->
       <ngldm_distance/>
       <!-- Difference level (alpha) for NGLDM -->
       <ngldm_difference_level/>
       <!-- Calculate NGLDM in 2d, 2.5d or 3d. Default: same as general/by_slice. -->
       <ngldm_spatial_method/>
-    </feature_extr>
-    <img_transform>
+    </feature_computation>
+    <image_transformation>
       <!-- Filter kernels to apply. Options: gabor, laplacian_of_gaussian, laws, mean, separable_wavelet,
             nonseparable_wavelet. See documentation for additional filter kernels. -->
       <filter_kernels/>
       <!-- Boundary conditions, i.e. how to calculate the filter response for voxels that are less than the
             filter width removed from the volume edge. This is the general setting. -->
       <boundary_condition/>
       <!-- Family of features to computed from response maps. Default: statistical. -->
@@ -269,10 +269,10 @@
       <!-- Boundary condition for mean filter kernels. Supersedes generic boundary condition tag. -->
       <mean_filter_boundary_condition/>
       <!-- Riesz-transformation order. If required, should be a 2 (2D filter), or 3-element (3D filter) integer
              vector, e.g. 0,0,1. Note: order is (z, y, x).-->
       <riesz_filter_order/>
       <!--Sigma for Gaussian filter used in steerable Riesz transformation. -->
       <riesz_filter_tensor_sigma/>
-    </img_transform>
+    </image_transformation>
   </config>
 </root>
```

### Comparing `mirp-2.2.1/mirp/data_import/import_image.py` & `mirp-2.2.2/mirp/data_import/import_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/data_import/import_image_and_mask.py` & `mirp-2.2.2/mirp/data_import/import_image_and_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/data_import/import_mask.py` & `mirp-2.2.2/mirp/data_import/import_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/deep_learning_preprocessing.py` & `mirp-2.2.2/mirp/deep_learning_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,28 +57,28 @@
     num_cpus: int, optional, default: None
         Number of CPU nodes that should be used for parallel processing. Image and mask processing can be
         parallelized using the ``ray`` package. If a ray cluster is defined by the user, this cluster will be used
         instead. By default, image and mask processing are processed sequentially.
 
     **kwargs:
         Keyword arguments passed for importing images and masks (
-        :func:`~mirp._data_import.import_image_and_mask.import_image_and_mask`) and configuring settings (notably
+        :func:`~mirp.data_import.import_image_and_mask.import_image_and_mask`) and configuring settings (notably
         :class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`,
         :class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`), among others.
 
     Returns
     -------
     None | list[Any]
         List of images and masks in the format indicated by ``image_export_format``, if ``export_images=True``.
 
     See Also
     --------
     Keyword arguments can be provided to configure the following:
 
-    * image and mask import (:func:`~mirp._data_import.import_image_and_mask.import_image_and_mask`)
+    * image and mask import (:func:`~mirp.data_import.import_image_and_mask.import_image_and_mask`)
     * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
     * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
     * image interpolation / resampling (:class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
       :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
     * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
 
     """
@@ -194,28 +194,28 @@
 
     write_dir: str, optional
         Path to directory where processed images and masks should be written. If not set, processed images and masks
         are returned by this function. Required if ``write_images=True``.
 
     **kwargs:
         Keyword arguments passed for importing images and masks (
-        :func:`~mirp._data_import.import_image_and_mask.import_image_and_mask`) and configuring settings (notably
+        :func:`~mirp.data_import.import_image_and_mask.import_image_and_mask`) and configuring settings (notably
         :class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`,
         :class:`~mirp.settings.settingsPerturbation.ImagePerturbationSettingsClass`), among others.
 
     Yields
     -------
     None | list[Any]
         List of images and masks in the format indicated by ``image_export_format``, if ``export_images=True``.
 
     See Also
     --------
     Keyword arguments can be provided to configure the following:
 
-    * image and mask import (:func:`~mirp._data_import.import_image_and_mask.import_image_and_mask`)
+    * image and mask import (:func:`~mirp.data_import.import_image_and_mask.import_image_and_mask`)
     * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
     * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
     * image interpolation / resampling (:class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
       :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
     * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
 
     """
```

### Comparing `mirp-2.2.1/mirp/deprecated.py` & `mirp-2.2.2/mirp/deprecated.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/extract_features_and_images.py` & `mirp-2.2.2/mirp/extract_features_and_images.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from mirp._workflows.standardWorkflow import StandardWorkflow
 
 
 def extract_features(
         write_features: None | bool = None,
         export_features: None | bool = None,
         write_dir: None | str = None,
+        num_cpus: None | int = None,
         **kwargs
 ) -> None | list[Any]:
     """
     Compute features from regions of interest in images. This function is a wrapper around
     :func:`~mirp.extractFeaturesAndImages.extract_features_and_images`.
 
     Parameters
@@ -26,16 +27,33 @@
     export_features: bool, optional
         Determines whether features computed from images should be returned by the function.
 
     write_dir: str, optional
         Path to directory where feature tables should be written. If not set, feature tables are returned by this
         function. Required if ``write_features=True``.
 
+    num_cpus: int, optional, default: None
+        Number of CPU nodes that should be used for parallel processing. Image processing and feature computation can be
+        parallelized using the ``ray`` package. If a ray cluster is defined by the user, this cluster will be used
+        instead. By default, images are processed sequentially.
+
     **kwargs:
-        Keyword arguments passed to :func:`~mirp.extractFeaturesAndImages.extract_features_and_images`.
+        Keyword arguments passed for importing images and masks (
+        :func:`mirp.data_import.import_image_and_mask.import_image_and_mask`) and configuring settings:
+
+        * general settings (:class:`~mirp.settings.general_parameters.GeneralSettingsClass`)
+        * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
+        * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
+        * image interpolation / resampling (
+          :class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
+          :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
+        * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
+        * image transformation (:class:`~mirp.settings.transformation_parameters.ImageTransformationSettingsClass`)
+        * feature computation / extraction (
+          :class:`~mirp.settings.feature_parameters.FeatureExtractionSettingsClass`)
 
     Returns
     -------
     None | list[Any]
         List of feature tables, if ``export_features=True``.
 
     See Also
@@ -45,14 +63,15 @@
     """
     return extract_features_and_images(
         write_features=write_features,
         export_features=export_features,
         write_images=False,
         export_images=False,
         write_dir=write_dir,
+        num_cpus=num_cpus,
         **kwargs
     )
 
 
 def extract_features_generator(
         write_features: bool = False,
         export_features: bool = True,
@@ -68,15 +87,27 @@
         Determines whether features computed from images should be written to the directory indicated by the
         ``write_dir`` keyword argument.
 
     export_features: bool, default: True
         Determines whether features computed from images should be returned by the function.
 
     **kwargs:
-        Keyword arguments passed to :func:`~mirp.extractFeaturesAndImages.extract_features_and_images_generator`.
+        Keyword arguments passed for importing images and masks (
+        :func:`mirp.data_import.import_image_and_mask.import_image_and_mask`) and configuring settings:
+
+        * general settings (:class:`~mirp.settings.general_parameters.GeneralSettingsClass`)
+        * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
+        * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
+        * image interpolation / resampling (
+          :class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
+          :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
+        * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
+        * image transformation (:class:`~mirp.settings.transformation_parameters.ImageTransformationSettingsClass`)
+        * feature computation / extraction (
+          :class:`~mirp.settings.feature_parameters.FeatureExtractionSettingsClass`)
 
     Returns
     -------
     None | list[Any]
         List of feature tables, if ``export_features=True``.
 
     See Also
@@ -93,14 +124,16 @@
     )
 
 
 def extract_images(
         write_images: None | bool = None,
         export_images: None | bool = None,
         write_dir: None | str = None,
+        image_export_format: str = "dict",
+        num_cpus: None | int = None,
         **kwargs
 ):
     """
     Process images and masks. This function is a wrapper around
     :func:`~mirp.extractFeaturesAndImages.extract_features_and_images`.
 
     Parameters
@@ -112,16 +145,36 @@
     export_images: bool, optional
         Determines whether processed images and masks should be returned by the function.
 
     write_dir: str, optional
         Path to directory where processed images and masks should be written. If not set, processed images and masks
         are returned by this function. Required if ``write_images=True``.
 
+    image_export_format: {"dict", "native", "numpy"}, default: "dict"
+        Return format for processed images and masks. ``"dict"`` returns dictionaries of images and masks as numpy
+        arrays and associated characteristics. ``"native"`` returns images and masks in their internal format.
+        ``"numpy"`` returns images and masks in numpy format. This argument is only used if ``export_images=True``.
+
+    num_cpus: int, optional, default: None
+        Number of CPU nodes that should be used for parallel processing. Image processing and feature computation can be
+        parallelized using the ``ray`` package. If a ray cluster is defined by the user, this cluster will be used
+        instead. By default, images are processed sequentially.
+
     **kwargs:
-        Keyword arguments passed to :func:`~mirp.extractFeaturesAndImages.extract_features_and_images`.
+        Keyword arguments passed for importing images and masks (
+        :func:`mirp.data_import.import_image_and_mask.import_image_and_mask`) and configuring settings:
+
+        * general settings (:class:`~mirp.settings.general_parameters.GeneralSettingsClass`)
+        * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
+        * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
+        * image interpolation / resampling (
+          :class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
+          :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
+        * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
+        * image transformation (:class:`~mirp.settings.transformation_parameters.ImageTransformationSettingsClass`)
 
     Returns
     -------
     None | list[Any]
         List of feature tables, if ``export_images=True``.
 
     See Also
@@ -131,21 +184,25 @@
     """
     return extract_features_and_images(
         write_features=False,
         export_features=False,
         write_images=write_images,
         export_images=export_images,
         write_dir=write_dir,
+        image_export_format=image_export_format,
+        num_cpus=num_cpus,
         **kwargs
     )
 
 
 def extract_images_generator(
         write_images: bool = False,
         export_images: bool = True,
+        write_dir: None | str = None,
+        image_export_format: str = "dict",
         **kwargs
 ):
     """
     Process images and masks. This generator is a wrapper around
     :func:`~mirp.extractFeaturesAndImages.extract_features_and_images_generator`.
 
     Parameters
@@ -153,16 +210,35 @@
     write_images: bool, default: True
        Determines whether processed images and masks should be written to the directory indicated by the
        ``write_dir`` keyword argument.
 
     export_images: bool, default: False
        Determines whether processed images and masks should be returned by the function.
 
+    write_dir: str, optional
+        Path to directory where processed images and masks should be written. If not set, processed images and masks
+        are returned by this function. Required if ``write_images=True``.
+
+    image_export_format: {"dict", "native", "numpy"}, default: "dict"
+        Return format for processed images and masks. ``"dict"`` returns dictionaries of images and masks as numpy
+        arrays and associated characteristics. ``"native"`` returns images and masks in their internal format.
+        ``"numpy"`` returns images and masks in numpy format. This argument is only used if ``export_images=True``.
+
     **kwargs:
-       Keyword arguments passed to :func:`~mirp.extractFeaturesAndImages.extract_features_and_images_generator`.
+        Keyword arguments passed for importing images and masks (
+        :func:`mirp.data_import.import_image_and_mask.import_image_and_mask`) and configuring settings:
+
+        * general settings (:class:`~mirp.settings.general_parameters.GeneralSettingsClass`)
+        * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
+        * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
+        * image interpolation / resampling (
+          :class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
+          :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
+        * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
+        * image transformation (:class:`~mirp.settings.transformation_parameters.ImageTransformationSettingsClass`)
 
     Yields
     ------
     None | list[Any]
        List of feature tables, if ``export_images=True``.
 
     See Also
@@ -171,41 +247,66 @@
 
     """
     yield from extract_features_and_images_generator(
         write_features=False,
         export_features=False,
         write_images=write_images,
         export_images=export_images,
+        write_dir=write_dir,
+        image_export_format=image_export_format,
         **kwargs
     )
 
 
 def extract_features_and_images(
+        write_features: None | bool = None,
+        export_features: None | bool = None,
+        write_images: None | bool = None,
+        export_images: None | bool = None,
+        write_dir: None | str = None,
         image_export_format: str = "dict",
         num_cpus: None | int = None,
         **kwargs
 ):
     """
     Processes images and computes features from regions of interest.
 
     Parameters
     ----------
+    write_features: bool, optional
+        Determines whether features computed from images should be written to the directory indicated by the
+        ``write_dir`` keyword argument.
+
+    export_features: bool, optional
+        Determines whether features computed from images should be returned by the function.
+
+    write_images: bool, optional
+        Determines whether processed images and masks should be written to the directory indicated by the
+        ``write_dir`` keyword argument.
+
+    export_images: bool, optional
+        Determines whether processed images and masks should be returned by the function.
+
+    write_dir: str, optional
+        Path to directory where features, processed images and masks should be written. If not set, features, processed images and masks
+        are returned by this function. Required if ``write_features=True`` or ``write_images=True``.
+
     image_export_format: {"dict", "native", "numpy"}, default: "dict"
         Return format for processed images and masks. ``"dict"`` returns dictionaries of images and masks as numpy
         arrays and associated characteristics. ``"native"`` returns images and masks in their internal format.
         ``"numpy"`` returns images and masks in numpy format. This argument is only used if ``export_images=True``.
 
     num_cpus: int, optional, default: None
         Number of CPU nodes that should be used for parallel processing. Image processing and feature computation can be
         parallelized using the ``ray`` package. If a ray cluster is defined by the user, this cluster will be used
         instead. By default, images are processed sequentially.
 
     **kwargs:
         Keyword arguments passed for importing images and masks (
-        :func:`mirp._data_import.import_image_and_mask.import_image_and_mask`) and configuring settings:
+        :func:`mirp.data_import.import_image_and_mask.import_image_and_mask`) and configuring settings:
 
         * general settings (:class:`~mirp.settings.general_parameters.GeneralSettingsClass`)
         * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
         * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
         * image interpolation / resampling (
           :class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
           :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
@@ -219,15 +320,15 @@
     None | list[Any]
         List of features, images and masks, depending on ``export_features`` and ``export_images``.
 
     See Also
     --------
     Keyword arguments can be provided to configure the following:
 
-    * image and mask import (:func:`~mirp._data_import.import_image_and_mask.import_image_and_mask`)
+    * image and mask import (:func:`~mirp.data_import.import_image_and_mask.import_image_and_mask`)
     * general settings (:class:`~mirp.settings.general_parameters.GeneralSettingsClass`)
     * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
     * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
     * image interpolation / resampling (:class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
       :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
     * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
     * image transformation (:class:`~mirp.settings.transformation_parameters.ImageTransformationSettingsClass`)
@@ -240,46 +341,84 @@
     if not external_ray and num_cpus is not None and num_cpus > 1:
         ray_init(num_cpus=num_cpus)
 
     if ray_is_initialized():
         # Parallel processing.
         results = [
             _ray_extractor.remote(workflow=workflow, image_export_format=image_export_format)
-            for workflow in _base_extract_features_and_images(**kwargs)
+            for workflow in _base_extract_features_and_images(
+                write_features=write_features,
+                export_features=export_features,
+                write_images=write_images,
+                export_images=export_images,
+                write_dir=write_dir,
+                **kwargs
+            )
         ]
 
         results = ray_get(results)
         if not external_ray:
             ray_shutdown()
 
     else:
         # Sequential processing.
-        workflows = list(_base_extract_features_and_images(**kwargs))
+        workflows = list(_base_extract_features_and_images(
+            write_features=write_features,
+            export_features=export_features,
+            write_images=write_images,
+            export_images=export_images,
+            write_dir=write_dir,
+            **kwargs
+        ))
+
         results = [workflow.standard_extraction(image_export_format=image_export_format) for workflow in workflows]
 
     return results
 
 
 def extract_features_and_images_generator(
+        write_features: None | bool = None,
+        export_features: None | bool = None,
+        write_images: None | bool = None,
+        export_images: None | bool = None,
+        write_dir: None | str = None,
         image_export_format: str = "dict",
         **kwargs
 ):
     """
     Processes images and computes features from regions of interest as a generator.
 
     Parameters
     ----------
-    image_export_format: {"dict", "native", "numpy"}, default: "numpy"
+    write_features: bool, optional
+        Determines whether features computed from images should be written to the directory indicated by the
+        ``write_dir`` keyword argument.
+
+    export_features: bool, optional
+        Determines whether features computed from images should be returned by the function.
+
+    write_images: bool, optional
+        Determines whether processed images and masks should be written to the directory indicated by the
+        ``write_dir`` keyword argument.
+
+    export_images: bool, optional
+        Determines whether processed images and masks should be returned by the function.
+
+    write_dir: str, optional
+        Path to directory where features, processed images and masks should be written. If not set, features, processed images and masks
+        are returned by this function. Required if ``write_features=True`` or ``write_images=True``.
+
+    image_export_format: {"dict", "native", "numpy"}, default: "dict"
         Return format for processed images and masks. ``"dict"`` returns dictionaries of images and masks as numpy
         arrays and associated characteristics. ``"native"`` returns images and masks in their internal format.
         ``"numpy"`` returns images and masks in numpy format. This argument is only used if ``export_images=True``.
 
     **kwargs:
         Keyword arguments passed for importing images and masks (
-        :func:`mirp._data_import.import_image_and_mask.import_image_and_mask`) and configuring settings:
+        :func:`mirp.data_import.import_image_and_mask.import_image_and_mask`) and configuring settings:
 
         * general settings (:class:`~mirp.settings.general_parameters.GeneralSettingsClass`)
         * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
         * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
         * image interpolation / resampling (
           :class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
           :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
@@ -293,27 +432,34 @@
     None | list[Any]
         List of features, images and masks, depending on ``export_features`` and ``export_images``.
 
     See Also
     --------
     Keyword arguments can be provided to configure the following:
 
-    * image and mask import (:func:`~mirp._data_import.import_image_and_mask.import_image_and_mask`)
+    * image and mask import (:func:`~mirp.data_import.import_image_and_mask.import_image_and_mask`)
     * general settings (:class:`~mirp.settings.general_parameters.GeneralSettingsClass`)
     * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
     * image perturbation / augmentation (:class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass`)
     * image interpolation / resampling (:class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass`
       and :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
     * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
     * image transformation (:class:`~mirp.settings.transformation_parameters.ImageTransformationSettingsClass`)
     * feature computation / extraction (:class:`~mirp.settings.feature_parameters.FeatureExtractionSettingsClass`)
 
     """
 
-    workflows = list(_base_extract_features_and_images(**kwargs))
+    workflows = list(_base_extract_features_and_images(
+        write_features=write_features,
+        export_features=export_features,
+        write_images=write_images,
+        export_images=export_images,
+        write_dir=write_dir,
+        **kwargs
+    ))
     for workflow in workflows:
         yield workflow.standard_extraction(image_export_format=image_export_format)
 
 
 @ray_remote
 def _ray_extractor(workflow: StandardWorkflow, image_export_format="dict"):
     # Limit internal threading by third-party libraries.
```

### Comparing `mirp-2.2.1/mirp/extract_image_parameters.py` & `mirp-2.2.2/mirp/extract_image_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/extract_mask_labels.py` & `mirp-2.2.2/mirp/extract_mask_labels.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/settings/feature_parameters.py` & `mirp-2.2.2/mirp/settings/feature_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/settings/general_parameters.py` & `mirp-2.2.2/mirp/settings/general_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/settings/generic.py` & `mirp-2.2.2/mirp/settings/generic.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/settings/image_processing_parameters.py` & `mirp-2.2.2/mirp/settings/image_processing_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     bias_field_correction_n_max_iterations: int or list of int, optional, default: 50
         The number of fitting iterations for the N4 bias field algorithm. A single integer, or a list of integers
         with a length equal to the number of fitting levels is expected.
 
     bias_field_convergence_threshold: float, optional, default: 0.001
         Convergence threshold for N4 bias field correction algorithm.
 
-    pet_suv_conversion: {"body_weight", "none"}, default: "body_weight"
+    pet_suv_conversion: {"body_weight", "body_surface_area", "lean_body_mass", "lean_body_mass_bmi", "ideal_body_weight". "none"}, default: "body_weight"
         Intensities in PET imaging are often stored as detected radiotracer activity. To make detected activity more
         comparable between patients, these are converted to standardised uptake values. The following are possible:
 
         * "body_weight": activity is normalised by body weight.
         * "body_surface_area": activity is normalised by body surface area according to DuBois (A formula to estimate
           the approximate surface area if height and weight be known. Arch intern med. 1916;17:863-71).
         * "lean_body_mass": activity is normalised by lean body mass according to James et al. (DHSS/MRC Group on
```

### Comparing `mirp-2.2.1/mirp/settings/import_config_parameters.py` & `mirp-2.2.2/mirp/settings/import_config_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,69 +7,69 @@
 from mirp.settings.transformation_parameters import get_image_transformation_settings
 from mirp.settings.feature_parameters import get_feature_extraction_settings
 from mirp.settings.resegmentation_parameters import get_mask_resegmentation_settings
 from mirp.settings.perturbation_parameters import get_perturbation_settings
 from mirp.settings.image_processing_parameters import get_post_processing_settings
 from mirp.settings.interpolation_parameters import get_image_interpolation_settings, get_mask_interpolation_settings
 from mirp.settings.general_parameters import get_general_settings
-from mirp.settings.utilities import update_settings_from_branch
+from mirp.settings.utilities import update_settings_from_branch, find_branch
 
 
 def create_settings_object(
     xml_tree: None | Element = None,
     **kwargs
 ) -> SettingsClass:
     kwargs = copy.deepcopy(kwargs)
 
     if isinstance(xml_tree, Element):
         # General settings
         update_settings_from_branch(
             kwargs=kwargs,
-            branch=xml_tree.find("general"),
+            branch=find_branch(xml_tree, "general"),
             settings=get_general_settings()
         )
 
         # Post-processing settings
         update_settings_from_branch(
             kwargs=kwargs,
-            branch=xml_tree.find("post_processing"),
+            branch=find_branch(xml_tree, ["post_processing", "image_processing"]),
             settings=get_post_processing_settings()
         )
 
         # Image interpolation settings
         if xml_tree.find("img_interpolate") is not None and xml_tree.find("img_interpolate").find("new_non_iso_spacing") is not None:
             warnings.warn(
                 f"The new_non_iso_spacing tag has been deprecated. Use the new_spacing tag instead.",
                 DeprecationWarning
             )
 
         update_settings_from_branch(
             kwargs=kwargs,
-            branch=xml_tree.find("img_interpolate"),
+            branch=find_branch(xml_tree, ["img_interpolate", "image_interpolation"]),
             settings=get_image_interpolation_settings()
         )
 
         # Mask interpolation settings
         update_settings_from_branch(
             kwargs=kwargs,
-            branch=xml_tree.find("roi_interpolate"),
+            branch=find_branch(xml_tree, ["roi_interpolate", "mask_interpolation"]),
             settings=get_mask_interpolation_settings()
         )
 
         # Perturbation settings
         update_settings_from_branch(
             kwargs=kwargs,
-            branch=xml_tree.find("vol_adapt"),
+            branch=find_branch(xml_tree, ["vol_adapt", "image_perturbation"]),
             settings=get_perturbation_settings()
         )
 
         # Mask resegmentation settings
         update_settings_from_branch(
             kwargs=kwargs,
-            branch=xml_tree.find("roi_resegment"),
+            branch=find_branch(xml_tree, ["roi_resegment", "mask_resegmentation"]),
             settings=get_mask_resegmentation_settings()
         )
 
         # Feature extraction settings
         if xml_tree.find("feature_extr") is not None and xml_tree.find("feature_extr").find("glcm_merge_method") is not None:
             warnings.warn(
                 "The glcm_merge_method tag has been deprecated. Use the glcm_spatial_method tag instead. This takes"
@@ -84,15 +84,15 @@
                 "takes the following values: `2d_average`, `2d_slice_merge`, '2.5d_direction_merge', "
                 "'2.5d_volume_merge', '3d_average', and `3d_volume_merge`",
                 DeprecationWarning
             )
 
         update_settings_from_branch(
             kwargs=kwargs,
-            branch=xml_tree.find("feature_extr"),
+            branch=find_branch(xml_tree, ["feature_extr", "feature_computation"]),
             settings=get_feature_extraction_settings()
         )
 
         # Image transformation settings
         if xml_tree.find("img_transform") is not None and xml_tree.find("img_transform").find("log_average") is not None:
             warnings.warn(
                 "The log_average tag has been deprecated. Use the laplacian_of_gaussian_pooling_method tag "
@@ -105,15 +105,15 @@
                 "The riesz_steered tag has been deprecated. Steerable Riesz filter are now identified by the name "
                 "of the filter kernel (filter_kernels parameter).",
                 DeprecationWarning
             )
 
         update_settings_from_branch(
             kwargs=kwargs,
-            branch=xml_tree.find("img_transform"),
+            branch=find_branch(xml_tree, ["img_transform", "image_transformation"]),
             settings=get_image_transformation_settings()
         )
 
         # Deep learning branch
         if xml_tree.find("deep_learning") is not None:
             warnings.warn(
                 "deep_learning parameter branch has been deprecated. Parameters for image "
```

### Comparing `mirp-2.2.1/mirp/settings/import_data_parameters.py` & `mirp-2.2.2/mirp/settings/import_data_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/settings/interpolation_parameters.py` & `mirp-2.2.2/mirp/settings/interpolation_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/settings/perturbation_parameters.py` & `mirp-2.2.2/mirp/settings/perturbation_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/settings/resegmentation_parameters.py` & `mirp-2.2.2/mirp/settings/resegmentation_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     .. note::
         Even though intensity range resegmentation is usually required to perform *Fixed Bin Size* discretisation,
         default values are available for computed tomography (CT) and positron emission tomography (PET) imaging,
         and are set to -1000.0 Hounsfield Units and 0.0 SUV, respectively.
 
     Parameters
     ----------
-    Sets parameters related to resegmentation of the segmentation mask.
-
     resegmentation_intensity_range: list of float, optional
         Intensity threshold for threshold-based re-segmentation ("threshold" and "range"). If set, requires two
         values for lower and upper range respectively. The upper range value can also be np.nan for half-open ranges.
 
     resegmentation_sigma: float, optional
         Number of standard deviations for outlier-based intensity re-segmentation ("sigma" and "outlier").
```

### Comparing `mirp-2.2.1/mirp/settings/transformation_parameters.py` & `mirp-2.2.2/mirp/settings/transformation_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/settings/utilities.py` & `mirp-2.2.2/mirp/settings/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,32 @@
         "class_key": class_key,
         "typing": typing,
         "to_list": to_list,
         "test_value": test
     }
 
 
+def find_branch(
+        tree: None | Element,
+        branch_name: str | list[str]
+) -> None | Element:
+    if tree is None:
+        return None
+
+    if isinstance(branch_name, str):
+        branch_name = [branch_name]
+
+    for current_branch_name in branch_name:
+        branch = tree.find(current_branch_name)
+        if isinstance(branch, Element):
+            return branch
+
+    return None
+
+
 def update_settings_from_branch(
         kwargs: dict[str, Any],
         branch: None | Element,
         settings: list[dict[str, Any]]
 ):
     from mirp._data_import.utilities import flatten_list
```

### Comparing `mirp-2.2.1/mirp/utilities/config_utilities.py` & `mirp-2.2.2/mirp/utilities/config_utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/utilities/parallel.py` & `mirp-2.2.2/mirp/utilities/parallel.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp/utilities/utilities.py` & `mirp-2.2.2/mirp/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/mirp.egg-info/PKG-INFO` & `mirp-2.2.2/mirp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirp
-Version: 2.2.1
+Version: 2.2.2
 Summary: A package for standardised processing of medical imaging and computation of quantitative features.
 Author-email: Alex Zwanenburg <alexander.zwanenburg@nct-dresden.de>
 License: European Union Public Licence
         V. 1.2
         
         EUPL © the European Union 2007, 2016
```

### Comparing `mirp-2.2.1/mirp.egg-info/SOURCES.txt` & `mirp-2.2.2/mirp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mirp-2.2.1/pyproject.toml` & `mirp-2.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mirp"
-version = "2.2.1"
+version = "2.2.2"
 description = "A package for standardised processing of medical imaging and computation of quantitative features."
 authors = [
     {name = "Alex Zwanenburg", email = "alexander.zwanenburg@nct-dresden.de"}
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 classifiers = [
@@ -44,14 +44,17 @@
 docs = ["sphinx>=5.0.0", "sphinx_rtd_theme>=2.0.0", "nbsphinx"]
 
 [tool.pytest.ini_options]
 addopts = ["--strict-markers"]
 markers = [
     "ci: marks tests for continuous integration"
 ]
+# filterwarnings = [
+#    "error:the matrix subclass"
+# ]
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["mirp*"]
 exclude = ["docs*"]
 
 [tool.setuptools.package-data]
```

