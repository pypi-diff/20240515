# Comparing `tmp/lycoris_lora-2.3.0.dev8.tar.gz` & `tmp/lycoris_lora-2.3.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-2.3.0.dev8.tar", last modified: Fri May  3 13:52:32 2024, max compression
+gzip compressed data, was "lycoris_lora-2.3.0.dev9.tar", last modified: Fri May  3 14:52:43 2024, max compression
```

## Comparing `lycoris_lora-2.3.0.dev8.tar` & `lycoris_lora-2.3.0.dev9.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.630822 lycoris_lora-2.3.0.dev8/
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-2.3.0.dev8/LICENSE.md
--rw-rw-rw-   0        0        0      527 2024-05-03 13:52:32.630822 lycoris_lora-2.3.0.dev8/PKG-INFO
--rw-rw-rw-   0        0        0    11988 2024-03-15 08:57:27.000000 lycoris_lora-2.3.0.dev8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.603990 lycoris_lora-2.3.0.dev8/lycoris/
--rw-rw-rw-   0        0        0      550 2024-02-05 11:33:28.000000 lycoris_lora-2.3.0.dev8/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.605990 lycoris_lora-2.3.0.dev8/lycoris/hcp/
--rw-rw-rw-   0        0        0      156 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/__init__.py
--rw-rw-rw-   0        0        0     5329 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/base.py
--rw-rw-rw-   0        0        0     2281 2024-02-12 10:32:01.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/diag_oft.py
--rw-rw-rw-   0        0        0     3391 2024-03-04 15:01:10.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/loha.py
--rw-rw-rw-   0        0        0     5643 2024-03-04 15:01:21.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/lokr.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.610507 lycoris_lora-2.3.0.dev8/lycoris/kohya/
--rw-rw-rw-   0        0        0    31784 2024-04-08 09:27:28.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    59991 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/model_utils.py
--rw-rw-rw-   0        0        0    61070 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/original_unet.py
--rw-rw-rw-   0        0        0    21297 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/sdxl_model_util.py
--rw-rw-rw-   0        0        0    42690 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/sdxl_original_unet.py
--rw-rw-rw-   0        0        0    19901 2024-03-11 06:16:36.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/test_hyperdream.py
--rw-rw-rw-   0        0        0     1514 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/utils.py
--rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-2.3.0.dev8/lycoris/logging.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.616511 lycoris_lora-2.3.0.dev8/lycoris/modules/
--rw-rw-rw-   0        0        0     4201 2024-05-03 13:52:01.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     8185 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/attention.py
--rw-rw-rw-   0        0        0     7015 2024-05-03 13:35:33.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/base.py
--rw-rw-rw-   0        0        0     7430 2024-05-03 13:35:44.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/boft.py
--rw-rw-rw-   0        0        0     6159 2024-05-03 13:36:17.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/diag_oft.py
--rw-rw-rw-   0        0        0     4395 2024-05-03 12:40:31.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0     4518 2024-05-03 13:36:02.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/full.py
--rw-rw-rw-   0        0        0    11788 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/glokr.py
--rw-rw-rw-   0        0        0     4978 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/glora.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.617511 lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/
--rw-rw-rw-   0        0        0       79 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/__init__.py
--rw-rw-rw-   0        0        0     8302 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/generater.py
--rw-rw-rw-   0        0        0     8339 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/text_encoder.py
--rw-rw-rw-   0        0        0     2078 2024-03-11 06:14:46.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    12663 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/lilora.py
--rw-rw-rw-   0        0        0    10526 2024-05-03 13:36:50.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    12851 2024-05-03 13:35:27.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    17858 2024-05-03 13:35:20.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0     2387 2024-05-03 13:35:13.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/norms.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.619014 lycoris_lora-2.3.0.dev8/lycoris/utils/
--rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/bnb.py
--rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/logger.py
--rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      196 2024-03-16 16:01:30.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/tensor_norm.py
--rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/xformers_utils.py
--rw-rw-rw-   0        0        0    18706 2024-03-16 16:01:01.000000 lycoris_lora-2.3.0.dev8/lycoris/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.629822 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      527 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       53 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 13:52:32.630822 lycoris_lora-2.3.0.dev8/setup.cfg
--rw-rw-rw-   0        0        0      638 2024-05-03 13:52:25.000000 lycoris_lora-2.3.0.dev8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.762148 lycoris_lora-2.3.0.dev9/
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-2.3.0.dev9/LICENSE.md
+-rw-rw-rw-   0        0        0      527 2024-05-03 14:52:43.762148 lycoris_lora-2.3.0.dev9/PKG-INFO
+-rw-rw-rw-   0        0        0    11988 2024-05-03 13:57:17.000000 lycoris_lora-2.3.0.dev9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.715648 lycoris_lora-2.3.0.dev9/lycoris/
+-rw-rw-rw-   0        0        0      550 2024-02-05 11:33:28.000000 lycoris_lora-2.3.0.dev9/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.719152 lycoris_lora-2.3.0.dev9/lycoris/hcp/
+-rw-rw-rw-   0        0        0      156 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/__init__.py
+-rw-rw-rw-   0        0        0     5329 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/base.py
+-rw-rw-rw-   0        0        0     2281 2024-02-12 10:32:01.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/diag_oft.py
+-rw-rw-rw-   0        0        0     3391 2024-03-04 15:01:10.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/loha.py
+-rw-rw-rw-   0        0        0     5643 2024-03-04 15:01:21.000000 lycoris_lora-2.3.0.dev9/lycoris/hcp/lokr.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.725674 lycoris_lora-2.3.0.dev9/lycoris/kohya/
+-rw-rw-rw-   0        0        0    31784 2024-04-08 09:27:28.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/__init__.py
+-rw-rw-rw-   0        0        0    59991 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/model_utils.py
+-rw-rw-rw-   0        0        0    61070 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/original_unet.py
+-rw-rw-rw-   0        0        0    21297 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/sdxl_model_util.py
+-rw-rw-rw-   0        0        0    42690 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/sdxl_original_unet.py
+-rw-rw-rw-   0        0        0    19901 2024-03-11 06:16:36.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/test_hyperdream.py
+-rw-rw-rw-   0        0        0     1514 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/kohya/utils.py
+-rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-2.3.0.dev9/lycoris/logging.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.734186 lycoris_lora-2.3.0.dev9/lycoris/modules/
+-rw-rw-rw-   0        0        0     4201 2024-05-03 13:52:01.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     8185 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/attention.py
+-rw-rw-rw-   0        0        0     7155 2024-05-03 14:44:58.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/base.py
+-rw-rw-rw-   0        0        0     7938 2024-05-03 14:40:49.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/boft.py
+-rw-rw-rw-   0        0        0     6702 2024-05-03 14:47:33.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/diag_oft.py
+-rw-rw-rw-   0        0        0     4395 2024-05-03 12:40:31.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0     4518 2024-05-03 13:36:02.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/full.py
+-rw-rw-rw-   0        0        0    11788 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/glokr.py
+-rw-rw-rw-   0        0        0     4978 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/glora.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.735186 lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/
+-rw-rw-rw-   0        0        0       79 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/__init__.py
+-rw-rw-rw-   0        0        0     8302 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/generater.py
+-rw-rw-rw-   0        0        0     8339 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/text_encoder.py
+-rw-rw-rw-   0        0        0     2078 2024-03-11 06:14:46.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    12663 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/lilora.py
+-rw-rw-rw-   0        0        0    10800 2024-05-03 14:47:33.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    13088 2024-05-03 14:47:00.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    17926 2024-05-03 14:47:33.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/lokr.py
+-rw-rw-rw-   0        0        0     2387 2024-05-03 13:35:13.000000 lycoris_lora-2.3.0.dev9/lycoris/modules/norms.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.739696 lycoris_lora-2.3.0.dev9/lycoris/utils/
+-rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/bnb.py
+-rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/logger.py
+-rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/preset.py
+-rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev9/lycoris/utils/xformers_utils.py
+-rw-rw-rw-   0        0        0    18706 2024-03-16 16:01:01.000000 lycoris_lora-2.3.0.dev9/lycoris/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:52:43.761143 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1261 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       53 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 14:52:43.000000 lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 14:52:43.763147 lycoris_lora-2.3.0.dev9/setup.cfg
+-rw-rw-rw-   0        0        0      638 2024-05-03 14:52:39.000000 lycoris_lora-2.3.0.dev9/setup.py
```

### Comparing `lycoris_lora-2.3.0.dev8/LICENSE.md` & `lycoris_lora-2.3.0.dev9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/PKG-INFO` & `lycoris_lora-2.3.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycoris_lora
-Version: 2.3.0.dev8
+Version: 2.3.0.dev9
 Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
 Home-page: https://github.com/KohakuBlueleaf/LyCORIS
 Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
 Author-email: apolloyeh0123@gmail.com
 Requires-Python: >=3.10
 License-File: LICENSE.md
 Requires-Dist: torch
