# Comparing `tmp/opensr-test-0.2.1.tar.gz` & `tmp/opensr_test-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensr-test-0.2.1.tar", last modified: Wed Mar 27 16:40:04 2024, max compression
+gzip compressed data, was "opensr_test-0.2.9.tar", max compression
```

## Comparing `opensr-test-0.2.1.tar` & `opensr_test-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,14 @@
-drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-27 16:40:04.256873 opensr-test-0.2.1/
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     1077 2024-02-09 11:36:31.000000 opensr-test-0.2.1/LICENSE
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    10581 2024-03-27 16:40:04.256873 opensr-test-0.2.1/PKG-INFO
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     9863 2024-03-24 14:19:46.000000 opensr-test-0.2.1/README.md
-drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-27 16:40:04.256873 opensr-test-0.2.1/opensr_test/
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      137 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/__init__.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     9265 2024-03-24 10:15:54.000000 opensr-test-0.2.1/opensr_test/config.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    17034 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/distance.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     3421 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/download.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     3998 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/hallucinations.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    11223 2024-03-24 10:13:37.000000 opensr-test-0.2.1/opensr_test/kernels.py
-drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-27 16:40:04.256873 opensr-test-0.2.1/opensr_test/lightglue/
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      263 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/__init__.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    26763 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/aliked.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     1751 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/disk.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     1500 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/dog_hardnet.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    25998 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/lightglue/lightglue.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     8194 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/sift.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     8618 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/superpoint.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     5511 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/lightglue/utils.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     5919 2024-02-09 11:46:15.000000 opensr-test-0.2.1/opensr_test/lightglue/viz2d.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    21719 2024-03-24 10:55:17.000000 opensr-test-0.2.1/opensr_test/main.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    15630 2024-03-23 18:34:25.000000 opensr-test-0.2.1/opensr_test/plot.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      916 2024-02-09 11:36:31.000000 opensr-test-0.2.1/opensr_test/reflectance.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    20856 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/spatial.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      918 2024-02-09 11:36:31.000000 opensr-test-0.2.1/opensr_test/spectral.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     8499 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/utils.py
-drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-27 16:40:04.256873 opensr-test-0.2.1/opensr_test.egg-info/
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    10581 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/PKG-INFO
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      778 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/SOURCES.txt
--rw-rw-r--   0 cesar     (1002) cesar     (1002)        1 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/dependency_links.txt
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      143 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/requires.txt
--rw-rw-r--   0 cesar     (1002) cesar     (1002)       12 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/top_level.txt
--rw-rw-r--   0 cesar     (1002) cesar     (1002)       38 2024-03-27 16:40:04.256873 opensr-test-0.2.1/setup.cfg
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     1513 2024-03-27 16:39:41.000000 opensr-test-0.2.1/setup.py
+-rw-r--r--   0        0        0     1070 2024-05-09 08:13:17.278355 opensr_test-0.2.9/LICENSE
+-rw-r--r--   0        0        0    12100 2024-05-13 15:41:27.379466 opensr_test-0.2.9/README.md
+-rw-r--r--   0        0        0      111 2024-05-10 17:01:30.595335 opensr_test-0.2.9/opensr_test/__init__.py
+-rw-r--r--   0        0        0     3303 2024-05-14 15:00:31.255299 opensr_test-0.2.9/opensr_test/config.py
+-rw-r--r--   0        0        0     3925 2024-05-14 15:04:04.089140 opensr_test-0.2.9/opensr_test/correctness.py
+-rw-r--r--   0        0        0     2154 2024-05-14 11:04:14.042783 opensr_test-0.2.9/opensr_test/dataset.py
+-rw-r--r--   0        0        0    17828 2024-05-14 14:54:26.605895 opensr_test-0.2.9/opensr_test/distance.py
+-rw-r--r--   0        0        0    20917 2024-05-14 15:17:02.456527 opensr_test-0.2.9/opensr_test/main.py
+-rw-r--r--   0        0        0    11321 2024-05-14 15:05:56.813535 opensr_test-0.2.9/opensr_test/plot.py
+-rw-r--r--   0        0        0     2200 2024-05-12 16:32:21.798342 opensr_test-0.2.9/opensr_test/spatial.py
+-rw-r--r--   0        0        0     4270 2024-05-14 11:12:03.733377 opensr_test-0.2.9/opensr_test/utils.py
+-rw-r--r--   0        0        0     2076 2024-05-15 05:42:10.708329 opensr_test-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 opensr_test-0.2.9/setup.py
+-rw-r--r--   0        0        0    12965 1970-01-01 00:00:00.000000 opensr_test-0.2.9/PKG-INFO
```

### Comparing `opensr-test-0.2.1/LICENSE` & `opensr_test-0.2.9/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-The MIT License (MIT)
+MIT License
 
-Copyright (c) 2023 OpenSR team
+Copyright (c) 2024, Cesar Aybar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,9 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
+
```

### Comparing `opensr-test-0.2.1/opensr_test/distance.py` & `opensr_test-0.2.9/opensr_test/distance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-from typing import List, Optional, Union
-
 from abc import ABC, abstractmethod
+from typing import List, Optional, Union
 
 import torch
-from opensr_test.config import Metric
-from opensr_test.utils import check_lpips, check_openclip
-from torchvision.transforms import Normalize
+from opensr_test.utils import check_lpips, check_openclip, check_huggingface_hub
 
 
 class DistanceMetric(ABC):
-    """ Metaclass to define the distance metrics
+    """An abstract class to compute the distance between two tensors.
 
     Parameters:
         method (str): The method to use. Either "pixel", "patch", or "image".
         patch_size (int): The patch size to use if the patch method is used.
         x (torch.Tensor): The SR harmonized image (C, H, W).
         y (torch.Tensor): The HR image (C, H, W).
         **kwargs: The parameters to pass to the distance function.
-        
+
     Abstract methods:
         compute_patch: Compute the distance metric at patch level.
         compute_image: Compute the distance metric at image level.
         compute_pixel: Compute the distance metric at image level.
         compute: Compute the distance metric.
-        
     """
 
     def __init__(
         self,
-        name: str,
         method: str,
         patch_size: int,
         x: torch.Tensor,
         y: torch.Tensor,
         **kwargs
     ):
         self.method = method
-        self.name = name
         self.patch_size = patch_size
         self.kwargs = kwargs
         self.axis: int = 0
         self.x = x
         self.y = y
 
     @staticmethod
     def do_square(tensor: torch.Tensor, patch_size: Optional[int] = 32) -> torch.Tensor:
-        """ Split a tensor into n_patches x n_patches patches and return
+        """Split a tensor into n_patches x n_patches patches and return
         the patches as a tensor.
-        
+
         Args:
             tensor (torch.Tensor): The tensor to split.
             n_patches (int, optional): The number of patches to split the tensor into.
                 If None, the tensor is split into the smallest number of patches.
 
         Returns:
             torch.Tensor: The patches as a tensor.
         """
+        
         # Check if it is a square tensor
         if tensor.shape[-1] != tensor.shape[-2]:
             raise ValueError("The tensor must be square.")
 
-        # tensor (C, H, W)
+        # Get the image size
         xdim = tensor.shape[1]
         ydim = tensor.shape[2]
 
+        # Get the patch size
         minimages_x = int(torch.ceil(torch.tensor(xdim / patch_size)))
         minimages_y = int(torch.ceil(torch.tensor(ydim / patch_size)))
 
+        # pad the tensor to be divisible by the patch size            
         pad_x_01 = int((minimages_x * patch_size - xdim) // 2)
         pad_x_02 = int((minimages_x * patch_size - xdim) - pad_x_01)
 
         pad_y_01 = int((minimages_y * patch_size - ydim) // 2)
         pad_y_02 = int((minimages_y * patch_size - ydim) - pad_y_01)
 
         padded_tensor = torch.nn.functional.pad(
@@ -92,38 +89,45 @@
         pass
 
     @abstractmethod
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         pass
 
     def compute_image(self) -> torch.Tensor:
-        return Metric(value=self._compute_image(self.x, self.y), description=self.name)
+        return self._compute_image(self.x, self.y)
 
     def compute_patch(self) -> torch.Tensor:
+        # Create the patches
         x_batched = self.do_square(self.x, self.patch_size)
         y_batched = self.do_square(self.y, self.patch_size)
+        
+        # Compute the metric for each patch
         metric_result = torch.zeros(x_batched.shape[:2])
-
         xrange, yrange = x_batched.shape[0:2]
-
         for x_index in range(xrange):
             for y_index in range(yrange):
                 x_batch = x_batched[x_index, y_index]
                 y_batch = y_batched[x_index, y_index]
-                metric_result[x_index, y_index] = self._compute_image(x_batch, y_batch)
+                metric_result[x_index, y_index] = self._compute_image(
+                    x_batch, y_batch
+                )
 
         # Go back to the original size
         metric_result = torch.nn.functional.interpolate(
-            metric_result[None, None], size=self.x.shape[-2:], mode="nearest"
+            metric_result[None, None],
+            size=self.x.shape[-2:],
+            mode="bicubic",
+            antialias=True,
+            align_corners=False
         ).squeeze()
-        
-        return Metric(value=metric_result, description=self.name)
+
+        return metric_result
 
     def compute_pixel(self) -> torch.Tensor:
-        return Metric(value=self._compute_pixel(self.x, self.y), description=self.name)
+        return self._compute_pixel(self.x, self.y)
 
     def compute(self) -> torch.Tensor:
         if self.method == "pixel":
             return self.compute_pixel()
         elif self.method == "image":
             return self.compute_image()
         elif self.method == "patch":
@@ -138,43 +142,43 @@
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
     ):
-        super().__init__(x=x, y=y, method=method, patch_size=patch_size, name="KL")
+        super().__init__(x=x, y=y, method=method, patch_size=patch_size)
 
         self.large_number = 1e2
         self.epsilon = 1e-8
 
+    def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         pbias_d = torch.abs(x / (y + self.epsilon))
         pbias_d[pbias_d > self.large_number] = self.large_number
         pbias_d[pbias_d < 1 / self.large_number] = 1 / self.large_number
-
-        self.pbias_d = pbias_d
-
-    def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        return torch.mean(x) * torch.log(torch.mean(self.pbias_d))
+        return torch.mean(x) * torch.log(torch.mean(pbias_d))
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        return torch.mean(x, axis=0) * torch.log(torch.mean(self.pbias_d, axis=0))
+        pbias_d = torch.abs(x / (y + self.epsilon))
+        pbias_d[pbias_d > self.large_number] = self.large_number
+        pbias_d[pbias_d < 1 / self.large_number] = 1 / self.large_number
+        return torch.mean(x, axis=0) * torch.log(torch.mean(pbias_d, axis=0))
 
 
 class L1(DistanceMetric):
     """Spectral information divergence between two tensors"""
 
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
     ):
-        super().__init__(x=x, y=y, method=method, patch_size=patch_size, name="L1")
+        super().__init__(x=x, y=y, method=method, patch_size=patch_size)
 
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         return torch.nanmean(torch.abs(x - y))
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         return torch.nanmean(torch.abs(x - y), axis=0)
 
@@ -185,15 +189,15 @@
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
     ):
