# Comparing `tmp/virtual_camera-0.0.3.tar.gz` & `tmp/virtual_camera-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtual_camera-0.0.3.tar", last modified: Tue May 14 11:53:26 2024, max compression
+gzip compressed data, was "virtual_camera-0.0.4.tar", last modified: Wed May 15 03:31:56 2024, max compression
```

## Comparing `virtual_camera-0.0.3.tar` & `virtual_camera-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 11:53:26.571020 virtual_camera-0.0.3/
--rw-rw-r--   0 alpha     (1000) alpha     (1000)     1952 2024-05-14 11:53:26.571020 virtual_camera-0.0.3/PKG-INFO
--rw-rw-r--   0 alpha     (1000) alpha     (1000)       38 2024-05-14 11:53:26.571020 virtual_camera-0.0.3/setup.cfg
--rw-rw-r--   0 alpha     (1000) alpha     (1000)      434 2024-05-14 11:43:14.000000 virtual_camera-0.0.3/setup.py
-drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 11:53:26.567021 virtual_camera-0.0.3/virtual_camera/
--rw-rw-r--   0 alpha     (1000) alpha     (1000)     1372 2024-05-14 11:53:01.000000 virtual_camera-0.0.3/virtual_camera/__init__.py
-drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 11:53:26.571020 virtual_camera-0.0.3/virtual_camera/data/
--rw-rw-r--   0 alpha     (1000) alpha     (1000)      537 2024-05-14 07:58:20.000000 virtual_camera-0.0.3/virtual_camera/data/calibration.yml
--rw-rw-r--   0 alpha     (1000) alpha     (1000)    55776 2024-05-14 07:56:45.000000 virtual_camera-0.0.3/virtual_camera/data/dst_image.jpg
--rw-rw-r--   0 alpha     (1000) alpha     (1000)    14224 2024-05-14 07:56:45.000000 virtual_camera-0.0.3/virtual_camera/data/mask.png
--rw-rw-r--   0 alpha     (1000) alpha     (1000)   135901 2024-05-14 07:56:44.000000 virtual_camera-0.0.3/virtual_camera/data/src_image.jpg
--rw-rw-r--   0 alpha     (1000) alpha     (1000)    14124 2024-05-14 11:29:49.000000 virtual_camera-0.0.3/virtual_camera/virtual_camera.py
-drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-14 11:53:26.567021 virtual_camera-0.0.3/virtual_camera.egg-info/
--rw-rw-r--   0 alpha     (1000) alpha     (1000)     1952 2024-05-14 11:53:26.000000 virtual_camera-0.0.3/virtual_camera.egg-info/PKG-INFO
--rw-rw-r--   0 alpha     (1000) alpha     (1000)      390 2024-05-14 11:53:26.000000 virtual_camera-0.0.3/virtual_camera.egg-info/SOURCES.txt
--rw-rw-r--   0 alpha     (1000) alpha     (1000)        1 2024-05-14 11:53:26.000000 virtual_camera-0.0.3/virtual_camera.egg-info/dependency_links.txt
--rw-rw-r--   0 alpha     (1000) alpha     (1000)       12 2024-05-14 11:53:26.000000 virtual_camera-0.0.3/virtual_camera.egg-info/requires.txt
--rw-rw-r--   0 alpha     (1000) alpha     (1000)       15 2024-05-14 11:53:26.000000 virtual_camera-0.0.3/virtual_camera.egg-info/top_level.txt
+drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-15 03:31:56.702317 virtual_camera-0.0.4/
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)     2072 2024-05-15 03:31:56.698317 virtual_camera-0.0.4/PKG-INFO
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)     1844 2024-05-14 12:31:27.000000 virtual_camera-0.0.4/README.md
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)       38 2024-05-15 03:31:56.702317 virtual_camera-0.0.4/setup.cfg
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)      492 2024-05-15 03:21:10.000000 virtual_camera-0.0.4/setup.py
+drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-15 03:31:56.698317 virtual_camera-0.0.4/virtual_camera/
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)     1372 2024-05-14 11:53:01.000000 virtual_camera-0.0.4/virtual_camera/__init__.py
+drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-15 03:31:56.698317 virtual_camera-0.0.4/virtual_camera/data/
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)      537 2024-05-14 07:58:20.000000 virtual_camera-0.0.4/virtual_camera/data/calibration.yml
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)    55776 2024-05-14 07:56:45.000000 virtual_camera-0.0.4/virtual_camera/data/dst_image.jpg
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)    14224 2024-05-14 07:56:45.000000 virtual_camera-0.0.4/virtual_camera/data/mask.png
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)   135901 2024-05-14 07:56:44.000000 virtual_camera-0.0.4/virtual_camera/data/src_image.jpg
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)    15016 2024-05-15 03:15:40.000000 virtual_camera-0.0.4/virtual_camera/virtual_camera.py
+drwxrwxr-x   0 alpha     (1000) alpha     (1000)        0 2024-05-15 03:31:56.698317 virtual_camera-0.0.4/virtual_camera.egg-info/
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)     2072 2024-05-15 03:31:56.000000 virtual_camera-0.0.4/virtual_camera.egg-info/PKG-INFO
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)      400 2024-05-15 03:31:56.000000 virtual_camera-0.0.4/virtual_camera.egg-info/SOURCES.txt
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)        1 2024-05-15 03:31:56.000000 virtual_camera-0.0.4/virtual_camera.egg-info/dependency_links.txt
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)       12 2024-05-15 03:31:56.000000 virtual_camera-0.0.4/virtual_camera.egg-info/requires.txt
+-rw-rw-r--   0 alpha     (1000) alpha     (1000)       15 2024-05-15 03:31:56.000000 virtual_camera-0.0.4/virtual_camera.egg-info/top_level.txt
```

### Comparing `virtual_camera-0.0.3/PKG-INFO` & `virtual_camera-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: virtual_camera
-Version: 0.0.3
+Version: 0.0.4
 Summary: Virtual Camera