```

### Comparing `lycoris_lora-2.3.0.dev8/README.md` & `lycoris_lora-2.3.0.dev9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
   ```bash
   git clone https://github.com/KohakuBlueleaf/LyCORIS
   cd LyCORIS
   pip install .
   ```
 
-A detilaed description of the network arguments is provided in [docs/Network-Args.md](docs/Network-Args.md).
+A detailed description of the network arguments is provided in [docs/Network-Args.md](docs/Network-Args.md).
 
 #### kohya script
 
 You can use this package's kohya module to run kohya's training script to train lycoris module for SD models
 
 - with command line arguments
```

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/__init__.py` & `lycoris_lora-2.3.0.dev9/lycoris/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/config.py` & `lycoris_lora-2.3.0.dev9/lycoris/config.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/hcp/base.py` & `lycoris_lora-2.3.0.dev9/lycoris/hcp/base.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/hcp/diag_oft.py` & `lycoris_lora-2.3.0.dev9/lycoris/hcp/diag_oft.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/hcp/loha.py` & `lycoris_lora-2.3.0.dev9/lycoris/hcp/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/hcp/lokr.py` & `lycoris_lora-2.3.0.dev9/lycoris/hcp/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/kohya/__init__.py` & `lycoris_lora-2.3.0.dev9/lycoris/kohya/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/kohya/model_utils.py` & `lycoris_lora-2.3.0.dev9/lycoris/kohya/model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/kohya/original_unet.py` & `lycoris_lora-2.3.0.dev9/lycoris/kohya/original_unet.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/kohya/sdxl_model_util.py` & `lycoris_lora-2.3.0.dev9/lycoris/kohya/sdxl_model_util.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/kohya/sdxl_original_unet.py` & `lycoris_lora-2.3.0.dev9/lycoris/kohya/sdxl_original_unet.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/kohya/test_hyperdream.py` & `lycoris_lora-2.3.0.dev9/lycoris/kohya/test_hyperdream.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/kohya/utils.py` & `lycoris_lora-2.3.0.dev9/lycoris/kohya/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/logging.py` & `lycoris_lora-2.3.0.dev9/lycoris/logging.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/__init__.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/attention.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/attention.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/base.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,15 +160,14 @@
         self.dropout = dropout
         self.rank_dropout = rank_dropout
         self.rank_dropout_scale = rank_dropout_scale
         self.module_dropout = module_dropout
 
         self.multiplier = multiplier
         self.org_module = [org_module]
-        self.org_forward = self.org_module[0].forward
 
     @property
     def org_weight(self):
         return self.org_module[0].weight
 
     @org_weight.setter
     def org_weight(self, value):
@@ -188,19 +187,25 @@
         self.org_weight = weight
         if bias is not None:
             if self.org_module[0].bias is not None:
                 self.org_module[0].bias.data.copy_(bias)
             else:
                 self.org_module[0].bias = nn.Parameter(bias)
 
+    def get_diff_weight(self, multiplier=1.0, shape=None, device=None):
+        raise NotImplementedError
+
     def get_merged_weight(self, multiplier=1.0, shape=None, device=None):
         raise NotImplementedError
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
         raise NotImplementedError
 
+    def bypass_forward_diff(self, x, scale=1):
+        raise NotImplementedError
+
     def bypass_forward(self, x, scale=1):
         raise NotImplementedError
 
     def forward(self, *args, **kwargs):
         raise NotImplementedError
```

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/boft.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/boft.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,36 +120,42 @@
             q_norm = torch.norm(q) + 1e-8
             if q_norm > self.constrain:
                 normed_q = q * self.constrain / q_norm
         # use float() to prevent unsupported type
         r = (I + normed_q) @ (I - normed_q).float().inverse()
         return r
 
