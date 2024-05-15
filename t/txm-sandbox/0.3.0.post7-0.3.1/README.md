# Comparing `tmp/txm_sandbox-0.3.0.post7.tar.gz` & `tmp/txm_sandbox-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txm_sandbox-0.3.0.post7.tar", last modified: Thu May  9 01:07:40 2024, max compression
+gzip compressed data, was "txm_sandbox-0.3.1.tar", last modified: Wed May 15 04:02:48 2024, max compression
```

## Comparing `txm_sandbox-0.3.0.post7.tar` & `txm_sandbox-0.3.1.tar`

### file list

```diff
@@ -1,97 +1,100 @@
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.939130 txm_sandbox-0.3.0.post7/
--rw-rw-r--   0 xianghui   (501) staff       (20)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post7/LICENSE
--rw-rw-r--   0 xianghui   (501) staff       (20)      203 2024-05-09 00:28:45.000000 txm_sandbox-0.3.0.post7/MANIFEST.in
--rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-09 01:07:40.938920 txm_sandbox-0.3.0.post7/PKG-INFO
--rw-rw-r--   0 xianghui   (501) staff       (20)     1964 2024-05-09 00:35:34.000000 txm_sandbox-0.3.0.post7/README.md
--rwxrwxr-x   0 xianghui   (501) staff       (20)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post7/TXM_GUI2.ipynb
--rw-r--r--   0 xianghui   (501) staff       (20)       38 2024-05-09 01:07:40.939170 txm_sandbox-0.3.0.post7/setup.cfg
--rw-rw-r--   0 xianghui   (501) staff       (20)     1130 2024-05-09 01:07:13.000000 txm_sandbox-0.3.0.post7/setup.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.928118 txm_sandbox-0.3.0.post7/txm_sandbox/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/__init__.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.929579 txm_sandbox-0.3.0.post7/txm_sandbox/config/
--rw-rw-r--   0 xianghui   (501) staff       (20)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/config/XANES2D_GUI_config.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/config/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/config/analysis_tool_gui_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/config/io_tomo_h5_data_structure.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/config/io_xanes2D_h5_data_structure.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/config/io_xanes3D_h5_data_structure.json
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.930240 txm_sandbox-0.3.0.post7/txm_sandbox/dicts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/dicts/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/dicts/config_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/dicts/customized_struct_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/dicts/sklearn_opt_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/dicts/xanes_analysis_dict.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.930467 txm_sandbox-0.3.0.post7/txm_sandbox/external/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/external/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/external/user_io.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.932782 txm_sandbox-0.3.0.post7/txm_sandbox/gui/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/conv_data_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/gen_algn_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    79463 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/gui_components.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/io_config_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/main_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/misc_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/tomo_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/xanes2D_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/xanes3D_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/xanes_analysis_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   203257 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/gui/xanes_fitting_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.933193 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/__init__.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.933951 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      786 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      957 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      899 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)     2389 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)     1362 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.934203 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/dicts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/dicts/__init__.py
--rw-r--r--   0 xianghui   (501) staff       (20)     5528 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/dicts/data_struct_dict.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.935176 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/
--rw-rw-r--   0 xianghui   (501) staff       (20)      106 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16170 2024-05-08 14:31:59.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/appl_mask_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     9799 2024-05-08 14:04:01.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/convert_data_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    27222 2024-05-07 07:45:10.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/tomo_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    24243 2024-05-08 12:40:21.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    54769 2024-05-08 11:49:58.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16157 2024-05-08 13:04:07.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.936187 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      605 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      599 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    15251 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     2428 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16610 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1197 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     2029 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
--rw-r--r--   0 xianghui   (501) staff       (20)     1533 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/txm_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.936531 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/utils/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/utils/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1264 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/utils/io.py
--rw-r--r--   0 xianghui   (501) staff       (20)    10590 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/utils/misc.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.936791 txm_sandbox-0.3.0.post7/txm_sandbox/tmp/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/tmp/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/tmp/readme.txt
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.938505 txm_sandbox-0.3.0.post7/txm_sandbox/utils/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/io.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/lineshapes.py
--rwxrwxr-x   0 xianghui   (501) staff       (20)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/misc.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/plotlib.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/reg_algs.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/tomo_recon_tools.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    41021 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_analysis.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_image_utils.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    23436 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_math.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_post_analysis.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    84774 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_regtools.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_spectra_filters.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-09 01:07:40.938686 txm_sandbox-0.3.0.post7/txm_sandbox.egg-info/
--rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-09 01:07:40.000000 txm_sandbox-0.3.0.post7/txm_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 xianghui   (501) staff       (20)     3045 2024-05-09 01:07:40.000000 txm_sandbox-0.3.0.post7/txm_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-09 01:07:40.000000 txm_sandbox-0.3.0.post7/txm_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-09 01:07:40.000000 txm_sandbox-0.3.0.post7/txm_sandbox.egg-info/not-zip-safe
--rw-r--r--   0 xianghui   (501) staff       (20)      170 2024-05-09 01:07:40.000000 txm_sandbox-0.3.0.post7/txm_sandbox.egg-info/requires.txt
--rw-r--r--   0 xianghui   (501) staff       (20)       12 2024-05-09 01:07:40.000000 txm_sandbox-0.3.0.post7/txm_sandbox.egg-info/top_level.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.038593 txm_sandbox-0.3.1/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1/LICENSE
+-rw-rw-r--   0 xianghui   (501) staff       (20)      203 2024-05-09 00:28:45.000000 txm_sandbox-0.3.1/MANIFEST.in
+-rw-r--r--   0 xianghui   (501) staff       (20)      706 2024-05-15 04:02:48.038407 txm_sandbox-0.3.1/PKG-INFO
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1964 2024-05-09 00:35:34.000000 txm_sandbox-0.3.1/README.md
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1/TXM_GUI2.ipynb
+-rw-r--r--   0 xianghui   (501) staff       (20)       38 2024-05-15 04:02:48.038633 txm_sandbox-0.3.1/setup.cfg
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1124 2024-05-15 04:00:27.000000 txm_sandbox-0.3.1/setup.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.010140 txm_sandbox-0.3.1/txm_sandbox/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.012446 txm_sandbox-0.3.1/txm_sandbox/config/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/XANES2D_GUI_config.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/analysis_tool_gui_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/io_tomo_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/io_xanes2D_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/config/io_xanes3D_h5_data_structure.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.013733 txm_sandbox-0.3.1/txm_sandbox/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/config_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/customized_struct_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/sklearn_opt_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/dicts/xanes_analysis_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.014142 txm_sandbox-0.3.1/txm_sandbox/external/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/external/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/external/user_io.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.021615 txm_sandbox-0.3.1/txm_sandbox/gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/conv_data_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/gen_algn_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    79148 2024-05-12 04:56:04.000000 txm_sandbox-0.3.1/txm_sandbox/gui/gui_components.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/io_config_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/main_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/misc_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/tomo_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/xanes2D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/xanes3D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/xanes_analysis_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   203257 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/gui/xanes_fitting_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.022312 txm_sandbox-0.3.1/txm_sandbox/napari_gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.024216 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      979 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      957 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      899 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2389 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1362 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.024576 txm_sandbox-0.3.1/txm_sandbox/napari_gui/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/dicts/__init__.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     8853 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/dicts/data_struct_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.028228 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      106 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16170 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/appl_mask_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     9799 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/convert_data_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     3929 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/extra_io_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    32957 2024-05-14 07:59:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/tomo_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    24243 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    67247 2024-05-15 03:58:02.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.030167 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     4223 2024-05-14 05:10:46.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      650 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      599 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15251 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2441 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16610 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1197 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     2029 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     1533 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/txm_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.031206 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/__init__.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     5157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/ext_io_lib.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1264 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/io.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    10590 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/misc.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.031756 txm_sandbox-0.3.1/txm_sandbox/tmp/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/tmp/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/tmp/readme.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.037845 txm_sandbox-0.3.1/txm_sandbox/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/io.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/lineshapes.py
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/misc.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/plotlib.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/reg_algs.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/tomo_recon_tools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    41021 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_image_utils.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    23436 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_math.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_post_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    84912 2024-05-14 13:37:48.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_regtools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1/txm_sandbox/utils/xanes_spectra_filters.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-15 04:02:48.038181 txm_sandbox-0.3.1/txm_sandbox.egg-info/
+-rw-r--r--   0 xianghui   (501) staff       (20)      706 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 xianghui   (501) staff       (20)     3196 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/not-zip-safe
+-rw-r--r--   0 xianghui   (501) staff       (20)      170 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/requires.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)       12 2024-05-15 04:02:47.000000 txm_sandbox-0.3.1/txm_sandbox.egg-info/top_level.txt
```

### Comparing `txm_sandbox-0.3.0.post7/LICENSE` & `txm_sandbox-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/PKG-INFO` & `txm_sandbox-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.0.post7
+Version: 0.3.1
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.0.post7/README.md` & `txm_sandbox-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/TXM_GUI2.ipynb` & `txm_sandbox-0.3.1/TXM_GUI2.ipynb`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/setup.py` & `txm_sandbox-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: xiao
 """
 
 from setuptools import setup, find_packages
 
 setup(name='txm_sandbox',
-      version='0.3.0.post7',
+      version='0.3.1',
       description='Integrated Spectro-Imaging Analysis Toolbox',
       url='https://github.com/xianghuix/TXM_Sandbox',
       author='Xianghui Xiao',
       author_email='xianghuix@gmail.com',
       license='MIT',
       packages=find_packages(),
       install_requires=[
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/config/XANES2D_GUI_config.json` & `txm_sandbox-0.3.1/txm_sandbox/config/XANES2D_GUI_config.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/config/io_xanes3D_h5_data_structure.json` & `txm_sandbox-0.3.1/txm_sandbox/config/io_xanes3D_h5_data_structure.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/dicts/config_dict.py` & `txm_sandbox-0.3.1/txm_sandbox/dicts/config_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/dicts/customized_struct_dict.py` & `txm_sandbox-0.3.1/txm_sandbox/dicts/customized_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/dicts/sklearn_opt_dict.py` & `txm_sandbox-0.3.1/txm_sandbox/dicts/sklearn_opt_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/dicts/xanes_analysis_dict.py` & `txm_sandbox-0.3.1/txm_sandbox/dicts/xanes_analysis_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/conv_data_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/conv_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/gen_algn_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/gen_algn_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/gui_components.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/gui_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,36 +232,31 @@
         global_h.GUI_cfg_file,
         {"cwd": new_cwd},
     )
 
 
 def check_file_availability(raw_h5_dir, scan_id=None, signature="", return_idx=False):
     if scan_id is None:
-        # data_files = glob.glob(os.path.join(raw_h5_dir, signature.format("*")))
         data_files = glob.glob(str(Path(raw_h5_dir).joinpath(signature.format("*"))))
     else:
-        # data_files = glob.glob(
-        #     os.path.join(raw_h5_dir, signature.format(scan_id)))
         data_files = glob.glob(
             str(Path(raw_h5_dir).joinpath(Path(signature.format(scan_id))))
         )
 
     if len(data_files) == 0:
         return []
     else:
         if return_idx:
             ids = []
             for fn in sorted(data_files):
-                # ids.append(os.path.basename(fn).split(".")[-2].split("_")[-1])
                 ids.append(Path(fn).name.split(".")[-2].split("_")[-1])
             return ids
         else:
             fns = []
             for fn in sorted(data_files):
-                # fns.append(os.path.basename(fn))
                 fns.append(Path(fn).name)
             return fns
 
 
 def create_widget(wtype, layout, **kwargs):
     if wtype == "VBox":
         hs = widgets.VBox(**kwargs)
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/io_config_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/io_config_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/main_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/misc_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/misc_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/tomo_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/xanes2D_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/xanes2D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/xanes3D_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/xanes3D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/xanes_analysis_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/xanes_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/gui/xanes_fitting_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/gui/xanes_fitting_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'xanes2d_reg'": "OrderedDict([('cfg_file', "*

 * *                  "'/Users/xianghui/Developments/Python_projects/txm_sandbox_test_data/aps_test_data/2D_trial_reg_cfg_Li05Co_xanes2d__005_2024-05-14-12-57-24.json')])"}*

```diff
@@ -4,14 +4,17 @@
     },
     "tomo_recon": {
         "cfg_file": "/media/usb2/XANES_test_2024/xanes3d_tomo_tplt_cfg_2024-04-28-10-11-21.json"
     },
     "xanes2d_fit": {
         "cfg_file": "/media/xiao/650a7301-d9d1-43d0-9a79-294552824932/Guiliang_2023-2/2D_trial_reg_multipos_2D_xanes_scan2_id_72584_repeat_00_pos_00_2023-12-09-11-54-24.h5"
     },
