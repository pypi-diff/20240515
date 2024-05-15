# Comparing `tmp/cellplot-1.7.tar.gz` & `tmp/cellplot-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellplot-1.7.tar", last modified: Thu Mar  7 10:39:07 2024, max compression
+gzip compressed data, was "cellplot-1.8.tar", last modified: Wed May 15 13:02:50 2024, max compression
```

## Comparing `cellplot-1.7.tar` & `cellplot-1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:39:07.099173 cellplot-1.7/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-07 10:39:07.099173 cellplot-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-07 10:39:04.000000 cellplot-1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:39:07.095173 cellplot-1.7/cellplot/
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-03-07 10:39:04.000000 cellplot-1.7/cellplot/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-03-07 10:39:04.000000 cellplot-1.7/cellplot/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-07 10:39:04.000000 cellplot-1.7/cellplot/multiview.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3922 2024-03-07 10:39:04.000000 cellplot-1.7/cellplot/patches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      739 2024-03-07 10:39:04.000000 cellplot-1.7/cellplot/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-07 10:39:04.000000 cellplot-1.7/cellplot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:39:07.099173 cellplot-1.7/cellplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-07 10:39:07.000000 cellplot-1.7/cellplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-07 10:39:07.000000 cellplot-1.7/cellplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 10:39:07.000000 cellplot-1.7/cellplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-07 10:39:07.000000 cellplot-1.7/cellplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-07 10:39:07.000000 cellplot-1.7/cellplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 10:39:07.099173 cellplot-1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-07 10:39:06.000000 cellplot-1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:02:50.748200 cellplot-1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 13:02:50.748200 cellplot-1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 13:02:48.000000 cellplot-1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:02:50.744200 cellplot-1.8/cellplot/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-15 13:02:48.000000 cellplot-1.8/cellplot/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-05-15 13:02:48.000000 cellplot-1.8/cellplot/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-15 13:02:48.000000 cellplot-1.8/cellplot/multiview.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3922 2024-05-15 13:02:48.000000 cellplot-1.8/cellplot/patches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      739 2024-05-15 13:02:48.000000 cellplot-1.8/cellplot/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-15 13:02:48.000000 cellplot-1.8/cellplot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:02:50.748200 cellplot-1.8/cellplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 13:02:50.000000 cellplot-1.8/cellplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 13:02:50.000000 cellplot-1.8/cellplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:02:50.000000 cellplot-1.8/cellplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 13:02:50.000000 cellplot-1.8/cellplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 13:02:50.000000 cellplot-1.8/cellplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:02:50.748200 cellplot-1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 13:02:50.000000 cellplot-1.8/setup.py
```

### Comparing `cellplot-1.7/cellplot/images.py` & `cellplot-1.8/cellplot/images.py`

 * *Files identical despite different names*

### Comparing `cellplot-1.7/cellplot/multiview.py` & `cellplot-1.8/cellplot/multiview.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import numpy as np
 from .utils import generate_rainbow_colors, convert_image_to_uint8
 from PIL import Image, ImageDraw, ImageFont
 from typing import List, Tuple, Optional, Literal
 import os
+from scipy.ndimage import zoom
 
 def create_multiview(
     image: np.ndarray, 
     colors: Optional[List[Tuple[int, int, int]]] = None, 
     shift: Optional[Tuple[float, float]] = (0.1, 0.1), #shift_y #shift_y
     shift_type: Literal["relative", "absolute"] = "relative", 
     margins: Tuple[float, float] = (0.1, 0.1), 
     fontsize: int = 15, 
-    channel_names: Optional[List[str]] = None):
+    channel_names: Optional[List[str]] = None,
+    image_scaling: Optional[float] = None,
+    channels_to_show: Optional[List[int]] = None):
     """
     Create a multiview image from a single multi-channel image.
 
     Args:
     image (np.ndarray): The input image with multiple channels.
     colors (Optional[List[Tuple[int, int, int]]]): List of RGB tuples for coloring each channel.
     shift (Optional[Tuple[float, float]]): Tuple of shift values with (x_shift, y_shift)
@@ -34,14 +37,20 @@
     """
     
     image = convert_image_to_uint8(image)
 
     # Check if the image has three dimensions (height, width, channels)
     if image.ndim != 3:
         raise ValueError("Input image must have three dimensions (height, width, channels)")
+    
+    if channels_to_show is not None:
+        image = image[..., channels_to_show]
+
+    # here code that scales the image hgiven in the formal W H C to the size W*image_scaling H*image_scaling C
+    image = zoom(image, (image_scaling, image_scaling, 1), order=3)  # order=3 for cubic interpolation
 
     # Transpose the image to get channels in the first dimension
     transposed_image = image.transpose(2, 0, 1)
     num_channels, im_height, im_width = transposed_image.shape
     
     # Ensure the shift type is valid
     assert shift_type in ["relative", "absolute"], "Unknown shift type please choose one of 'relative' or 'absolute'."
```

### Comparing `cellplot-1.7/cellplot/patches.py` & `cellplot-1.8/cellplot/patches.py`

 * *Files identical despite different names*

### Comparing `cellplot-1.7/cellplot/segmentation.py` & `cellplot-1.8/cellplot/segmentation.py`

 * *Files identical despite different names*

### Comparing `cellplot-1.7/cellplot/utils.py` & `cellplot-1.8/cellplot/utils.py`

 * *Files identical despite different names*

### Comparing `cellplot-1.7/setup.py` & `cellplot-1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_requirements():
     with open('requirements.txt', 'r') as file:
         return [line.strip() for line in file.readlines()]
 
 setup(
     name=package_name,
-    version='1.7',
+    version='1.8',
     packages=find_packages(),
     install_requires=read_requirements(),
     author="Simon Gutwein",
     include_package_data=True,
     author_email="simon.gutwein@ccri.at",
     description="",
     long_description=open('README.md').read(),
```