+Home-page: https://github.com/AlphaLFC/virtual_camera
 Author: AlphaLFC
-Author-email: 
+Author-email: alphali@motovis.com
 Description-Content-Type: text/markdown
 
 # Virtual Camera
 
 ## Install
 ```bash
 pip install virtual_camera
@@ -41,15 +42,17 @@
 cfg = yaml.safe_load(open(yaml_file, 'r'))
 camera_real = vc.FisheyeCamera.init_from_motovis_cfg(cfg)
 ```
 Read the real image.
 ```python
 src_image = plt.imread('data/src_image.jpg')
 ```
-![src_image](data/src_image.jpg)
+![src_image](virtual_camera/data/src_image.jpg)
+
 Convert the image to a virtual image. Alongside with mask.
 ```python
 dst_image, mask = vc.render_image(src_image, camera_real, vc.VCAMERA_PERSPECTIVE_FRONT)
 ```
-![dst_image](data/dst_image.jpg)
 
-![mask](data/mask.png)
+![dst_image](virtual_camera/data/dst_image.jpg)
+
+![mask](virtual_camera/data/mask.png)
```

### Comparing `virtual_camera-0.0.3/virtual_camera/__init__.py` & `virtual_camera-0.0.4/virtual_camera/__init__.py`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.3/virtual_camera/data/calibration.yml` & `virtual_camera-0.0.4/virtual_camera/data/calibration.yml`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.3/virtual_camera/data/dst_image.jpg` & `virtual_camera-0.0.4/virtual_camera/data/dst_image.jpg`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.3/virtual_camera/data/mask.png` & `virtual_camera-0.0.4/virtual_camera/data/mask.png`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.3/virtual_camera/data/src_image.jpg` & `virtual_camera-0.0.4/virtual_camera/data/src_image.jpg`

 * *Files identical despite different names*

### Comparing `virtual_camera-0.0.3/virtual_camera/virtual_camera.py` & `virtual_camera-0.0.4/virtual_camera/virtual_camera.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 import cv2
-import yaml
 import numpy as np
 