+    "xanes2d_reg": {
+        "cfg_file": "/Users/xianghui/Developments/Python_projects/txm_sandbox_test_data/aps_test_data/2D_trial_reg_cfg_Li05Co_xanes2d__005_2024-05-14-12-57-24.json"
+    },
     "xanes3d_auto_cen": {
         "cfg_file": "/media/usb2/XANES_test_2024/xanes3d_autocen&reg--_2024-04-28-10-29-34.json"
     },
     "xanes3d_fit": {
         "cfg_file": "/media/usb2/Tongchao_2024-1/pass-312475/3D_trial_reg_scan_id_83719-83721_2024-04-27-10-20-35_pytxm.h5"
     }
 }
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/dicts/data_struct_dict.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/dicts/data_struct_dict.py`

 * *Files 24% similar despite different names*

```diff
@@ -144,7 +144,81 @@
         },
         "tomo_raw_fn_template": "fly_scan_id_{0}.h5",
         "xanes3D_recon_dir_template": "recon_fly_scan_id_{0}",
         "xanes3D_recon_fn_template": "recon_fly_scan_id_{0}_{1}.tiff",
         "customized_reader": {"user_xanes3D_reader": ""},
     },
 }
+
+APS_TXM_CFG = {
+    "io_data_structure_tomo": {
+        "use_h5_reader": True,
+        "structured_h5_reader": {
+            "io_data_structure": {
+                "data_path": "/exchange/data",
+                "flat_path": "/exchange/data_white",
+                "dark_path": "/exchange/data_dark",
+                "theta_path": "/exchange/theta",
+            },
+            "io_data_info": {
+                "item00_path": "/exchange/data",
+                "item01_path": "/exchange/theta",
+                "item02_path": "/measurement/instrument/detection_system/objective/magnification",
+                "item03_path": "/measurement/instrument/detector/pixel_size",
+                "item04_path": "/measurement/instrument/monochromator/energy",
+                "item05_path": "measurement/sample/description_1",
+                "item06_path": "/process/acquisition/start_date",
+                "item07_path": "/measurement/sample/file/name",
+            },
+        },
+        "tomo_raw_fn_template": "{0}_{1}.h5",
+        "customized_reader": {"user_tomo_reader": ""},
+    },
+    "io_data_structure_xanes2D": {
+        "use_h5_reader": True,
+        "structured_h5_reader": {
+            "io_data_structure": {
+                "data_path": "/exchange/data",
+                "flat_path": "/exchange/data_white",
+                "dark_path": "/exchange/data_dark",
+                "eng_path": "/measurement/instrument/monochromator/energy",
+            },
+            "io_data_info": {
+                "item00_path": "/exchange/data",
+                "item01_path": "/measurement/instrument/monochromator/energy",
+                "item02_path": "/measurement/instrument/detection_system/objective/magnification",
+                "item03_path": "/measurement/instrument/detector/pixel_size",
+                "item04_path": "measurement/sample/description_1",
+                "item05_path": "/process/acquisition/start_date",
+                "item06_path": "",
+                "item07_path": "",
+            },
+        },
+        "xanes2D_raw_fn_template": "{0}_{1}.h5",
+        "customized_reader": {"user_xanes2D_reader": ""},
+    },
+    "io_data_structure_xanes3D": {
+        "use_h5_reader": True,
+        "structured_h5_reader": {
+            "io_data_structure": {
+                "data_path": "/exchange/data",
+                "flat_path": "/exchange/data_white",
+                "dark_path": "/exchange/data_dark",
+                "eng_path": "/measurement/instrument/monochromator/energy",
+            },
+            "io_data_info": {
+                "item00_path": "/exchange/data",
+                "item01_path": "/exchange/theta",
+                "item02_path": "/measurement/instrument/detection_system/objective/magnification",
+                "item03_path": "/measurement/instrument/detector/pixel_size",
+                "item04_path": "/measurement/instrument/monochromator/energy",
+                "item05_path": "measurement/sample/description_1",
+                "item06_path": "/process/acquisition/start_date",
+                "item07_path": "",
+            },
+        },
+        "tomo_raw_fn_template": "{0}_{1}.h5",
+        "xanes3D_recon_dir_template": "recon_{0}_{1}",
+        "xanes3D_recon_fn_template": "recon_{0}_{1}_{2}.tiff",
+        "customized_reader": {"user_xanes3D_reader": ""},
+    },
+}
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/appl_mask_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/appl_mask_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/convert_data_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/convert_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/tomo_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/tomo_gui.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 import numpy as np
 import os
+import sys
+from copy import deepcopy
 
 import json
 import glob
 import h5py
 import datetime
 from pathlib import Path
 import matplotlib.pyplot as plt
 from magicgui import widgets
 
+# from PyQt5.QtWidgets import QApplication
+# from PyQt5 import QtWidgets, QtCore
+from qtpy import QtWidgets, QtCore
+from magicgui.widgets import request_values
+from magicgui import magicgui
+
 from ...utils.io import data_reader, tomo_h5_reader
 from ...utils.tomo_recon_tools import rm_redundant
 from ...gui.gui_components import (
     check_file_availability,
 )
 from ..utils.misc import (
     set_data_widget,
     rm_gui_viewers,
     disp_progress_info,
     info_reader,
     update_layer_in_viewer,
     show_layers_in_viewer,
 )
-from ..dicts.data_struct_dict import ZFLY_CFG, FLY_CFG
+from ..dicts.data_struct_dict import ZFLY_CFG, FLY_CFG, APS_TXM_CFG
+
+from ..utils.ext_io_lib import show_io_win, mk_aps_cfg
 
 
 h5_reader = data_reader(tomo_h5_reader)
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 tomo_rec_script_fn = Path(__file__).parents[1] / "scripts/tomo_recon_cmd.py"
 tomo_batch_rec_script_fn = Path(__file__).parents[1] / "scripts/tomo_batch_recon_cmd.py"
@@ -52,36 +62,42 @@
     global _TOMO_TRL_SCN_ID_CHOICES
     return _TOMO_TRL_SCN_ID_CHOICES
 
 
 ################################################################################
 #             do trial recon for a single slice of a given scan                #
 ################################################################################