-        super().__init__(x=x, y=y, method=method, patch_size=patch_size, name="L2")
+        super().__init__(x=x, y=y, method=method, patch_size=patch_size)
 
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         return torch.nanmean((x - y) ** 2)
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         return torch.nanmean((x - y) ** 2, axis=0)
 
@@ -204,114 +208,101 @@
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
     ):
-        super().__init__(x=x, y=y, method=method, patch_size=patch_size, name="PBIAS")
-
+        super().__init__(x=x, y=y, method=method, patch_size=patch_size)
+        
+        self.large_number = 1e2
+        self.epsilon = 1e-8
+        
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        return torch.nanmean((x - y) ** 2)
+        ratio = torch.abs((x - y) / (y + self.epsilon))
+        ratio[ratio > self.large_number] = self.large_number
+        ratio[ratio < 1 / self.large_number] = 1 / self.large_number
+        return torch.nanmean(ratio)
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        return torch.nanmean((x - y) ** 2, axis=0)
+        ratio = torch.abs((x - y) / (y + self.epsilon))
+        ratio[ratio > self.large_number] = self.large_number
+        ratio[ratio < 1 / self.large_number] = 1 / self.large_number
+        return torch.nanmean(ratio, axis=0)
 
 
-class PSNR(DistanceMetric):
-    """Spectral information divergence between two tensors"""
+class IPSNR(DistanceMetric):
+    """Inverse Peak signal to noise ratio between two tensors"""
 
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
     ):
-        super().__init__(x=x, y=y, method=method, patch_size=patch_size, name="PSNR")
+        super().__init__(x=x, y=y, method=method, patch_size=patch_size)
 
         self.data_range = torch.tensor(1)
         self.epsilon = torch.tensor(1e-10)
 
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         l2_distance = torch.nanmean((x - y) ** 2)
         l2_distance[l2_distance < self.epsilon] = self.epsilon
-        return 10 * torch.log10(self.data_range ** 2 / l2_distance)
+        return 1 / (10 * torch.log10(self.data_range**2 / l2_distance))
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         l2_distance = torch.nanmean((x - y) ** 2, axis=0)
         l2_distance[l2_distance < self.epsilon] = self.epsilon
-        return 1/(10 * torch.log10(self.data_range ** 2 / l2_distance))
+        return 1 / (10 * torch.log10(self.data_range**2 / l2_distance))
 
 
 class SAD(DistanceMetric):
-    """Spectral information divergence between two tensors"""
+    """Spectral Angle distance between two tensors"""
 
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
     ):
-        super().__init__(x=x, y=y, method=method, patch_size=patch_size, name="SAD")
+        super().__init__(x=x, y=y, method=method, patch_size=patch_size)
 
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        dot_product = (x * y).sum(dim=0)
-        preds_norm = x.norm(dim=0)
-        target_norm = y.norm(dim=0)
-        sam_score = torch.clamp(dot_product / (preds_norm * target_norm), -1, 1).acos()
-        return torch.rad2deg(sam_score)
-
-    def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         dot_product = (x * y).squeeze().sum()
         preds_norm = x.squeeze().norm()
         target_norm = y.squeeze().norm()
         sam_score = torch.clamp(dot_product / (preds_norm * target_norm), -1, 1).acos()
         return torch.rad2deg(sam_score)
 
-
-class SAD(DistanceMetric):
-    """Spectral information divergence between two tensors"""
-
-    def __init__(
-        self,
-        x: torch.Tensor,
-        y: torch.Tensor,
-        method: str = "image",
-        patch_size: int = 32,
-    ):
-        super().__init__(x=x, y=y, method=method, patch_size=patch_size, name="SAD")
-
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         dot_product = (x * y).sum(dim=0)
         preds_norm = x.norm(dim=0)
         target_norm = y.norm(dim=0)
         sam_score = torch.clamp(dot_product / (preds_norm * target_norm), -1, 1).acos()
         return torch.rad2deg(sam_score)
 
-    def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        dot_product = (x * y).sum()
-        preds_norm = x.norm()
-        target_norm = y.norm()
-        sam_score = torch.clamp(dot_product / (preds_norm * target_norm), -1, 1).acos()
-        return torch.rad2deg(sam_score)
 
 
 class LPIPS(DistanceMetric):
-    """Spectral information divergence between two tensors"""
+    """Learned Perceptual Image Patch Similarity between two tensors"""
 
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
         device: Union[str, torch.device] = "cpu",
     ):
+        if method == "patch":
+            if patch_size < 32:
+                raise ValueError("The patch size must be at least 32.")
+
         # if extra_requires (setup.py) is not fulfilled, raise error
         check_lpips()
         import lpips
 
         if method == "patch":
             if patch_size < 32:
                 raise ValueError("The patch size must be at least 32.")
@@ -322,143 +313,174 @@
         # Normalize the tensors to [-1, 1]
         y = (y - y.min()) / (y.max() - y.min())
         y = y * 2 - 1
 
         x = (x - x.min()) / (x.max() - x.min())
         x = x * 2 - 1
 
-        super().__init__(x=x, y=y, method=method, patch_size=patch_size, name="LPIPS")
+        super().__init__(x=x, y=y, method=method, patch_size=patch_size)
 
     @torch.no_grad()
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         return self.model(x, y).mean()
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError("LPIPS cannot be computed at pixel level.")
 
 
-class CLIPscore(DistanceMetric):
-    """Estimate the CLIPscore between two tensors"""
+class CLIP(DistanceMetric):
+    """Estimate the CLIP score between two tensors"""
 
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
         device: Union[str, torch.device] = "cpu",
     ):
+        if method == "patch":
+            if patch_size < 32:
+                raise ValueError("The patch size must be at least 32.")
+                    
         # if extra_requires (setup.py) is not fulfilled, raise error
         check_openclip()
-        import open_clip
-
-        if method != "patch":
-            raise ValueError(
-                "CLIPscore can only be computed at patch level of 256x256."
-            )
+        check_huggingface_hub()
 
-        if method == "patch":
-            if patch_size != 256:
-                raise ValueError("The patch size must be 256.")
+        import open_clip
+        from huggingface_hub import hf_hub_download
 