-    def make_weight(self, scale=1, device=None):
+    def make_weight(self, scale=1, device=None, diff=False):
         m = self.boft_m
         b = self.boft_b
         r_b = b // 2
         r = self.get_r()
         inp = self.org_weight.to(device, dtype=r.dtype)
 
         for i in range(m):
             bi = r[i]  # b_num, b_size, b_size
             if i == 0:
                 # Apply multiplier/scale and rescale into first weight
-                bi = bi * scale + (1 - scale) * self.I
                 if self.rescaled:
                     bi = bi * self.rescale
+            bi = bi * scale - scale * self.I + (self.I if diff else 0)
             inp = rearrange(inp, "(c g k) ... -> (c k g) ...", g=2, k=2**i * r_b)
             inp = rearrange(inp, "(d b) ... -> d b ...", b=b)
             inp = torch.einsum("b i j, b j ... -> b i ...", bi, inp)
             inp = rearrange(inp, "d b ... -> (d b) ...")
             inp = rearrange(inp, "(c k g) ... -> (c g k) ...", g=2, k=2**i * r_b)
 
         return inp
 
+    def get_diff_weight(self, multiplier=1, shape=None, device=None):
+        diff = self.make_weight(scale=multiplier, device=device, diff=True)
+        if shape is not None:
+            diff = diff.view(shape)
+        return diff
+
     def get_merged_weight(self, multiplier=1, shape=None, device=None):
         diff = self.make_weight(scale=multiplier, device=device)
         if shape is not None:
             diff = diff.view(shape)
         return diff, None
 
     @torch.no_grad()