-class tomo_gui:
+class tomo_gui(QtCore.QObject):
     def __init__(self, viewer):
+        super().__init__()
         self.viewer = viewer
+        self._io_win_dir = ""
         self._tomo_cfg = ZFLY_CFG["io_data_structure_tomo"]
         self._scn_fn = None
         self._wedge_data_avg = 0
         self._trial_cen_rec_done = False
         self._multi_trial_cen_rec_done = False
         self._cen = None
         self._wedge_autodet_fig = None
         self._viewers = ["proj_prev", "data_center", "tomo_viewer"]
+        # self.extra_io_signal = QtCore.Signal()
+        # self.extra_io_signal.connect(self._show_io_win)
 
         self.label0 = widgets.Label(
             value="-------------------     Tomo Recon    --------------------",
         )
         self.label1 = widgets.Label(
             name="Step 1",
             value="--------------------     Trial Cen    --------------------",
         )
         self.top_dir = widgets.FileEdit(mode="d", value=Path.home())
         self.file_type = widgets.ComboBox(
-            choices=["tomo_zfly", "fly_scan"], value="tomo_zfly", name="scan type"
+            choices=["tomo_zfly", "fly_scan", "APS_tomo"],
+            value="tomo_zfly",
+            name="scan type",
         )
         self.find_multi_cen = widgets.CheckBox(
             value=False, text="find cen for multiple scans", enabled=False
         )
         self.scan_id = widgets.ComboBox(
             enabled=False, choices=get_self_avail_scn_id_choices, name="scan id"
         )
@@ -160,14 +176,58 @@
                 self.trial_cen_done,
                 self.vol_rec,
                 self.close_file,
                 self.op_status,
             ]
         )
 