-        # Set the model        
-        self.model = open_clip.create_model_and_transforms(
-            "ViT-B-16-SigLIP-256",
-            pretrained='webli',
-            device=device
-        )[0]
-        
-        # Normalize the tensors
-        normalize = Normalize(
-            mean=(0.48145466, 0.4578275, 0.40821073),
-            std=(0.26862954, 0.26130258, 0.27577711)
+        # Set the model
+        # Copy the pretrained model in the current directory
+        checkpoint_path = hf_hub_download(
+            "chendelong/RemoteCLIP",
+            f"RemoteCLIP-RN50.pt",
+            cache_dir='checkpoints'
         )
-        x_norm = normalize(x)
-        y_norm = normalize(y)
-
+        ckpt = torch.load(checkpoint_path, map_location=device)
+        model, _, preprocess = open_clip.create_model_and_transforms("RN50")
+        model.load_state_dict(ckpt)
+        model.to(device)
+
+        # desactivate the gradients
+        for param in model.parameters():
+            param.requires_grad = False
+
+        # Scale the tensors values to [0, 1]
+        # we found better results with this normalization
+        x_norm = (x - x.min()) / (x.max() - x.min())
+        y_norm = (y - y.min()) / (y.max() - y.min())
+        self.model = model
         super().__init__(
-            x=x_norm, y=y_norm, method=method, patch_size=patch_size, name="CLIPscore"
+            x=x_norm, y=y_norm, method=method, patch_size=patch_size
         )
 
     @torch.no_grad()
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        x_emb = self.model.encode_image(x[None]).squeeze()
-        y_emb = self.model.encode_image(y[None]).squeeze()
+        # Scale image to be always Bx3x224x224
+        if x.shape != (3, 224, 224):
+            x = torch.nn.functional.interpolate(
+                x[None],
+                size=224,
+                mode="bilinear",
+                antialias=True
+            )
+        
+        if y.shape != (3, 224, 224):
+            y = torch.nn.functional.interpolate(
+                y[None],
+                size=224,
+                mode="bilinear",
+                antialias=True
+            )
+        
+        # Run the CLIP model
+        with torch.no_grad():
+            x_emb = self.model.encode_image(x).squeeze()
+            y_emb = self.model.encode_image(y).squeeze()
+
         return torch.nn.functional.l1_loss(x_emb, y_emb)
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        raise NotImplementedError("CLIPscore cannot be computed at pixel level.")
+        raise NotImplementedError("CLIP cannot be computed at pixel level.")
 
 
-
-class CROSSMTF(DistanceMetric):
-    """Spectral information divergence between two tensors"""
+class MTF(DistanceMetric):
+    """Estimate the cross-modulation transfer function between two tensors"""
 
     def __init__(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         method: str = "image",
         patch_size: int = 32,
         scale: int = 4,
     ):
         super().__init__(
-            x=x, y=y, method=method, patch_size=patch_size, name="CROSSMTF"
+            x=x, y=y, method=method, patch_size=patch_size
         )
 
         if method == "patch":
             if patch_size < 32:
                 raise ValueError("The patch size must be at least 32.")
 
         self.scale = scale
 
     def _compute_image(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+        # do computation in cpu to avoid problems with fft
+        x = x.cpu()
+        y = y.cpu()
+
         # Compute mask
         freq = torch.fft.fftfreq(x.shape[-1])
         freq = torch.fft.fftshift(freq)
         kfreq2D = torch.meshgrid(freq, freq, indexing="ij")
         knrm = torch.sqrt(kfreq2D[0] ** 2 + kfreq2D[1] ** 2)
         tensormask = (knrm > (0.5 * 1 / self.scale)) & (knrm < (0.5))
 
         fft_preds = torch.abs(torch.fft.fftshift(torch.fft.fft2(x)))
         fft_target = torch.abs(torch.fft.fftshift(torch.fft.fft2(y)))
 
-        mtf = torch.masked_select(fft_preds / fft_target, tensormask)
+        mtf = torch.masked_select((fft_target - fft_preds) / fft_target, tensormask)
+        mtf = torch.abs(mtf)
 
         return torch.mean(torch.clamp(mtf, 0, 1))
 
     def _compute_pixel(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        raise NotImplementedError("CROSSMTF cannot be computed at pixel level.")
+        raise NotImplementedError("MTF cannot be computed at pixel level.")
+
 
 
 def get_distance(
     x: torch.Tensor,
     y: torch.Tensor,
     method: str,
     agg_method: str,
     patch_size: int = 32,
     scale: int = 4,
     device: Union[str, torch.device] = "cpu",
     rgb_bands: Optional[List[int]] = [0, 1, 2],
 ):
-    """ Estimate the unsystematic error between the SR and HR image.
+    """Estimate the distance between two tensors. All the distances
+    are normalized to be between 0 and n,  where n is the maximum
+
 
     Args:
         x (torch.Tensor): The SR harmonized image (C, H, W).
         hr (torch.Tensor): The HR image (C, H, W).
         method (str): The method to use. Either "psnr" or "cpsnr".
         agg_method (str): The method to use to aggregate the distance.
             Either "pixel", "image", or "patch".
-        patch_size (int, optional): The patch size to use if the patch 
+        patch_size (int, optional): The patch size to use if the patch
             method is used.
         scale (int, optional): The scale of the super-resolution.
-        space_search (int, optional): This parameter is used to search 
-            for the best shift that maximizes the PSNR. By default, it is 
+        space_search (int, optional): This parameter is used to search
+            for the best shift that maximizes the PSNR. By default, it is
             the same as the super-resolution scale.
-        
+
     Returns:
         torch.Tensor: The metric value.
     """
     if x.shape[0] != y.shape[0]:
         raise ValueError("The number of channels in x and y must be the same.")
 
     if x.shape[1] != y.shape[1]:
@@ -468,31 +490,31 @@
         distance_fn = KL(x=x, y=y, method=agg_method, patch_size=patch_size)
     elif method == "l1":
         distance_fn = L1(x=x, y=y, method=agg_method, patch_size=patch_size)
     elif method == "l2":
         distance_fn = L2(x=x, y=y, method=agg_method, patch_size=patch_size)
     elif method == "pbias":
         distance_fn = PBIAS(x=x, y=y, method=agg_method, patch_size=patch_size)
-    elif method == "ipsnr":
-        distance_fn = PSNR(x=x, y=y, method=agg_method, patch_size=patch_size)
+    elif method == "psnr":
+        distance_fn = IPSNR(x=x, y=y, method=agg_method, patch_size=patch_size)
     elif method == "sad":
         distance_fn = SAD(x=x, y=y, method=agg_method, patch_size=patch_size)
-    elif method == "crossmtf":
-        distance_fn = CROSSMTF(
+    elif method == "mtf":
+        distance_fn = MTF(
             x=x, y=y, method=agg_method, patch_size=patch_size, scale=scale
         )
     elif method == "lpips":
         x_rgb = x[rgb_bands, :, :]
         y_rgb = y[rgb_bands, :, :]
         distance_fn = LPIPS(
             x_rgb, y_rgb, method=agg_method, patch_size=patch_size, device=device
         )
     elif method == "clip":
         x_rgb = x[rgb_bands, :, :]
         y_rgb = y[rgb_bands, :, :]
-        distance_fn = CLIPscore(
+        distance_fn = CLIP(
             x_rgb, y_rgb, method=agg_method, patch_size=patch_size, device=device
         )
     else:
         raise ValueError("No valid distance method.")
 
-    return distance_fn
+    return distance_fn.compute()
```

### Comparing `opensr-test-0.2.1/opensr_test/hallucinations.py` & `opensr_test-0.2.9/opensr_test/correctness.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import numpy as np
 import torch
 from opensr_test.distance import get_distance
 
 
 def sigm(x):
@@ -15,88 +15,84 @@
     distance_method: str = "l1",
     agg_method: str = "pixel",
     scale: int = 4,
     patch_size: Optional[int] = 32,
     rgb_bands: Optional[List[int]] = [0, 1, 2],
     device: str = "cpu",
 ):
-    """ Obtain the distances between metrics in a 2D space.
-        In the 2D space the y-axis is the distance between the SR and HR
-        (error) and the x-axis is the distance between the LR and HR 
-        (high-frequency).
+    """ Obtain the distances between the LR, SR and HR images.
         
-
     Args:
         lr_to_hr (torch.Tensor): The LR image upscaled to HR.
         sr_harm (torch.Tensor): The SR image harmonized to HR.
         hr (torch.Tensor): The HR image.
-        distance_method (str, optional): The distance method to use. Defaults to 
-            "psnr". Available methods are: psnr, kl, l1, l2, psnr, sad, lpips.
+        distance_method (str, optional): The distance method to use. 
+            Defaults to "psnr". Available methods are: "kl", "l1", 
+            "l2", "pbias", "psnr", "sad", "mtf", "lpips", "clip".
 
     Returns:
-        torch.Tensor: The distances between the metrics.
+        Tuple[torch.Tensor, torch.Tensor, torch.Tensor]: The distances
+            between the LR and HR, SR and HR, and SR and LR images.
     """
-
     reference = get_distance(
         x=lr_to_hr,
         y=hr,
         method=distance_method,
         agg_method=agg_method,
         patch_size=patch_size,
         device=device,
         scale=scale,
         rgb_bands=rgb_bands,
-    ).compute()
+    )
 
     dist_sr_to_hr = get_distance(
         x=sr_harm,
         y=hr,
         method=distance_method,
         agg_method=agg_method,
         patch_size=patch_size,
         device=device,
         scale=scale,
         rgb_bands=rgb_bands,
-    ).compute()
+    )
 
     dist_sr_to_lr = get_distance(
         x=sr_harm,
         y=lr_to_hr,
         method=distance_method,
         agg_method=agg_method,
         patch_size=patch_size,
         device=device,
         scale=scale,
         rgb_bands=rgb_bands,
-    ).compute()
+    )
 
-    return reference.value, dist_sr_to_hr.value, dist_sr_to_lr.value
+    return reference, dist_sr_to_hr, dist_sr_to_lr
 
 
 def tc_improvement(
     d_im: torch.Tensor,
     d_om: torch.Tensor,
     plambda: float = 0.85
 ) -> torch.Tensor:
-    """ Obtain the relative distance to the center
-    of the improvement space
+    """ Obtain the relative distance to the center of the improvement space
 
     Args:
         d_im (torch.Tensor): The distance to the improvement space
         d_om (torch.Tensor): The distance to the omission space
         plambda (float): The parameter calibrated according to the
             human perception of the quality of the super-resolved
             image. Defaults to 0.85.
 
     Returns:
         torch.Tensor: The relative distance to the center 
         of the improvement space
     """
     H = d_im + d_om -1  
-    return d_im + d_om*(1 - np.exp(-H*plambda))
+    return d_im + d_om*(1 - torch.exp(-H*plambda))
 
 def tc_omission(
     d_im: torch.Tensor,
     d_om: torch.Tensor,
     plambda: float = 0.85
 ) -> torch.Tensor:
     """ Obtain the relative distance to the center
@@ -110,31 +106,32 @@
             image. Defaults to 0.85.
 
     Returns:
         torch.Tensor: The relative distance to the center 
         of the improvement space
     """
     H = d_im + d_om -1  
-    return d_om + d_im*(1 - np.exp(-H*plambda))
+    return d_om + d_im*(1 - torch.exp(-H*plambda))
 
 
 def tc_hallucination(
     d_im: torch.Tensor,
     d_om: torch.Tensor,
     plambda: float = 0.85
 ) -> torch.Tensor:
     """ Obtain the relative distance to the center
