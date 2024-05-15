# Comparing `tmp/pydlutils-0.0.5.tar.gz` & `tmp/pydlutils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydlutils-0.0.5.tar", last modified: Mon Dec 18 11:26:03 2023, max compression
+gzip compressed data, was "pydlutils-0.0.6.tar", last modified: Wed May 15 06:51:25 2024, max compression
```

## Comparing `pydlutils-0.0.5.tar` & `pydlutils-0.0.6.tar`

### file list

```diff
@@ -1,52 +1,58 @@
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-18 11:26:03.105987 pydlutils-0.0.5/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1964 2023-12-18 11:26:03.105987 pydlutils-0.0.5/PKG-INFO
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      796 2023-06-16 11:56:23.000000 pydlutils-0.0.5/README.md
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-18 11:26:03.101987 pydlutils-0.0.5/pydlutils/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/__init__.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-18 11:26:03.101987 pydlutils-0.0.5/pydlutils/basic/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.5/pydlutils/basic/__init__.py
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1802 2023-06-16 11:56:23.000000 pydlutils-0.0.5/pydlutils/basic/registry.py
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1746 2023-06-16 11:56:23.000000 pydlutils-0.0.5/pydlutils/basic/yaml.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-18 11:26:03.101987 pydlutils-0.0.5/pydlutils/peft/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-07 06:38:10.000000 pydlutils-0.0.5/pydlutils/peft/__init__.py
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      135 2023-12-07 06:38:10.000000 pydlutils-0.0.5/pydlutils/peft/registry.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-18 11:26:03.101987 pydlutils-0.0.5/pydlutils/thirdparty/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.5/pydlutils/thirdparty/__init__.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-18 11:26:03.105987 pydlutils-0.0.5/pydlutils/thirdparty/colmap/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:49:23.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/__init__.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    23189 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/build.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     3756 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/build_windows_app.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     4805 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/bundler_to_ply.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2644 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/clang_format_code.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     5449 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/crawl_camera_specs.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    12581 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/database.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     3430 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/export_inlier_matches.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     3237 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/export_inlier_pairs.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     6693 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/export_to_bundler.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     6570 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/export_to_visualsfm.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     6378 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/flickr_downloader.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2692 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/merge_ply_files.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     4817 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/nvm_to_ply.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    26202 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/plyfile.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     5222 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/read_write_dense.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     5069 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/read_write_fused_vis.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    21497 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/read_write_model.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2475 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/test_read_write_dense.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2686 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/test_read_write_fused_vis.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     4812 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/test_read_write_model.py
--rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     7090 2023-06-16 10:29:03.000000 pydlutils-0.0.5/pydlutils/thirdparty/colmap/visualize_model.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-18 11:26:03.105987 pydlutils-0.0.5/pydlutils/torch/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.5/pydlutils/torch/__init__.py
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      355 2023-06-16 11:56:23.000000 pydlutils-0.0.5/pydlutils/torch/registry.py
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      682 2023-12-07 06:38:27.000000 pydlutils-0.0.5/pydlutils/torch/seed.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-18 11:26:03.105987 pydlutils-0.0.5/pydlutils/transformers/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-07 06:38:10.000000 pydlutils-0.0.5/pydlutils/transformers/__init__.py
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      346 2023-12-07 06:38:10.000000 pydlutils-0.0.5/pydlutils/transformers/registry.py
-drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-18 11:26:03.101987 pydlutils-0.0.5/pydlutils.egg-info/
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1964 2023-12-18 11:26:03.000000 pydlutils-0.0.5/pydlutils.egg-info/PKG-INFO
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1571 2023-12-18 11:26:03.000000 pydlutils-0.0.5/pydlutils.egg-info/SOURCES.txt
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        1 2023-12-18 11:26:03.000000 pydlutils-0.0.5/pydlutils.egg-info/dependency_links.txt
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       57 2023-12-18 11:26:03.000000 pydlutils-0.0.5/pydlutils.egg-info/requires.txt
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       10 2023-12-18 11:26:03.000000 pydlutils-0.0.5/pydlutils.egg-info/top_level.txt
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       38 2023-12-18 11:26:03.105987 pydlutils-0.0.5/setup.cfg
--rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1971 2023-12-18 11:25:50.000000 pydlutils-0.0.5/setup.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.710123 pydlutils-0.0.6/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1964 2024-05-15 06:51:25.710123 pydlutils-0.0.6/PKG-INFO
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      796 2024-05-15 06:48:29.000000 pydlutils-0.0.6/README.md
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.702123 pydlutils-0.0.6/pydlutils/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/__init__.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.702123 pydlutils-0.0.6/pydlutils/basic/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.6/pydlutils/basic/__init__.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1802 2023-06-16 11:56:23.000000 pydlutils-0.0.6/pydlutils/basic/registry.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1746 2023-06-16 11:56:23.000000 pydlutils-0.0.6/pydlutils/basic/yaml.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.702123 pydlutils-0.0.6/pydlutils/engine/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:50:30.000000 pydlutils-0.0.6/pydlutils/engine/__init__.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      412 2024-05-15 06:50:30.000000 pydlutils-0.0.6/pydlutils/engine/light_det.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     5401 2024-05-15 06:50:30.000000 pydlutils-0.0.6/pydlutils/engine/light_trial.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     3593 2024-05-15 06:50:30.000000 pydlutils-0.0.6/pydlutils/engine/mlflow_helper.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.702123 pydlutils-0.0.6/pydlutils/peft/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-07 06:38:10.000000 pydlutils-0.0.6/pydlutils/peft/__init__.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      135 2023-12-07 06:38:10.000000 pydlutils-0.0.6/pydlutils/peft/registry.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.706123 pydlutils-0.0.6/pydlutils/thirdparty/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.6/pydlutils/thirdparty/__init__.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.710123 pydlutils-0.0.6/pydlutils/thirdparty/colmap/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-25 10:49:23.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/__init__.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    23189 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/build.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     3756 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/build_windows_app.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     4805 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/bundler_to_ply.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2644 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/clang_format_code.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     5449 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/crawl_camera_specs.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    12581 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/database.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     3430 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/export_inlier_matches.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     3237 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/export_inlier_pairs.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     6693 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/export_to_bundler.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     6570 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/export_to_visualsfm.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     6378 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/flickr_downloader.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2692 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/merge_ply_files.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     4817 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/nvm_to_ply.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    26202 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/plyfile.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     5222 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/read_write_dense.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     5069 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/read_write_fused_vis.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)    21497 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/read_write_model.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2475 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/test_read_write_dense.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     2686 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/test_read_write_fused_vis.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     4812 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/test_read_write_model.py
+-rwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)     7090 2023-06-16 10:29:03.000000 pydlutils-0.0.6/pydlutils/thirdparty/colmap/visualize_model.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.710123 pydlutils-0.0.6/pydlutils/torch/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-06-16 11:56:23.000000 pydlutils-0.0.6/pydlutils/torch/__init__.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      355 2023-06-16 11:56:23.000000 pydlutils-0.0.6/pydlutils/torch/registry.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      682 2024-05-15 06:50:30.000000 pydlutils-0.0.6/pydlutils/torch/seed.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      871 2024-05-15 06:50:30.000000 pydlutils-0.0.6/pydlutils/torch/timer.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.710123 pydlutils-0.0.6/pydlutils/transformers/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        0 2023-12-07 06:38:10.000000 pydlutils-0.0.6/pydlutils/transformers/__init__.py
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)      346 2023-12-07 06:38:10.000000 pydlutils-0.0.6/pydlutils/transformers/registry.py
+drwxrwxr-x   0 deepmirror  (1000) deepmirror  (1000)        0 2024-05-15 06:51:25.702123 pydlutils-0.0.6/pydlutils.egg-info/
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1964 2024-05-15 06:51:25.000000 pydlutils-0.0.6/pydlutils.egg-info/PKG-INFO
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1721 2024-05-15 06:51:25.000000 pydlutils-0.0.6/pydlutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)        1 2024-05-15 06:51:25.000000 pydlutils-0.0.6/pydlutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       42 2024-05-15 06:51:25.000000 pydlutils-0.0.6/pydlutils.egg-info/requires.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       10 2024-05-15 06:51:25.000000 pydlutils-0.0.6/pydlutils.egg-info/top_level.txt
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)       38 2024-05-15 06:51:25.710123 pydlutils-0.0.6/setup.cfg
+-rw-rw-r--   0 deepmirror  (1000) deepmirror  (1000)     1971 2024-05-15 06:50:30.000000 pydlutils-0.0.6/setup.py
```

### Comparing `pydlutils-0.0.5/PKG-INFO` & `pydlutils-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlutils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utility library for deep learning
 Home-page: https://github.com/zebincai/pydlutils
 Author: zebincai
 Author-email: 1028798080@qq.com
 License: Apache
 Download-URL: https://github.com/zebincai/pydlutils/tags
 Description: # pydlutils