+    # def __io_win(self, dtype="APS_tomo"):
+    #     self._io_win = QtWidgets.QDialog()
+    #     self._io_win.setWindowTitle("extra data info")
+
+    #     layout = QtWidgets.QVBoxLayout()
+    #     label = QtWidgets.QLabel("This is a pop-up window")
+    #     file = QtWidgets.QFileDialog(
+    #         caption="pick a tomo file", directory=self._io_win_dir, filter="*.h5"
+    #     )
+    #     sel_file = QtWidgets.QPushButton("Click me")
+    #     # sel_file.clicked.connect()
+    #     layout.addWidget(label)
+    #     # layout.addWidget(file)
+    #     layout.addWidget(sel_file)
+    #     self._io_win.setLayout(layout)
+
+    #     # Show the pop-up window as a modal dialog
+    #     self._io_win.exec_()
+
+    # def _show_io_win(self, dtype="APS_tomo"):
+    #     # @magicgui(main_window=True,
+    #     #           )
+    #     # def create_io_win()
+    #     vals = request_values(
+    #         name={
+    #             "annotation": Path,
+    #             "label": "pick a tomo file",
+    #             "options": {"mode": "r", "filter": "tomo data file (*.h5)"},
+    #         },
+    #         title="pick a tomo file from 3D XANES data series",
+    #     )
+    #     print(repr(vals))
+
+    # def create_io_win(dtype=dtype):
+    #     win = extra_io_win(self, dtype=dtype)
+    #     # win.show()
+    #     win.show(run=True)
+
+    # create_io_win(dtype=dtype)
+
+    # app = QtWidgets.QApplication.instance() or QtWidgets.QApplication(sys.argv)
+    # QtCore.QTimer.singleShot(0, create_io_win)
+    # app.exec_()
+
     @disp_progress_info("data directory info read")
     def __check_avail_data(self):
         global _TOMO_TRL_SCN_ID_CHOICES
         ids = check_file_availability(
             str(self.top_dir.value),
             scan_id=None,
             signature=self._tomo_cfg["tomo_raw_fn_template"],
@@ -177,17 +237,22 @@
             _TOMO_TRL_SCN_ID_CHOICES = ids
         else:
             _TOMO_TRL_SCN_ID_CHOICES = []
         self.scan_id.reset_choices()
 
     def __comp_scn_fn(self):
         if self.scan_id.value:
-            self._scn_fn = self.top_dir.value / self._tomo_cfg[
-                "tomo_raw_fn_template"
-            ].format(self.scan_id.value)
+            if self.file_type.value == "APS_tomo":
+                self._scn_fn = self.top_dir.value / self._tomo_cfg[
+                    "tomo_raw_fn_template"
+                ].format(str(self.scan_id.value).zfill(3))
+            else:
+                self._scn_fn = self.top_dir.value / self._tomo_cfg[
+                    "tomo_raw_fn_template"
+                ].format(self.scan_id.value)
         else:
             self._scn_fn = None
 
     def __set_trial_cen_rec_widgets(self):
         if (self._scn_fn is None) or (not self._scn_fn.exists()):
             """
             self.find_multi_cen.enabled = False
@@ -263,15 +328,15 @@
         self._wedge_data_avg = 0
         self._trial_cen_rec_done = False
         self._multi_trial_cen_rec_done = False
         self._cen = None
         self._wedge_autodet_fig = None
         self._trial_cen_dir = None
 
-        self.find_multi_cen.enabled = False        
+        self.find_multi_cen.enabled = False
         self.scan_id.enabled = False
         self.proj_prev.enabled = False
         self.cen_sch_s.enabled = False
         self.ref_sli.enabled = False
         self.is_wedge.enabled = False
         self.wedge_thsh.enabled = False
         self.phase_retrieval.enabled = False
@@ -307,16 +372,59 @@
         self.scan_id.reset_choices()
 
         self._close_file()
 
     def _sel_in_file_type(self):
         if self.file_type.value == "tomo_zfly":
             self._tomo_cfg = ZFLY_CFG["io_data_structure_tomo"]
-        else:
+            self.top_dir.enabled = True
+        elif self.file_type.value == "fly_scan":
             self._tomo_cfg = FLY_CFG["io_data_structure_tomo"]
+            self.top_dir.enabled = True
+        elif self.file_type.value == "APS_tomo":
+            _cfg = deepcopy(APS_TXM_CFG)
+            name = show_io_win(dtype="APS_tomo")
+            if name is not None:
+                fn_tplt = name["name"].stem.rsplit("_", maxsplit=1)[0]
+                # tem = (
+                #     _tomo_cfg["io_data_structure_tomo"]["tomo_raw_fn_template"]
+                #     .replace("{0}", fn_tplt)
+                #     .replace("{1}", "{0}")
+                # )
+                # _tomo_cfg["io_data_structure_tomo"]["tomo_raw_fn_template"] = tem
+                # _tomo_cfg["io_data_structure_xanes2D"]["xanes2D_raw_fn_template"] = tem
+                # _tomo_cfg["io_data_structure_xanes3D"]["tomo_raw_fn_template"] = tem
+                # _tomo_cfg["io_data_structure_xanes3D"]["xanes3D_recon_dir_template"] = (
+                #     "recon_" + str(Path(tem).stem)
+                # )
+                # _tomo_cfg["io_data_structure_xanes3D"]["xanes3D_recon_fn_template"] = (
+                #     "recon_" + str(Path(tem).stem) + "_{1}.tiff"
+                # )
+                # self._tomo_cfg = _tomo_cfg
+                self._tomo_cfg = mk_aps_cfg(fn_tplt, _cfg, dtype="APS 3D XANES")[
+                    "io_data_structure_tomo"
+                ]
+                print(f"{self._tomo_cfg=}")
+                self.__reset_widgets()
+                self.top_dir.value = name["name"].parent
+                self._trial_cen_dir = self.top_dir.value / "data_center"
+                self.top_dir.enabled = False
+
+            # self._tomo_cfg
+            # # app = QApplication(sys.argv)
+            # win = extra_io_win(self, dtype="APS_tomo")
+
+            # app = QtWidgets.QApplication.instance()
+            # if app is None:
+            #     app = QtWidgets.QApplication(sys.argv)
+            # # win.show()
+            # QtCore.QMetaObject.invokeMethod(win, "show", QtCore.Qt.QueuedConnection)
+            # app.exec_()
+            # # win.show(run=True)
+
         self.__check_avail_data()
         self.__comp_scn_fn()
         self.__set_trial_cen_rec_widgets()
         self.__set_vol_rec_widgets()
 
     def _sel_top_dir(self):
         self.__reset_widgets()
@@ -350,37 +458,56 @@
         self.proj_prev.value = False
         self.__comp_scn_fn()
         self.__set_vol_rec_widgets()
 
     @disp_progress_info("data file read")
     def _proj_prev(self):
         rm_gui_viewers(self.viewer, ["proj_prev"])
-        if self.proj_prev.value:
-            if self.file_type.value == "tomo_zfly":
-                update_layer_in_viewer(
-                    self.viewer,
-                    h5py.File(self._scn_fn, "r")[
-                        ZFLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
-                            "io_data_structure"
-                        ]["data_path"]
-                    ],
-                    "proj_prev",
-                )
-                show_layers_in_viewer(self.viewer, ["proj_prev"])
-            else:
-                update_layer_in_viewer(
-                    self.viewer,
-                    h5py.File(self._scn_fn, "r")[
-                        FLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
-                            "io_data_structure"
-                        ]["data_path"]
-                    ],
-                    "proj_prev",
-                )
-                show_layers_in_viewer(self.viewer, ["proj_prev"])
+        # if self.proj_prev.value:
+        #     if self.file_type.value == "tomo_zfly":
+        #         update_layer_in_viewer(
+        #             self.viewer,
+        #             h5py.File(self._scn_fn, "r")[
+        #                 ZFLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
+        #                     "io_data_structure"
+        #                 ]["data_path"]
+        #             ],
+        #             "proj_prev",
+        #         )
+        #         show_layers_in_viewer(self.viewer, ["proj_prev"])
+        #     elif self.file_type.value == "fly_scan":
+        #         update_layer_in_viewer(
+        #             self.viewer,
+        #             h5py.File(self._scn_fn, "r")[
+        #                 FLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
+        #                     "io_data_structure"
+        #                 ]["data_path"]
+        #             ],
+        #             "proj_prev",
+        #         )
+        #         show_layers_in_viewer(self.viewer, ["proj_prev"])
+        #     elif self.file_type.value == "APS_tomo":
+        #         update_layer_in_viewer(
+        #             self.viewer,
+        #             h5py.File(self._scn_fn, "r")[
+        #                 FLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
+        #                     "io_data_structure"
+        #                 ]["data_path"]
+        #             ],
+        #             "proj_prev",
+        #         )
+        #         show_layers_in_viewer(self.viewer, ["proj_prev"])
+        update_layer_in_viewer(
+            self.viewer,
+            h5py.File(self._scn_fn, "r")[
+                self._tomo_cfg["structured_h5_reader"]["io_data_structure"]["data_path"]
+            ],
+            "proj_prev",
+        )
+        show_layers_in_viewer(self.viewer, ["proj_prev"])
 
     @disp_progress_info("missing angle calculate")
     def _is_wedge(self):
         self._cen = None
         self._trial_cen_rec_done = False
         self.__set_vol_rec_widgets()
         if self.is_wedge.value:
@@ -505,20 +632,21 @@
         )
         xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["recon_top_dir"] = str(
             self.top_dir.value
         )
         xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["wedge_ang_auto_det_ref_fn"] = (
             str(
                 self.top_dir.value
-                / f"{self.file_type.value}_id_{self.scan_id.value}.h5"
+                / self._tomo_cfg["tomo_raw_fn_template"].format(self.scan_id.value)
             )
         )
+
         xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["io_confg"] = self._tomo_cfg
         xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["hardware_trig_type"] = (
-            True if self.file_type.value == "tomo_zfly" else False
+            True if self.file_type.value in ["tomo_zfly", "APS_tomo"] else False
         )
 
         xanes3d_tomo_tplt_cfg["scan id"]["recon_config"]["recon_type"] = "Trial Cent"
         xanes3d_tomo_tplt_cfg["scan id"]["recon_config"][
             "is_wedge"
         ] = self.is_wedge.value
 
@@ -551,24 +679,36 @@
             ]["io_data_structure"]["eng_path"] = ZFLY_CFG["io_data_structure_xanes3D"][
                 "structured_h5_reader"
             ][
                 "io_data_structure"
             ][
                 "eng_path"
             ]
-        else:
+        elif self.file_type.value == "fly_scan":
             xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["io_confg"][
                 "structured_h5_reader"
             ]["io_data_structure"]["eng_path"] = FLY_CFG["io_data_structure_xanes3D"][
                 "structured_h5_reader"
             ][
                 "io_data_structure"
             ][
                 "eng_path"
             ]
+        elif self.file_type.value == "APS_tomo":
+            xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["io_confg"][
+                "structured_h5_reader"
+            ]["io_data_structure"]["eng_path"] = APS_TXM_CFG[
+                "io_data_structure_xanes3D"
+            ][
+                "structured_h5_reader"
+            ][
+                "io_data_structure"
+            ][
+                "eng_path"
+            ]
 
         if self.phase_retrieval.value:
             xanes3d_tomo_tplt_cfg["scan id"]["flt_params"]["2"] = {
                 "filter_name": "phase retrieval",
                 "params": {
                     "filter": "paganin",
                     "pad": "True",
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/xanes_fit_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/xanes_reg_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import os
 import glob
+from copy import deepcopy
 
 import tifffile
 import h5py
 import json
 import dask.array as da
 import datetime
 from pathlib import Path
@@ -18,25 +19,30 @@
     set_data_widget,
     overlap_roi,
     update_layer_in_viewer,
     show_layers_in_viewer,
     rm_gui_viewers,
     disp_progress_info,
 )
-from ..dicts.data_struct_dict import ZFLY_CFG, FLY_CFG
+from ..dicts.data_struct_dict import ZFLY_CFG, FLY_CFG, APS_TXM_CFG
+from ..utils.ext_io_lib import mk_aps_cfg
 
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 xanes3d_auto_cen_reg_script_fn = (
     Path(__file__).parents[1] / "scripts/xanes3d_tomo_autocent_cmd.py"
 )
 xanes2d_img_auto_cen_script_fn = (
     Path(__file__).parents[1] / "scripts/xanes2d_image_autoreg_cmd.py"
 )
 
+aps_xanes2d_img_auto_cen_script_fn = (
+    Path(__file__).parents[1] / "scripts/aps_xanes2d_image_autoreg_cmd.py"
+)
+
 with open(
     Path(__file__).parents[1] / "configs/xanes3d_tomo_autocent_cfg.json", "r"
 ) as f:
     xanes3d_tomo_autocent_cfg = json.load(f)
 
 with open(
     Path(__file__).parents[1] / "configs/xanes2d_image_autoreg_cfg.json", "r"
@@ -126,15 +132,15 @@
         ]
 
         self.label1 = widgets.Label(
             value="-------------------- Auto Cen & Align --------------------",
         )
         self.data_type = widgets.ComboBox(
             name="data type",
-            choices=["2D XANES", "3D XANES"],
+            choices=["3D XANES", "APS 3D XANES", "2D XANES", "APS 2D XANES"],
             value="3D XANES",
             enabled=True,
         )
         self.tomo_tplt_fn = widgets.FileEdit(
             mode="r",
             filter="*.json",
             name="xanes file",
@@ -242,33 +248,45 @@
         ids = check_file_availability(
             self._ref_rec_tplt["file_params"]["raw_data_top_dir"],
             scan_id=None,
             signature=self._tomo_cfg["tomo_raw_fn_template"],
             return_idx=True,
         )
         if ids:
-            _TOMO_XANES3D_REC_ID_S_CHOICES = ids
+            _TOMO_XANES3D_REC_ID_S_CHOICES = sorted(ids)
         else:
             _TOMO_XANES3D_REC_ID_S_CHOICES = []
         self.scan_id_s.reset_choices()
 
     def __3dxanes_tomo_check_avail_id_e(self):
         global _TOMO_XANES3D_REC_ID_E_CHOICES
         ids = check_file_availability(
             self._ref_rec_tplt["file_params"]["raw_data_top_dir"],
             scan_id=None,
             signature=self._tomo_cfg["tomo_raw_fn_template"],
             return_idx=True,
         )
         if ids:
-            _TOMO_XANES3D_REC_ID_E_CHOICES = ids
+            _TOMO_XANES3D_REC_ID_E_CHOICES = sorted(ids)
         else:
             _TOMO_XANES3D_REC_ID_E_CHOICES = []
         self.scan_id_e.reset_choices()
 
+    def _3dxanes_check_scan_id_s(self):
+        if int(self.scan_id_s.value) > int(self.ref_scan_id.value):
+            self.scan_id_s.value = self.ref_scan_id.value
+        self.__reset_run_states()
+        self.__reset_run_buttons()
+
+    def _3dxanes_check_scan_id_e(self):
+        if int(self.scan_id_e.value) < int(self.ref_scan_id.value):
+            self.scan_id_e.value = self.ref_scan_id.value
+        self.__reset_run_states()
+        self.__reset_run_buttons()
+
     def __3dxanes_tomo_if_new_rec(self):
         if (
             (self._tomo_tplt_fn_old_val != self.tomo_tplt_fn.value)
             or (self._scn_id_s_old_val != self.scan_id_s.value)
             or (self._scn_id_e_old_val != self.scan_id_e.value)
         ):
             self._3dxanes_new_rec_info = f"{xanes3d_tomo_autocent_cfg['aut_xns3d_pars']['scn_id_s']}-{xanes3d_tomo_autocent_cfg['aut_xns3d_pars']['scn_id_e']}_{datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S')}"
@@ -307,15 +325,15 @@
                 self.scan_id_e.value = self.scan_id_s.choices[-1]
         except:
             self.op_status.value = "There is no valid scan series available for XANES3D autocent operation!"
             print(
                 "There is no valid scan series available for XANES3D autocent operation!"
             )
 
-    def __3dxanes_set_widget(self):
+    def __3dxanes_set_widgets(self):
         if (self.rec_fntpl is None) or (
             not Path(
                 str(self.rec_fntpl).format(
                     self.ref_scan_id.value,
                     str(self.ref_sli.value).zfill(5),
                 )
             ).exists()
@@ -590,26 +608,14 @@
                 [
                     int(dim[0] / 4),
                     int(dim[0] * 3 / 4),
                 ],
                 dim[0] - 1,
             )
 
-    def _3dxanes_check_scan_id_s(self):
-        if int(self.scan_id_s.value) > int(self.ref_scan_id.value):
-            self.scan_id_s.value = self.ref_scan_id.value
-        self.__reset_run_states()
-        self.__reset_run_buttons()
-
-    def _3dxanes_check_scan_id_e(self):
-        if int(self.scan_id_e.value) < int(self.ref_scan_id.value):
-            self.scan_id_e.value = self.ref_scan_id.value
-        self.__reset_run_states()
-        self.__reset_run_buttons()
-
     def _3dxanes_tomo_auto_cen_dft_roi(self):
         if self.auto_cen_dft_roi.value:
             self.auto_cen_roix.enabled = False
             self.auto_cen_roiy.enabled = False
         else:
             self.auto_cen_roix.enabled = True
             self.auto_cen_roiy.enabled = True
@@ -623,78 +629,202 @@
         ):
             overlap_roi(self.viewer, self, mode="auto_cen")
         self.__reset_run_states()
         self.__reset_run_buttons()
 
     @disp_progress_info("xanes2d data loading")
     def __2dxanes_check_in_file(self):
-        if self._2dxanes_fn_p is None:
-            try:
+        if self.data_type.value == "2D XANES":
+            if self._2dxanes_fn_p is None:
+                try:
+                    self._2dxanes_fn_p = h5py.File(self._2dxanes_fn, "r")
+                except Exception as e:
+                    self._2dxanes_fn_p = None
+                    self.op_status.value = "Invalid data file!"
+                    print(e)
+            else:
+                self._2dxanes_fn_p.close()
                 self._2dxanes_fn_p = h5py.File(self._2dxanes_fn, "r")
-            except Exception as e:
-                self._2dxanes_fn_p = None
-                self.op_status.value = "Invalid data file!"
-                print(e)
-        else:
-            self._2dxanes_fn_p.close()
-            self._2dxanes_fn_p = h5py.File(self._2dxanes_fn, "r")
-        if (
-            (self._2dxanes_fn_p is not None)
-            and (self._2dxanes_fn_p["X_eng"].shape[0] > 1)
-            and len(self._2dxanes_fn_p["img_xanes"].shape) == 3
-            and self._2dxanes_fn_p["X_eng"].shape[0]
-            == self._2dxanes_fn_p["img_xanes"].shape[0]
-        ):
-            try:
-                self._2dxanes_eng_lst = self._2dxanes_fn_p["X_eng"][:]
-                dark = self._2dxanes_fn_p["img_dark"][:].squeeze()
-                flat = self._2dxanes_fn_p["img_bkg"][:].squeeze()
-                tem = -np.log(
-                    (da.from_array(self._2dxanes_fn_p["img_xanes"]) - dark)
-                    / (flat - dark)
-                )
-                tem[np.isinf(tem)] = 0
-                tem[np.isnan(tem)] = 0
-                self._2dxanes_data = tem.compute()
-                self.viewer.layers["xanes_raw_viewer"].data = self._2dxanes_data
-                self.viewer.layers["xanes_raw_viewer"].refresh()
-                self.viewer.reset_view()
-                self._2dxanes_data_ready = True
-            except Exception as e:
-                self.op_status.value = (
-                    "Something is wrong. Please check terminal for more information."
+            if (
+                (self._2dxanes_fn_p is not None)
+                and (
+                    self._2dxanes_fn_p[
+                        self._2dxanes_cfg["structured_h5_reader"]["eng_path"]
+                    ].shape[0]
+                    > 1
                 )
-                print(str(e))
-                self._2dxanes_fn_p.close()
+                and len(
+                    self._2dxanes_fn_p[
+                        self._2dxanes_cfg["structured_h5_reader"]["data_path"]
+                    ].shape
+                )
+                == 3
+                and self._2dxanes_fn_p[
+                    self._2dxanes_cfg["structured_h5_reader"]["eng_path"]
+                ].shape[0]
+                == self._2dxanes_fn_p[
+                    self._2dxanes_cfg["structured_h5_reader"]["data_path"]
+                ].shape[0]
+            ):
+                try:
+                    self._2dxanes_eng_lst = self._2dxanes_fn_p[
+                        self._2dxanes_cfg["structured_h5_reader"]["eng_path"]
+                    ][:]
+                    dark = self._2dxanes_fn_p[
+                        self._2dxanes_cfg["structured_h5_reader"]["dark_path"]
+                    ][:].squeeze()
+                    flat = self._2dxanes_fn_p[
+                        self._2dxanes_cfg["structured_h5_reader"]["flat_path"]
+                    ][:].squeeze()
+                    tem = -np.log(
+                        (
+                            da.from_array(
+                                self._2dxanes_fn_p[
+                                    self._2dxanes_cfg["structured_h5_reader"][
+                                        "data_path"
+                                    ]
+                                ]
+                            )
+                            - dark
+                        )
+                        / (flat - dark)
+                    )
+                    tem[np.isinf(tem)] = 0
+                    tem[np.isnan(tem)] = 0
+                    self._2dxanes_data = tem.compute()
+                    update_layer_in_viewer(
+                        self.viewer,
+                        self._2dxanes_data,
+                        "xanes_raw_viewer",
+                    )
+                    # self.viewer.layers["xanes_raw_viewer"].data = self._2dxanes_data
+                    # self.viewer.layers["xanes_raw_viewer"].refresh()
+                    self.viewer.reset_view()
+                    self._2dxanes_data_ready = True
+                except Exception as e:
+                    self.op_status.value = "Something is wrong. Please check terminal for more information."
+                    print(str(e))
+                    self._2dxanes_fn_p.close()
+                    self._2dxanes_fn_p = None
+                    self._2dxanes_data = None
+                    self._2dxanes_eng_lst = None
+                    self._2dxanes_fn = None
+                    self._2dxanes_data_ready = False
+            else:
+                self._2dxanes_fn_p = None
+                self._2dxanes_data = None
+                self._2dxanes_eng_lst = None
+                self._2dxanes_fn = None
+                self._2dxanes_data_ready = False
+        elif self.data_type.value == "APS 2D XANES":
+            top_dir = self._2dxanes_fn.parent
+            fn_tplt = self._2dxanes_fn.stem.rsplit("_", maxsplit=1)[0]
+            _cfg = deepcopy(APS_TXM_CFG)
+            self._2dxanes_cfg = mk_aps_cfg(
+                fn_tplt,
+                _cfg,
+                dtype="APS 2D XANES",
+            )["io_data_structure_xanes2D"]
+            ids = check_file_availability(
+                top_dir,
+                scan_id=None,
+                signature=self._2dxanes_cfg["xanes2D_raw_fn_template"],
+                return_idx=True,
+            )
+            if ids:
+                ids = sorted(ids)
+                try:
+                    eng_lst = []
+                    data = []
+                    for ii in ids:
+                        with h5py.File(
+                            top_dir
+                            / self._2dxanes_cfg["xanes2D_raw_fn_template"].format(ii),
+                            "r",
+                        ) as f:
+                            if f[
+                                self._2dxanes_cfg["structured_h5_reader"][
+                                    "io_data_structure"
+                                ]["eng_path"]
+                            ].shape:
+                                eng = f[
+                                    self._2dxanes_cfg["structured_h5_reader"][
+                                        "io_data_structure"
+                                    ]["eng_path"]
+                                ][()][0]
+                            else:
+                                eng = f[
+                                    self._2dxanes_cfg["structured_h5_reader"][
+                                        "io_data_structure"
+                                    ]["eng_path"]
+                                ][()]
+                            eng_lst.append(eng)
+                            dark = f[
+                                self._2dxanes_cfg["structured_h5_reader"][
+                                    "io_data_structure"
+                                ]["dark_path"]
+                            ][0].squeeze()
+                            flat = f[
+                                self._2dxanes_cfg["structured_h5_reader"][
+                                    "io_data_structure"
+                                ]["flat_path"]
+                            ][0].squeeze()
+                            tem = -np.log(
+                                (
+                                    f[
+                                        self._2dxanes_cfg["structured_h5_reader"][
+                                            "io_data_structure"
+                                        ]["data_path"]
+                                    ][0]
+                                    - dark
+                                )
+                                / (flat - dark)
+                            )
+                            tem[np.isinf(tem)] = 0
+                            tem[np.isnan(tem)] = 0
+                            data.append(tem)
+                    self._2dxanes_eng_lst = np.array(eng_lst)
+                    self._2dxanes_data = np.array(data)
+                    update_layer_in_viewer(
+                        self.viewer,
+                        self._2dxanes_data,
+                        "xanes_raw_viewer",
+                    )
+                    self.viewer.reset_view()
+                    self._2dxanes_data_ready = True
+                except Exception as e:
+                    self.op_status.value = "Something is wrong. Please check terminal for more information."
+                    print(str(e))
+                    self._2dxanes_data = None
+                    self._2dxanes_eng_lst = None
+                    self._2dxanes_fn = None
+                    self._2dxanes_cfg = APS_TXM_CFG["io_data_structure_xanes2D"]
+                    self._2dxanes_data_ready = False
+            else:
                 self._2dxanes_fn_p = None
                 self._2dxanes_data = None
                 self._2dxanes_eng_lst = None
                 self._2dxanes_fn = None
                 self._2dxanes_data_ready = False
-        else:
-            self._2dxanes_fn_p = None
-            self._2dxanes_data = None
-            self._2dxanes_eng_lst = None
-            self._2dxanes_fn = None
-            self._2dxanes_data_ready = False
         self._test_run_done = False
         self._continue_run_confirmed = False
 
-    def __2dxanes_set_widget(self):
+    def __2dxanes_set_widgets(self):
         if self._2dxanes_data_ready:
             self.scan_id_s.enabled = False
             self.scan_id_e.enabled = False
             self.auto_cen_dft_roi.enabled = False
             self.auto_cen_dft_roi.value = False
-            self.auto_cen_roix.enabled = True
-            self.auto_cen_roiy.enabled = True
-            self.ref_sli.enabled = True
-            self.rec_roix.enabled = True
-            self.rec_roiy.enabled = True
-            self.rec_roiz.enabled = True
+            # self.auto_cen_roix.enabled = True
+            # self.auto_cen_roiy.enabled = True
+            # self.ref_sli.enabled = True
+            # self.rec_roix.enabled = True
+            # self.rec_roiy.enabled = True
+            # self.rec_roiz.enabled = True
+            self.__2dxanes_set_roi_widgets()
             self.sli_srch_range.enabled = False
             self.cen_srch_range.enabled = False
             self.ang_corr.enabled = False
             self.ang_corr_range.enabled = False
             self.test_run.enabled = True
             if self._test_run_done:
                 self.confirm_test_run.enabled = True
@@ -784,16 +914,31 @@
                     self.op_status.value = "Something is wrong. Please check terminal for more information."
                     print(str(e))
                     sta = False
         if sta:
             self._2dxanes_reg_roiz_old_val = self.rec_roiz.value
             self.viewer.reset_view()
 
+    def __2dxanes_set_roi_widgets(self):
+        if not self._continue_run_confirmed:
+            self.auto_cen_roix.enabled = True
+            self.auto_cen_roiy.enabled = True
+            self.ref_sli.enabled = True
+            self.rec_roiz.enabled = True
+            self.rec_roix.enabled = False
+            self.rec_roiy.enabled = False
+        else:
+            self.auto_cen_roix.enabled = False
+            self.auto_cen_roiy.enabled = False
+            self.ref_sli.enabled = False
+            self.rec_roiz.enabled = False
+            self.rec_roix.enabled = True
+            self.rec_roiy.enabled = True
+
     def __2dxanes_set_roi_lims(self):
-        # if self._2dxanes_data_ready:
         dim = self._2dxanes_data.shape
         set_data_widget(
             self.ref_sli,
             0,
             int(dim[0] / 2),
             dim[0] - 1,
         )
@@ -857,14 +1002,52 @@
             )
             self._tomo_tplt_fn_old_val = self.tomo_tplt_fn.value
             self._2dxanes_reg_roix_old_val = self.auto_cen_roix.value
             self._2dxanes_reg_roiy_old_val = self.auto_cen_roiy.value
             self._2dxanes_reg_ref_im_old_val = self.ref_sli.value
         else:
             self._2dxanes_if_new_reg = False
+        # if "2D XANES" == self.data_type.value:
+        #     if (
+        #         (self._tomo_tplt_fn_old_val != self.tomo_tplt_fn.value)
+        #         or (self._2dxanes_reg_roix_old_val != self.auto_cen_roix.value)
+        #         or (self._2dxanes_reg_roiy_old_val != self.auto_cen_roiy.value)
+        #         or (self._2dxanes_reg_ref_im_old_val != self.ref_sli.value)
+        #     ):
+        #         self._2dxanes_if_new_reg = True
+        #         self._2dxanes_new_reg_info = (
+        #             f"{datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S')}"
+        #         )
+        #         self._tomo_tplt_fn_old_val = self.tomo_tplt_fn.value
+        #         self._2dxanes_reg_roix_old_val = self.auto_cen_roix.value
+        #         self._2dxanes_reg_roiy_old_val = self.auto_cen_roiy.value
+        #         self._2dxanes_reg_ref_im_old_val = self.ref_sli.value
+        #     else:
+        #         self._2dxanes_if_new_reg = False
+        # elif "APS 2D XANES" == self.data_type.value:
+        #     if (
+        #         (self._tomo_tplt_fn_old_val != self.tomo_tplt_fn.value)
+        #         or (self._2dxanes_reg_roix_old_val != self.auto_cen_roix.value)
+        #         or (self._2dxanes_reg_roiy_old_val != self.auto_cen_roiy.value)
+        #         or (self._2dxanes_reg_ref_im_old_val != self.ref_sli.value)
+        #         or (self._scn_id_s_old_val != self.scan_id_s.value)
+        #         or (self._scn_id_e_old_val != self.scan_id_e.value)
+        #     ):
+        #         self._2dxanes_if_new_reg = True
+        #         self._2dxanes_new_reg_info = (
+        #             f"{datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S')}"
+        #         )
+        #         self._tomo_tplt_fn_old_val = self.tomo_tplt_fn.value
+        #         self._2dxanes_reg_roix_old_val = self.auto_cen_roix.value
+        #         self._2dxanes_reg_roiy_old_val = self.auto_cen_roiy.value
+        #         self._2dxanes_reg_ref_im_old_val = self.ref_sli.value
+        #         self._scn_id_s_old_val = self.scan_id_s.value
+        #         self._scn_id_e_old_val = self.scan_id_e.value
+        #     else:
+        #         self._2dxanes_if_new_reg = False
 
     def __2dxanes_check_if_new_align(self):
         if (
             (self._2dxanes_align_roix_old_val != self.rec_roix.value)
             or (self._2dxanes_align_roiy_old_val != self.rec_roiy.value)
             or (self._2dxanes_align_roiz_old_val != self.rec_roiz.value)
         ):
@@ -948,15 +1131,20 @@
         )
         set_data_widget(
             self.auto_cen_roiy,
             1,
             [540, 740],
             1280,
         )
-        self.ref_sli.value = 540
+        set_data_widget(
+            self.ref_sli,
+            1,
+            540,
+            1080,
+        )
         set_data_widget(
             self.rec_roix,
             1,
             [540, 740],
             1280,
         )
         set_data_widget(
@@ -979,14 +1167,15 @@
 
     def __reset_run_states(self):
         self._test_run_done = False
         self.confirm_test_run.value == "No"
         self._continue_run_confirmed = False
 
     def __reset_run_buttons(self):
+        self.test_run.enabled = True
         if self._test_run_done:
             self.confirm_test_run.enabled = True
         else:
             self.confirm_test_run.enabled = False
             self.confirm_test_run.value == "No"
             self._continue_run_confirmed = False
         if self._continue_run_confirmed:
@@ -1004,28 +1193,29 @@
         self._2dxanes_fn = None
         if self._2dxanes_reg_fn_p is not None:
             self._2dxanes_reg_fn_p.close()
             self._2dxanes_reg_fn_p = None
         self._2dxanes_reg_fn = None
 
     def _sel_in_data_type(self):
+        self._close_file()
         self.__reset_data_states()
         self.__reset_widgets_val()
-        if self.data_type.value == "3D XANES":
+        if "3D XANES" in self.data_type.value:
             self.tomo_tplt_fn.filter = "*.json"
-            self.__3dxanes_set_widget()
+            self.__3dxanes_set_widgets()
         else:
             self.tomo_tplt_fn.filter = "*.h5"
-            self.__2dxanes_set_widget()
+            self.__2dxanes_set_widgets()
         self.__reset_run_states()
         self.__reset_run_buttons()
-        self._close_file()
 
     @disp_progress_info("data directory info read")
     def _xanes_set_fn(self):
+        self._close_file()
         self.__reset_data_states()
         self.__reset_widgets_val()
         if self.data_type.value == "3D XANES":
             self._tomo_tplt_fn = self.tomo_tplt_fn.value
             cfg_type = check_cfg_type(self._tomo_tplt_fn)
             if cfg_type == "xanes3d_tomo_tplt":
                 with open(self._tomo_tplt_fn, "r") as f:
@@ -1046,15 +1236,15 @@
                     ]
                 ):
                     self._tomo_cfg = FLY_CFG["io_data_structure_xanes3D"]
                 self.__3dxanes_comp_tomo_fntpl()
                 self.__3dxanes_tomo_check_avail_id_s()
                 self.__3dxanes_tomo_check_avail_id_e()
                 self.__3dxanes_set_scan_id_lims()
-                self.__3dxanes_set_widget()
+                self.__3dxanes_set_widgets()
                 self.__3dxanes_set_roi_lims()
                 if (self.rec_fntpl is None) or (
                     not Path(
                         str(self.rec_fntpl).format(
                             self.ref_scan_id.value,
                             str(self.ref_sli.value).zfill(5),
                         )
@@ -1064,18 +1254,81 @@
             else:
                 self.op_status.value = (
                     "wrong type of json cfg file. check error message in terminal"
                 )
                 print(
                     "The required json file should have file name starting with 'xanes3d_tomo_tplt_cfg'."
                 )
-        else:
+        elif self.data_type.value == "APS 3D XANES":
+            _cfg = deepcopy(APS_TXM_CFG)
+            self._tomo_tplt_fn = self.tomo_tplt_fn.value
+            cfg_type = check_cfg_type(self._tomo_tplt_fn)
+            if cfg_type == "xanes3d_tomo_tplt":
+                with open(self._tomo_tplt_fn, "r") as f:
+                    tem = json.load(f)
+                    self.ref_scan_id.value = list(tem.keys())[0]
+                    self._ref_rec_tplt = tem[list(tem.keys())[0]]
+                fn_tplt = Path(
+                    tem[list(tem.keys())[0]]["file_params"]["io_confg"][
+                        "tomo_raw_fn_template"
+                    ]
+                ).stem.rsplit("_", maxsplit=1)[0]
+                self._tomo_cfg = mk_aps_cfg(fn_tplt, _cfg, dtype="APS 3D XANES")[
+                    "io_data_structure_xanes3D"
+                ]
+                self.__3dxanes_comp_tomo_fntpl()
+                self.__3dxanes_tomo_check_avail_id_s()
+                self.__3dxanes_tomo_check_avail_id_e()
+                self.__3dxanes_set_scan_id_lims()
+                self.__3dxanes_set_widgets()
+                self.__3dxanes_set_roi_lims()
+                if (self.rec_fntpl is None) or (
+                    not Path(
+                        str(self.rec_fntpl).format(
+                            self.ref_scan_id.value,
+                            str(self.ref_sli.value).zfill(5),
+                        )
+                    ).exists()
+                ):
+                    self.__3dxanes_tomo_show_sli(mode="auto_cen")
+            else:
+                self.op_status.value = (
+                    "wrong type of json cfg file. check error message in terminal"
+                )
+                print(
+                    "The required json file should have file name starting with 'xanes3d_tomo_tplt_cfg'."
+                )
+        elif self.data_type.value == "2D XANES":
+            self._2dxanes_cfg = ZFLY_CFG["io_data_structure_xanes2D"]
             self._2dxanes_fn = self.tomo_tplt_fn.value
             self.__2dxanes_check_in_file()
-            self.__2dxanes_set_widget()
+            self.__2dxanes_set_widgets()
+            if self._2dxanes_data_ready:
+                self.__2dxanes_set_roi_lims()
+                self.__2dxanes_show_sli(mode="auto_reg")
+                _min = (
+                    self.viewer.layers["xanes_raw_viewer"]
+                    .data[self.ref_sli.value]
+                    .min()
+                )
+                _max = (
+                    self.viewer.layers["xanes_raw_viewer"]
+                    .data[self.ref_sli.value]
+                    .max()
+                )
+                rng = _max - _min
+                self.viewer.layers["xanes_raw_viewer"].contrast_limits = [
+                    _min + 0.1 * rng,
+                    _max - 0.1 * rng,
+                ]
+        elif self.data_type.value == "APS 2D XANES":
+            self._2dxanes_cfg = APS_TXM_CFG["io_data_structure_xanes2D"]
+            self._2dxanes_fn = self.tomo_tplt_fn.value
+            self.__2dxanes_check_in_file()
+            self.__2dxanes_set_widgets()
             if self._2dxanes_data_ready:
                 self.__2dxanes_set_roi_lims()
                 self.__2dxanes_show_sli(mode="auto_reg")
                 _min = (
                     self.viewer.layers["xanes_raw_viewer"]
                     .data[self.ref_sli.value]
                     .min()
@@ -1090,15 +1343,15 @@
                     _min + 0.1 * rng,
                     _max - 0.1 * rng,
                 ]
         self.__reset_run_states()
         self.__reset_run_buttons()
 
     def _xanes_tomo_auto_cen_roix(self):
-        if self.data_type.value == "3D XANES":
+        if "3D XANES" in self.data_type.value:
             if (self.rec_fntpl is not None) and (
                 Path(
                     str(self.rec_fntpl).format(
                         self.ref_scan_id.value,
                         str(self.ref_sli.value).zfill(5),
                     )
                 ).exists()
@@ -1109,15 +1362,15 @@
             if self._2dxanes_data_ready:
                 overlap_roi(self.viewer, self, mode="auto_cen")
                 show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
         self.__reset_run_states()
         self.__reset_run_buttons()
 
     def _xanes_tomo_auto_cen_roiy(self):
-        if self.data_type.value == "3D XANES":
+        if "3D XANES" in self.data_type.value:
             if (self.rec_fntpl is not None) and (
                 Path(
                     str(self.rec_fntpl).format(
                         self.ref_scan_id.value,
                         str(self.ref_sli.value).zfill(5),
                     )
                 ).exists()
@@ -1128,15 +1381,15 @@
             if self._2dxanes_data_ready:
                 overlap_roi(self.viewer, self, mode="auto_cen")
                 show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
         self.__reset_run_states()
         self.__reset_run_buttons()
 
     def _xanes_tomo_auto_cen_ref_sli(self):
-        if self.data_type.value == "3D XANES":
+        if "3D XANES" in self.data_type.value:
             if (self.rec_fntpl is not None) and (
                 Path(
                     str(self.rec_fntpl).format(
                         self.ref_scan_id.value,
                         str(self.ref_sli.value).zfill(5),
                     )
                 ).exists()
@@ -1149,51 +1402,51 @@
                 self.__2dxanes_show_sli(mode="auto_reg")
                 overlap_roi(self.viewer, self, mode="auto_cen")
                 show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
         self.__reset_run_states()
         self.__reset_run_buttons()
 
     def _xanes_tomo_rec_roix(self):
-        if self.data_type.value == "3D XANES":
+        if "3D XANES" in self.data_type.value:
             if (self.rec_fntpl is not None) and (
                 Path(
                     str(self.rec_fntpl).format(
                         self.ref_scan_id.value,
                         str(self.ref_sli.value).zfill(5),
                     )
                 ).exists()
             ):
                 overlap_roi(self.viewer, self, mode="recon_roi")
                 show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
         else:
             if self._2dxanes_data_ready:
                 overlap_roi(self.viewer, self, mode="recon_roi")
                 show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
-            self.confirm_test_run.value = "No"
+            # self.confirm_test_run.value = "No"
 
     def _xanes_tomo_rec_roiy(self):
-        if self.data_type.value == "3D XANES":
+        if "3D XANES" in self.data_type.value:
             if (self.rec_fntpl is not None) and (
                 Path(
                     str(self.rec_fntpl).format(
                         self.ref_scan_id.value,
                         str(self.ref_sli.value).zfill(5),
                     )
                 ).exists()
             ):
                 overlap_roi(self.viewer, self, mode="recon_roi")
                 show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
         else:
             if self._2dxanes_data_ready:
                 overlap_roi(self.viewer, self, mode="recon_roi")
                 show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
-            self.confirm_test_run.value = "No"
+            # self.confirm_test_run.value = "No"
 
     def _xanes_tomo_rec_roiz(self):
-        if self.data_type.value == "3D XANES":
+        if "3D XANES" in self.data_type.value:
             if self.rec_roiz.value[0] > (
                 self.ref_sli.value - self.sli_srch_range.value
             ):
                 self.rec_roiz.value = [
                     self.ref_sli.value - self.sli_srch_range.value,
                     self.rec_roiz.value[1],
                 ]
@@ -1220,15 +1473,16 @@
                 self.__2dxanes_show_sli(mode="auto_algn")
                 overlap_roi(self.viewer, self, mode="recon_roi")
                 show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
             self.confirm_test_run.value = "No"
 
     @disp_progress_info("xanes auto registration test run")
     def _xanes_test_run(self):
-        if self.data_type.value == "3D XANES":
+        if "3D XANES" in self.data_type.value:
+            self.__reset_run_states()
             self.__3dxanes_tomo_if_new_rec()
             self.__3dxnaes_tomo_def_autocent_cfg()
 
             sig = os.system(f"ipython {xanes3d_auto_cen_reg_script_fn}")
             print(f"{sig=}")
 
             if sig == 0:
@@ -1244,29 +1498,32 @@
                         trial_imgs.append(
                             f[f"/auto_centering/{key}/optimization itr 1/trial_rec"][:]
                         )
                 update_layer_in_viewer(
                     self.viewer, np.array(trial_imgs), "autocent_check"
                 )
                 show_layers_in_viewer(self.viewer, ["autocent_check"])
-            if sig == 0:
                 self._test_run_done = True
             else:
                 self._test_run_done = False
                 self.op_status.value = "auto centering fails"
                 print("auto centering fails")
             self.confirm_test_run.value == "No"
             self._continue_run_confirmed = False
             self.__reset_run_buttons()
-        else:
+        elif "2D XANES" in self.data_type.value:
+            self.__reset_run_states()
             self.__2dxanes_check_if_new_reg()
             self.__2dxanes_def_img_autoreg_cfg()
 
             if self._2dxanes_if_new_reg:
-                sig = os.system(f"ipython {xanes2d_img_auto_cen_script_fn}")
+                if self.data_type.value == "2D XANES":
+                    sig = os.system(f"ipython {xanes2d_img_auto_cen_script_fn}")
+                elif self.data_type.value == "APS 2D XANES":
+                    sig = os.system(f"ipython {aps_xanes2d_img_auto_cen_script_fn}")
 
                 if sig == 0:
                     with open(cfg_fn, "r") as f:
                         tem = json.load(f)
                     with open(tem["xanes2d_reg"]["cfg_file"], "r") as f:
                         tem = json.load(f)
                     if self._2dxanes_reg_fn_p is None:
@@ -1285,44 +1542,49 @@
                     self._test_run_done = True
                 else:
                     self._test_run_done = False
                     self.op_status.value = "auto alignment fails"
                     print("auto alignment fails")
                 self.confirm_test_run.value == "No"
                 self._continue_run_confirmed = False
+                self.__2dxanes_set_roi_widgets()
                 self.__reset_run_buttons()
             else:
                 self.op_status.value = "Nothing is changed from last auto-registration."
                 print("Nothing is changed from last auto-registration.")
 
     def _xanes_confirm_to_run(self):
         if self.confirm_test_run.value == "Yes":
             self._continue_run_confirmed = True
-            if self.data_type.value == "3D XANES":
+            if "3D XANES" in self.data_type.value:
                 self.reg_run.enabled = True
             else:
+                self.__2dxanes_set_roi_widgets()
                 if (self.auto_cen_roix.value == self.rec_roix.value) and (
                     self.auto_cen_roiy.value == self.rec_roiy.value
                 ):
                     self.reg_run.enabled = False
                     self.op_status.value = (
                         "2D XANES registration is done! Nothing is left in this page."
                     )
                     print(
                         "2D XANES registration is done! Nothing is left in this page."
                     )
                 else:
                     self.reg_run.enabled = True
         else:
             self._continue_run_confirmed = False
-            self.reg_run.enabled = False
+            if "3D XANES" in self.data_type.value:
+                self.reg_run.enabled = False
+            else:
+                self.__2dxanes_set_roi_widgets()
 
     @disp_progress_info("xanes auto registration")
     def _xanes_reg_run(self):
-        if self.data_type.value == "3D XANES":
+        if "3D XANES" in self.data_type.value:
             self.__3dxanes_tomo_if_new_rec()
             self.__3dxnaes_tomo_def_autocent_cfg()
 
             sig = os.system(f"ipython {xanes3d_auto_cen_reg_script_fn}")
             if sig == 0:
                 self.op_status.value = "autocen and registration are finished. please check the results in 'XANES Analysis'."
                 print(
@@ -1331,24 +1593,27 @@
             else:
                 self.op_status.value = (
                     "something went wrong during autocen or registration processes."
                 )
                 print("something went wrong during autocen or registration processes.")
                 self.reg_run.enabled = False
         else:
-            self.__2dxanes_check_if_new_reg()
+            # self.__2dxanes_check_if_new_reg()
             self.__2dxanes_def_img_autoreg_cfg()
             self.__2dxanes_check_if_new_align()
 
             if self._2dxanes_if_new_align:
                 rm_gui_viewers(self.viewer, ["autocent_check"])
                 if self._2dxanes_reg_fn_p is not None:
                     self._2dxanes_reg_fn_p.close()
 
-                sig = os.system(f"ipython {xanes2d_img_auto_cen_script_fn}")
+                if self.data_type.value == "2D XANES":
+                    sig = os.system(f"ipython {xanes2d_img_auto_cen_script_fn}")
+                elif self.data_type.value == "APS 2D XANES":
+                    sig = os.system(f"ipython {aps_xanes2d_img_auto_cen_script_fn}")
 
                 if sig == 0:
                     with open(cfg_fn, "r") as f:
                         tem = json.load(f)
                     with open(tem["xanes2d_reg"]["cfg_file"], "r") as f:
                         tem = json.load(f)
                     if self._2dxanes_reg_fn_p is None:
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/guis/xanes_vis_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from txm_sandbox.utils.tomo_recon_tools import run_engine
 from txm_sandbox.utils.io import data_reader, tomo_h5_reader, data_info, tomo_h5_info
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
 
 with open(cfg_fn, "r") as f:
-    with open(json.load(f)["tomo_batch_recon"]["cfg_file"], "r") as ft:
+    with open(json.load(f)["tomo_recon"]["cfg_file"], "r") as ft:
         tem = json.load(ft)
 
 params = tem[list(tem.keys())[0]]
 params["file_params"]["reader"] = data_reader(tomo_h5_reader)
 params["file_params"]["info_reader"] = data_info(tomo_h5_info)
 
 if __name__ == "__main__":
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from txm_sandbox.utils.tomo_recon_tools import run_engine
 from txm_sandbox.utils.io import data_reader, tomo_h5_reader, data_info, tomo_h5_info
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
 
 with open(cfg_fn, "r") as f:
-    with open(json.load(f)["tomo_recon"]["cfg_file"], "r") as ft:
+    with open(json.load(f)["tomo_batch_recon"]["cfg_file"], "r") as ft:
         tem = json.load(ft)
 
 params = tem[list(tem.keys())[0]]
 params["file_params"]["reader"] = data_reader(tomo_h5_reader)
 params["file_params"]["info_reader"] = data_info(tomo_h5_info)
 
 if __name__ == "__main__":
-    run_engine(**params)
+    for scn_id in list(tem.keys()):
+        run_engine(**tem[scn_id])
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 import dask.array as da
 
 from txm_sandbox.utils import xanes_regtools as xr
 
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
-with open(cfg_fn, "r") as f:
-    with open(json.load(f)["xanes2d_reg"]["cfg_file"], "r") as ft:
-        reg_cfg = json.load(ft)
 
 if __name__ == "__main__":
+    with open(cfg_fn, "r") as f:
+        with open(json.load(f)["xanes2d_reg"]["cfg_file"], "r") as ft:
+            reg_cfg = json.load(ft)
+
     freeze_support()
     reg = xr.regtools(reg_cfg)
     with h5py.File(reg_cfg["file"]["XANES2D_raw_fn"], "r") as f:
         reg.eng_lst = f["X_eng"][
             reg_cfg["data"]["im_id_s"] : reg_cfg["data"]["im_id_e"]
         ]
         dark = da.from_array(f["img_dark"][:]).squeeze()
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/txm_gui.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/txm_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/utils/io.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/napari_gui/utils/misc.py` & `txm_sandbox-0.3.1/txm_sandbox/napari_gui/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/io.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/lineshapes.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/lineshapes.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/misc.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/plotlib.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/plotlib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/reg_algs.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/reg_algs.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/tomo_recon_tools.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/tomo_recon_tools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_analysis.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_image_utils.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_image_utils.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_math.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_math.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_post_analysis.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_post_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_regtools.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_regtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         self.use_chunk = reg_cfg["reg"]["use_chnk"]
         self.chunk_sz = reg_cfg["reg"]["chnk_sz"]
         self.xanes3D_sli_srch_half_range = reg_cfg["reg"]["XANES3D_sli_srch_half_range"]
         self.xanes3D_fixed_ref_sli = reg_cfg["reg"]["XANES3D_fixed_ref_sli"]
 
         self.im_id_s = reg_cfg["data"]["im_id_s"]
         self.im_id_e = reg_cfg["data"]["im_id_e"]
-        print(f"{self.im_id_e=}")
         self.im_id_fxd = reg_cfg["data"]["im_id_fixed"]
         self.xanes3D_scn_ids = list(reg_cfg["data"]["XANES3D_scn_ids"])
         self.im_roi = reg_cfg["data"]["roi"]
 
         self.xanes3D_rec_path_tplt = reg_cfg["file"]["XANES3D_rec_path_tplt"]
         self.xanes3D_raw_h5_top_dir = reg_cfg["file"]["XANES3D_raw_h5_top_dir"]
         self.xanes2D_raw_fn = reg_cfg["file"]["XANES2D_raw_fn"]
@@ -121,16 +120,20 @@
 
         self.eng_list = reg_cfg["meta"]["eng_list"]
 
         if self.data_type == "3D_XANES":
             self.anchor_loc = self.xanes3D_scn_ids.index(self.im_id_fxd)
             self.data_pnts = len(self.xanes3D_scn_ids)
         else:
-            self.anchor_loc = self.im_id_fxd - self.im_id_s
-            self.data_pnts = self.im_id_e - self.im_id_s
+            self.anchor_loc = self.xanes3D_scn_ids.index(
+                self.im_id_fxd
+            ) - self.xanes3D_scn_ids.index(self.im_id_s)
+            self.data_pnts = self.xanes3D_scn_ids.index(
+                self.im_id_e
+            ) - self.xanes3D_scn_ids.index(self.im_id_s)
         self.sav_dir = str(Path(self.sav_fn).parent)
         self.ref_im = None
         self.im = None
         self.msk = None
         self.eng_dict = {}
         self.im_ids_dict = {}
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox/utils/xanes_spectra_filters.py` & `txm_sandbox-0.3.1/txm_sandbox/utils/xanes_spectra_filters.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox.egg-info/PKG-INFO` & `txm_sandbox-0.3.1/txm_sandbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.0.post7
+Version: 0.3.1
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.0.post7/txm_sandbox.egg-info/SOURCES.txt` & `txm_sandbox-0.3.1/txm_sandbox.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -44,27 +44,30 @@
 txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
 txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
 txm_sandbox/napari_gui/dicts/__init__.py
 txm_sandbox/napari_gui/dicts/data_struct_dict.py
 txm_sandbox/napari_gui/guis/__init__.py
 txm_sandbox/napari_gui/guis/appl_mask_gui.py
 txm_sandbox/napari_gui/guis/convert_data_gui.py
+txm_sandbox/napari_gui/guis/extra_io_gui.py
 txm_sandbox/napari_gui/guis/tomo_gui.py
 txm_sandbox/napari_gui/guis/xanes_fit_gui.py
 txm_sandbox/napari_gui/guis/xanes_reg_gui.py
 txm_sandbox/napari_gui/guis/xanes_vis_gui.py
 txm_sandbox/napari_gui/scripts/__init__.py
+txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py
 txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
 txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
 txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
 txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
 txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
 txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
 txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
 txm_sandbox/napari_gui/utils/__init__.py
+txm_sandbox/napari_gui/utils/ext_io_lib.py
 txm_sandbox/napari_gui/utils/io.py
 txm_sandbox/napari_gui/utils/misc.py
 txm_sandbox/tmp/__init__.py
 txm_sandbox/tmp/readme.txt
 txm_sandbox/utils/__init__.py
 txm_sandbox/utils/io.py
 txm_sandbox/utils/lineshapes.py
```