-    of the omission space
+    of the hallucination space
 
     Args:
         d_im (torch.Tensor): The distance to the improvement space
         d_om (torch.Tensor): The distance to the omission space
         plambda (float): The parameter calibrated according to the
             human perception of the quality of the super-resolved
             image. Defaults to 0.85.
 
     Returns:
         torch.Tensor: The relative distance to the center 
         of the improvement space
     """
-    Q = np.exp(-d_im * d_om * plambda)
+    Q = torch.exp(-d_im * d_om * plambda)
     return Q
+
```

### Comparing `opensr-test-0.2.1/opensr_test/main.py` & `opensr_test-0.2.9/opensr_test/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,70 @@
 from typing import Any, Optional, Union
 
 import warnings
-
-import opensr_test.plot
 import torch
-from opensr_test.config import (
-    Auxiliar,
-    Config,
-    Consistency,
-    Correctness,
-    Distance,
-    Results,
-)
-from opensr_test.hallucinations import (
-    get_distances,
-    tc_hallucination,
-    tc_improvement,
-    tc_omission,
-)
-from opensr_test.kernels import apply_downsampling, apply_upsampling
-from opensr_test.reflectance import reflectance_metric
-from opensr_test.spatial import (
-    SpatialMetric,
-    spatial_aligment,
-    spatial_model_transform_pixel,
-    spatial_setup_model,
-)
-from opensr_test.spectral import spectral_metric
-from opensr_test.utils import get_zeros_at_edges, hq_histogram_matching, seed_everything
 
+from opensr_test.utils import (
+    apply_downsampling, apply_upsampling,
+    apply_mask, hq_histogram_matching,
+    seed_everything
+)
+from opensr_test.spatial import SpatialMetricAlign
+from opensr_test.config import Config, Results, Consistency, Synthesis, Correctness, Auxiliar
+from opensr_test.distance import get_distance
+from opensr_test.correctness import get_distances, tc_improvement, tc_omission, tc_hallucination
+from opensr_test import plot
 
 class Metrics:
     def __init__(
         self,
         params: Optional[Config] = None,
-        device: Union[str, torch.device, None] = "cpu",        
+        **kwargs
     ) -> None:
-        """ A class to evaluate the performance of a image 
-        enhancement algorithm considering the triplets: LR[input], 
+        """ A class to evaluate the performance of a super
+        resolution algorithms considering the triplets: LR[input],
         SR[enhanced], HR[ground truth].
 
         Args:
             params (Optional[Config], optional): The parameters to
                 setup the opensr-test experiment. Defaults to None.
                 If None, the default parameters are used. See 
                 config.py for more information.
-            device (Union[str, torch.device, None], optional): The
-                device to use. Defaults to "cpu".
         """
         
-
         # Set the parameters
         if params is None:
-            self.params = Config()
+            if kwargs:
+                self.params = Config(**kwargs)
+            else:
+                self.params = Config()
         else:
             self.params = params
+
+        
+            
         
         # If patch size is 1, then the aggregation method must be pixel
         if self.params.patch_size == 1:
             self.params.agg_method = "pixel"
 
         # Global parameters
         self.method = self.params.agg_method
-        self.device = device
+        self.run_setup = True
 
         # Set the spatial grid regulator
         self.apply_upsampling = apply_upsampling
         self.apply_downsampling = apply_downsampling
 