```

### Comparing `pydlutils-0.0.5/README.md` & `pydlutils-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/basic/registry.py` & `pydlutils-0.0.6/pydlutils/basic/registry.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/basic/yaml.py` & `pydlutils-0.0.6/pydlutils/basic/yaml.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/build.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/build.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/build_windows_app.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/build_windows_app.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/bundler_to_ply.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/bundler_to_ply.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/clang_format_code.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/clang_format_code.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/crawl_camera_specs.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/crawl_camera_specs.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/database.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/database.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/export_inlier_matches.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/export_inlier_matches.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/export_inlier_pairs.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/export_inlier_pairs.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/export_to_bundler.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/export_to_bundler.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/export_to_visualsfm.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/export_to_visualsfm.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/flickr_downloader.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/flickr_downloader.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/merge_ply_files.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/merge_ply_files.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/nvm_to_ply.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/nvm_to_ply.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/plyfile.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/plyfile.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/read_write_dense.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/read_write_dense.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/read_write_fused_vis.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/read_write_fused_vis.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/read_write_model.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/read_write_model.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/test_read_write_dense.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/test_read_write_dense.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/test_read_write_fused_vis.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/test_read_write_fused_vis.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/test_read_write_model.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/test_read_write_model.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/thirdparty/colmap/visualize_model.py` & `pydlutils-0.0.6/pydlutils/thirdparty/colmap/visualize_model.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils/torch/seed.py` & `pydlutils-0.0.6/pydlutils/torch/seed.py`

 * *Files identical despite different names*

### Comparing `pydlutils-0.0.5/pydlutils.egg-info/PKG-INFO` & `pydlutils-0.0.6/pydlutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlutils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utility library for deep learning
 Home-page: https://github.com/zebincai/pydlutils
 Author: zebincai
 Author-email: 1028798080@qq.com
 License: Apache
 Download-URL: https://github.com/zebincai/pydlutils/tags
 Description: # pydlutils