@@ -161,36 +167,42 @@
 
         scaled = norm != desired
         if scaled:
             self.oft_blocks *= ratio
 
         return scaled, orig_norm * ratio
 
-    def bypass_forward(self, x, scale=1):
+    def _bypass_forward(self, x, scale=1, diff=False):
         m = self.boft_m
         b = self.boft_b
         r_b = b // 2
         r = self.get_r()
         inp = self.org_forward(x)
 
         for i in range(m):
             bi = r[i]  # b_num, b_size, b_size
             if i == 0:
                 # Apply multiplier/scale and rescale into first weight
-                bi = bi * scale + (1 - scale) * self.I
                 if self.rescaled:
                     bi = bi * self.rescale
+            bi = bi * scale - scale * self.I + (self.I if diff else 0)
             inp = rearrange(inp, "... (c g k) ->... (c k g)", g=2, k=2**i * r_b)
             inp = rearrange(inp, "... (d b) -> ... d b", b=b)
             inp = torch.einsum("b i j, ... b j -> ... b i", bi, inp)
             inp = rearrange(inp, "... d b -> ... (d b)")
             inp = rearrange(inp, "... (c k g) -> ... (c g k)", g=2, k=2**i * r_b)
 
         return inp
 
+    def bypass_forward_diff(self, x, scale=1):
+        return self._bypass_forward(x, scale, diff=True)
+
+    def bypass_forward(self, x, scale=1):
+        return self._bypass_forward(x, scale, diff=False)
+
     def forward(self, x, *args, **kwargs):
         if self.module_dropout and self.training:
             if torch.rand(1) < self.module_dropout:
                 return self.org_forward(x)
         scale = self.multiplier
 
         if self.bypass_mode:
```

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/diag_oft.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/diag_oft.py`

 * *Files 19% similar despite different names*

```diff
@@ -94,34 +94,40 @@
             q_norm = torch.norm(q) + 1e-8
             if q_norm > self.constrain:
                 normed_q = q * self.constrain / q_norm
         # use float() to prevent unsupported type
         r = (I + normed_q) @ (I - normed_q).float().inverse()
         return r
 
-    def make_weight(self, scale=1, device=None):
+    def make_weight(self, scale=1, device=None, diff=False):
         r = self.get_r()
         org_weight = self.org_weight.to(device, dtype=r.dtype)
         org_weight = rearrange(
             org_weight,
             "(k n) ... -> k n ...",
             k=self.block_num,
             n=self.block_size,
         )
         # Init R=0, so add I on it to ensure the output of step0 is original model output
         weight = torch.einsum(
             "k n m, k n ... -> k m ...",
-            r * scale + (1 - scale) * self.I,
+            r * scale - scale * self.I + (self.I if diff else 0),
             org_weight,
         )
         weight = rearrange(weight, "k m ... -> (k m) ...")
         if self.rescaled:
             weight = self.rescale * weight
         return weight
 
+    def get_diff_weight(self, multiplier=1, shape=None, device=None):
+        diff = self.make_weight(scale=multiplier, device=device, diff=True)
+        if shape is not None:
+            diff = diff.view(shape)
+        return diff
+
     def get_merged_weight(self, multiplier=1, shape=None, device=None):
         diff = self.make_weight(scale=multiplier, device=device)
         if shape is not None:
             diff = diff.view(shape)
         return diff, None
 
     @torch.no_grad()
@@ -133,33 +139,41 @@
 
         scaled = norm != desired
         if scaled:
             self.oft_blocks *= ratio
 
         return scaled, orig_norm * ratio
 
-    def bypass_forward(self, x, scale=1):
+    def _bypass_forward(self, x, scale=1, diff=False):
         r = self.get_r()
         org_out = self.org_forward(x)
         if self.op == F.conv2d:
             org_out = org_out.transpose(1, -1)
         org_out = rearrange(
             org_out,
             "... (k n) ->... k n",
             k=self.block_num,
             n=self.block_size,
         )
         oft_out = torch.einsum(
-            "k n m, ... k n -> ... k m", r * scale + (1 - scale) * self.I, org_out
+            "k n m, ... k n -> ... k m",
+            r * scale - scale * self.I + (self.I if diff else 0),
+            org_out,
         )
         out = rearrange(oft_out, "... k m -> ... (k m)")
         if self.op == F.conv2d:
             out = out.transpose(1, -1)
         return out
 
+    def bypass_forward_diff(self, x, scale=1):
+        return self._bypass_forward(x, scale, diff=True)
+
+    def bypass_forward(self, x, scale=1):
+        return self._bypass_forward(x, scale, diff=False)
+
     def forward(self, x: torch.Tensor, *args, **kwargs):
         if self.module_dropout and self.training:
             if torch.rand(1) < self.module_dropout:
                 return self.org_forward(x)
         scale = self.multiplier
 
         if self.bypass_mode:
```

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/dylora.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/full.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/full.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/glokr.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/glokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/glora.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/generater.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/generater.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/text_encoder.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/hypernet/text_encoder.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/ia3.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/lilora.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/lilora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/locon.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/locon.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,25 +170,30 @@
             drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
             if self.rank_dropout_scale:
                 drop /= drop.mean()
             weight *= drop
 
         return weight * self.scalar.to(device)
 