-        # Setup the spatial model
-        self.spatial_model = spatial_setup_model(
-            features=self.params.spatial_features,
-            matcher=self.params.spatial_matcher,
+        # Set the spatial aligner
+        self.spatial_aligner = SpatialMetricAlign(
+            method=self.params.spatial_method,
+            max_translations=self.params.spatial_threshold_distance,
             max_num_keypoints=self.params.spatial_max_num_keypoints,
-            device=device,
+            device=self.params.device
         )
 
         # Initial triplets: LR[input], SR[enhanced], HR[ground truth]
         self.lr = None
         self.sr = None
         self.hr = None
 
@@ -90,17 +77,14 @@
         # to evaluate the spectral information in the HR space.
         self.lr_to_hr = None
 
         # The SR in the LR space: (C, H*scale, W*scale) -> (C, H, W)
         # using a bilinear interpolation (zero-parameter model).
         self.sr_to_lr = None
 
-        # The landuse map (H, W)
-        self.landuse = None
-
         # The scale value of the experiment. Obtained from the
         # ratio between the HR and LR image sizes.
         self.scale_factor = None
 
         # RGB pairs (used for plotting and some metrics [spatial
         # & perceptual])
         self.lr_RGB = None
@@ -134,62 +118,56 @@
         self.om_percentage = None
         self.im_percentage = None
 
     def setup(
         self,
         lr: torch.Tensor,
         sr: torch.Tensor,
-        hr: torch.Tensor,
-        landuse: Optional[torch.Tensor] = None
+        hr: torch.Tensor
     ) -> None:
         """ Obtain the performance metrics of the SR image.
 
         Args:
             lr (torch.Tensor): The LR image as a tensor (C, H, W).
             sr (torch.Tensor): The SR image as a tensor (C, H, W).
             hr (torch.Tensor): The HR image as a tensor (C, H, W).
         """
         # Check if SR has gradients
         if sr.requires_grad:
             raise ValueError("The SR image must not have gradients.")
 
-        # If patch size is higher than the image size, then
-        # return an error.
+        # If patch size is higher than the image size, then return an error.
         if self.params.patch_size is not None:
             if (self.params.patch_size > sr.shape[1]) or (self.params.patch_size > sr.shape[2]):
                 raise ValueError("The patch size must be lower than the image size.")
 
         # Obtain the scale factor
         scale_factor = hr.shape[-1] / lr.shape[-1]
         if not scale_factor.is_integer():
             raise ValueError("The scale factor must be an integer.")
         self.scale_factor = int(scale_factor)
 
         # Move all the images to the same device
-        self.lr = self.apply_mask(lr.to(self.device), self.params.mask // self.scale_factor)
-        self.sr = self.apply_mask(sr.to(self.device), self.params.mask)
-        self.hr = self.apply_mask(hr.to(self.device), self.params.mask)
-        self.landuse = self.apply_mask(landuse.to(self.device), self.params.mask // self.scale_factor) if landuse is not None else None
-
+        self.lr = apply_mask(lr.to(self.params.device), self.params.border_mask // self.scale_factor)
+        self.sr = apply_mask(sr.to(self.params.device), self.params.border_mask)
+        self.hr = apply_mask(hr.to(self.params.device), self.params.border_mask)
 
         # Obtain the LR in the HR space
         if self.scale_factor > 1:
             self.lr_to_hr = self.apply_downsampling(
-                X=self.lr[None], 
-                scale=self.scale_factor, 
-                method=self.params.downsample_method
+                x=self.lr[None], 
+                scale=self.scale_factor
             ).squeeze(0)
         else:
             self.lr_to_hr = self.lr
 
         # Obtain the SR in the LR space
         self.sr_to_lr = self.apply_upsampling(
-            X=self.sr,
-            scale=self.scale_factor,
-            method=self.params.upsample_method
+            x=self.sr,
+            scale=self.scale_factor
         ).squeeze(0)
 
         # Obtain the RGB images
         if self.lr.shape[0] >= 3:
             self.lr_RGB = self.lr[self.params.rgb_bands]
             self.hr_RGB = self.hr[self.params.rgb_bands]
             self.sr_RGB = self.sr[self.params.rgb_bands]
@@ -200,429 +178,441 @@
             self.hr_RGB = self.hr[0][None]
             self.sr_RGB = self.sr[0][None]
             self.lr_to_hr_RGB = self.lr_to_hr[0][None]
             self.sr_to_lr_RGB = self.sr_to_lr[0][None]
 
         return None
 
+
     def sr_harm_setup(self) -> None:
-        """ Remove the systematic error from the SR image.
+        """ Remove the systematic error from the SR image. After
+        super-resolving an image, the SR image may contain systematic
+        errors. These errors are removed to only evaluate the high-frequency
+        information added after the super-resolution process.
                         
         Returns:
             torch.Tensor: The SR image without systematic error.        
         """
 
         # Remove systematic reflectance error
         if self.params.harm_apply_spectral:
             sr_harm = hq_histogram_matching(self.sr, self.hr)
         else:            
             sr_harm = self.sr
 
+        # Remove systematic spatial error
         if self.params.harm_apply_spatial:
-            sr_harm, matching_points, spatial_offset = spatial_aligment(
-                sr=sr_harm,
-                hr=self.hr,
-                spatial_model=self.spatial_model,
-                threshold_n_points=self.params.spatial_threshold_npoints,
-                threshold_distance=self.params.spatial_threshold_distance,
-                rgb_bands=self.params.rgb_bands,
-            )
-            self.matching_points_02 = matching_points
+            sr_harm = self.spatial_aligner.get_metric(sr_harm, self.hr)[0]
         else:
-            self.sr_harm = sr_harm
-            self.matching_points_02 = False
+            sr_harm = sr_harm
 
-        # Remove the black edges
-        xmin, xmax, ymin, ymax = get_zeros_at_edges(sr_harm, self.scale_factor)
-        self.sr_harm = sr_harm[:, xmin: xmax, ymin: ymax]
-        self.lr_to_hr = self.lr_to_hr[:, xmin: xmax, ymin: ymax]
-        self.sr = self.sr[:, xmin: xmax, ymin: ymax]
-        self.hr = self.hr[:, xmin: xmax, ymin: ymax]
-        self.hr_RGB = self.hr[self.params.rgb_bands]
-        self.lr = self.lr[:, xmin//self.scale_factor: xmax//self.scale_factor, ymin//self.scale_factor: ymax//self.scale_factor]
-        self.lr_RGB = self.lr[self.params.rgb_bands]
+        self.sr_harm = sr_harm
 
-        if self.lr.shape[0] >= 3:
-            self.sr_harm_RGB = self.sr_harm[self.params.rgb_bands]
+        # Obtain the RGB images
+        if self.sr_harm.shape[0] >= 3:
+            self.sr_harm_RGB = sr_harm[self.params.rgb_bands]
         else:
-            self.sr_harm_RGB = self.sr_harm[0][None]
+            self.sr_harm_RGB = sr_harm[0][None]
 
-    def _reflectance_metric(self) -> None:
+    def _reflectance_distance(self) -> None:
         """ Estimate the spectral global error by comparing the
         reflectance of the LR and SR images.
         
         Returns:
-            Value: The spectral global error.
+            Value: The reflectance global error.
         """        
-        self.reflectance_value = reflectance_metric(
-            lr=self.lr,
-            sr_to_lr=self.sr_to_lr,
-            metric=self.params.reflectance_method,
+        self.reflectance_error = get_distance(
+            x=self.lr,
+            y=self.sr_to_lr,
+            method=self.params.reflectance_distance,
             agg_method=self.params.agg_method,
             patch_size=self.params.patch_size,
+            scale=self.scale_factor
         )
-
-    def _spectral_metric(self) -> None:
-        """ Estimate the spectral local error by comparing the
+    
+    def _spectral_distance(self) -> None:
+        """ Estimate the spectral global error by comparing the
         reflectance of the LR and SR images.
-
+        
         Returns:
-            float: The spectral local error.
+            Value: The spectral global error.
         """
-        self.spectral_value = spectral_metric(
-            lr=self.lr,
-            sr_to_lr=self.sr_to_lr,
-            metric=self.params.spectral_method,
+        self.spectral_error = get_distance(
+            x=self.lr,
+            y=self.sr_to_lr,
+            method=self.params.spectral_distance,
             agg_method=self.params.agg_method,
             patch_size=self.params.patch_size,
+            scale=self.scale_factor
         )
-
-    def _spatial_metric(self) -> None:
-        """ Estimate the spatial error by comparing the
-        spatial information of the LR and SR images.
+    
+    def _spatial_alignment(self) -> None:
+        """ Estimate the spatial global error by comparing the
+        spatial alignment of the SR and HR images.
         
         Returns:
-            Value: The spatial error.
+            Value: The spatial global error.
         """
-        # Spatial parameters that control the set of
-        # point used to fit the LINEAR spatial model.
-        threshold_distance = self.params.spatial_threshold_distance
-        threshold_npoints = self.params.spatial_threshold_npoints
-        spatial_description = "%s & %s" % (
-            self.params.spatial_features,
-            self.params.spatial_matcher,
-        )
-
-        spatial_metric_result = SpatialMetric(
-            x=self.lr_RGB,
-            y=self.sr_to_lr_RGB,
-            spatial_model=self.spatial_model,
-            name=spatial_description,
-            threshold_n_points=threshold_npoints,
-            threshold_distance=threshold_distance,
-            method="pixel",
-            patch_size=self.params.patch_size,
-            device=self.device,
-        )
+        self.spatial_error = self.spatial_aligner.get_metric(
+            self.lr_RGB, self.sr_to_lr_RGB
+        )[1]
 
-        self.spatial_aligment_value = spatial_metric_result.compute()
-        self.matching_points_01 = spatial_metric_result.matching_points
+    def _create_mask(
+        self,
+        d_ref: torch.Tensor,
+        d_im: torch.Tensor,
+        d_om: torch.Tensor,
+        gradient_threshold: Union[float, str] = "auto"
+    ) -> None:
+        """ The goal of this mask is to avoid the pixels with
+        gradients below a certain threshold. This mask is always
+        created using l1 distance at pixel level.
 
-    def _create_mask(self, stability_threshold: float = 0.) -> None:
-        d_ref, d_im, d_om = get_distances(
-            lr_to_hr=self.lr_to_hr,
-            sr_harm=self.sr_harm,
-            hr=self.hr,
-            distance_method="l1",
-            agg_method="pixel"
-        )
+
+        Args:
+            stability_threshold (float, optional): The threshold
+                to avoid the pixels with gradients below this value.
+                Defaults to 0.05.
+
+        Returns:
+            torch.Tensor: The mask to avoid the pixels with gradients
+                below a certain threshold.
+        """
+
+        # Get the optimal threshold based on quantiles
+        if isinstance(gradient_threshold, str):
+            if gradient_threshold == "auto":
+                gradient_threshold = "auto75"
+            t1 = int(gradient_threshold.replace("auto", ""))/100
+            gradient_threshold = d_ref.flatten().kthvalue(
+                int(t1 * d_ref.numel())
+            ).values.item()
 
         # create mask
-        mask1 = (d_ref > stability_threshold)*1
-        mask2 = (d_im > stability_threshold)*1
-        mask3 = (d_om > stability_threshold)*1
+        mask1 = (d_ref > gradient_threshold)*1
+        mask2 = (d_im > gradient_threshold)*1
+        mask3 = (d_om > gradient_threshold)*1
         mask = ((mask1 + mask2 + mask3) > 0) * 1.0
         mask[mask == 0] = torch.nan
-        self.tc_mask = mask
         return mask
 
-    def _distance_metric(self, stability_threshold: float = 0.) -> None:
-        self.d_ref, self.d_im, self.d_om = get_distances(
+
+    def consistency(
+        self,
+        lr: torch.Tensor,
+        sr: torch.Tensor
+    ) -> None:
+        """ Obtain the consistency metrics trough comparing the 
+        LR and SR images.
+
+        Args:
+            lr (torch.Tensor): The LR image as a tensor (C, H, W).
+            sr (torch.Tensor): The SR image as a tensor (C, H, W).
+            run_setup (bool, optional): Run the setup method. 
+                Defaults to True.
+        """
+        # Make the experiment reproducible
+        seed_everything(42)
+        
+        # Setup the LR and SR images
+        self.setup(lr=lr, sr=sr, hr=sr)
+
+        # Run the consistency metrics
+        self._reflectance_distance()
+        self._spectral_distance()
+        self._spatial_alignment()
+
+        return {
+            "reflectance": self.reflectance_error.nanmean().item(),
+            "spectral": self.spectral_error.nanmean().item(),
+            "spatial": self.spatial_error.nanmean().item()
+        }
+        
+
+    def synthesis(
+        self,
+        lr: torch.Tensor,
+        sr: torch.Tensor,
+        hr: Optional[torch.Tensor] = None
+    ) -> None:
+        """ Obtain the synthesis metrics trough comparing the
+        LR, SR, and HR images.
+
+        Args:
+            lr (torch.Tensor): The LR image as a tensor (C, H, W).
+            sr (torch.Tensor): The SR image as a tensor (C, H, W).
+            hr (Optional[torch.Tensor], optional): The HR image as a 
+                tensor (C, H, W). Defaults to None. If HR is set the
+                SR is first harmonized using the HR image as a 
+                reference. To deactivate harmonization, modify the
+                Config object.
+        """
+        
+        if hr is None:
+                self.setup(lr=lr, sr=sr, hr=sr)
+        else:
+                self.setup(lr=lr, sr=sr, hr=hr)
+            
+        # Obtain the SR image without systematic error
+        self.sr_harm_setup()
+        
+        # Obtain the distance between the SR and HR images
+        self.synthesis_distance_value = get_distance(
+            x=self.lr_to_hr,
+            y=self.sr_harm,
+            method=self.params.synthesis_distance,
+            agg_method=self.params.agg_method,
+            patch_size=self.params.patch_size,
+            scale=self.scale_factor
+        )
+
+        return {
+            "synthesis": self.synthesis_distance_value.nanmean().item()
+        }
+    
+    def correctness(
+        self,
+        lr: torch.Tensor,
+        sr: torch.Tensor,
+        hr: torch.Tensor,
+        gradient_threshold: float = 0.1
+    ) -> None:
+        """ Obtain the correctness metrics trough comparing the
+        LR, SR, and HR images.
+
+        Args:
+            lr (torch.Tensor): The LR image as a tensor (C, H, W).
+            sr (torch.Tensor): The SR image as a tensor (C, H, W).
+            hr (torch.Tensor): The HR image as a tensor (C, H, W).
+            gradient_threshold (float, optional): Ignore the pixels
+                with gradients below this threshold. Defaults to 0.1.
+        """
+
+        # Make the experiment reproducible
+        seed_everything(42)
+        
+        # Setup the LR, SR, and HR images
+        self.setup(lr=lr, sr=sr, hr=hr)
+        self.sr_harm_setup()
+
+        # Obtain the distance between the LR, SR, and HR images
+        d_ref, d_im, d_om = get_distances(
             lr_to_hr=self.lr_to_hr,
             sr_harm=self.sr_harm,
             hr=self.hr,
-            distance_method=self.params.distance_method,
+            distance_method=self.params.correctness_distance,
             agg_method=self.params.agg_method,
+            scale=self.scale_factor,
             patch_size=self.params.patch_size,
             rgb_bands=self.params.rgb_bands,
-            device=self.device,
+            device=self.params.device
         )
 
-        # Apply mask
-        mask = self._create_mask(stability_threshold)
+        # Apply the mask to remove the pixels with gradients 
+        mask = self._create_mask(
+            d_ref=d_ref,
+            d_im=d_im,
+            d_om=d_om,
+            gradient_threshold=gradient_threshold
+        )
         self.potential_pixels = torch.nansum(mask)
-        self.d_ref_masked = self.d_ref * mask
-        self.d_im_masked = self.d_im * mask
-        self.d_om_masked = self.d_om * mask
-
+        self.d_ref = d_ref * mask
+        self.d_im =  d_im * mask
+        self.d_om =  d_om * mask
+        
         # Compute relative distance
-        self.d_im_ref = self.d_im_masked / self.d_ref_masked
-        self.d_om_ref = self.d_om_masked / self.d_ref_masked
-
-        if sum(self.d_im_ref.shape) == 0:
-            self.d_im_ref = self.d_im_ref.reshape(-1)
-            self.d_om_ref = self.d_om_ref.reshape(-1)
+        self.d_im_ref = self.d_im / self.d_ref
+        self.d_om_ref = self.d_om / self.d_ref
 
-    def _improvement(self, im_score: float = 0.80) -> None:
-        self.improvement = tc_improvement(
+        # Estimate Hallucination
+        self.hallucination = tc_hallucination(
             d_im=self.d_im_ref,
             d_om=self.d_om_ref,
-            plambda=im_score
+            plambda=self.params.ha_score
         )
 
-    def _omission(self, om_score: float = 0.80) -> None:
+        # Estimate Omission
         self.omission = tc_omission(
             d_im=self.d_im_ref,
             d_om=self.d_om_ref,
-            plambda=om_score
+            plambda=self.params.om_score
         )
 
-    def _hallucination(self, ha_score: float = 0.80) -> None:
-        self.hallucination = tc_hallucination(
+        # Estimate Improvement
+        self.improvement = tc_improvement(
             d_im=self.d_im_ref,
             d_om=self.d_om_ref,
-            plambda=ha_score
+            plambda=self.params.im_score
         )
-        
-        correctness_stack = torch.stack([
+
+        # Classify the pixels based on the distance
+        tensor_stack = torch.stack([
             self.improvement,
             self.omission,
             self.hallucination
         ], dim=0)
-        
-        self.classification = torch.argmin(correctness_stack, dim=0) * self.tc_mask
-        
+        self.classification = torch.argmin(tensor_stack, dim=0) * mask
+
+        # Get the percentage of omission, improvement, and hallucination
         self.im_percentage = torch.sum(self.classification==0) / self.potential_pixels
         self.om_percentage = torch.sum(self.classification==1) / self.potential_pixels
-        self.ha_percentage = torch.sum(self.classification==2) / self.potential_pixels
-
-    def _prepare(self) -> None:
-        self.results = Results(
-            consistency=Consistency(
-                reflectance=dict(self.reflectance_value),
-                spectral=dict(self.spectral_value),
-                spatial=dict(self.spatial_aligment_value),
-            ),
-            distance=Distance(
-                lr_to_hr=self.d_ref,
-                sr_to_hr=self.d_im,
-                sr_to_lr=self.d_om
-            ),
-            correctness=Correctness(
-                omission=self.omission,
-                improvement=self.improvement,
-                hallucination=self.hallucination,
-                classification=self.classification
-            ),
-            auxiliar=Auxiliar(
-                sr_harm=self.sr_harm,
-                lr_to_hr=self.lr_to_hr,
-                matching_points_lr=self.matching_points_01,
-                matching_points_hr=self.matching_points_02,
-            ),
-        )
-    
-    def summary(self) -> dict:
+        self.ha_percentage = torch.sum(self.classification==2) / self.potential_pixels        
+            
         return {
-            "reflectance": float(self.reflectance_value.value.nanmean()),
-            "spectral": float(self.spectral_value.value.nanmean()),
-            "spatial": float(self.spatial_aligment_value.value.nanmean()),
-            "synthesis": float(self.d_om.nanmean()),
-            "ha_percent": float(self.ha_percentage),
-            "om_percent": float(self.om_percentage),
-            "im_percent": float(self.im_percentage),
+            "ha_percent": self.ha_percentage.item(),
+            "om_percent": self.om_percentage.item(),
+            "im_percent": self.im_percentage.item()
         }
 
     def compute(
         self,
         lr: torch.Tensor,
         sr: torch.Tensor,
-        hr: Optional[torch.Tensor] = None,
-        landuse: Optional[torch.Tensor] = None,
-        stability_threshold: Optional[float] = 0.01,
-        im_score: Optional[float] = 0.8,
-        om_score: Optional[float] = 0.8,
-        ha_score: Optional[float] = 0.8,
+        hr: torch.Tensor,
+        gradient_threshold: Optional[Union[float, str]] = "auto"
     ) -> None:
-
         """ Obtain the performance metrics of the SR image.
-        
+
         Args:
             lr (torch.Tensor): The LR image as a tensor (C, H, W).
             sr (torch.Tensor): The SR image as a tensor (C, H, W).
             hr (torch.Tensor): The HR image as a tensor (C, H, W).
-            grid (Optional[bool], optional): Whether to return the
-                metrics as grids or not. Defaults to False.
-            only_value (Optional[bool], optional): Whether to return
-                only the values of the metrics or the full Value 
-                object (with description). Defaults to True.
-                
-        Returns:
-            dict: The performance metrics for the SR image.
+            gradient_threshold (float, optional): Ignore the pixels
+                with gradients below this threshold. Defaults "auto",
+                which means that the threshold is automatically
+                generated based on LR-HR distance.
         """
+        # Make the experiment reproducible
         seed_everything(42)
         
-        # Run the setup
-        if hr is None:
-            self.setup(lr=lr, sr=sr, hr=sr, landuse=landuse)
-        else:
-            self.setup(lr=lr, sr=sr, hr=hr, landuse=landuse)
-
-        # Obtain the RS metrics
-        self._reflectance_metric()
-        self._spectral_metric()
-        self._spatial_metric()
-        
-        # Create SR' without systematic error
-        self.sr_harm_setup()
-        
-        # Obtain the distance metrics
-        self._distance_metric(stability_threshold)
+        # Obtain the correctness metrics
+        correctness = self.correctness(
+            lr=lr,
+            sr=sr,
+            hr=hr,
+            gradient_threshold=gradient_threshold
+        )
 
-        # Obtain the improvement metrics
-        self._improvement(im_score)
+        # Obtain the consistency metrics
+        consistency = self.consistency(lr=lr, sr=sr)
 
-        # Obtain the omission metrics
-        self._omission(om_score)
+        # Obtain the synthesis metrics
+        synthesis = self.synthesis(lr=lr, sr=sr, hr=hr)
 
-        # Obtain the hallucination metrics
-        self._hallucination(ha_score)
-        
         # Prepare the results
         self._prepare()
 
-        if hr is None:
-            methods = ["reflectance", "spectral", "spatial"]
-            return {k: self.summary()[k] for k in methods}
-        else:
-            return self.summary()
-
+        # merge the results
+        consistency.update(synthesis)
+        consistency.update(correctness)
+        
+        return consistency
+    
+    def _prepare(self) -> None:
+        self.results = Results(
+            consistency=Consistency(
+                reflectance=self.reflectance_error,
+                spectral=self.spectral_error,
+                spatial=self.spatial_error
+            ),
+            synthesis=Synthesis(
+                distance=self.synthesis_distance_value
+            ),
+            correctness=Correctness(
+                omission=self.omission,
+                improvement=self.improvement,
+                hallucination=self.hallucination,
+                classification=self.classification
+            ),
+            auxiliar=Auxiliar(
+                sr_harm=self.sr_harm,
+                lr_to_hr=self.lr_to_hr,
+                d_ref=self.d_ref,
+                d_im=self.d_im,
+                d_om=self.d_om
+            )
+        )
+    
     def plot_triplets(self, stretch: Optional[str] = "linear"):
-        return opensr_test.plot.triplets(
-            lr_img=self.lr_RGB,
-            sr_img=self.sr_harm_RGB,
-            hr_img=self.hr_RGB,
+        return plot.triplets(
+            lr_img=self.lr_RGB.to("cpu"),
+            sr_img=self.sr_harm_RGB.to("cpu"),
+            hr_img=self.hr_RGB.to("cpu"),
             stretch=stretch,
         )
-
-    def plot_quadruplets(
-        self, apply_harm: bool = True, stretch: Optional[str] = "linear"
-    ):
-        return opensr_test.plot.quadruplets(
-                lr_img=self.lr_RGB,
-                sr_img=self.sr_RGB,
-                hr_img=self.hr_RGB,
-                landuse_img=self.landuse,
-                stretch=stretch,
-            )
     
-    def plot_spatial_matches(self, stretch: Optional[str] = "linear"):
-        
-        # Retrieve the linear affine model and the matching points
-        if self.results.auxiliar.matching_points_lr is False:
-            warnings.warn("Spatial model is nan. No spatial matches will be plotted.")
-            return None
-
-        matching_points = self.results.auxiliar.matching_points_lr
-
-        # plot it!
-        return opensr_test.plot.spatial_matches(
-            lr=self.lr_RGB,
-            sr_to_lr=self.sr_to_lr_RGB,
-            points0=matching_points["points0"],
-            points1=matching_points["points1"],
-            matches01=matching_points["matches01"],
-            threshold_distance=self.params.spatial_threshold_distance,
-            stretch=stretch,
-        )        
-
     def plot_summary(self, stretch: Optional[str] = "linear"):
         contion1 = self.params.agg_method == "pixel"
         contion2 = self.method == "patch"
-        if (contion1 and contion2):
+        if not (contion1 or contion2):
             raise ValueError(
-                "This method only works for pixel and patch evaluation."
+                "This method is only available for the "
+                "pixel and patch aggregation methods."
             )
-
+        
         # Reflectance metric
-        e1 = self.results.consistency.reflectance.value
-        e1_title = self.results.consistency.reflectance.description
+        e1 = self.results.consistency.reflectance
+        e1_title = "Reflectance (%s)" % self.params.reflectance_distance
         e1_subtitle = "%.04f" % float(e1.nanmean())
 
         # Spectral metric
-        e2 = self.results.consistency.spectral.value
-        e2_title = self.results.consistency.spectral.description
+        e2 = self.results.consistency.spectral
+        e2_title = "Spectral (%s)" % self.params.spectral_distance
         e2_subtitle = "%.04f" % float(e2.nanmean())
-
-        # Spatial error
-        e3 = self.results.consistency.spatial.value
-        e3_p_np = (
-            self.results.auxiliar.matching_points_lr["points0"]
-            .clone()
-            .detach()
-            .cpu()
-            .numpy()
-        )
-
-        # if patch, then divide by the scale factor
-        e3_points = [list(x.flatten().astype(int)) for x in e3_p_np]
-        e3_title = self.results.consistency.spatial.description
+        
+        # Distance to omission space
+        e3 = self.results.correctness.omission
+        e3_title = "Omission"
         e3_subtitle = "%.04f" % float(e3.nanmean())
 
-        # High frequency
-        e4 = self.results.distance.sr_to_lr
-        e4_title = self.params.distance_method.upper()
+        # Distance to improvement space
+        e4 = self.results.correctness.improvement
+        e4_title = "Improvement"
         e4_subtitle = "%.04f" % float(e4.nanmean())
 
-        # Error grids
-        e5 = self.results.distance.sr_to_hr
-        e5_title = self.params.distance_method.upper()
+        # Distance to hallucination space
+        e5 = self.results.correctness.hallucination
+        e5_title = "Hallucination"
         e5_subtitle = "%.04f" % float(e5.nanmean())
 
         # Plot high frequency
-        fig, axs = opensr_test.plot.display_results(
-            lr=self.lr_RGB,
-            lrdown=self.lr_to_hr_RGB,
-            sr=self.sr_RGB,
-            srharm=self.sr_harm_RGB,
-            hr=self.hr_RGB,
-            e1=e1,
-            e2=e2,
-            e3=e3,
-            e4=e4,
-            e5=e5,
+        fig, axs = plot.display_results(
+            lr=self.lr_RGB.to("cpu"),
+            lrdown=self.lr_to_hr_RGB.to("cpu"),
+            sr=self.sr_RGB.to("cpu"),
+            srharm=self.sr_harm_RGB.to("cpu"),
+            hr=self.hr_RGB.to("cpu"),
+            e1=e1.to("cpu"),
+            e2=e2.to("cpu"),
+            e3=e3.to("cpu"),
+            e4=e4.to("cpu"),
+            e5=e5.to("cpu"),
             e1_title=e1_title,
             e2_title=e2_title,
             e3_title=e3_title,
             e4_title=e4_title,
             e5_title=e5_title,
             e1_subtitle=e1_subtitle,
             e2_subtitle=e2_subtitle,
             e3_subtitle=e3_subtitle,
             e4_subtitle=e4_subtitle,
             e5_subtitle=e5_subtitle,
-            e3_points=e3_points,
-            stretch=stretch,
-        )
+            stretch=stretch
+        )        
         return fig, axs
 
     def plot_tc(
-        self, 
+        self,
         log_scale: Optional[bool] = True,
         stretch: Optional[str] = "linear"
     ):
-        return opensr_test.plot.display_tc_score(
-            sr_rgb=self.sr_harm_RGB,
-            d_im_ref=self.d_im_ref,
-            d_om_ref=self.d_om_ref,
-            tc_score=self.classification,
+        return plot.display_tc_score(
+            sr_rgb=self.sr_harm_RGB.to("cpu"),
+            d_im_ref=self.d_im_ref.to("cpu"),
+            d_om_ref=self.d_om_ref.to("cpu"),
+            tc_score=self.classification.to("cpu"),
             log_scale=log_scale,
             stretch=stretch
         )
 
     def __call__(self) -> Any:
-        return self.compute()
-
-    def apply_mask(self, X: torch.Tensor, mask: int) -> torch.Tensor:
-        if mask is None:
-            return X
-        
-        if mask == 0:
-            return X
-        
-        # C, H, W
-        if len(X.shape) == 3:
-            return X[:, mask: -mask, mask: -mask]
-        elif len(X.shape) == 2:
-            return X[mask: -mask, mask: -mask]
-        else:
-            raise ValueError("The tensor must be 2D or 3D.")
+        return self.compute()
```

### Comparing `opensr-test-0.2.1/opensr_test/plot.py` & `opensr_test-0.2.9/opensr_test/plot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Dict, Optional, Tuple
 
 import matplotlib.colors as colors
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
-from opensr_test.lightglue import viz2d
 from skimage import exposure
 
 
 def min_max_range(tensor):
     """ 
     Return the min and max range of a tensor
     """
@@ -77,125 +76,14 @@
         container.append(img_rescale)
     new_img = np.array(container)
     if permute:
         new_img = np.moveaxis(new_img, 0, -1)
     return torch.from_numpy(new_img).float()
 
 
-def quadruplets(
-    lr_img: torch.Tensor,
-    sr_img: torch.Tensor,
-    hr_img: torch.Tensor,
-    landuse_img: Optional[torch.Tensor] = None,
-    stretch: Optional[str] = "linear",
-) -> Tuple[plt.figure, plt.Axes]:
-    """ Display LR, SR, HR and Landuse images in a single figure.
-
-    Args:
-        lr_img (torch.Tensor): The LR RGB (3xHxW) image.
-        sr_img (torch.Tensor): The SR RGB (3xHxW) image.
-        hr_img (torch.Tensor): The HR RGB (3xHxW) image.
-        landuse_img (torch.Tensor): The landuse grayscale (HxW) image.
-            Optional, defaults to None.
-        stretch (Optional[str], optional): Option to stretch the values 
-            to increase contrast: "lin" (linear) or "hist" (histogram)
-
-    Raises:
-        ValueError: The LR image must be a RGB (3xHxW) image.
-        ValueError: The SR image must be a RGB (3xHxW) image.
-        ValueError: The HR image must be a RGB (3xHxW) image.
-        ValueError: The landuse image must be a grayscale (HxW) image.
-
-    Returns:
-        Tuple[plt.figure, plt.Axes]: The figure and axes to plot.
-    """
-    if lr_img.shape[0] == 4:
-        raise ValueError("The LR image must be a RGB (3xHxW) image.")
-    if sr_img.shape[0] == 4:
-        raise ValueError("The SR image must be a RGB (3xHxW) image.")
-    if hr_img.shape[0] == 4:
-        raise ValueError("The HR image must be a RGB (3xHxW) image.")
-
-    if landuse_img is None:
-        return triplets(lr_img, sr_img, hr_img, stretch=stretch)
-
-    # Apply the stretch
-    if stretch == "linear":
-        lr_img = linear_fix(lr_img)
-        sr_img = linear_fix(sr_img)
-        hr_img = linear_fix(hr_img)
-    elif stretch == "histogram":
-        lr_img = equalize_hist(lr_img)
-        sr_img = equalize_hist(sr_img)
-        hr_img = equalize_hist(hr_img)
-
-    # Define the categorical values and colors
-    values = [10, 20, 30, 40, 50, 60, 70, 80, 90, 95, 100]
-    colors_list = [
-        "#006400",
-        "#ffbb22",
-        "#ffff4c",
-        "#f096ff",
-        "#fa0000",
-        "#b4b4b4",
-        "#f0f0f0",
-        "#0064c8",
-        "#0096a0",
-        "#00cf75",
-        "#fae6a0",
-    ]
-    labels = [
-        "Tree cover (10)",
-        "Shrubland (20)",
-        "Grassland (30)",
-        "Cropland (40)",
-        "Built-up (50)",
-        "Bare / sparse vegetation (60)",
-        "Snow and ice (70)",
-        "Permanent water bodies (80)",
-        "Herbaceous wetland (90)",
-        "Mangroves (95)",
-        "Moss and lichen (100)",
-    ]
-
-    # Set bounds and ticks
-    bounds = [values[i] - 2.5 for i in range(len(values))]
-    bounds.append(values[-1] + 2.5)
-    ticks = [values[i] for i in range(len(values))]
-
-    # Create a iterable colormap
-    cmap = colors.ListedColormap(colors_list)
-    norm = colors.BoundaryNorm(bounds, cmap.N)
-    sm = plt.cm.ScalarMappable(cmap=cmap, norm=norm)
-    sm.set_array([])
-
-    # Plot the images
-    scale_factor = hr_img.shape[0] / lr_img.shape[0]
-    fig, axs = plt.subplots(1, 4, figsize=(25, 5))
-    axs[0].imshow(lr_img)
-    axs[0].set_title("LR")
-    axs[1].imshow(sr_img)
-    axs[1].set_title("SR")
-    axs[2].imshow(hr_img)
-    axs[2].set_title("HR")
-    axs[3].imshow(landuse_img, cmap=cmap, interpolation="nearest", norm=norm)
-    axs[3].set_title("LandUse")
-
-    # Add the colorbar
-    cbar_ax = axs[0].inset_axes([1.05, 0, 0.05, 1], transform=axs[3].transAxes)
-    cbar = fig.colorbar(sm, cax=cbar_ax, ticks=ticks, boundaries=bounds)
-    cbar.ax.set_yticklabels(labels)
-
-    # Add the suptitle
-    fig.suptitle("Scale factor: %.2f" % scale_factor, fontsize=16)
-
-    # return the figure to plot
-    return fig, axs
-
-
 def triplets(
     lr_img: torch.Tensor,
     sr_img: torch.Tensor,
     hr_img: torch.Tensor,
     stretch: Optional[str] = "linear",
 ) -> Tuple[plt.figure, plt.Axes]:
     """ Display LR, SR, HR and Landuse images in a single figure.
@@ -250,58 +138,27 @@
     # Add the suptitle
     fig.suptitle("Scale factor: %.2f" % scale_factor, fontsize=16)
     
     # return the figure to plot
     return fig, axs
 
 
-def spatial_matches(
-    lr: torch.Tensor,
-    sr_to_lr: torch.Tensor,
-    points0: torch.Tensor,
-    points1: torch.Tensor,
-    matches01: Dict[str, torch.Tensor],
-    threshold_distance: Optional[int] = 5,
-    stretch: Optional[str] = "linear",
-):
-
-    if stretch == "linear":
-        sr_to_lr = linear_fix(sr_to_lr, permute=False)
-        lr = linear_fix(lr, permute=False)
-    elif stretch == "histogram":
-        sr_to_lr = equalize_hist(sr_to_lr, permute=False)
-        lr = equalize_hist(lr, permute=False)
-
-    # if the distance between the points is higher than
-    # threshold_distance pixels, it is considered a bad match
-    dist = torch.sqrt(torch.sum((points0 - points1) ** 2, dim=1))
-    thres = dist < threshold_distance
-    p0 = points0[thres]
-    p1 = points1[thres]
-
-    axes = viz2d.plot_images([lr, sr_to_lr], titles=["LR", "SR to LR"])
-    viz2d.plot_matches(p0, p1, color="lime", lw=0.2)
-    viz2d.add_text(0, f'Stop after {matches01["stop"]} layers', fs=20)
-    return axes
-
-
 def display_results(
     lr: torch.Tensor,
     lrdown: torch.Tensor,
     sr: torch.Tensor,
     srharm: torch.Tensor,
     hr: torch.Tensor,
     e1: torch.Tensor,
     e1_title: str,
     e1_subtitle: str,
     e2: torch.Tensor,
     e2_title: str,
     e2_subtitle: str,
     e3: torch.Tensor,
-    e3_points: Tuple[torch.Tensor, torch.Tensor],
     e3_title: str,
     e3_subtitle: str,
     e4: torch.Tensor,
     e4_title: str,
     e4_subtitle: str,
     e5: torch.Tensor,
     e5_title: str,
@@ -373,49 +230,51 @@
     axs[0, 2].set_title("SR", fontsize=20, fontweight="bold")
     axs[0, 3].imshow(srharm)
     axs[0, 3].set_title("SRharm", fontsize=20, fontweight="bold")
     axs[0, 4].imshow(hr)
     axs[0, 4].set_title("HR", fontsize=20, fontweight="bold")
 
     # Display the local reflectance map error
-    axs[1, 0].imshow(e1)
+    axs[1, 0].imshow(e1.cpu().clone())
     axs[1, 0].set_title(
         "%s \n %s: %s" % (r"$\bf{Reflectance\ Consistency \downarrow}$", e1_title, e1_subtitle)
     )
 
     # Display the spectral map error
-    axs[1, 1].imshow(e2)
+    axs[1, 1].imshow(e2.cpu().clone())
     axs[1, 1].set_title(
         "%s \n %s: %s" % (r"$\bf{Spectral\ Consistency \downarrow}$", e2_title, e2_subtitle)
     )
 
-    # Display the Spatial consistency
-    if len(torch.tensor(e3).shape) == 0:
-        axs[1, 2].imshow(e2 * torch.nan)
-    else:
-        axs[1, 2].imshow(e3, vmin=e3.min(), vmax=e3.max(), cmap="RdBu")
-        axs[1, 2].plot(
-            [x[0] for x in e3_points], [x[1] for x in e3_points], "r*", markersize=5
-        )
+    # Display the distance to the omission space
+    e3p = e3[~torch.isnan(e3)]
+    p5, p95 = np.percentile(e3p.flatten().cpu().clone().numpy(), [2, 98])
+    axs[1, 2].imshow(e3, vmin=p5, vmax=p95)
     axs[1, 2].set_title(
-        "%s \n %s: %s" % (r"$\bf{Spatial\ Consistency \downarrow}$", e3_title, e3_subtitle)
+        "%s \n %s: %s"
+        % (r"$\bf{Distance\ to\ Omission\ Space \uparrow}$", e3_title, e3_subtitle)
     )
 
-    # Display the distance to the ommission space
-    axs[1, 3].imshow(e4)
+    # Display the distance to the hallucination space
+    e5p = e5[~torch.isnan(e5)]
+    p5, p95 = np.percentile(e5p.flatten().cpu().clone().numpy(), [2, 98])
+    axs[1, 3].imshow(e5, vmin=p5, vmax=p95)
     axs[1, 3].set_title(
         "%s \n %s: %s"
-        % (r"$\bf{Distance\ to\ Omission\ Space \uparrow}$", e4_title, e4_subtitle)
+        % (r"$\bf{Distance\ to\ Hallucination\ Space \uparrow}$", e5_title, e5_subtitle)
     )
 
-    # Display the Hallucination error
-    axs[1, 4].imshow(e5)
+
+    # Display the distance to the improvement space
+    e4p = e4[~torch.isnan(e4)]
+    p5, p95 = np.percentile(e4p.flatten().cpu().clone().numpy(), [2, 98])
+    axs[1, 4].imshow(e4, vmin=p5, vmax=p95)
     axs[1, 4].set_title(
         "%s \n %s: %s"
-        % (r"$\bf{Distance\ to\ Improvement\ Space \downarrow}$", e5_title, e5_subtitle)
+        % (r"$\bf{Distance\ to\ Improvement\ Space \downarrow}$", e4_title, e4_subtitle)
     )
 
     return fig, axs
 
 
 def display_tc_score(
     sr_rgb: torch.Tensor,
@@ -430,44 +289,47 @@
         sr_rgb = linear_fix(sr_rgb)
     elif stretch == "histogram":
         sr_rgb = equalize_hist(sr_rgb)
     else:
         sr_rgb = do_nothing(sr_rgb)
 
     # Custom categorical colormap - Blue[0], Green[1], Red[2]
-    colorbar = colors.ListedColormap(["blue", "green", "red"])
-    
+    categorical_map = colors.ListedColormap(["blue", "green", "red"])
+    bounds = [0, 0.5, 1.5, 2.5]
+    norm = colors.BoundaryNorm(bounds, categorical_map.N)
+
     # Define triplets
-    p1 = d_im_ref.ravel()
+    p1 = d_im_ref.ravel().cpu().clone()
     p1 = p1[~torch.isnan(p1)]
 
-    p2 = d_om_ref.ravel()
+    p2 = d_om_ref.ravel().cpu().clone()
     p2 = p2[~torch.isnan(p2)]
     
-    p3 = tc_score.ravel()
+    p3 = tc_score.ravel().cpu().clone()
     p3 = p3[~torch.isnan(p3)]
     
     if log_scale:
         fig, ax = plt.subplots(1, 3, figsize=(15, 5))
         ax[0].imshow(sr_rgb)
         ax[0].set_title("SR RGB", fontsize=20, fontweight="bold")
-        ax[1].imshow(tc_score, cmap=colorbar)
+        ax[1].imshow(tc_score, cmap=categorical_map, norm=norm)
         ax[1].set_title("TC score - GRID", fontsize=20, fontweight="bold")
-        ax[2].scatter(p1, p2, c=p3, cmap=colorbar)
+        ax[2].scatter(p1, p2, c=p3, cmap=categorical_map, norm=norm)
         ax[2].set_ylabel("$d_{im}$", fontsize=18)
         ax[2].set_xlabel("$d_{om}$", fontsize=18)
         ax[2].set_title("TC score - 2D", fontsize=20, fontweight="bold")
         ax[2].set_yscale("log")
         ax[2].set_xscale("log")    
         # make square and equal
         ax[2].set_aspect(1.0/ax[2].get_data_ratio(), adjustable='box')
     else:
         fig, ax = plt.subplots(1, 3, figsize=(15, 5))
         ax[0].imshow(sr_rgb.permute(1, 2, 0)*3)
         ax[0].set_title("SR RGB", fontsize=20, fontweight="bold")
-        ax[1].imshow(tc_score, cmap=colorbar)
+        ax[1].imshow(tc_score, cmap=categorical_map, norm=norm)
         ax[1].set_title("TC score - GRID", fontsize=20, fontweight="bold")
-        ax[2].scatter(p1, p2, c=p3, cmap=colorbar)        
+        ax[2].scatter(p1, p2, c=p3, cmap=categorical_map, norm=norm)  
         ax[2].set_ylabel("$d_{im}$", fontsize=18)
         ax[2].set_xlabel("$d_{om}$", fontsize=18)
-        ax[2].set_title("TC score - 2D", fontsize=20, fontweight="bold")        
+        ax[2].set_title("TC score - 2D", fontsize=20, fontweight="bold")
     return fig, ax
+
```