```

### Comparing `pydlutils-0.0.5/pydlutils.egg-info/SOURCES.txt` & `pydlutils-0.0.6/pydlutils.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 pydlutils.egg-info/SOURCES.txt
 pydlutils.egg-info/dependency_links.txt
 pydlutils.egg-info/requires.txt
 pydlutils.egg-info/top_level.txt
 pydlutils/basic/__init__.py
 pydlutils/basic/registry.py
 pydlutils/basic/yaml.py
+pydlutils/engine/__init__.py
+pydlutils/engine/light_det.py
+pydlutils/engine/light_trial.py
+pydlutils/engine/mlflow_helper.py
 pydlutils/peft/__init__.py
 pydlutils/peft/registry.py
 pydlutils/thirdparty/__init__.py
 pydlutils/thirdparty/colmap/__init__.py
 pydlutils/thirdparty/colmap/build.py
 pydlutils/thirdparty/colmap/build_windows_app.py
 pydlutils/thirdparty/colmap/bundler_to_ply.py
@@ -33,9 +37,10 @@
 pydlutils/thirdparty/colmap/test_read_write_dense.py
 pydlutils/thirdparty/colmap/test_read_write_fused_vis.py
 pydlutils/thirdparty/colmap/test_read_write_model.py
 pydlutils/thirdparty/colmap/visualize_model.py
 pydlutils/torch/__init__.py
 pydlutils/torch/registry.py
 pydlutils/torch/seed.py
+pydlutils/torch/timer.py
 pydlutils/transformers/__init__.py
 pydlutils/transformers/registry.py
```

### Comparing `pydlutils-0.0.5/setup.py` & `pydlutils-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = "Utility library for deep learning"
 
 
 def main():
     INSTALL_REQUIRES = []
     DEPENDENCY_LINKS = []
```