-    def get_merged_weight(self, multiplier=1, shape=None, device=None):
+    def get_diff_weight(self, multiplier=1, shape=None, device=None):
         scale = self.scale * multiplier
         diff = self.make_weight(device=device) * scale
         if shape is not None:
             diff = diff.view(shape)
         if device is not None:
             diff = diff.to(device)
-        merged = self.org_module[0].weight.data + diff
+        return diff
+
+    def get_merged_weight(self, multiplier=1, shape=None, device=None):
+        merged = self.org_module[0].weight.data + self.get_diff_weight(
+            multiplier=multiplier, shape=shape, device=device
+        )
         if self.wd:
             merged = self.apply_weight_decompose(merged)
-        return merged
+        return merged, None
 
     def apply_weight_decompose(self, weight):
         weight = weight.to(self.dora_scale.dtype)
         weight_norm = (
             weight.transpose(0, 1)
             .reshape(weight.shape[1], -1)
             .norm(dim=1, keepdim=True)
@@ -218,15 +223,15 @@
 
         scaled = norm != desired
         if scaled:
             self.scalar *= ratio
 
         return scaled, orig_norm * ratio
 
-    def bypass_forward(self, x, scale=1):
+    def bypass_forward_diff(self, x, scale=1):
         if self.tucker:
             mid = self.lora_mid(self.lora_down(x))
         else:
             mid = self.lora_down(x)
 
         if self.rank_dropout and self.training:
             drop = (
@@ -236,17 +241,18 @@
                 drop /= drop.mean()
             if (dims := len(x.shape)) == 4:
                 drop = drop.view(1, -1, 1, 1)
             else:
                 drop = drop.view(*[1] * (dims - 1), -1)
             mid = mid * drop
 
-        return self.org_forward(x) + self.dropout(
-            self.lora_up(mid) * self.scalar * self.scale * scale
-        )
+        return self.dropout(self.lora_up(mid) * self.scalar * self.scale * scale)
+
+    def bypass_forward(self, x, scale=1):
+        return self.org_forward(x) + self.bypass_forward_diff(x, scale=scale)
 
     def forward(self, x):
         if self.module_dropout and self.training:
             if torch.rand(1) < self.module_dropout:
                 return self.org_forward(x)
         scale = self.scale * self.multiplier
```

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/loha.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/loha.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,20 +243,25 @@
             drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(weight.dtype)
             drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
             if self.rank_dropout_scale:
                 drop /= drop.mean()
             weight *= drop
         return weight
 
-    def get_merged_weight(self, multiplier=1, shape=None, device=None):
+    def get_diff_weight(self, multiplier=1, shape=None, device=None):
         scale = self.scale * multiplier
         diff = self.get_weight(shape) * scale
         if device is not None:
             diff = diff.to(device)
-        merged = self.org_module[0].weight.data + diff
+        return diff
+
+    def get_merged_weight(self, multiplier=1, shape=None, device=None):
+        merged = self.org_module[0].weight.data + self.get_diff_weight(
+            multiplier=multiplier, shape=shape, device=device
+        )
         if self.wd:
             merged = self.apply_weight_decompose(merged)
         return merged
 
     def apply_weight_decompose(self, weight):
         weight = weight.to(self.dora_scale.dtype)
         weight_norm = (
@@ -292,18 +297,20 @@
 
         scaled = norm != desired
         if scaled:
             self.scalar *= ratio
 
         return scaled, orig_norm * ratio
 
-    def bypass_forward(self, x, scale=1):
+    def bypass_forward_diff(self, x, scale=1):
         diff_weight = self.get_weight(self.shape) * self.scalar * scale
-        print(diff_weight.shape, x.shape, self.shape)
-        return self.org_forward(x) + self.op(x, diff_weight, **self.kw_dict)
+        return self.op(x, diff_weight, **self.kw_dict)
+
+    def bypass_forward(self, x, scale=1):
+        return self.org_forward(x) + self.bypass_forward_diff(x, scale=scale)
 
     def forward(self, x: torch.Tensor, *args, **kwargs):
         if self.module_dropout and self.training:
             if torch.rand(1) < self.module_dropout:
                 return self.op(
                     x,
                     self.org_module[0].weight.data,
```

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/lokr.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/lokr.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,19 +372,18 @@
                 if self.tucker:
                     self.lokr_t2 *= ratio ** (1 / modules)
                 self.lokr_w2_a *= ratio ** (1 / modules)
                 self.lokr_w2_b *= ratio ** (1 / modules)
 
         return scaled, orig_norm * ratio
 
-    def bypass_forward(self, h):
+    def bypass_forward_diff(self, h):
         if len(self.shape) > 2 and self.shape[2] > 1:
             return (
-                self.org_forward(h)
-                + self.op(h, self.get_weight(self.shape), **self.kw_dict)
+                self.op(h, self.get_weight(self.shape), **self.kw_dict)
                 * self.multiplier
             )
         if self.module_type.startswith("conv"):
             h = h.transpose(1, -1)
         if self.use_w2:
             ba = self.lokr_w2
         else:
@@ -409,15 +408,18 @@
         h_cross_group = hb.transpose(-1, -2)
         hc = F.linear(h_cross_group, c)
 
         h = rearrange(hc, "b ... vp up -> b ... (up vp)")
         if self.module_type.startswith("conv"):
             h = h.transpose(1, -1)
 
-        return h * self.multiplier + self.org_forward(h)
+        return h * self.multiplier
+
+    def bypass_forward(self, x, scale=1):
+        return self.org_forward(x) + self.bypass_forward_diff(x, scale=scale)
 
     def forward(self, x: torch.Tensor, *args, **kwargs):
         if self.module_dropout and self.training:
             if torch.rand(1) < self.module_dropout:
                 return self.op(
                     x,
                     self.org_module[0].weight.data,
```

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/modules/norms.py` & `lycoris_lora-2.3.0.dev9/lycoris/modules/norms.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/utils/__init__.py` & `lycoris_lora-2.3.0.dev9/lycoris/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/utils/logger.py` & `lycoris_lora-2.3.0.dev9/lycoris/utils/logger.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris/wrapper.py` & `lycoris_lora-2.3.0.dev9/lycoris/wrapper.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/PKG-INFO` & `lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycoris_lora
-Version: 2.3.0.dev8
+Version: 2.3.0.dev9
 Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
 Home-page: https://github.com/KohakuBlueleaf/LyCORIS
 Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
 Author-email: apolloyeh0123@gmail.com
 Requires-Python: >=3.10
 License-File: LICENSE.md
 Requires-Dist: torch
```

### Comparing `lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-2.3.0.dev9/lycoris_lora.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 lycoris/modules/hypernet/__init__.py
 lycoris/modules/hypernet/generater.py
 lycoris/modules/hypernet/text_encoder.py
 lycoris/utils/__init__.py
 lycoris/utils/bnb.py
 lycoris/utils/logger.py
 lycoris/utils/preset.py
-lycoris/utils/tensor_norm.py
 lycoris/utils/xformers_utils.py
 lycoris_lora.egg-info/PKG-INFO
 lycoris_lora.egg-info/SOURCES.txt
 lycoris_lora.egg-info/dependency_links.txt
 lycoris_lora.egg-info/not-zip-safe
 lycoris_lora.egg-info/requires.txt
 lycoris_lora.egg-info/top_level.txt
```

### Comparing `lycoris_lora-2.3.0.dev8/setup.py` & `lycoris_lora-2.3.0.dev9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lycoris_lora",
     packages=find_packages(),
-    version="2.3.0.dev8",
+    version="2.3.0.dev9",
     url="https://github.com/KohakuBlueleaf/LyCORIS",
     description="Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion",
     author="Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao",
     author_email="apolloyeh0123@gmail.com",
     zip_safe=False,
     install_requires=[
         "torch",
```