-# import matplotlib.pyplot as plt
-# %matplotlib inline
-
-from pathlib import Path
 from functools import partial
 from scipy.optimize import curve_fit
 from scipy.spatial.transform import Rotation
 
 
 def get_extrinsic_from_euler(x, y, z, pitch, yaw, roll):
     R = Rotation.from_euler(
@@ -118,21 +113,22 @@
         - pytorch3d-style: x-y-z left-up-forward
     """
     def __init__(self, resolution, extrinsic, intrinsic, fov=None, ego_mask=None):
         """## Args:
         - resolution : tuple (w, h)
         - extrinsic : list or tuple (R, t) in motovis-style ego system
         - intrinsic : list or tuple (cx, cy, fx, fy, p0, p1, p2, p3)
+        - fov : float, in degree
+        - ego_mask : in shape (h, w)
         """
-        super().__init__(resolution, extrinsic, intrinsic)
+        super().__init__(resolution, extrinsic, intrinsic, ego_mask=ego_mask)
         if fov is None:
             self.fov = 225
         else:
             self.fov = fov
-        self.ego_mask = ego_mask
 
     def project_points_from_camera_to_image(self, camera_points):
         # camera_points in image-style: x-y-z right-down-forward
         cx, cy, fx, fy, p0, p1, p2, p3 = self.intrinsic
         xx = camera_points[0]
         yy = camera_points[1]
         zz = camera_points[2]
@@ -210,15 +206,24 @@
         else:
             self.camera_mask = self.ego_mask
     
         return self.camera_mask
 
     
     def _to_motovis_cfg(self):
-        pass
+        cfg_camera = {}
+        cfg_camera['sensor_model'] = 'src.sensors.cameras.OpenCVFisheyeCamera'
+        cfg_camera['image_size'] = self.resolution
+        quant = Rotation.from_matrix(self.R_e).as_quat()
+        cfg_camera['extrinsic'] = list(self.t_e) + list(quant)
+        cfg_camera['pp'] = self.intrinsic[:2]
+        cfg_camera['focal'] = self.intrinsic[2:4]
+        cfg_camera['inv_poly'] = self.intrinsic[4:]
+        cfg_camera['fov_fit'] = self.fov
+        return cfg_camera
 
 
     @classmethod
     def init_from_motovis_cfg(cls, cfg_camera, use_default_fov=True):
         camera_model = cfg_camera['sensor_model']
         assert camera_model in ['src.sensors.cameras.OpenCVFisheyeCamera']
 
@@ -244,21 +249,22 @@
     """
     Camera Coordinate System: image-style, normalized coords.
         - motovis-style: x-y-z right-forward-up
         - openGL-style: x-y-z right-up-backward
         - image-style: x-y-z right-down-forward
         - pytorch3d-style: x-y-z left-up-forward
     """
-    def __init__(self, resolution, extrinsic, intrinsic):
+    def __init__(self, resolution, extrinsic, intrinsic, ego_mask=None):
         """## Args:
         - resolution : tuple (w, h)
         - extrinsic : list or tuple (R, t) in motovis-style ego system
         - intrinsic : list or tuple (cx, cy, fx, fy)
+        - ego_mask : in shape (h, w)
         """
-        super().__init__(resolution, extrinsic, intrinsic)
+        super().__init__(resolution, extrinsic, intrinsic, ego_mask=ego_mask)
     
     def unproject_points_from_image_to_camera(self):
         W, H = self.resolution
         cx, cy, fx, fy = self.intrinsic
         
         uu, vv = np.meshgrid(
             np.linspace(0, W - 1, W), 
@@ -277,15 +283,22 @@
         img_points = np.matmul(self.K, camera_points.reshape(3, -1)).reshape(camera_points.shape)
         img_points[2, np.abs(img_points[2]) < 1e-5] = 1e-5
         uu = np.float32(img_points[0] / img_points[2])
         vv = np.float32(img_points[1] / img_points[2])
         return uu, vv
     
     def _to_motovis_cfg(self):
-        pass
+        cfg_camera = {}
+        cfg_camera['sensor_model'] = 'src.sensors.cameras.PerspectiveCamera'
+        cfg_camera['image_size'] = self.resolution
+        quant = Rotation.from_matrix(self.R_e).as_quat()
+        cfg_camera['extrinsic'] = list(self.t_e) + list(quant)
+        cfg_camera['pp'] = self.intrinsic[:2]
+        cfg_camera['focal'] = self.intrinsic[2:4]
+        return cfg_camera
 
     @classmethod
     def init_from_nuscense_cfg(cls, cfg):
         pass
 
     @classmethod
     def init_from_av2_cfg(cls, cfg):
@@ -309,14 +322,15 @@
 
         #cx, cy, fx, fy
         intrinsic = cfg_camera['pp'] + cfg_camera['focal']
 
         return cls(resolution, extrinsic, intrinsic)
 
 
+
 AVAILABLE_CAMERA_TYPES = [FisheyeCamera, PerspectiveCamera]
 
 
 
 def _check_camera_type(camera):
     return any([isinstance(camera, camera_type) for camera_type in AVAILABLE_CAMERA_TYPES])
```

### Comparing `virtual_camera-0.0.3/virtual_camera.egg-info/PKG-INFO` & `virtual_camera-0.0.4/virtual_camera.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: virtual-camera
-Version: 0.0.3
+Version: 0.0.4
 Summary: Virtual Camera
+Home-page: https://github.com/AlphaLFC/virtual_camera
 Author: AlphaLFC
-Author-email: 
+Author-email: alphali@motovis.com
 Description-Content-Type: text/markdown
 
 # Virtual Camera
 
 ## Install
 ```bash
 pip install virtual_camera
@@ -41,15 +42,17 @@
 cfg = yaml.safe_load(open(yaml_file, 'r'))
 camera_real = vc.FisheyeCamera.init_from_motovis_cfg(cfg)
 ```
 Read the real image.
 ```python
 src_image = plt.imread('data/src_image.jpg')
 ```
-![src_image](data/src_image.jpg)
+![src_image](virtual_camera/data/src_image.jpg)
+
 Convert the image to a virtual image. Alongside with mask.
 ```python
 dst_image, mask = vc.render_image(src_image, camera_real, vc.VCAMERA_PERSPECTIVE_FRONT)
 ```
-![dst_image](data/dst_image.jpg)
 
-![mask](data/mask.png)
+![dst_image](virtual_camera/data/dst_image.jpg)
+
+![mask](virtual_camera/data/mask.png)
```

