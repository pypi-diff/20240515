# Comparing `tmp/detectools-0.1.5.tar.gz` & `tmp/detectools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detectools-0.1.5.tar", last modified: Fri May  3 10:11:05 2024, max compression
+gzip compressed data, was "detectools-0.1.6.tar", last modified: Wed May 15 08:27:59 2024, max compression
```

## Comparing `detectools-0.1.5.tar` & `detectools-0.1.6.tar`

### file list

```diff
@@ -1,42 +1,55 @@
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.733847 detectools-0.1.5/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1087 2024-05-03 10:08:37.000000 detectools-0.1.5/LICENSE.txt
--rw-r--r--   0 jbernigauds  (1000) jbernigauds  (1000)     3107 2024-05-03 10:11:05.733847 detectools-0.1.5/PKG-INFO
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1637 2024-05-03 10:08:37.000000 detectools-0.1.5/README.md
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      599 2024-05-03 10:08:37.000000 detectools-0.1.5/README_deployment.md
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1442 2024-05-03 10:08:37.000000 detectools-0.1.5/pyproject.toml
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)       38 2024-05-03 10:11:05.733847 detectools-0.1.5/setup.cfg
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      145 2024-05-03 10:08:37.000000 detectools-0.1.5/setup.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.709847 detectools-0.1.5/src/
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.717847 detectools-0.1.5/src/detectools/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2051 2024-05-03 10:10:21.000000 detectools-0.1.5/src/detectools/__init__.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2417 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/augmentation.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    10779 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/dataset.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.725847 detectools-0.1.5/src/detectools/formats/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     3989 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/__init__.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    13188 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/base.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     7175 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/detection_format.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     7057 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/mask.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     9748 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/segmentation_format.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     6555 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/inference.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2209 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/metrics.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.725847 detectools-0.1.5/src/detectools/models/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      330 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/__init__.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2641 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/base.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    11002 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/mask2former.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    10950 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/yolo.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    16751 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/yolov8_seg.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     8112 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/trainer.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.729847 detectools-0.1.5/src/detectools/utils/
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/__init__.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     3401 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/data_management.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     6207 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/inference.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2775 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/mask_utils.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    16319 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/metrics.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1202 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/trainer.py
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     4708 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/visualisation.py
-drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.729847 detectools-0.1.5/src/detectools.egg-info/
--rw-r--r--   0 jbernigauds  (1000) jbernigauds  (1000)     3107 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/PKG-INFO
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1016 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/SOURCES.txt
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)        1 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/dependency_links.txt
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      218 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/requires.txt
--rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)       11 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)       67 2024-05-14 07:30:49.000000 detectools-0.1.6/LICENSE.txt
+-rw-r--r--   0 lucas     (1002) lucas     (1002)     2086 2024-05-15 08:27:59.012578 detectools-0.1.6/PKG-INFO
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1637 2024-03-21 11:28:28.000000 detectools-0.1.6/README.md
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      599 2024-04-17 13:45:59.000000 detectools-0.1.6/README_deployment.md
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1582 2024-05-14 07:30:49.000000 detectools-0.1.6/pyproject.toml
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)       38 2024-05-15 08:27:59.012578 detectools-0.1.6/setup.cfg
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      145 2024-03-21 13:29:41.000000 detectools-0.1.6/setup.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.008578 detectools-0.1.6/src/
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.008578 detectools-0.1.6/src/detectools/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1460 2024-05-15 08:26:07.000000 detectools-0.1.6/src/detectools/__init__.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.008578 detectools-0.1.6/src/detectools/data/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      174 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/data/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2585 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/data/augmentation.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    13633 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/data/dataset.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     3354 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/data_management.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/formats/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      678 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    16146 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/base.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     8238 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/detect_mask.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     9274 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/formats/detection_format.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     5788 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/formats/interfaces.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2936 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/mask_utils.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    12611 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/segmentation_format.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/inference/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      111 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/inference/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     6742 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/inference/engine.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     9141 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/inference/predictor.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/metrics/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      277 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/metrics/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     4389 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/metrics/available_metrics.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    13368 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/metrics/base.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     3128 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/metrics/functionnals.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/models/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      350 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/models/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     3156 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/models/base.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    12308 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/models/mask2former.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    13114 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/models/yolo.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    18835 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/models/yolov8_seg.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/train/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      138 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/train/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1580 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/train/loss_aggregator.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    10960 2024-05-15 08:25:33.000000 detectools-0.1.6/src/detectools/train/trainer.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/utils/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      233 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/utils/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      241 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/utils/data.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      320 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/utils/display.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      751 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/utils/load_and_write.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     5043 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/visualisation.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools.egg-info/
+-rw-r--r--   0 lucas     (1002) lucas     (1002)     2086 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1378 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)        1 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      218 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)       11 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/top_level.txt
```

### Comparing `detectools-0.1.5/README.md` & `detectools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `detectools-0.1.5/README_deployment.md` & `detectools-0.1.6/README_deployment.md`

 * *Files identical despite different names*

### Comparing `detectools-0.1.5/pyproject.toml` & `detectools-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,21 @@
     "seaborn==0.13.0",
     "pycocotools==2.0.7",
     "torchmetrics==1.3.0",
     "ultralytics==8.1.7",
     "transformers==4.39.2"
 ]
 
+
 license = {file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://forgemia.inra.fr/ue-apc/librairies/python/detectools"
 Issues = "https://forgemia.inra.fr/ue-apc/librairies/python/detectools/-/issues"
+Documentation = "https://detectools.readthedocs.io/en/latest/"
+Repository = "https://forgemia.inra.fr/ue-apc/librairies/python/detectools"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.dynamic]
 version = {attr = "detectools.__version__"}
```

### Comparing `detectools-0.1.5/src/detectools/augmentation.py` & `detectools-0.1.6/src/detectools/data/augmentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 from typing import List, Tuple
 
 import torchvision.transforms.v2 as T
 from torch import Tensor
 from torchvision.tv_tensors import BoundingBoxes, Image, Mask
-import torch
 from detectools.formats import Format, SegmentationFormat
-from detectools.formats.mask import DetectMask
+from detectools.formats.detect_mask import DetectMask
 
 
 class Augmentation:
-    def __init__(self, augmentations: List[T.Transform] = [], min_size: int = 1):
-        """Generate Augmentation instance with list of transformations.
+    """Augmentation class allow augmentation of both images and targets as BaseFormat.
+
+    Args:
+            augmentations (``List[T.Transform]``, **optional**): List of torchvision v2 transforms. Defaults to [].
+    
+     Attributes
+    ----------
+
+    Attributes:
+        transform (``T.Compose``): Composition of torchvision transforms.
+    
+    Methods
+    ----------
+    """
+    def __init__(self, augmentations: List[T.Transform] = []):
 
-        Args:
-            augmentations (List[T.Transform], optional): List of torchvision v2 transforms. Defaults to [].
-        """
         # Make the compose of all the augmentations
-        self.min_size = min_size
         self.transform = T.Compose(augmentations)
 
     def __call__(self, image: Tensor, target: Format) -> Tuple[Tensor, Format]:
-        """Apply intern transfomrations to image & target and return augmented pair.
+        """Apply  transformations to image & target and return augmented pair.
 
         Args:
-            image (Tensor): RGB tensor image.
-            target (Format): All targets for image.
+            image (``Tensor``): RGB Tensor image.
+            target (``Format``): Target as BaseFormat.
 
         Returns:
-            Tuple[Tensor, Format]: Pair of augmented image & Format.
+            ``Tuple[Tensor, Format]``:
+                - Augmented image.
+                - Augmented target.
         """
+        
         # send image & annotations to TVTensors
         image = Image(image)
         labels, boxes = target.get("labels", "boxes")
         boxes: BoundingBoxes = target.get("boxes")
         # wrap into list
         originals = [image, labels, boxes]
         if isinstance(target, SegmentationFormat):
```

### Comparing `detectools-0.1.5/src/detectools/formats/base.py` & `detectools-0.1.6/src/detectools/formats/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,143 @@
 from __future__ import annotations
 
-from abc import ABC, abstractclassmethod
+from abc import ABC, abstractmethod
 from typing import Any, Dict, Generator, List, Literal, Sequence, Tuple, Union
 
 import torch
 from torch import Tensor
 from torchvision.ops import nms, remove_small_boxes
 from torchvision.transforms.v2 import ConvertBoundingBoxFormat
-from torchvision.tv_tensors import BoundingBoxes, Mask
-from detectools.formats.mask import DetectMask
+from torchvision.tv_tensors import BoundingBoxes
+from detectools.formats.detect_mask import DetectMask
 
 
 class BaseAnnotation(ABC):
-    """Base class for annotations objects."""
+    """Abstract class for Annotation data container.
+    
+    Attributes:
+    -----------
+
+    Attributes:
+        boxe (``BoundingBoxes``): Boxe coordinates in XYWH format.
+        label (``Tensor``): Class label of object.
+        spatial_size (``Tuple[int, int]``): Size of corresponding image (H, W)
+        score (``Tensor``): Confidence score of the object (for prediction). 
+    
+    Methods:
+    -----------
+    """
+    boxe : BoundingBoxes
+    label : Tensor
+    spatial_size: Tuple[int, int]
+    score: Tensor
 
-    @abstractclassmethod
+    @abstractmethod
     def __init__(self):
         pass
 
-    @abstractclassmethod
+    @abstractmethod
     def object_to_coco(
         self, annotation_id: int = 1, image_id: int = 1
     ) -> Dict[str, Any]:
-        """Return COCO annotation dict from self.
+        """Return Annotation data as COCO like dict.
 
         Args:
-            annotation_id (int): id to write on "id" field in annotation dict.
-            image_id (int): id to write for "image_id" field in annotation dict.
+            annotation_id (``int``, **optional**): Id of the annotation. Defaults to 1.
+            image_id (``int``, **optional**): Id of the corresponding image. Defaults to 1.
 
         Returns:
-            Dict[str, Any]: COCO like annotation dict.
+            ``Dict[str, Any]``:
+                - COCO like dict with Annotation instance data.
         """
         pass
 
 
 class BaseFormat(ABC):
-    """Base class for data formats in detectools. This base class is the parent class of DetectionFormat & InstanceFormat.
-    Formats in detectool store target & results informations as tensors in the argument data (dict with key/Tensors.). Basic and advanced operations
-    can be done directly onf formats objects (padding, cropping, NMS, etc..)."""
+    """Abstract class for detection data container classes in detectools. Store target and predictions data. This data format
+    support basics and advanced operations (padding, cropping, NMS, etc.).
 
+    Attributes:
+    -----------
+
+    Attributes:
+        box_format (``Literal["XYWH", "XYXY", "CXCYWH"]``): Format of bounding boxes.
+        spatial_size (``Tuple[int, int]``): Size of corresponding image (H, W)
+        size (``int``): Number of objects in BaseFormat.
+        data: (``Dict[str, Tensor]``): Data dict that contains objects informations in it's keys (labels, boxes, scores, masks).
+    
+    Methods:
+    -----------
+    
+    """
     spatial_size: Tuple[
         int, int
     ]  # Store the H, W image size corresponding to objects boxes/masks stored in BaseFormat.
     data: Dict[
         str, Tensor
     ]  # Store all values (labels, boxes/masks at least) corresponding to objects in an image.
     size: int  # Number of objects in image.
     box_format: Literal["XYWH", "XYXY", "CXCYWH"]  # format for bounding boxes.
 
     ### Class methods that returns a BaseFormat
     def from_coco(
         cls, coco_annotations: List[Dict[str, Any]], spatial_size: Tuple[int]
     ) -> BaseFormat:
-        """Create a format from a list of COCO annotations.
+        """Return BaseFormat from an image COCO data dictionnary.
 
         Args:
-            coco_annotations (List[Dict[str, Any]]): List of annotations (from COCO json file or other COCO data structure).
-            spatial_size (Tuple[int]): Dimension of corresponding image.
+            coco_annotations (``List[Dict[str, Any]]``): Coco data dictionnary.
+            spatial_size (``Tuple[int]``): Size (H, W) of the corresponding image.
 
         Returns:
-            BaseFormat: Format with COCO objects informations stored in data dict.
+            ``BaseFormat``:
+                - BaseFormat instance.
         """
         pass
 
-    @abstractclassmethod
+    @abstractmethod
     def empty(spatial_size: Tuple[int]) -> BaseFormat:
-        """Return an empty BaseFormat.
+        """Return an empty instance of BaseFormat (DetectionFormat or SegmentationFormat depending on the Task mode).
 
         Args:
-            spatial_size (Tuple[int]): Spatial size for future objects in BaseFormat.
+            spatial_size (``Tuple[int]``): Size (H, W) of the corresponding image.
 
         Returns:
-            BaseFormat: BaseFormat with no objects in.
+            ``BaseFormat``:
+                - BaseFormat instance.
         """
         pass
 
     def clone(self) -> BaseFormat:
-        """Clone self and return identical BaseFormat with detached clones tensors of data.
+        """Return a clone of BaseFormat.
 
         Returns:
-            BaseFormat: Clone of self.
+            ``BaseFormat``:
+                - Cloned BaseFormat.
         """
         clone = type(self).empty(spatial_size=self.spatial_size)
         clone.size = self.size
         for key, value in self.data.items():
             if isinstance(value, DetectMask):
                 clone.data[key] = DetectMask(value._mask.clone().detach())
             else:
                 clone.data[key] = value.clone().detach()
 
         return clone
 
     ### Magic methods
     def __getitem__(self, indexes: Union[int, Sequence[int]]) -> BaseFormat:
-        """Return a subset BaseFormat by keeping only elements of data dict values (tensors) at positions of indexes.
+        """ Return a subset BaseFormat by keeping only elements of data dict values (tensors) at positions of indexes.
 
         Args:
-            indexes (Union[int, Sequence[int]]): Indexes to slice objects data.
+            indexes (``Union[int, Sequence[int]]``): Indexes to slice objects data.
 
         Returns:
-            BaseFormat: Format with n objects for n indexes in indexes.
+            ``BaseFormat``:
+                - BaseFormat with n objects for n indexes in indexes.
         """
         sliced = self.clone()
         # slice each elements of data dict
         for key, value in self.data.items():
             # general case
             if not isinstance(value, BoundingBoxes):
                 sliced.data[key] = value[indexes]
@@ -113,48 +147,72 @@
         sliced.set_boxes_format(self.box_format)
         return sliced
 
     def __contains__(self, key: str) -> bool:
         """Return True if key in self.data dict, else False.
 
         Args:
-            key (str): Data dictionnary key.
+            key (``str``): Data dictionnary key
+
         Returns:
-            bool: True if key in self.data else False.
+            ``bool``:
+                - True if key in self.data else False.
         """
         return key in self.data.keys()
 
     def __iter__(self) -> Generator[BaseAnnotation]:
         """Iterate through BaseFormat and yield at each index i a BaseAnnotation object
-        that contains all informations for object at position i."""
+        that contains all informations for object at position i.
+
+        Yields:
+            ``BaseAnnotation``: BaseAnnotation at position x.
+        """
 
         for object_id in range(self.size):
             yield self.get_object(object_id)
 
     # Acessibility methods: get or set objects into BaseFormat
     def get_device(self) -> torch.device:
-        """Verify that all tensors of data dict are on same device and return device."""
+        """Verify that all tensors of data dict are on same device and return device.
+
+        Returns:
+            ``torch.device``:
+                - Device that hold tensor values of data dict.
+        """
         devices = [value.device for value in self.data.values()]
         devices_set = set(devices)
         assert (
             len(devices_set) == 1
         ), f"All tensors on data dict should be on the same device, got {len(devices_set)} devices : {devices_set}."
         return list(devices_set)[0]
 
     def set_device(self, device: Union[torch.device, Literal["cuda", "cpu"]]):
-        """Set all values in self.data dict to device."""
+        """Send all torch values of data dict on device.
+
+        Args:
+            device (``Union[torch.device, Literal['cuda', 'cpu']]``): Device to send tensors on.
+        """
         for key, value in self.data.items():
             self.data[key] = value.to(device)
 
     def get(self, *keys: str) -> Union[Tensor, Tuple[Tensor]]:
-        """Return data values for each key in *keys.
+        """Return tensor data values from data dict for each key in keys.
+
         Args:
-            keys: Key(s) of self.data dict.
+            keys (``str``): Key(s) of data dict.
+
         Returns:
-            Union[Tensor, Tuple[Tensor]]: Values for each keys.
+            ``Union[Tensor, Tuple[Tensor]]``:
+                - Corresponding key's values to gather from data dict.
+        
+        .. highlight:: python
+        .. code-block:: python
+
+            >>> format: BaseFormat
+            >>> labels, boxes = format.get("labels", "boxes")
         """
 
         outputs = []
         for key in keys:
             assert (
                 key in self
             ), f"{key} should be in self.data, got only {list(self.data.keys())}."
@@ -164,47 +222,74 @@
             output = tuple(outputs)
         else:
             output = outputs[0]  # single element
 
         return output
 
     def set(self, key: str, value: Tensor):
-        """Set a new pair of key/value. Value should be of shape (N, ...) with N == self.size."""
+        """Set a new pair of key/value. Value should be of shape (N, ...) with N == self.size.
+
+        Args:
+            key (``str``): Key of value to set.
+            value (``Tensor``): Data as tensor.
+        """
 
         # get shape of new value and assert it's equal to self.size
         data_size = value.size()[0] if value.nelement() else 0
         assert (
             data_size == self.size
         ), f"New value size should be equal to self.size, got {data_size} and {self.size}."
         # assign value to key with correct device
         device = self.get_device()
         value = value.to(device)
         self.data[key] = value
 
-    @abstractclassmethod
+    @abstractmethod
     def get_object(self, indice: int) -> BaseAnnotation:
-        """Return a BaseAnnotation object at position indice."""
+        """Return a BaseAnnotation object at position indice.
+
+        Args:
+            indice (``int``): Position of object to gather.
+
+        Returns:
+            ``BaseAnnotation``:
+                - Annotation instance.
+        """
         pass
 
     # Methods that changes internal states of Formats
-    @abstractclassmethod
+    @abstractmethod
     def crop(self, top: int, left: int, height: int, width: int):
-        """Crop boxes and mask and update spatial size."""
+        """Crop boxes and mask from top corner pixel and update spatial size.
+
+        Args:
+            top (``int``): Position to crop from top border.
+            left (``int``): Position to crop from left border.
+            height (``int``): height of the crop.
+            width (``int``): Width of the crop.
+        """
         pass
 
-    @abstractclassmethod
+    @abstractmethod
     def pad(self, left: int, top: int, right: int, bottom: int):
-        """Pad boxes and mask and update spatial size."""
+        """Pad boxes and mask and update spatial size.
+
+        Args:
+            left (``int``): Pad value on left border.
+            top (``int``): Pad value on top border.
+            right (``int``): Pad value on right border.
+            bottom (``int``): Pad value on bottom border.
+        """
         pass
 
     def set_boxes_format(self, box_format: Literal["XYWH", "XYXY", "CXCYWH"]):
         """Change boxes format.
 
         Args:
-            box_format (Literal[XYWH, XYXY, CXCYWH]): Format to set for boxes.
+            box_format (``Literal['XYWH', 'XYXY', 'CXCYWH']``): Format to set for boxes.
         """
         assert box_format in [
             "XYWH",
             "XYXY",
             "CXCYWH",
         ], f"box_format should be one of these [XYWH, XYXY, CXCYWH], got {box_format}."
         converter = ConvertBoundingBoxFormat(box_format)
@@ -212,15 +297,15 @@
         self.data["boxes"] = converter(boxes)
         self.box_format = box_format
 
     def convert_labels(self, convert_labels_dict: Dict[int, int]):
         """Convert labels of Format.
 
         Args:
-            convert_dict (Dict[int,int]): Conversion dict for labels.
+            convert_labels_dict (``Dict[int, int]``): Dict of converion {old_labels:new_labels}.
         """
         labels = self.get("labels")
         new_labels = self.get("labels")
         for key, value in convert_labels_dict.items():
             new_labels[labels == key] = value
         self.set("labels", new_labels)
 
@@ -253,66 +338,81 @@
             device=self.get_device(),
         )
         self.set("boxes", boxes)
 
     # Method to process objects selection
 
     def sanitize(self, min_box_sides: float) -> BaseFormat:
-        """Remove objects with boxes that have one of their sides smaller than min_box_sides."""
+        """Remove objects with boxes that have one of their sides smaller than min_box_sides.
+
+        Args:
+            min_box_sides (``float``): Minimum size of border to keep boxes.
+
+        Returns:
+            ``BaseFormat``:
+                - BaseFormat without small boxes.
+        """
         format_boxes = ConvertBoundingBoxFormat("XYXY")
         boxes = format_boxes(self.get("boxes"))
         safe_objects_indexes = remove_small_boxes(boxes, min_box_sides)
         return self[safe_objects_indexes]
 
     def sort_by_scores(self, descending: bool = True) -> BaseFormat:
         """Sort objects by scores in decreasing order.
 
         Args:
-            descending (bool, optional): To sort objects in descending order or ascending. Defaults to True.
+            descending (``bool``, **optional**): To sort objects in format with decreasing score order. Defaults to True.
 
         Returns:
-            BaseFormat: Sorted format.
+            ``BaseFormat``:
+                - Sorted BaseFormat.
         """
         assert "scores" in self, "Format should contain scores to run sort_by_scores."
         indexes = torch.argsort(self.get("scores"), descending=descending)
         return self[indexes]
 
     def max_detections(self, maximum_objects: int) -> BaseFormat:
         """Retrieve N (maximum objects) with highest scores.
 
         Args:
-            maximum_objects (int): Number of object to keep.
+            maximum_objects (``int``): Number of object to keep.
+
         Returns:
-            BaseFormat: Format with N objects with highest scores.
+            ``BaseFormat``:
+                - Format with N objects with highest scores.
         """
         assert "scores" in self, "Format should contain scores to run max_detection."
         return self.sort_by_scores()[:maximum_objects]
 
     def confidence(self, confidence_threshold: float = 0.5) -> BaseFormat:
         """Keep only objects with confidence above confidence_threshold.
 
         Args:
-            confidence_threshold (float): confidence threshold. Defaut to 0.5.
+            confidence_threshold (``float``, **optional**): Minimum confidence to keep object. Defaults to 0.5.
+
         Returns:
-            BaseFormat: Format with only objects with scores > confidence_thr.
+            ``BaseFormat``:
+                -  Format with only objects with scores > confidence_thr.
         """
         assert "scores" in self, "Format should contain scores to run confidence."
         if self.size == 0:
             return self
         scores = self.get("scores")
         indexes = scores >= confidence_threshold
         return self[indexes]
 
     def nms(self, iou_threshold=0.5) -> BaseFormat:
         """Apply non maximum suppression algorithm to format.
 
         Args:
-            iou_threshold (float, optional): Threshold to consider boxes as overlapping. Defaults to 0.5.
+            iou_threshold (``float``, **optional**): Threshold to consider boxes as overlapping. Defaults to 0.5.
+
         Returns:
-            BaseFormat: Format with objects selected by NMS.
+            ``BaseFormat``:
+                - Format with objects selected by NMS
         """
         assert "scores" in self, f"Format should contain scores to run nms."
         if self.size == 0:
             return self
         boxes, scores = self.get("boxes", "scores")
         format_convert = ConvertBoundingBoxFormat("XYXY")
         boxes: BoundingBoxes = format_convert(boxes)
@@ -326,19 +426,20 @@
 
         # Method to export Formats objects
 
     def coco(self, image_id: int = 1, annotation_id: int = 1) -> List[Dict[str, Any]]:
         """Export data as COCO annotations.
 
         Args:
-            image_id (int): id to write for "image_id" field in annotation dict.
-            starting_ann_id (int): id to write on the first annotation dict "id" field. Following ones have id count from this one.
+            image_id (``int``, **optional**): Id to write for "image_id" field in annotation dict. Defaults to 1.
+            annotation_id (``int``, **optional**): Id to write on the first annotation dict "id" field. Following ones have id indent from this one. Defaults to 1.
 
         Returns:
-            List[Dict[str, Any]]: Coco annotations list for Format corresponding image.
+            ``List[Dict[str, Any]]``:
+                -  Coco annotations list for Format corresponding image.
         """
 
         coco_annotations = []
         for detection_object in self:
             coco_annotations.append(
                 detection_object.object_to_coco(
                     image_id=image_id, annotation_id=annotation_id
@@ -346,16 +447,24 @@
             )
             annotation_id += 1
 
         return coco_annotations
 
     # Protection methods
 
-    def match(format1: BaseFormat, format2: BaseFormat):
+    def match(format1: BaseFormat, format2: BaseFormat) -> bool:
         """Check if 2 Formats match for combinations:
         - check if both contains same keys on data dictionnary.
         - check if spatial size is equivalent.
+
+        Args:
+            format1 (``BaseFormat``): BaseFormat 1.
+            format2 (``BaseFormat``): BaseFormat 2.
+
+        Returns:
+            ``bool``:
+                - True if BaseFormats matchs else False.
         """
 
         keys1 = set(list(format1.data.keys()))
         keys2 = set(list(format2.data.keys()))
         return (keys1 == keys2) and format1.spatial_size == format2.spatial_size
```

### Comparing `detectools-0.1.5/src/detectools/formats/detection_format.py` & `detectools-0.1.6/src/detectools/formats/detection_format.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,33 @@
 from detectools.formats.base import BaseAnnotation, BaseFormat
 from torch import Tensor
 from torchvision.transforms.v2.functional import crop_bounding_boxes, pad_bounding_boxes
 from torchvision.tv_tensors import BoundingBoxes
 
 
 class DetectionAnnotation(BaseAnnotation):
-    """Class to wrap informations of detection objects."""
+    """BaseAnnotation child class for detection task.
+
+    Attributes:
+    -----------
+
+    Attributes:
+        boxe (``BoundingBoxes``): Boxe coordinates in XYWH format.
+        label (``Tensor``): Class label of object.
+        spatial_size (``Tuple[int, int]``): Size of corresponding image (H, W)
+        score (``Tensor``): Confidence score of the object (for prediction). 
+    
+    Methods:
+    -----------
+    """
+
+    boxe : BoundingBoxes
+    label : Tensor
+    spatial_size: Tuple[int, int]
+    score: Tensor
 
     def __init__(
         self,
         spatial_size: Tuple[int],
         label: Tensor,
         boxe: Tensor,
         score: Tensor = None,
@@ -25,92 +43,117 @@
         self.label = label
         self.spatial_size = spatial_size
         self.score = score
 
     def object_to_coco(
         self, annotation_id: int = 1, image_id: int = 1
     ) -> Dict[str, Any]:
-        """Return COCO annotation dict from self.
+        """Return detection annotation data as COCO like dict.
 
         Args:
-            annotation_id (int): id to write on "id" field in annotation dict.
-            image_id (int): id to write for "image_id" field in annotation dict.
+            annotation_id (``int``, **optional**): Id of the annotation. Defaults to 1.
+            image_id (``int``, **optional**): Id of the corresponding image. Defaults to 1.
 
         Returns:
-            Dict[str, Any]: COCO like annotation dict.
+            ``Dict[str, Any]``:
+                - COCO like dict with Annotation instance data.
         """
         annotation = {
             "id": annotation_id,
             "bbox": self.boxe.tolist(),
             "category_id": self.label.item(),
             "image_id": image_id,
         }
         if isinstance(self.score, Tensor):
             annotation["score"] = self.score.item()
 
         return annotation
 
 
 class DetectionFormat(BaseFormat):
-    """Data format for detection task. Contains only boxes & labels data."""
+    """BaseFormat child class for detection task.
+
+    Args:
+        spatial_size (``Tensor``): Spatial size (H, W) of corresponding images.
+        labels (``Tensor``): Tensor of shape (N,) with class labels for each object.
+        boxes (``Tensor``): Tensor of shape (N, 4). N for N objects and 4 for boxes coordinates.
+        scores (``Tensor``, **optional**): Tensor of shape (N,) with objects confidence score. Defaults to None.
+        box_format (``Literal['XYWH', 'XYXY', 'CXCYWH']``, **optional**): Format of bounding boxes. Defaults to 'XYWH'.
+        
+    
+    Attributes:
+    -----------
+
+    Attributes:
+        box_format (``Literal["XYWH", "XYXY", "CXCYWH"]``): Format of bounding boxes.
+        spatial_size (``Tuple[int, int]``): Size of corresponding image (H, W)
+        size (``int``): Number of objects in BaseFormat.
+        data: (``Dict[str, Tensor]``): Data dict that contains objects informations in it's keys (labels, boxes, scores).
+    
+    Methods:
+    -----------
+    
+    """
+    spatial_size: Tuple[
+        int, int
+    ]  # Store the H, W image size corresponding to objects boxes/masks stored in BaseFormat.
+    data: Dict[
+        str, Tensor
+    ]  # Store all values (labels, boxes/masks at least) corresponding to objects in an image.
+    size: int  # Number of objects in image.
+    box_format: Literal["XYWH", "XYXY", "CXCYWH"]  # format for bounding boxes.
 
     # override
     def empty(spatial_size: Tuple[int]) -> DetectionFormat:
-        """Return an empty DetectionFormat.
+        """Return an empty instance DetectionFormat.
 
         Args:
-            spatial_size (Tuple[int]): Spatial size for future objects in DetectionFormat.
+            spatial_size (``Tuple[int]``): Size (H, W) of the corresponding image.
 
         Returns:
-            DetectionFormat: DetectionFormat with no objects in.
+            ``DetectionFormat``:
+                - DetectionFormat instance.
         """
         boxes = BoundingBoxes([[]], canvas_size=spatial_size, format="XYWH")
         labels = torch.tensor([])
         detection_format = DetectionFormat(
             spatial_size=spatial_size,
             labels=labels,
             boxes=boxes,
         )
         return detection_format
 
     # override
     def from_coco(
         coco_annotations: List[Dict[str, Any]], spatial_size: Tuple[int]
     ) -> DetectionFormat:
-        """Create a DetectionFormat from a list of COCO annotations.
+        """Return DetectionFormat from an image COCO data dictionnary.
 
         Args:
-            coco_annotations (List[Dict[str, Any]]): List of annotations (from COCO json file or other COCO data structure).
-            spatial_size (Tuple[int]): Dimension of corresponding image.
+            coco_annotations (``List[Dict[str, Any]]``): Coco data dictionnary.
+            spatial_size (``Tuple[int]``): Size (H, W) of the corresponding image.
 
         Returns:
-            DetectionFormat: Format with COCO objects informations stored in data dict.
+            ``DetectionFormat``:
+                - DetectionFormat instance.
         """
         boxes = torch.tensor([ann["bbox"] for ann in coco_annotations])
         labels = torch.tensor([ann["category_id"] for ann in coco_annotations])
         detection_format = DetectionFormat(spatial_size, labels, boxes)
         return detection_format
 
     def __init__(
         self,
         spatial_size: Tensor,
         labels: Tensor,
         boxes: Tensor,
         scores: Tensor = None,
         box_format: Literal["XYWH", "XYXY", "CXCYWH"] = "XYWH",
     ):
-        """Create DetectionFormat object.
-
-        Args:
-            boxes (Tensor): Sequence of sequences of 4 integers for bounding boxes coordinates.
-            labels (Tensor): Sequence of label class value for each box.
-            spatial_size (Tuple[int]): Spatial size (H, W) of corresponding images.
-            scores (Tensor, optionnal): Confidence scores of objects.
-            box_format (Literal["XYWH", "XYXY", "CXCYWH"]): Format of bounding boxes.
-        """
+        
         # assert Task mode is "instance_segmentation"
         assert (
             Task.mode == "detection"
         ), f"Task mode should be 'detection' to construct DetectionFormat object, got {Task.mode}."
 
         self.spatial_size = spatial_size
         self.size = labels.nelement()
@@ -121,21 +164,22 @@
         )
         # store all data in data dict
         self.data: Dict[str, Tensor] = {"boxes": boxes, "labels": labels}
         if scores != None:
             self.data["scores"] = scores
 
     def __getitem__(self, indexes: Union[int, Tensor]) -> DetectionFormat:
-        """ "Return a subset DetectionFormat by keeping only elements of data dict values (tensors) at positions of indexes.
+        """ Return a subset DetectionFormat by keeping only elements of data dict values (tensors) at positions of indexes.
 
         Args:
-            indexes (Union[int, Sequence[int]]): Indexes to slice objects data.
+            indexes (``Union[int, Sequence[int]]``): Indexes to slice objects data.
 
         Returns:
-            DetectionFormat: Format with N objects for N indexess.
+            ``DetectionFormat``:
+                - DetectionFormat with n objects for n indexes in indexes.
         """
         sliced = super().__getitem__(indexes)
         if "boxes" in self:
             boxes = self.get("boxes")[indexes]
             boxes = BoundingBoxes(
                 boxes,
                 canvas_size=self.spatial_size,
@@ -143,27 +187,42 @@
                 device=self.get_device(),
             )
             sliced.data["boxes"] = boxes
 
         return sliced
 
     def get_object(self, indice: int) -> DetectionAnnotation:
-        """Return a DetectionAnnotation object at position indice."""
+        """Return DetectionAnnotation object at position indice.
+
+        Args:
+            indice (``int``): Position of object to gather.
+
+        Returns:
+            ``DetectionAnnotation``:
+                - DetectionAnnotation instance.
+        """
         single_object_format = self[indice]
         bbox, label = single_object_format.get("boxes", "labels")
         detection_object = DetectionAnnotation(self.spatial_size, label, bbox.squeeze())
         if "scores" in single_object_format:
             detection_object.score = single_object_format.get("scores")
 
         return detection_object
 
     # Methods that changes internal states of Formats
     # override
     def crop(self, top: int, left: int, height: int, width: int):
-        """Crop boxes and update spatial size."""
+        """Crop boxes from top corner pixel and update spatial size.
+
+        Args:
+            top (``int``): Position to crop from top border.
+            left (``int``): Position to crop from left border.
+            height (``int``): height of the crop.
+            width (``int``): Width of the crop.
+        """
         if self.size == 0:
             self.spatial_size = (height, width)
             return self
         boxes = self.get("boxes")
         boxes, canvas_size = crop_bounding_boxes(
             boxes,
             format=self.box_format,
@@ -181,15 +240,22 @@
                 device=self.get_device(),
             ),
         )
         self.spatial_size = canvas_size
 
     # override
     def pad(self, left: int, top: int, right: int, bottom: int):
-        """Pad boxes and update spatial size."""
+        """Pad boxes and update spatial size.
+
+        Args:
+            left (``int``): Pad value on left border.
+            top (``int``): Pad value on top border.
+            right (``int``): Pad value on right border.
+            bottom (``int``): Pad value on bottom border.
+        """
         if self.size == 0:
             h, w = self.spatial_size
             self.spatial_size = (h + top + bottom, w + left + right)
             return
 
         boxes: BoundingBoxes = self.get("boxes")
         boxes, canvas_size = pad_bounding_boxes(
```

### Comparing `detectools-0.1.5/src/detectools/formats/mask.py` & `detectools-0.1.6/src/detectools/formats/detect_mask.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,192 +1,244 @@
 from __future__ import annotations
 
-from torchvision.tv_tensors import Mask
-from torch import Tensor
+from typing import Any, Literal, Tuple, Union
+
 import torch
-from torch import is_floating_point
-from typing import Union, Any, Tuple, Literal
+from torch import Tensor, is_floating_point
 from torch.nn.functional import one_hot
+from torchvision.tv_tensors import Mask
+
+
+class DetectMask:
+    """Mask class for detectools that contain object masks in a stacked tensor to save memory. Values are from 0 (background) to N (for N objects).
 
+    Args:
+        mask (``Tensor``): Tensor of shape (H,W).
+
+    Attributes:
+    -----------
 
-class DetectMask():
-    """Mask class for detectools. It inherits from Mask TV_Tensors contain methods to insure that detection data
-    are well stored for instance segmentation objects."""
+    Attributes:
+        _mask (``Tensor``): Mask Tensor (H, W).
+
+    Methods:
+    -----------
+    """
 
     def from_binary_masks(masks: Tensor) -> DetectMask:
-        """Generate DetectMask from stack of binary masks (N,H,W)."""
+        """Generate DetectMask from binary masks.
+
+        Args:
+            masks (``Tensor``): Stack of binary masks (N,H,W).
+
+        Returns:
+            ``DetectMask``:
+                - Detect mask instance.
+        """
         detect_mask = DetectMask(torch.zeros(masks.shape[-2:], device=masks.device))
         for i, m in enumerate(masks):
             detect_mask.add_binary_mask(m, i)
         return detect_mask
 
-    def __init__(self, mask:Tensor):
+    def __init__(self, mask: Tensor):
+
         self._mask = mask.int()
-    
+
     @property
-    def device(self):
+    def device(self) -> torch.device:
+        """Return device that contain DetectMask.
+
+        Returns:
+            ``torch.device``:
+                - Device where DetecMask is.
+        """
         return self._mask.device
-        
+
     def to(self, device: Literal["cpu", "cuda"]):
         self._mask = self._mask.to(device)
         return self
 
     def reindex(self) -> Tensor:
         """Replace mask values such that mask values are in 0 - N range with 0 for background and
         1 - N indices of objects.
 
         Returns:
-            Tensor: Object ids (0 - N-1 objects).
+            ``Tensor``:
+                - Object ids (0 - N-1 objects).
         """
         if not self.n_objects:
             return torch.tensor([])
-        object_ids = torch.unique(self._mask[self._mask!=0]).int()
-        new_ids = torch.tensor(range(1, torch.max(object_ids)+1), device=self._mask.device).int()
+        object_ids = torch.unique(self._mask[self._mask != 0]).int()
+        new_ids = torch.tensor(
+            range(1, torch.max(object_ids) + 1), device=self._mask.device
+        ).int()
         idxs = torch.nonzero(self._mask.unsqueeze(-1) == object_ids, as_tuple=True)
         self._mask[idxs[:-1]] = new_ids[idxs[2]]
 
         return object_ids - 1
 
-    
     def add_binary_mask(self, mask: Tensor, value: int = None):
         """Add a binary mask corresponding do one instance segmentation object.
 
-            Args:
-                value(int): value to assign to mask==1 in DetectMask. Default to None so value will be max of self +1.        
+        Args:
+            mask (``Tensor``): Binary mask to add (H,W).
+            value (``int``, **optional**): value to assign to mask==1 in DetectMask. Default to None so value will be max of self +1. Defaults to None.
         """
 
         assert is_binary(mask), f"Mask to add is not binary."
 
         self_max = torch.max(self._mask)
-        if  value != None:
+        if value != None:
             value += 1
         else:
             value = self_max + 1
-        self._mask[mask==1] = value
-    
-    def __getitem__(self, indexes) -> DetectMask:
+        self._mask[mask == 1] = value
 
+    def __getitem__(self, indexes) -> DetectMask:
+        """Return subset of DetectMask with N objects for N indexes. Also reindex the values of kept objects so that they are in range 0-n_objects.
+        Returns:
+            ``DetectMask``:
+                - _description_
+        """
         if isinstance(indexes, int):
             indexes = torch.tensor([indexes])
         elif isinstance(indexes, list):
             indexes = torch.tensor(indexes)
         elif isinstance(indexes, slice):
             indexes = torch.tensor(list(range(self.n_objects))[indexes])
 
         if indexes.dtype == torch.bool:
             indexes = indexes.nonzero().flatten()
-        
-        assert torch.sum(indexes > self.n_objects) == 0, f"Some indexes are higher than the number of objects in mask: indexes {indexes} & number of objects: {self.n_objects}"
+
+        assert (
+            torch.sum(indexes > self.n_objects) == 0
+        ), f"Some indexes are higher than the number of objects in mask: indexes {indexes} & number of objects: {self.n_objects}"
         get_mask = DetectMask(self._mask)
-        retrieve_mask = torch.isin(get_mask._mask, indexes.to(get_mask.device) + 1) # 1 to avoid background 0
+        retrieve_mask = torch.isin(
+            get_mask._mask, indexes.to(get_mask.device) + 1
+        )  # 1 to avoid background 0
         get_mask = DetectMask(torch.where(retrieve_mask, get_mask._mask, 0))
         get_mask.reindex()
 
         return get_mask
-    
+
     def __iter__(self):
         """Iterate over Mask return binary mask for each value in 1-N range with N objects. Do not iter over
-        background class 0."""
-        object_ids = torch.unique(self._mask)[torch.unique(self._mask)!=0]
+        background class 0.
+
+        Yields:
+            ``DetectMask``: DetectMask with only 1 object.
+        """
+        object_ids = torch.unique(self._mask)[torch.unique(self._mask) != 0]
         for x in object_ids:
-            yield self[x-1]
+            yield self[x - 1]
 
     def to_binary_masks(self) -> Tensor:
         """Return one-hot encoded binary masks of shape (N, H, W) with one binary mask (0-1) for each
         of N objects. Do not return binary mask for background with value 0.
 
         Returns:
-            Tensor: Binary masks.
+            ``Tensor``:
+                - Binary masks (N,H,W).
         """
         self_values = torch.unique(self._mask)
         binary_masks = one_hot(self._mask.long()).permute(2, 0, 1)
         # remove background binary mask
         if 0 in self_values:
             binary_masks = binary_masks[1:]
-        
+
         return binary_masks
-    
+
     def __add__(self, mask: DetectMask, other_mask: DetectMask) -> DetectMask:
         """Concatenate masks stacked mask by managing values (positions of objects).
-
         Args:
-            mask (Tensor): Mask with indexes for objects in mask.
-            other_mask (Tensor): Mask with indexes for objects in other_mask
+            mask (``DetectMask``): Mask with indexes for objects in mask.
+            other_mask (``DetectMask``):  Mask with indexes for objects in other_mask.
+
+        Returns:
+            ``DetectMask``:
+                - Concatenated DetectMask.
         """
         # get max index of mask
         mask_max = torch.max(mask._mask)
         other_mask._mask[other_mask._mask > 0] += mask_max
         # add max index to toher mask at nonzero positions
         mask._mask += other_mask._mask
         mask._mask[other_mask._mask > 0] = other_mask._mask[other_mask._mask > 0]
 
         return DetectMask(mask._mask)
-    
+
     @property
     def n_objects(self):
-        """Return number of objjects in mask"""
+        """Return number of objects in mask"""
         return len(torch.unique(self._mask).nonzero())
-    
+
     def merge(
-    mask: DetectMask, other_mask: DetectMask, scores: Tensor, other_scores: Tensor
-) -> Tuple[Tensor, ...]:
+        mask: DetectMask, other_mask: DetectMask, scores: Tensor, other_scores: Tensor
+    ) -> Tuple[Tensor, ...]:
         """Merge 2 DetectMask with informations of scores. Objects masks are added in the  ascending order of scores such
         that lower score masks are overwritted by higer masks scores.
 
         Args:
-            mask (DetectMask): Stacked mask.
-            other_mask (DetectMask): Stacked_mask.
-            scores (Tensor): Scores for objects in mask 1.
-            other_scores (Tensor): Scores of objects in other mask.
+            mask (``DetectMask``): DetectMask 1.
+            other_mask (``DetectMask``): DetectMask 2
+            scores (``Tensor``): Scores for objects in mask 1.
+            other_scores (``Tensor``): Scores of objects in other mask.
 
         Returns:
-            DetectMask: Merged DetectMask.
-            Tensor: List of indices of stacked masks that are not overwritted in original values.
+            ``Tuple[DetectMask, Tensor]``:
+                - Merged DetectMask.
+
+                - List of indices of stacked masks that are not overwritted in original values.
         """
-        assert mask._mask.shape == other_mask._mask.shape, "Both mask should have the same shape."
+        assert (
+            mask._mask.shape == other_mask._mask.shape
+        ), "Both mask should have the same shape."
         # add number of objects of mask 1 to mask values of masks 2 for nonzero values
         other_mask._mask[other_mask._mask > 0] += torch.max(mask._mask)
 
         # merge all scores
         merged_scores = torch.cat([scores, other_scores])
         _, indices = torch.sort(merged_scores)
-        merged_mask = DetectMask(torch.zeros(mask._mask.shape, device=mask.device).long())
+        merged_mask = DetectMask(
+            torch.zeros(mask._mask.shape, device=mask.device).long()
+        )
         value = 1
         valid_indices = []
 
         for i in indices:
             if i > torch.max(mask._mask):
                 indice_mask = (other_mask._mask == i + 1) * value
             else:
                 indice_mask = (mask._mask == i + 1) * value
             # do not add empty masks
             if indice_mask.sum() == 0:
                 continue
-            
+
             merged_mask._mask[indice_mask > 0] = indice_mask[indice_mask > 0].int()
 
             value += 1
             valid_indices.append(i)
 
         return merged_mask, torch.tensor(valid_indices)
-        
 
 
 def is_binary(mask: Tensor) -> bool:
     """Check if a mask is binary (values in 0 - 1).
 
     Args:
-        mask (Tensor): Tensor to check.
+        mask (``Tensor``): Tensor to check.
 
     Returns:
-        bool: True if mask is binary
+        ``bool``:
+            - True if mask is binary else False.
     """
     binary = True
     if is_floating_point(mask):
         binary = False
     if mask.ndim != 2:
         binary = False
-    is_in01 = torch.isin(torch.unique(mask), torch.tensor([0,1], device=mask.device))
+    is_in01 = torch.isin(torch.unique(mask), torch.tensor([0, 1], device=mask.device))
     if False in is_in01:
         binary = False
-    
+
     return binary
```

### Comparing `detectools-0.1.5/src/detectools/formats/segmentation_format.py` & `detectools-0.1.6/src/detectools/formats/segmentation_format.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,45 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Literal, Tuple, Union
 
 import torch
 from detectools import Task
 from detectools.formats.detection_format import DetectionAnnotation, DetectionFormat
-from detectools.utils.mask_utils import cocopolygons2mask, cocoseg2masks, mask2polygons
+from detectools.formats.mask_utils import cocopolygons2mask, cocoseg2masks, mask2polygons
 from torch import Tensor, is_floating_point
 from torch.nn.functional import one_hot
 from torchvision.ops import masks_to_boxes
 from torchvision.transforms.v2 import ConvertBoundingBoxFormat
 from torchvision.transforms.v2.functional import crop_mask, pad_mask
 from torchvision.tv_tensors import BoundingBoxes, Mask
-from detectools.formats.mask import DetectMask
+from detectools.formats.detect_mask import DetectMask
 
 class SegmentationAnnotation(DetectionAnnotation):
-    """Class to wrap informations of detection objects."""
+    """BaseAnnotation child class for SegmentationAnnotation task.
+
+    Attributes:
+    -----------
+
+    Attributes:
+        boxe (``BoundingBoxes``): Boxe coordinates in XYWH format.
+        label (``Tensor``): Class label of object.
+        spatial_size (``Tuple[int, int]``): Size of corresponding image (H, W)
+        score (``Tensor``): Confidence score of the object (for prediction).
+        mask (``Tensor``): Object segmentation binary mask (H, W).
+    
+    Methods:
+    -----------
+    """
+
+    boxe : BoundingBoxes
+    label : Tensor
+    spatial_size: Tuple[int, int]
+    score: Tensor
+    mask: Tensor
 
     def __init__(
         self,
         spatial_size: Tuple[int],
         label: Tensor,
         boxe: Tensor,
         mask: Tensor,
@@ -32,22 +52,23 @@
         # assert mask is a stacked class maks
         super().__init__(spatial_size, label, boxe, score)
         self.mask = mask
 
     def object_to_coco(
         self, annotation_id: int = 1, image_id: int = 1
     ) -> Dict[str, Any]:
-        """Return COCO annotation dict from self.
+        """Return instance segmentation annotation data as COCO like dict.
 
         Args:
-            annotation_id (int): id to write on "id" field in annotation dict.
-            image_id (int): id to write for "image_id" field in annotation dict.
+            annotation_id (``int``, **optional**): Id of the annotation. Defaults to 1.
+            image_id (``int``, **optional**): Id of the corresponding image. Defaults to 1.
 
         Returns:
-            Dict[str, Any]: COCO like annotation dict.
+            ``Dict[str, Any]``:
+                - COCO like dict with annotation instance data.
         """
         # convert mask tensor to polygons
         polygons, area = mask2polygons(self.mask)
         annotation = {
             "id": annotation_id,
             "bbox": self.boxe.tolist(),
             "segmentation": polygons,
@@ -58,46 +79,78 @@
         if self.score:
             annotation["score"] = self.score.item()
 
         return annotation
 
 
 class SegmentationFormat(DetectionFormat):
-    """Data format for instance segmentation task. Contain labels, boxes & masks data."""
+    """BaseFormat child class for instance segmentation task.
+
+    Args:
+        spatial_size (``Tensor``): Spatial size (H, W) of corresponding images.
+        labels (``Tensor``): Tensor of shape (N,) with class labels for each object.
+        boxes (``Tensor``): Tensor of shape (N, 4). N for N objects and 4 for boxes coordinates.
+        scores (``Tensor``, **optional**): Tensor of shape (N,) with objects confidence score. Defaults to None.
+        box_format (``Literal['XYWH', 'XYXY', 'CXCYWH']``, **optional**): Format of bounding boxes. Defaults to 'XYWH'.
+        masks (``Tensor``): Tensor of shape (H,W) with values from 0 to N, one value/object.
+    
+    Attributes:
+    -----------
+
+    Attributes:
+        box_format (``Literal["XYWH", "XYXY", "CXCYWH"]``): Format of bounding boxes.
+        spatial_size (``Tuple[int, int]``): Size of corresponding image (H, W)
+        size (``int``): Number of objects in BaseFormat.
+        data: (``Dict[str, Tensor]``): Data dict that contains objects informations in it's keys (labels, boxes, scores, masks).
+    
+    Methods:
+    -----------
+    """
+    
+    spatial_size: Tuple[
+        int, int
+    ]  # Store the H, W image size corresponding to objects boxes/masks stored in BaseFormat.
+    data: Dict[
+        str, Tensor
+    ]  # Store all values (labels, boxes/masks at least) corresponding to objects in an image.
+    size: int  # Number of objects in image.
+    box_format: Literal["XYWH", "XYXY", "CXCYWH"]  # format for bounding boxes.
 
     # override
     def empty(spatial_size: Tuple[int]) -> SegmentationFormat:
-        """Return an empty SegmentationFormat.
+        """Return an empty instance SegmentationFormat.
 
         Args:
-            spatial_size (Tuple[int]): Spatial size for future objects in SegmentationFormat.
+            spatial_size (``Tuple[int]``): Size (H, W) of the corresponding image.
 
         Returns:
-            SegmentationFormat: SegmentationFormat with no objects in.
+            ``SegmentationFormat``:
+                - SegmentationFormat instance.
         """
         boxes = torch.tensor([[]])
         labels = torch.tensor([])
         masks = Mask(torch.zeros((spatial_size)).int())  # mask full of 0
         detection_format = SegmentationFormat(
             spatial_size=spatial_size, labels=labels, boxes=boxes, masks=masks
         )
         return detection_format
 
     # override
     def from_coco(
         coco_annotations: List[Dict[str, Any]], spatial_size: Tuple[int]
     ) -> SegmentationFormat:
-        """Create a format from a list of COCO annotations.
+        """Return SegmentationFormat from an image COCO data dictionnary.
 
         Args:
-            coco_annotations (List[Dict[str, Any]]): List of annotations (from COCO json file or other COCO data structure).
-            spatial_size (Tuple[int]): Dimension of corresponding image.
+            coco_annotations (``List[Dict[str, Any]]``): Coco data dictionnary.
+            spatial_size (``Tuple[int]``): Size (H, W) of the corresponding image.
 
         Returns:
-            DetectionFormat: Format with COCO objects informations stored in data dict.
+            ``SegmentationFormat``:
+                - SegmentationFormat instance.
         """
         boxes = torch.tensor([ann["bbox"] for ann in coco_annotations])
         labels = torch.tensor([ann["category_id"] for ann in coco_annotations])
         masks: DetectMask = DetectMask(torch.zeros(spatial_size))
         # assign obj id to DetecMask
         for i, ann in enumerate(coco_annotations):
             ann_mask = cocoseg2masks(ann["segmentation"], spatial_size)
@@ -146,14 +199,18 @@
         self.box_format = box_format
         self.size = labels.nelement()
         self.spatial_size = spatial_size
 
     def set(self, key: str, value: Tensor):
         """Set a new pair of key/value. Value should be of shape (N, ...) with N == self.size.
         if key is "masks" and value is binary masks (N, H, W), size is N, if value is stacked mask (H,W). size is unstacked_masks.
+
+        Args:
+            key (``str``): Key of value to set.
+            value (``Tensor``): Data as tensor.
         """
 
         # get shape of new value and assert it's equal to self.size
         if key == "masks":
             if not isinstance(value, DetectMask):
                 value: DetectMask = DetectMask(value)
             data_size = value.n_objects
@@ -165,41 +222,63 @@
         ), f"New value size should be equal to self.size, got {data_size} and {self.size}."
         # assign value to key with correct device
         device = self.get_device()
         value = value.to(device)
         self.data[key] = value
 
     def get_object(self, indice: int) -> SegmentationAnnotation:
-        """Return a SegmentationAnnotation object at position indice."""
+        """Return SegmentationAnnotation object at position indice.
+
+        Args:
+            indice (``int``): Position of object to gather.
+
+        Returns:
+            ``SegmentationAnnotation``:
+                - SegmentationAnnotation instance.
+        """
         single_object_format = self[indice]
         bbox, label, mask = single_object_format.get("boxes", "labels", "masks")
         segmentation_object = SegmentationAnnotation(
             self.spatial_size, label, bbox.squeeze(), mask._mask
         )
         if "scores" in single_object_format:
             segmentation_object.score = single_object_format.get("scores")
 
         return segmentation_object
 
     # Methods that changes internal states of Formats
     def crop(self, top: int, left: int, height: int, width: int):
-        """Crop boxes and mask and update spatial size."""
+        """Crop boxes and mask from top corner pixel and update spatial size.
+
+        Args:
+            top (``int``): Position to crop from top border.
+            left (``int``): Position to crop from left border.
+            height (``int``): height of the crop.
+            width (``int``): Width of the crop.
+        """
         self.spatial_size = (height, width)
         if self.size == 0:
             return self
         super().crop(top, left, height, width)
         masks: DetectMask = self.get("masks")
         cropped_masks = crop_mask(masks._mask, top=top, left=left, height=height, width=width)
         cropped_masks = DetectMask(cropped_masks)
         keep_indexes = cropped_masks.reindex()
         self.__dict__ = self[keep_indexes].__dict__.copy() # only copy dict to avoid duplicating object and loose masks change
         self.set("masks", cropped_masks)
 
     def pad(self, left: int, top: int, right: int, bottom: int):
-        """Pad boxes and mask and update spatial size."""
+        """Pad boxes and mask and update spatial size.
+
+        Args:
+            left (``int``): Pad value on left border.
+            top (``int``): Pad value on top border.
+            right (``int``): Pad value on right border.
+            bottom (``int``): Pad value on bottom border.
+        """
         super().pad(left, top, right, bottom)
         if self.size == 0:
             return
         masks: DetectMask = self.get("masks")
         padded_masks = pad_mask(masks._mask, padding=[left, top, right, bottom])
         self.set("masks", padded_masks)
```

### Comparing `detectools-0.1.5/src/detectools/models/mask2former.py` & `detectools-0.1.6/src/detectools/models/mask2former.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,56 @@
 
 import torch
 from detectools import Task
 from detectools.formats import BatchedFormats, SegmentationFormat
 from detectools.models import BaseModel
 from torch import Tensor
 from torchvision.ops import masks_to_boxes
-from detectools.formats.mask import DetectMask
+from detectools.formats.detect_mask import DetectMask
 from transformers import (
     Mask2FormerConfig,
     Mask2FormerForUniversalSegmentation,
     Mask2FormerImageProcessor,
 )
 from transformers.models.mask2former.modeling_mask2former import (
     Mask2FormerForUniversalSegmentationOutput,
 )
 
 
 class Mask2Former(Mask2FormerForUniversalSegmentation, BaseModel):
-    """Detectools class for Mask2Former."""
+    """Mask2Former model class in detectools. This class inheriths from Mask2FormerForUniversalSegmentation_ (HuggingFace, transformers) and BaseModel (detectools).
+    Construct Mask2Former model from huggingface/transformer model architectures.
+        
+    .. _Mask2FormerForUniversalSegmentation:
+            https://huggingface.co/docs/transformers/model_doc/mask2former
+
+    Args:
+        num_classes (``int``, **optional**): Number of classes. Defaults to 1.
+        pretrain (``Literal['large', 'medium', 'small', 'tiny']``, **optional**): Size of the pretrained model. Defaults to "tiny".
+        overlap_mask_thr (``float``, **optional**):  Mask threshold to merge masks from Mask2FormerOutput. Defaults to 0.8.
+
+    Attributes:
+    -----------
+
+    Attributes:
+        confidence_thr (``float``): Confidence score threshold to consider object as true prediction.
+        max_detection (``int``): Maximum number of object to predict on one image.
+        nms_threshold (``float``): IoU threshold to consider 2 boxes as overlapping for Non Max Suppression algorithm.
+        num_classes (``int``): Number of classes. 
+        size_configs (``Dict[str, str]``): Dict of existing depth configuration for Mask2Former.
+    
+    Methods:
+    -----------
+    """
+
+    confidence_thr: float = 0.5
+    max_detection: int = 300
+    nms_threshold: float = 0.45
+    num_classes: int = 1
+    overlap_mask_thr: float = 0.8
 
     # different model size from huggingface
     size_configs = {
         "large": "facebook/mask2former-swin-large-coco-instance",
         "medium": "facebook/mask2former-swin-base-coco-instance",
         "small": "facebook/mask2former-swin-small-coco-instance",
         "tiny": "facebook/mask2former-swin-tiny-coco-instance",
@@ -31,20 +60,15 @@
 
     def __init__(
         self,
         num_classes: int = 1,
         pretrain: Literal["large", "medium", "small", "tiny"] = "tiny",
         overlap_mask_thr: float = 0.8,
     ):
-        """
-        Args:
-            num_classes (int, optional): Number of classes. Defaults to 1.
-            pretrain (Literal[large, medium, small, tiny], optional): Size of the model. Defaults to "tiny".
-            overlap_mask_thr (float, optional): Mask threshold to merge masks from Mask2FormerOutput. Defaults to 0.8.
-        """
+        
         # assert Task mode is "instance_segmentation"
         assert (
             Task.mode == "instance_segmentation"
         ), f"Task mode should be 'instance_segmentation' to construct Mask2Former object, got {Task.mode}"
 
         if pretrain:
             pretrain_config = Mask2Former.size_configs[pretrain]
@@ -62,49 +86,55 @@
             do_resize=False, do_normalize=False, do_rescale=False, ignore_index=255
         )
 
         self.overlap_mask_thr = overlap_mask_thr
         self.num_classes = num_classes
 
     def to_device(self, device: Literal["cpu", "cuda"]):
-        """Send both model & all dependencies (like criterion) to device."""
+        """Send model to device.
+
+        Args:
+            device (``Literal['cpu', 'cuda']``): Device to send model on.
+        """
         self.to(device)
 
     def prepare_target(
         self, target: SegmentationFormat
     ) -> Tuple[Tensor, Dict[int, int]]:
         """Prepare targets for Mask2Former model.
 
         Args:
-            target (SegmentationFormat): target.
+            target (``SegmentationFormat``): Target.
 
         Returns:
-            Tuple[Tensor, Dict[int, int]]:  Segmentation map, correspondance dict between object idd and object label.
+            ``Tuple[Tensor, Dict[int, int]]``:
+                - Segmentation map.
+                - Dict of correspondance {object_id : object_label}.
         """
 
         labels = target.get("labels").clone()
         labels = torch.cat([torch.tensor([0], device=labels.device), labels + 1])
         instance_labels_dict = dict(zip(range(0, target.size + 1), labels.tolist()))
         masks = target.get("masks")._mask.clone()
 
         return masks, instance_labels_dict
 
     def prepare(
         self, images: Tensor, targets: BatchedFormats = None
     ) -> Dict[str, Union[Tensor, Dict[Any, Any]]]:
-        """Transform images and targets into model specific format for prediction & loss computation.
+        """Transform images and targets into Mask2Former specific format for prediction & loss computation.
 
         Args:
-            images: (Tensor): Batch images.
-            targets (BaseFormat): Targets from DetectionDataset.
+            images (``Tensor``): Batch images.
+            targets (``BatchedFormats``, **optional**): Batched targets from DetectionDataset.
 
         Returns:
-            (Union[Any, Tuple[Any]]) : In function of target input either:
-                - Image prepared for model
-                - Image prepared for model + Target prepared for model
+            ``Union[Any, Tuple[Any]]``:
+                - Images data prepared for Mask2Former.
+                - If targets: images + targets prepared for Mask2Former.
         """
 
         if targets:
             instance_labels = []
             segmentation_maps = []
             for target in targets.formats.values():
                 target_masks, target_dict = self.prepare_target(target)
@@ -122,21 +152,22 @@
                 images=list(images.unbind()),
                 return_tensors="pt",
             )
 
         return model_input
 
     def build_boxes(self, masks: Tensor) -> Tensor:
-        """Build boxes from segmentation masks.
+        """Build boxes from segmentation mask.
 
         Args:
-            masks (Tensor): _description_
+            masks (``Tensor``): Segmentation mask.
 
         Returns:
-            Tensor: _description_
+            ``Tensor``:
+                - Boxes (N, 4).
         """
         # do not infer boxes from background pixels (-1)
         mask_values = torch.unique(masks)
         if -1 in mask_values:
             mask_values = mask_values[1:]
 
         boxes = []
@@ -147,20 +178,23 @@
 
     # override
     def build_results(
         self,
         raw_outputs: Mask2FormerForUniversalSegmentationOutput,
         spatial_size: Tuple[int, int],
     ) -> BatchedFormats:
-        """Transform model outputs into Format for results.
+        """Transform model outputs into BatchedFormats for results.
 
         Args:
-            raw_outputs (Mask2FormerForUniversalSegmentationOutput): Mask2Former output.
+            raw_outputs (``Mask2FormerForUniversalSegmentationOutput``): Mask2Former output.
+            spatial_size (``Tuple[int, int]``): Size of original image (H, W).
+
         Returns:
-            (BatchedFormats): Model output as BatchedFormats.
+            ``BatchedFormats``:
+                - Model output as BatchedFormats.
         """
         # Process raw output wtih Mask2Former processor.
         batch_size = raw_outputs.masks_queries_logits.shape[0]
         predictions = self.processor.post_process_instance_segmentation(
             raw_outputs,
             overlap_mask_area_threshold=self.overlap_mask_thr,
             threshold=self.confidence_thr,
@@ -235,23 +269,26 @@
                 input[k] = v.to(device)
 
         return input
 
     def run_forward(
         self, images: Tensor, targets: BatchedFormats, predict: bool = False
     ) -> Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], BatchedFormats]]:
-        """Either only compute loss from images or, if target pass, compute loss & return both images
+        """Compute loss from images and if target passed, compute loss & return both loss dict
         and results.
 
         Args:
-            images (Tensor): Batch RGB images.
-            target (DetectionTarget): Batched DetectionTarget.
+            images (``Tensor``): Batch RGB images.
+            targets (``BatchedFormats``): Batch targets.
+            predict (``bool``, **optional**): To return predictions or not. Defaults to False.
 
         Returns:
-            Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], DetectionTarget]]: Loss Dict & otpionnaly SegmentationFormat.
+            ``Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], BatchedFormats]]``:
+                - Loss dict.
+                - If predict: Predictions.
         """
         assert predict == (
             not self.training
         ), f"Model mode should be equal to predict boolean, got {self.training} & {predict}"
         # prepare inputs
         spatial_size = images.shape[-2:]
         model_input = self.prepare(images, targets=targets)
@@ -271,19 +308,19 @@
         else:
             return loss_dict
 
     def get_predictions(self, images: Tensor) -> BatchedFormats:
         """Prepare images, Apply model forward pass and build results.
 
         Args:
-            images (Tensor): RGB images Tensor.
-            nms_thr (float): Threhsold for NMS algorithm.
-            confidence_thr: Confidence threshold for predicted instances selection.
+            images (``Tensor``): RGB images Tensor.
+
         Returns:
-            (BatchedFormats): Predictions for images as BatchedFormats.
+            ``BatchedFormats``:
+                - Predictions for images as BatchedFormats.
         """
         self.eval()
         spatial_size = images.shape[-2:]
         model_input = self.prepare(images)
         model_input = self.inputs_to_device(model_input, self.device)
         # predict
         output: Mask2FormerForUniversalSegmentationOutput = self(
```

### Comparing `detectools-0.1.5/src/detectools/models/yolo.py` & `detectools-0.1.6/src/detectools/models/yolo.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,32 +10,61 @@
 from ultralytics.cfg import get_cfg
 from ultralytics.models.yolo.detect.train import DetectionModel
 from ultralytics.nn.tasks import attempt_load_one_weight
 from ultralytics.utils import DEFAULT_CFG
 
 
 class YoloDetection(DetectionModel, BaseModel):
+    """YOLO detection model class in detectools. This class inheriths from DetectionModel_ (Ultralytics) and BaseModel (detectools).
+    Load yolo architecture from ultralytics repository. If pretrained load a pretrain model from ultralytics.
+
+    .. _DetectionModel:
+            https://docs.ultralytics.com/reference/nn/tasks/?h=detectionmodel#ultralytics.nn.tasks.DetectionModel.__init__
+
+    Args:
+        architecture (``str``, **optional**): Architecture to use to build YOLO model. Check Ultralytics availables architectures_ . Defaults to "yolov8m".
+        num_classes (``int``, **optional**): Number of classes in the task. Defaults to 1.
+        pretrained (``bool``, **optional**): To use pretrained weights. Defaults to True.
+        confidence_thr (``float``, **optional**): Confidence score threshold to consider object as true prediction. Defaults to 0.5.
+        max_detection (``int``, **optional**): Maximum number of object to predict on one image. Defaults to 300.
+        nms_threshold (``float``, **optional**): IoU threshold to consider 2 boxes as overlapping for Non Max Suppression algorithm.. Defaults to 0.45.
+    
+    .. _architectures:
+        https://docs.ultralytics.com/models/yolov8/#supported-tasks-and-modes
+
+    Attributes:
+    -----------
+
+    Attributes:
+        confidence_thr (``float``): Confidence score threshold to consider object as true prediction.
+        max_detection (``int``): Maximum number of object to predict on one image.
+        nms_threshold (``float``): IoU threshold to consider 2 boxes as overlapping for Non Max Suppression algorithm.
+        num_classes (``int``): Number of classes. 
+    
+    Methods:
+    -----------
+    """
+
+    confidence_thr: float = 0.5
+    max_detection: int = 300
+    nms_threshold: float = 0.45
+    num_classes: int = 1
 
     def __init__(
         self,
         architecture: str = "yolov8m",
         num_classes: int = 1,
         pretrained=True,
         confidence_thr: float = 0.5,
         max_detection: int = 300,
         nms_threshold: float = 0.45,
         *args,
         **kwargs,
     ):
-        """Load yolo architecture from ultralytics repository. If pretrained load the clasic pretrain model from ultralytics.
-
-        Args:
-            architecture (str) : Type of Yolo to load.
-            pretrained (bool): to download model or not.
-        """
+        
         # assert Task mode is "instance_segmentation"
         assert (
             Task.mode == "detection"
         ), f"Task mode should be 'detection' to construct YoloDetection object, got {Task.mode}"
         # build model from ultralytics config
         super().__init__(f"{architecture}.yaml", nc=num_classes, *args, **kwargs)
         self.args = get_cfg(DEFAULT_CFG)
@@ -49,41 +78,50 @@
             architecture = attempt_load_one_weight(
                 f"{architecture}.pt",
             )
             self.load(architecture[0])
 
     # override
     def to_device(self, device: Literal["cpu", "cuda"]):
-        """Send both model & criterion to device."""
+        """Send model & criterion to device.
+
+        Args:
+            device (``Literal['cpu', 'cuda']``): Device to send model on.
+        """
         self.to(device)
         self.criterion = self.init_criterion()
 
-    def prepare_image(self, images: Tensor) -> Tuple[int]:
+    def prepare_image(self, images: Tensor) -> Tuple[Tensor, Tuple[int]]:
         """Pad images if needed & return padding values.
 
         Args:
-            images (Tensor): Batch_images.
+            images (``Tensor``): Batch_images.
 
         Returns:
-            Tuple[int]: Padded images & coordinates.
+            ``Tuple[Tensor, Tuple[int]]``:
+                - Padded images.
+                - Padding values.
         """
         # get borders padding
-        coordinates = self.yolo_pad_requirements(images)
+        padding_values = self.yolo_pad_requirements(images)
         # pad images
-        images = F.pad(images, list(coordinates))
-        return images, coordinates
+        images = F.pad(images, list(padding_values))
+        return images, padding_values
+
+    def prepare_target(self, targets: BatchedFormats) -> Dict[str, Tensor]:
+        """Transform DetectionFormat targets into yolo targets format.
 
-    def prepare_target(self, targets: BatchedFormats) -> Tensor:
-        """Transform detection target into yolo targets format.
         Args:
-            target (Format): Detectools Target.
+            targets (``BatchedFormats``): Batch targets.
+
         Returns:
-            (Tensor) targets in yolo shape.
+            ``Dict[str, Tensor]``:
+                - Targets in YOLO format.
         """
-        # transfor boxes
+        # transform boxes
         targets.apply("set_boxes_format", "CXCYWH")
         targets.apply("normalize")
         # get values
         targets: List[DetectionFormat] = targets.split()
         boxes = torch.cat([t.get("boxes") for t in targets])
         labels = torch.cat([t.get("labels") for t in targets])
         device = labels.device
@@ -97,25 +135,25 @@
         batch_targets = {"batch_idx": indexes, "cls": classes, "bboxes": boxes}
 
         return batch_targets
 
     # override
     def prepare(
         self, images: Tensor, targets: BatchedFormats = None
-    ) -> Union[Any, Tuple[Any]]:
-        """Transform images and targets into model specific format for prediction & loss computation.
+    ) -> Union[Tensor, Tuple[Tensor, Dict[str, Tensor]]]:
+        """Transform images and targets into YOLO specific format for prediction & loss computation.
 
         Args:
-            images: (Tensor): Batch images.
-            targets (Format): Targets from DetectionDataset.
+            images (``Tensor``): Batch images.
+            targets (``BatchedFormats``, **optional**): Batched targets from DetectionDataset.
 
         Returns:
-            (Union[Any, Tuple[Any]]) : In function of target input either:
-                - Image prepared for model
-                - Image prepared for model + Target prepared for model
+            ``Union[Tensor, Tuple[Tensor, Dict[str, Tensor]]]``:
+                - Images data prepared for YOLO.
+                - If targets: images + targets prepared for YOLO.
         """
 
         (left, top, right, bottom) = self.yolo_pad_requirements(images)
         # pad images & target
         images = F.pad(images, list((left, top, right, bottom)))
         if targets:
             prepared_targets = targets.clone()
@@ -128,15 +166,19 @@
 
     def yolo_pad_requirements(
         self, input_object: Union[Tensor, DetectionFormat]
     ) -> List[int]:
         """Return values for padding to fit 'divisible by 32' requirement.
 
         Args:
-            input_object (Union[Tensor, Format]): Batch images.
+            input_object (``Union[Tensor, DetectionFormat]``): Input to pad (image or DetectionFormat).
+
+        Returns:
+            ``List[int]``:
+                - Padding values.
         """
         # get spatial size
         if isinstance(input_object, DetectionFormat):
             h, w = input_object.spatial_size
         elif isinstance(input_object, Tensor):
             h, w = input_object.shape[-2:]  # (H,W)
         # get pad values
@@ -156,42 +198,45 @@
             left, top, right, bottom = (0, 0, 0, 0)
         return (left, top, right, bottom)
 
     def retrieve_spatial_size(self, raw_outputs: List[Tensor]) -> Tuple[int]:
         """Retrieve image shape from raw_outputs and stride values.
 
         Args:
-            raw_outputs (List[Tensor]): Yolo model output.
+            raw_outputs (``List[Tensor]``): Raw ouptuts from YOLO model.
 
         Returns:
-            Tuple[int]: H, W shape of input.
+            ``Tuple[int]``:
+                - Size of input image (H, W).
         """
         h = int(raw_outputs[0].shape[-2] * self.stride[0])
         w = int(raw_outputs[0].shape[-1] * self.stride[0])
         return (h, w)
 
     # override
     def build_results(
-        self, raw_outputs: List[Tensor], prebuild_output: Tensor
+        self, raw_outputs: List[Tensor], prebuild_outputs: Tensor
     ) -> BatchedFormats:
-        """Transform model outputs into Format for results.
+        """Transform model outputs into Batch DetectionFormat for results.
 
         Args:
-            raw_outputs (Any): Model outputs.
-            prebuild_outptu (Tensor): Extracted boxes from yolo raw outputs.
+            raw_outputs (``List[Tensor]``): Model outputs.
+            prebuild_outputs (``Tensor``): Extracted boxes from YOLO raw outputs.
+
         Returns:
-            (Format): Model output as Format.
+            ``BatchedFormats``:
+                - Batched predictions.
         """
 
-        prebuild_output = prebuild_output.unbind()
+        prebuild_outputs = prebuild_outputs.unbind()
         h, w = self.retrieve_spatial_size(raw_outputs)
         # create empty Format to merge batch results
         results = []
         # for each prediction
-        for prediction in prebuild_output:
+        for prediction in prebuild_outputs:
             # send pred in good pshape
             prediction = prediction.permute(1, 0)
             # get best class and corresponding score
             best_class = torch.argmax(prediction[:, 4:], dim=1)
             confidence = torch.max(prediction[:, 4:], dim=1)
             # gather box cxcywh coordinates
             boxes_coordinates = prediction[:, :4]
@@ -215,50 +260,54 @@
         if len(results) == 0:
             results = DetectionFormat.empty((h, w))
 
         results = BatchedFormats(results)
         return results
 
     def compute_loss(
-        self, raw_outputs: Any, targets: DetectionFormat
+        self, raw_outputs: Tensor, targets: Dict[str, Tensor]
     ) -> Dict[str, Tensor]:
         """Compute loss with predictions & targets.
 
         Args:
-            predictions (Any): Raw output of model.
-            targets (Format): Prepared targets for loss.
+            raw_outputs (``Any``): Raw output of model.
+            targets (``DetectionFormat``): Targets in YOLO format.
 
         Returns:
-            Dict[str, Tensor]: Loss dict with global loss (key: "loss") & sublosses.
+            ``Dict[str, Tensor]``:
+                - Loss dict with total loss (key: "loss") & sublosses.
         """
         loss, loss_detail = self.criterion(raw_outputs, targets)
         loss_dict = {
             "loss": loss,
             "loss_box": loss_detail[0],
             "loss_cls": loss_detail[1],
             "loss_dfl": loss_detail[2],
         }
         return loss_dict
 
     # override
     def run_forward(
         self,
         images: Tensor,
-        targets: DetectionFormat,
+        targets: BatchedFormats,
         predict: bool = False,
-    ) -> Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], DetectionFormat]]:
-        """Either only compute loss from images or, if target pass, compute loss & return both images
+    ) -> Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], BatchedFormats]]:
+        """Compute loss from images and if target passed, compute loss & return both loss dict
         and results.
 
         Args:
-            images (Tensor): Batch RGB images.
-            target (Format): Batched Format.
+            images (``Tensor``): Batch RGB images.
+            targets (``BatchedFormats``): Batch targets.
+            predict (``bool``, **optional**): To return predictions or not. Defaults to False.
 
         Returns:
-            Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], Format]]: Loss Dict & otpionnaly Format.
+            ``Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], BatchedFormats]]``:
+                - Loss dict.
+                - If predict: predictions.
         """
         assert predict == (
             not self.training
         ), f"Model mode should be equal to predict boolean, got {self.training} & {predict}"
         # prepare inputs
         prepared_images, prepared_targets = self.prepare(images, targets=targets)
         # run forward pass
@@ -275,23 +324,23 @@
             h, w = images.shape[-2:]
             predictions.apply("crop", top, left, h, w)
             return loss_dict, predictions
         else:
             return loss_dict
 
     # override
-    def get_predictions(self, images: Tensor) -> DetectionFormat:
-        """Prepare images, Apply model forward pass and build results.
+    def get_predictions(self, images: Tensor) -> BatchedFormats:
+        """Prepare images, Apply YOLO forward pass and build results.
 
         Args:
-            images (Tensor): RGB images Tensor.
-            nms_thr (float): Threhsold for NMS algorithm.
-            confidence_thr: Confidence threshold for predicted instances selection.
+            images (``Tensor``): RGB images Tensor.
+
         Returns:
-            (Format): predictions for images as Format.
+            ``BatchedFormats``:
+                - Predictions for images as BatchedFormats.
         """
         self.eval()
         # get original spatial size
         ori_h, ori_w = images.shape[-2:]
         # pad images
         images, (left, top, _, _) = self.prepare_image(images)
         # predict
```

### Comparing `detectools-0.1.5/src/detectools/models/yolov8_seg.py` & `detectools-0.1.6/src/detectools/models/yolov8_seg.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,36 +10,61 @@
 from torchvision.ops import nms
 from torchvision.transforms.v2 import ConvertBoundingBoxFormat
 from torchvision.tv_tensors import BoundingBoxes
 from ultralytics.cfg import get_cfg
 from ultralytics.nn.tasks import SegmentationModel, attempt_load_one_weight
 from ultralytics.utils import DEFAULT_CFG
 from ultralytics.utils.ops import scale_masks
-from detectools.formats.mask import DetectMask
+from detectools.formats.detect_mask import DetectMask
 
 
 class Yolov8Segmentation(SegmentationModel, BaseModel):
 
+    """YOLO segmentation model class in detectools. This class inheriths from SegmentationModel_ (Ultralytics) and BaseModel (detectools).
+    Load yolo architecture from ultralytics repository. If pretrained load a pretrain model from ultralytics.
+
+    .. _SegmentationModel:
+            https://docs.ultralytics.com/reference/nn/tasks/?h=detectionmodel#ultralytics.nn.tasks.SegmentationModel.__init__
+
+
+    Args:
+        architecture (``str``, **optional**): Architecture to use to build YOLO model. Check Ultralytics availables architectures_ . Defaults to "yolov8m".
+        num_classes (``int``, **optional**): Number of classes in the task. Defaults to 1.
+        pretrained (``bool``, **optional**): To use pretrained weights. Defaults to True.
+        confidence_thr (``float``, **optional**): Confidence score threshold to consider object as true prediction. Defaults to 0.5.
+        max_detection (``int``, **optional**): Maximum number of object to predict on one image. Defaults to 300.
+        nms_threshold (``float``, **optional**): IoU threshold to consider 2 boxes as overlapping for Non Max Suppression algorithm.. Defaults to 0.45.
+    
+    .. _architectures:
+        https://docs.ultralytics.com/models/yolov8/#supported-tasks-and-modes
+
+    Attributes:
+    -----------
+
+    Attributes:
+        confidence_thr (``float``): Confidence score threshold to consider object as true prediction.
+        max_detection (``int``): Maximum number of object to predict on one image.
+        nms_threshold (``float``): IoU threshold to consider 2 boxes as overlapping for Non Max Suppression algorithm.
+        num_classes (``int``): Number of classes. 
+    
+    Methods:
+    -----------
+    """
+
     def __init__(
         self,
         architecture: str = "yolov8n-seg",
         pretrained=True,
         confidence_thr: float = 0.5,
         max_detection: int = 300,
         nms_threshold: float = 0.45,
         num_classes: int = 1,
         *args,
         **kwargs,
     ):
-        """Load yolo architecture from ultralytics repository. If pretrained load the clasic pretrain model from ultralytics.
-
-        Args:
-            architecture (str) : Type of Yolo to load.
-            pretrained (bool): to download model or not.
-        """
         # assert Task mode is "instance_segmentation"
         assert (
             Task.mode == "instance_segmentation"
         ), f"Task mode should be 'instance_segmentation' to construct Yolov8Segmentation object, got {Task.mode}"
         # build model from ultralytics config
         super().__init__(f"{architecture}.yaml", nc=num_classes, *args, **kwargs)
         self.args = get_cfg(DEFAULT_CFG)
@@ -52,31 +77,35 @@
         if pretrained:
             architecture = attempt_load_one_weight(
                 f"{architecture}.pt",
             )
             self.load(architecture[0])
 
     def to_device(self, device: Literal["cpu", "cuda"]):
-        """Send both model & criterion to device."""
+        """Send model & criterion to device.
+
+        Args:
+            device (``Literal['cpu', 'cuda']``): Device to send model on.
+        """
         self.to(device)
         self.criterion = self.init_criterion()
 
     def prepare(
         self, images: Tensor, targets: BatchedFormats = None
     ) -> Union[Any, Tuple[Any]]:
-        """Transform images and targets into model specific format for prediction & loss computation.
+        """Transform images and targets into YOLO specific format for prediction & loss computation.
 
         Args:
-            images: (Tensor): Batch images.
-            targets (InstanceFormat): Targets from DetectionDataset.
+            images (``Tensor``): Batch images.
+            targets (``BatchedFormats``, **optional**): Batched targets from DetectionDataset.
 
         Returns:
-            (Union[Any, Tuple[Any]]) : In function of target input either:
-                - Image prepared for model
-                - Image prepared for model + Target prepared for model
+            ``Union[Tensor, Tuple[Tensor, Dict[str, Tensor]]]``:
+                - Images data prepared for YOLO.
+                - If targets: images + targets prepared for YOLO.
         """
 
         (left, top, right, bottom) = self.yolo_pad_requirements(images)
         # pad images & target
         images = F.pad(images, list((left, top, right, bottom)))
         if targets:
             prepared_targets = targets.clone()
@@ -87,21 +116,23 @@
         else:
             return images
 
     def build_results(
         self,
         raw_output: Tuple[Tensor, ...],
     ) -> BatchedFormats:
-        """Build results from eval mode raw outputs of architecture.
+        """Transform model outputs into Batch SegmentationFormat for results.
 
         Args:
-            raw_output (Tuple[Tensor, ...]): Raw output of eval mode.
+            raw_outputs (``List[Tensor]``): Model outputs.
+            prebuild_outputs (``Tensor``): Extracted boxes from YOLO raw outputs.
 
         Returns:
-            BatchedFormats: BatchedFormats with 1 format for each image passed in forward.
+            ``BatchedFormats``:
+                - Batched predictions.
         """
 
         # TODO reduce size of this function by splitting in smaller ones
         # extract informations from raw_results
         boxes, cls_scores, mask_weights, protos = self.prebuild_output(raw_output)
         # gather device & spatila_size
         spatial_size = self.retrieve_spatial_size(raw_output)
@@ -190,23 +221,26 @@
 
         results = BatchedFormats(results)
         return results
 
     def run_forward(
         self, images: Tensor, targets: BatchedFormats, predict: bool = False
     ) -> Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], BatchedFormats]]:
-        """Either only compute loss from images or, if target pass, compute loss & return both images
+        """Compute loss from images and if target passed, compute loss & return both loss dict
         and results.
 
         Args:
-            images (Tensor): Batch RGB images.
-            target (DetectionTarget): Batched DetectionTarget.
+            images (``Tensor``): Batch RGB images.
+            targets (``BatchedFormats``): Batch targets.
+            predict (``bool``, **optional**): To return predictions or not. Defaults to False.
 
         Returns:
-            Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], DetectionTarget]]: Loss Dict & otpionnaly SegmentationFormat.
+            ``Union[Dict[str, Tensor], Tuple[Dict[str, Tensor], BatchedFormats]]``:
+                - Loss dict.
+                - If predict: predictions.
         """
         assert predict == (
             not self.training
         ), f"Model mode should be equal to predict boolean, got {self.training} & {predict}"
         # prepare inputs
         prepared_images, prepared_targets = self.prepare(images, targets=targets)
         # run forward pass
@@ -223,22 +257,22 @@
             h, w = images.shape[-2:]
             predictions.apply("crop", top, left, h, w)
             return loss_dict, predictions
         else:
             return loss_dict
 
     def get_predictions(self, images: Tensor) -> BatchedFormats:
-        """Prepare images, Apply model forward pass and build results.
+        """Prepare images, Apply YOLO forward pass and build results.
 
         Args:
-            images (Tensor): RGB images Tensor.
-            nms_thr (float): Threhsold for NMS algorithm.
-            confidence_thr: Confidence threshold for predicted instances selection.
+            images (``Tensor``): RGB images Tensor.
+
         Returns:
-            (BatchedFormats): Predictions for images as BatchedFormats.
+            ``BatchedFormats``:
+                - Predictions for images as BatchedFormats.
         """
         self.eval()
         # get original spatial size
         ori_h, ori_w = images.shape[-2:]
         # pad images
         images, (left, top, _, _) = self.prepare_image(images)
         # predict
@@ -248,51 +282,58 @@
         results.apply("crop", top, left, ori_h, ori_w)
         return results
 
     def prebuild_output(self, raw_output: Tuple[Tensor, ...]) -> Tuple[Tensor, ...]:
         """Unpack Yolov8-seg (eval mode) raw results.
 
         Args:
-            raw_output (Tuple): Yolov8 raw eval mode results
+            raw_output (``Tuple[Tensor, ...]``): Yolov8 raw eval mode results.
 
         Returns:
-            Tuple[Tensor]: boxes (N_batch, N_obj, cxcywh), cls_scores (N_batch, N_cls), mask_weights (N_batch, N_obj, 32), protos (N_batch, protos)
+            ``Tuple[Tensor, ...]``:
+                - boxes (N_batch, N_obj, cxcywh).
+                - cls_scores (N_batch, N_cls).
+                - mask_weights (N_batch, N_obj, 32).
+                - protos (N_batch, protos).
         """
         output0, output1 = raw_output
         output0 = output0.permute(0, 2, 1)  # permute in N_batch, N_obj, obj_length
         boxes = output0[:, :, 0:4]
         cls_indx = 4 + self.num_classes
         cls_scores = output0[:, :, 4:cls_indx]
         mask_weights = output0[:, :, -32:]
         protos = output1[2]
         return boxes, cls_scores, mask_weights, protos
 
     def prepare_image(self, images: Tensor) -> Tuple[Tensor, int]:
         """Pad images if needed & return padding values.
 
         Args:
-            images (Tensor): Batch_images.
+            images (``Tensor``): Batch_images.
 
         Returns:
-            Tuple[int]: Padded images & coordinates.
+            ``Tuple[Tensor, Tuple[int]]``:
+                - Padded images.
+                - Padding values.
         """
         # get borders padding
         coordinates = self.yolo_pad_requirements(images)
         # pad images
         images = F.pad(images, list(coordinates))
         return images, coordinates
 
     def prepare_target(self, target: BatchedFormats) -> Dict[str, Tensor]:
-        """Convert InstanceFormat to a yolov8-seg loss computation compatible format.
+        """Transform SegmentationFormat targets into yolo-seg targets format.
 
         Args:
-            InstanceFormat (InstanceFormat): The target to transform.
+            targets (``BatchedFormats``): Batch targets.
 
         Returns:
-            Dict: a dict containing all info as per yolov8-seg loss format.
+            ``Dict[str, Tensor]``:
+                - Targets in YOLO format.
         """
         target.apply("set_boxes_format", "CXCYWH")
         target.apply("normalize")
         targets: List[SegmentationFormat] = target.split()
         boxes = torch.cat([t.get("boxes") for t in targets])
         labels = torch.cat([t.get("labels") for t in targets])
         device = labels.device
@@ -313,15 +354,19 @@
 
     def yolo_pad_requirements(
         self, input_object: Union[Tensor, SegmentationFormat]
     ) -> Tuple[int, ...]:
         """Return values for padding to fit 'divisible by 32' requirement.
 
         Args:
-            input_object (Union[Tensor, Format]): Batch images.
+            input_object (``Union[Tensor, DetectionFormat]``): Input to pad (image or DetectionFormat).
+
+        Returns:
+            ``List[int]``:
+                - Padding values.
         """
         # get spatial size
         if isinstance(input_object, SegmentationFormat):
             h, w = input_object.spatial_size
         elif isinstance(input_object, Tensor):
             h, w = input_object.shape[-2:]  # (H,W)
         # get pad values
@@ -341,76 +386,81 @@
             left, top, right, bottom = (0, 0, 0, 0)
         return (left, top, right, bottom)
 
     def retrieve_spatial_size(self, raw_outputs: List[Tensor]) -> Tuple[int, int]:
         """Retrieve image shape from raw_outputs and stride values.
 
         Args:
-            raw_outputs (List[Tensor]): Yolo model output.
+            raw_outputs (``List[Tensor]``): Raw ouptuts from YOLO model.
 
         Returns:
-            Tuple[int]: H, W shape of input.
+            ``Tuple[int]``:
+                - Size of input image (H, W).
         """
         if self.training:
             h = int(raw_outputs[0][0].shape[-2] * self.stride[0])
             w = int(raw_outputs[0][0].shape[-1] * self.stride[0])
         else:
             h = int(raw_outputs[1][0][0].shape[-2] * self.stride[0])
             w = int(raw_outputs[1][0][0].shape[-1] * self.stride[0])
         return (h, w)
 
     def compute_loss(self, predictions: Tuple, target: Dict) -> Dict[str, Tensor]:
-        """Compute yolov8-seg loss.
+        """Compute loss with predictions & targets.
 
         Args:
-            predictions (Tuple): forward from yolo model
-            target (Dict): batch target in yolo_format
+            raw_outputs (``Any``): Raw output of model.
+            targets (``DetectionFormat``): Targets in YOLO format.
 
         Returns:
-            (Dict[str, Tensor]) : yolov8-seg loss and detailled losses.
+            ``Dict[str, Tensor]``:
+                - Loss dict with total loss (key: "loss") & sublosses.
         """
         loss, loss_detail = self.criterion(predictions, target)
         loss_dict = {
             "loss": loss,
             "loss_box": loss_detail[0],
             "loss_seg": loss_detail[1],
             "loss_cls": loss_detail[2],
             "loss_dfl": loss_detail[3],
         }
         return loss_dict
 
     def mask2yolo(self, mask: Tensor) -> Tensor:
-        """convert stacked binary to yolo mask, i.e (1, h, w) with values in [0, ... , Nobjs]
+        """Convert stacked binary to yolo mask, i.e (1, h, w) with values in [0, ... , Nobjs]
         This shape is suitable for yolov8 loss.
 
         Args:
-            mask (Tensor): stacked binary mask (1 per obj)
+            mask (``Tensor``): Stacked binary mask (N, H, W).
 
         Returns:
-            (Tensor) : yolo mask
+            ``Tensor``:
+                - YOLO segmentation mask.
         """
         if mask.ndim < 3:
             mask = mask[None, :]
         reindexing = torch.tensor(range(1, mask.shape[0] + 1)).to(mask.device)
         # convert to yolomask: stacked h, w with values in [0, ..., Nobjs], 0 being absence of object
         yolomask, _ = torch.max(mask * reindexing[:, None, None], dim=0)
         return yolomask[None, :]
 
     def proto2mask(
         self, protos: Tensor, weights: Tensor, boxes: Tensor, shape: Tuple[int]
     ) -> Tensor:
-        """combine protos and weights to get masks, then crop instances from boxes
-            Useful in predictions
+        """Combine protos and weights to get masks, then crop instances from boxes (Useful in predictions).
+
         Args:
-            protos (Tensor) : normal is 32 sub masks
-            weights (Tensor) : yolo weights (normal is 32)
-            boxes (Tensor) : [N, 4] in xyxy
-            shape : original image size (h, w)
+            protos (``Tensor``): Sub masks (32, ...).
+            weights (``Tensor``): YOLO mask weights (32, ...).
+            boxes (``Tensor``): Boxes (N, 4) in XYXY format.
+            shape (``Tuple[int]``): Original image size (H, W).
+
         Returns:
-            (Tensor) : yolo mask
+            ``Tensor``:
+                - YOLO segmentation mask.
         """
         c, mh, mw = protos.shape  # CHW
         masks = (weights @ protos.float().view(c, -1)).sigmoid().view(-1, mh, mw)
         masks: Tensor = scale_masks(masks[None], shape)[0]  # CHW
         for m in range(masks.shape[0]):
             xl, yl, xr, yr = boxes.int()[m]
             masks[m, 0:yl, :] = 0
```

### Comparing `detectools-0.1.5/src/detectools/trainer.py` & `detectools-0.1.6/src/detectools/train/trainer.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,43 +5,86 @@
 import torch
 from torch import Tensor
 from torch.optim import Optimizer
 from torch.utils.tensorboard import SummaryWriter
 from torchmetrics import Metric
 from tqdm import tqdm
 
-from detectools.dataset import DetectionLoader
+from detectools.data.dataset import DetectionLoader
 from detectools.models.base import BaseModel
 from detectools.formats import BatchedFormats
-from detectools.utils.trainer import Aggregator
+from detectools.train.loss_aggregator import Aggregator
 
 
 class Trainer:
+    """Trainer wrap the whole training process.
+
+    Args:
+        model (``BaseModel``): Detectools model.
+        otpimizer (``Optimizer``): Optimizer (from ``torch.optim``).
+        log_dir (``str``, **optional**): Path to store tensorboard logs. Defaults to "" (no log).
+        metrics (``List[Metric]``, **optional**): List of detectools metrics that will be computed at valid. Defaults to [].
+        device (``Literal['cpu', 'cuda']``, **optional**): Device to use for trainning. Defaults to "cpu".
+        nms_thr (``float``, **optional**): IoU threshold to consider 2 boxes as overlapping in NMS algorithm using for valid loop. Defaults to 0.45.
+        confidence_thr (``float``, **optional**): Minimum confidence score for each predicted object to be kept, used for valid loop. Defaults to 0.5.
+    
+        Example: Trainning loop.
+    -----------------------------
+
+    .. highlight:: python
+    .. code-block:: python
+
+        >>> from detectools.dataset import DetectionDataset, DetectionLoader
+        >>> from torch.utils.data import random_split
+        >>> import torch
+        >>> trainer : Trainer # Trainer already built
+        >>> data_path = \"path/to/data\"
+        >>> dataset = DetectionDataset(data_path)
+        >>> train_set, valid_set, test_set = random_split(dataset, 0.8,0.2,0.0)
+        >>> train_loader, valid_loader = DetectionLoader(train_set), DetectionLoader(valid_set)
+        >>> for e in range(10):
+        >>>     trainer.train_epoch(train_loader)
+        >>>     trainer.valid_epoch(valid_loader)
+        >>> torch.save(trainer.model, "/model/path/model.pth")
+    
+    Attributes:
+    -----------
+
+    Attributes:
+        model (``BaseModel``): Detectools model.
+        otpimizer (``Optimizer``): Optimizer (from ``torch.optim``).
+        log_dir (``str``, **optional**): Path to store tensorboard logs.
+        metrics (``List[Metric]``, **optional**): List of detectools metrics that will be computed at valid.
+        device (``Literal['cpu', 'cuda']``, **optional**): Device to use for trainning.
+        nms_thr (``float``, **optional**): IoU threshold to consider 2 boxes as overlapping in NMS algorithm using for valid loop.
+        confidence_thr (``float``, **optional**): Minimum confidence score for each predicted object to be kept, used for valid loop.
+    
+    Methods
+    ----------
+
+    """
+
+    model: BaseModel
+    otpimizer: Optimizer
+    log_dir: str
+    metrics: List[Metric]
+    device: Literal["cpu", "cuda"]
+    nms_threshold: float
+    confidence_threshold: float
 
     def __init__(
         self,
         model: BaseModel,
         otpimizer: Optimizer,
         log_dir: str = "",
         metrics: List[Metric] = [],
         device: Literal["cpu", "cuda"] = "cpu",
         nms_threshold: float = 0.45,
         confidence_threshold: float = 0.5,
     ):
-        """Create Trainer object.
-
-        Args:
-            model (BaseModel): Model from detectools.
-            otpimizer (Optimizer): Optimizer (from torch.optim).
-            log_dir (str, optional): Path to store tensorboard logs. Defaults to "".
-            metrics (List[Metric], optional): List of detectools metrics that will be computed at valid. Defaults to [].
-            device (Literal['cpu', 'cuda'], optional): Device to use for trainning. Defaults to "cpu".
-            nms_thr (float, optional): IoU threshold to consider 2 boxes as overlapping in NMS algorithm using for valid loop. Defaults to 0.45.
-            confidence_thr (float, optional): Minimum confidence score for each predicted object to be kept, used for valid loop. Defaults to 0.5.
-        """
 
         self.model = model
         self.model.to_device(device)
         self.optimizer = otpimizer
         metrics = [metric.to(device) for metric in metrics]
         self.metrics = metrics
         self.log_dir = log_dir
@@ -57,44 +100,50 @@
 
             Path(log_dir).mkdir(parents=True)
             self.board = SummaryWriter(log_dir)
         else:
             self.board = False
 
     def train_step(self, images: Tensor, targets: BatchedFormats) -> Dict[str, Tensor]:
-        """Run train step, return loss dict.
+        """Run forward pass, loss computation and backward pass.
 
         Args:
-            images (Tensor): Batch images RGB
-            target (BatchedFormats): Batched target.
+            images (``Tensor``): Batch images
+            targets (``BatchedFormats``): Batch targets.
 
         Returns:
-        Dict [str, Tensor]: Dict of losses containing gobal loss : "loss"
+            ``Dict[str, Tensor]``:
+                - Dict of losses containing (total loss at key 'loss').
         """
 
         loss_dict = self.model.run_forward(images, targets, predict=False)
         loss = loss_dict["loss"]
         loss.backward()
         self.optimizer.step()
         self.optimizer.zero_grad()
 
         return loss_dict
 
     def compute_metrics(
-        self, predictions: BatchedFormats, targets: BatchedFormats, batch_size: int
+        self, predictions: BatchedFormats, targets: BatchedFormats
     ) -> Dict[str, Tensor]:
         """Compute metrics.
 
         Args:
             predictions (BatchedFormats): Predictions.
             targets (BatchedFormats): Targets.
-            batch_size (int): Batch size to not forget image or predictions with no objects in splitting.
+
+
+        Args:
+            predictions (``BatchedFormats``): Predictions.
+            targets (``BatchedFormats``): Targets.
 
         Returns:
-            Dict[Dict[str, float]]: Dict of metrics.
+            ``Dict[str, Tensor]``:
+                - Metric values.
         """
         # split predictions to compute metric individual images # TODO make batchification possible
         splitted_predictions = predictions.split()
         splitted_targets = targets.split()
         # for each pair pred/target
         for i, target in enumerate(splitted_targets):
             pred = splitted_predictions[i]
@@ -111,36 +160,37 @@
 
     def valid_step(
         self, images: Tensor, targets: BatchedFormats
     ) -> Tuple[Dict[str, Tensor], Dict[str, Dict[str, Tensor]]]:
         """Run train step, return loss dict.
 
         Args:
-            images (Tensor): Batch images RGB
-            target (BatchedFormats): Batched target.
+            images (``Tensor``): Batch images.
+            targets (``BatchedFormats``): Targets.
 
         Returns:
-        Tuple[Dict [str, Tensor], Dict [str, Tensor]]: Dict of losses containing gobal loss : "loss" and dict of metrics.
+            ``Tuple[Dict[str, Tensor], Dict[str, Dict[str, Tensor]]]``:
+                - Losses and metrics values.
         """
         if self.model.training:
             self.model.eval()
-        batch_size = images.shape[0]
         loss_dict, predictions = self.model.run_forward(images, targets, predict=True)
-        predictions.apply("set_device",self.device)
-        metrics = self.compute_metrics(predictions, targets, batch_size)
+        predictions.apply("set_device", self.device)
+        metrics = self.compute_metrics(predictions, targets)
         return loss_dict, metrics
 
     def log_string(self, epoch_dict: Dict[str, Tensor]) -> str:
-        """Get epoch dict and return string to display in terminal.
+        """Transform epoch dict in string.
 
         Args:
-            epoch_dict (Dict[str, Tensor]): Dict of metric & loss values to display.
+            epoch_dict (``Dict[str, Tensor]``): Dict of epoch values to display.
 
         Returns:
-            str: string to print with epoch values.
+            ``str``:
+                - String to print with epoch values.
         """
         flattened_dict = epoch_dict.copy()
         for key, value in flattened_dict.items():
             if isinstance(value, dict):
                 flattened_dict[key] = value[list(value.keys())[0]]
 
         log = ""
@@ -155,25 +205,28 @@
         ep_number: int,
         mode: Literal["Train", "Valid"] = "Train",
         tag: str = "",
     ) -> Dict[str, Tensor]:
         """Run trainning epoch.
 
         Args:
-            loader (DetectionLoader): DetectionLoader.
-            ep_number (int): Epoch nb.
+            loader (``DetectionLoader``): DetectionLoader.
+            ep_number (``int``): Epoch number.
+            mode (``Literal['Train', 'Valid']``, **optional**): Mode of epoch, if "Valid" metrics are computed and gradient shuted down. Defaults to "Train".
+            tag (``str``, **optional**): Tag to link to epoch. Defaults to "".
 
         Returns:
-            Dict[str, Tensor]: Loss dict.
+            ``Dict[str, Tensor]``:
+                - Epochs values (Losses & metrics).
         """
         # create aggregator for loss averged accros samples
         loss_aggregator = Aggregator()
         iterator = tqdm(loader, total=len(loader), desc=f"Epoch {ep_number}/{tag}")
         # iterate over batches
-        for images, targets, names in iterator:
+        for images, targets, _ in iterator:
             batch_size = images.shape[0]
             # send to device
             images = images.to(self.device)
             targets: BatchedFormats
             targets.apply("set_device", self.device)
             # gather loss & metrics (if valid)
             if mode == "Train":
@@ -204,26 +257,52 @@
     def train_epoch(
         self,
         loader: DetectionLoader,
         ep_number: int,
         tag: str = "Train",
         *args,
         **kwargs,
-    ):
+    ) -> Dict[str, Tensor]:
+        """Run train epoch.
+
+        Args:
+            loader (``DetectionLoader``): DetectionLoader.
+            ep_number (``int``): Epoch number.
+            tag (``str``, **optional**): Tag to link to epoch. Defaults to "Train".
+
+        Returns:
+            ``Dict[str, Tensor]``:
+                - Epochs values (Losses).
+        """
         torch.set_grad_enabled(True)
         self.model.train()
-        epoch_dict = self.epoch(loader, ep_number, mode="Train", tag=tag, *args, **kwargs)
+        epoch_dict = self.epoch(
+            loader, ep_number, mode="Train", tag=tag, *args, **kwargs
+        )
         return epoch_dict
 
     def valid_epoch(
         self,
         loader: DetectionLoader,
         ep_number: int,
         tag: str = "Valid",
         *args,
         **kwargs,
-    ):
+    ) -> Dict[str, Tensor]:
+        """Run train epoch.
+
+        Args:
+            loader (``DetectionLoader``): DetectionLoader.
+            ep_number (``int``): Epoch number.
+            tag (``str``, **optional**): Tag to link to epoch. Defaults to "Valid".
+
+        Returns:
+            ``Dict[str, Tensor]``:
+                - Epochs values (Losses & metrics).
+        """
         torch.set_grad_enabled(False)
         self.model.eval()
-        epoch_dict = self.epoch(loader, ep_number, mode="Valid", tag=tag, *args, **kwargs)
+        epoch_dict = self.epoch(
+            loader, ep_number, mode="Valid", tag=tag, *args, **kwargs
+        )
         torch.set_grad_enabled(True)
         return epoch_dict
```

### Comparing `detectools-0.1.5/src/detectools/utils/data_management.py` & `detectools-0.1.6/src/detectools/data_management.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import json
 from pathlib import Path
 from typing import Any, Dict, List, Tuple, Union
 
-from detectools import load_json, raw_cocodict
-from detectools.dataset import DetectionDataset
+from detectools.data.dataset import DetectionDataset
+from detectools.utils import load_json, raw_cocodict
 from torch.utils.data import random_split
 
-
 def merge_jsons(
     jsonfiles: List[str], output_json: str, categories: List[Dict[str, Any]]
 ):
     """Take a list of json files paths and merge them in one respecting
-    the images/annotations correspondance id
+    the images/annotations correspondance id.
 
     Args:
-        jsonfiles (List[str]): List of paths of jsons to merge.
-        output_json (str): Path to store merged json.
-        categories (List[Dict[str, Any]]): List of categories as COCO format.
+        jsonfiles (``List[str]``): List of paths of jsons to merge.
+        output_json (``str``): Path to store merged json.
+        categories (``List[Dict[str, Any]]``): List of categories as COCO format.
     """
     # initialize counter and output json
     image_id = 0
     annotation_id = 0
     cocodict = raw_cocodict()
     cocodict["categories"] = categories
     # for each json file, read the file
@@ -56,18 +55,17 @@
     destination: str,
     proportions: Tuple[float] = (0.8, 0.2, 0.0),
 ) -> None:
     """Split one or multiple dataset folder according to split proportions and write a new dataset
     with the fusion same split for each datqset (train, valid, test).
 
     Args:
-        source_datasets (Union[str, List[str]]): Path to ad dataset or list of dataset.
-        destination (str): Path of Splitted datset.
-        proportions (Tuple[float], optional): prportions for train, valid & test resptively. Defaults to (0.8, 0.2, 0.0).
-        scaling_off (bool): To disable scaling during dataset get item.
+        source_datasets (``Union[str, List[str]]``): Path to ad dataset or list of dataset.
+        destination (``str``): Path tostore subsets.
+        proportions (``Tuple[float]``, **optional**): Proportions for train, valid & test. Defaults to (0.8, 0.2, 0.0).
     """
     # if source_datasets is a string wrap it in list
     if isinstance(source_datasets, str):
         source_datasets = [source_datasets]
     # for each source dataset do the split
     for dataset_path in source_datasets:
         print(f"Splitting dataset: {dataset_path}")
@@ -79,8 +77,8 @@
         # for each subset
         for subset_dataset, subset_name in subsets:
             print(f"Export {subset_name} data:")
             subset_path = Path(destination) / subset_name
             dataset.export_dataset(
                 f"{subset_path}",
                 indices=subset_dataset.indices,
-            )
+            )
```

### Comparing `detectools-0.1.5/src/detectools/utils/inference.py` & `detectools-0.1.6/src/detectools/inference/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,73 @@
 from itertools import product
 from math import ceil, floor
 from typing import Tuple
+
 import torch
+from detectools import Task
+from detectools.formats import BaseFormat, Format
+from detectools.formats.detect_mask import DetectMask
 from torch import List, Tensor
 from torchvision.transforms.v2.functional import crop, pad
-from detectools.formats import Format
-from detectools import Task
-from detectools.formats.mask import DetectMask
 
 
 def add_offset(image: Tensor, offset: int) -> Tensor:
     """Pad fix number of pixels around sides of image
-
     Args:
-        image (Tensor): Image to pad.
-        offset (int): Number of pixels to pad.
+        image (``Tensor``): Image to pad.
+        offset (``int``): Number of pixels to pad.
 
     Returns:
-        Tensor: Image padded.
+        ``Tensor``:
+            - Padded image.
     """
     return pad(image, offset)
 
 
 def remove_offset(image: Tensor, offset: int) -> Tensor:
     """Remove fix number of pixels on each side of image.
 
     Args:
         image (Tensor): Image.
         offset (int): Border size to remove.
 
     Returns:
         Tensor: Image without offset.
+
+    Args:
+        image (``Tensor``): Image to pad.
+        offset (``int``): Number of pixels to remove.
+
+    Returns:
+        ``Tensor``:
+            - Cropped image.
     """
     h, w = image.shape[-2:]
     new_h, new_w = h - 2 * offset, w - 2 * offset
     return crop(image, offset, offset, new_h, new_w)
 
 
 def pad_to(image: Tensor, size: Tuple, fill_value: int = 0) -> Tensor:
-    """Pad array with fill value to fit size with origin image in center of padded image.
+    """Pad Image with fill value to fit size with origin image in center of padded image.
 
     Args:
         image (Tensor): Image to be padded.
         size (Tuple, optional): Size to fit with padding.
         fill_value (int) : value to use for filling new pixels.
     Returns:
         Tensor: Padded image
+
+    Args:
+        image (``Tensor``): Image to be padded.
+        size (``Tuple``):  Size to fit with padding.
+        fill_value (``int``, **optional**): Value to use for filling new pixels. Defaults to 0.
+
+    Returns:
+        ``Tensor``:
+            - Padded Image
     """
     # get sizes
     h, w = image.shape[-2:]
     padded_h, padded_w = size
     # compute difference
     delta_h = padded_h - h
     delta_w = padded_w - w
@@ -58,22 +76,23 @@
     left, right = ceil(delta_w / 2), floor(delta_w / 2)
     # pad image
     padded = pad(image, padding=[left, top, right, bot], fill=fill_value)
     return padded
 
 
 def crop_to(image: Tensor, size: Tuple) -> Tensor:
-    """Crop array in center.
+    """Crop Image in center.
 
     Args:
-        image (Tensor): Image to crop.
-        size (Tuple): Cropped size.
+        image (``Tensor``): Image to crop.
+        size (``Tuple``): Cropped size.
 
     Returns:
-        Tensor: image cropped.
+        ``Tensor``:
+            - Cropped Image.
     """
     # get sizes
     h, w = image.shape[-2:]
     cropped_h, cropped_w = size
     # compute delta of sizes
     delta_h = h - cropped_h
     delta_w = w - cropped_w
@@ -87,19 +106,22 @@
 def patchification(
     image: Tensor, patch_size: Tuple, overlap: float
 ) -> Tuple[Tensor, List[Tuple[int]], Tuple[int]]:
     """Cut image in patches according to patch size and overlapping.
     If needed padding is applied to fit patch size multiplicator on H & W.
 
     Args:
-        image (Tensor): Large image to patchify.
-        patch_size (Tuple): size of patch.
-        overlap (float): Overlap between patches.
+        image (``Tensor``): Large image to patchify.
+        patch_size (``Tuple``): Size of patch.
+        overlap (``float``): Overlap between patches.
+
     Returns:
-        Tuple[Tensor, List[Tuple[int]]]: Tensor of N pacthes & coordinates according to padded image.
+        ``Tuple[Tensor, List[Tuple[int]], Tuple[int]]``:
+            - Tensor of N patches (N, patch_height, patch_width)
+            - Coordinates of patches.
     """
     # get shapes of image and pateches
     c, h, w = image.shape[-3:]
     h_patch, w_patch = patch_size
     # compute strides values
     stride_h = h_patch - round(h_patch * overlap)
     stride_w = w_patch - round(w_patch * overlap)
@@ -121,28 +143,30 @@
     )
     #  Fill the patches tensors
     for idx, (y, x) in enumerate(origins):
         patches[idx] = padded_image[:, y : y + h_patch, x : x + w_patch]
 
     return patches, origins, (h_padded, w_padded)
 
+
 def unpatchification(
-    predictions: List[Format],
+    predictions: List[BaseFormat],
     coordinates: List[Tuple[int]],
     spatial_size: Tuple[int],
-) -> Format:
+) -> BaseFormat:
     """Build a prediction from multiple patch predictions and coordinates.
 
     Args:
-        predictions (List[Format]): Patches predictions.
-        coordinates (List[Tuple[int]]): List of Y, X coordinates.
-        spatial_size (Tuple[int]): Size of merged prediction.
-        nms_threshold (float): Iou Threshold to consider boxes as overlapping for NMS algorithm.
+        predictions (``List[BaseFormat]``): Patches predictions.
+        coordinates (``List[Tuple[int]]``): List of Y, X coordinates.
+        spatial_size (``Tuple[int]``): Size of merged prediction.
+
     Returns:
-        (Format): Target of whole image.
+        ``BaseFormat``:
+            -  BaseFormat of whole image.
     """
     h, w = spatial_size
     # remove 0 size patchs
     non_empty_predictions = [p for p in predictions if p.size > 0]
     if len(non_empty_predictions) == 0:
         return Format.empty(spatial_size=spatial_size)
```

### Comparing `detectools-0.1.5/src/detectools/utils/mask_utils.py` & `detectools-0.1.6/src/detectools/formats/mask_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,69 +4,80 @@
 import numpy as np
 import torch
 from torch import Tensor
 from pycocotools import mask as mask_utils
 from typing import Any, List, Literal
 
 def cocopolygons2mask(polygons: List, size: Tuple[int]) -> Tensor:
-    """convert coco segmentation polygons to binary masks.
+    """Convert coco segmentation polygons to binary masks.
 
     Args:
-        polygons (List): coco polygons list.
-        mask_size (Tuple): size of corresponding image (H, W).
+        polygons (``List``): List of coco polygons.
+        size (``Tuple[int]``): size of corresponding image (H, W).
 
     Returns:
-        Tensor : Binary mask of shape (size).
+        ``Tensor``:
+            - Binary mask of shape (H, W).
     """
     finale_polygon = []
     mask = np.zeros(size, dtype=np.int32)
     # extract full polygon in list[subpolygons]
     for seg in polygons:
         finale_polygon.append(np.array(seg).astype("int64").reshape(int(len(seg) / 2), 2))
     # convert polygon to a final mask
     mask = cv2.fillPoly(mask, finale_polygon, 1)
     return torch.tensor(mask)
 
 def cocoseg2masks(segmentation: Any, mask_size: Tuple[int]) -> Tensor:
-    """From COCO segmentation return masks. 
+    """From COCO segmentation return mask.
 
     Args:
-        segmentation (Any): Segmentation in COCO json (polygons, compressed RLE or uncompressed RLE).
-        mask_size (Tuple[int]): H, W shape of image.
-        mask_mode (Literal["binary", "stacked"]): To return  binary masks or stacked mask. Default to 'stacked' for memory saving.
+        segmentation (``Any``): Segmentation in COCO json (polygons, compressed RLE or uncompressed RLE).
+        mask_size (``Tuple[int]``): H, W shape of image.
 
     Returns:
-        Tensor: N binary masks (for N objects) (N, H, W).
+        ``Tensor``:
+            - Binary mask (H, W).
     """
 
     if isinstance(segmentation, list):
         mask = cocopolygons2mask(segmentation, mask_size)
     elif isinstance(segmentation, dict) and "counts" in segmentation.keys():
         if isinstance(segmentation["counts"], list):
             mask = uncompressed_rle_to_mask(segmentation)
         elif isinstance(segmentation["counts"], str):
             mask = mask_utils.decode()
     
     return mask
 
-def uncompressed_rle_to_mask(uncompressed_rle):
+def uncompressed_rle_to_mask(uncompressed_rle: Any) -> Tensor:
+    """From uncompressed RLE segmentation return mask.
+
+    Args:
+        uncompressed_rle (``Any``): Uncompressed RLE mask encoding.
+
+    Returns:
+        ``Tensor``:
+            - Binary mask (H, W).
+    """
     h, w = uncompressed_rle["size"][:2]
     compressed_rle = mask_utils.frPyObjects(uncompressed_rle, h,w)
     binary_mask = torch.tensor(mask_utils.decode(compressed_rle))
     return binary_mask
 
 
 def mask2polygons(mask: Tensor) -> Tuple[List[List], float]:
     """convert one mask to polygon for coco export
 
     Args:
-        mask (torch.Tensor): binary mask.
+        mask (``Tensor``): Binary mask.
 
     Returns:
-        Tuple[List[List], float]: list of polygons part, area
+        ``Tuple[List[List], float]``:
+            - List of polygons (one by continuous mask), area.
     """
     if mask.ndim == 0:
         segmentation = [[]]
         area = 0
         return segmentation, area
     
     if mask.ndim == 3:
```

### Comparing `detectools-0.1.5/src/detectools/utils/metrics.py` & `detectools-0.1.6/src/detectools/metrics/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,16 @@
 from typing import Any, Callable, Dict, List, Tuple
 
 import torch
 from torch import Tensor
 from torchmetrics import Metric
 from torchmetrics.classification import StatScores
-from torchvision.ops import box_iou
 from detectools import Task
 from detectools.formats import Format
-
-
-def match_boxes(
-    prediction: Format, target: Format, iou_threshold: float = 0.5
-) -> Tuple[Tensor, Tensor, Tensor, Tuple[Tensor, Tensor]]:
-    """Match better prediction boxes candidates with target boxes. Return indexes of
-    prediction and target boxes that match and compute statistics of detection quality (Tp, FP, FN).
-
-    Args:
-        prediction (Format): Prediction.
-        target (Format): Target.
-        iou_threshold (float, optional): IoU threshold to discard some matchs with overlapping < to thr. Defaults to 0.5.
-
-    Returns:
-        Tuple[Tensor, Tensor, Tensor, Tuple[Tensor, Tensor]]: Detection statsitics (TP, FN, FN)
-        & prediction and target boxes indexes that match well.
-    """
-    # set box format to XYXY for torch box iou computation
-    assert prediction.box_format == target.box_format, f"Predictio and taget should have the same box_format, got {prediction.box_format} & {target.box_format}"
-    origin_box_format = prediction.box_format
-    prediction.set_boxes_format("XYXY")
-    target.set_boxes_format("XYXY")
-    # extract boxes
-    pred_boxes = prediction.get("boxes")
-    target_boxes = target.get("boxes")
-    # compute cross matrix of ious
-    cross_ious = box_iou(pred_boxes, target_boxes)
-    # boolean matrix of max pred iou == max target iou --> true positives candidates
-    max_matchs = (
-        torch.max(cross_ious, dim=1)[0][..., None]
-        == torch.max(cross_ious, dim=0)[0][None, ...]
-    ).view(cross_ious.shape)
-
-    # true positive if iou of max_matchs > iou threshold
-    tp = torch.sum((max_matchs > 0) & (cross_ious > iou_threshold))
-    # false positive: all boxes with no match with targets
-    fp = torch.sum(pred_boxes.shape[0] - torch.sum(tp))
-    # false negative if target has no pred box with iou > threshold
-    fn = torch.sum(torch.max(cross_ious, dim=0)[0] < 0.5)
-    # tp pairs index
-    pred_idxs, target_idxs = torch.where(
-        (max_matchs > 0) & (cross_ious > iou_threshold)
-    )
-    # extract indexes
-    pred_idxs = pred_idxs.tolist() if pred_idxs.nelement() > 0 else []
-    target_idxs = target_idxs.tolist() if target_idxs.nelement() > 0 else []
-    match_idxs = (torch.tensor(pred_idxs).long(), torch.tensor(target_idxs).long())
-    # send back box format to original format
-    prediction.set_boxes_format(origin_box_format)
-    target.set_boxes_format(origin_box_format)
-
-    return tp, fp, fn, match_idxs
-
-
-# functionnals metrics
-def f1score(tp, fp, tn, fn):
-    return (2 * tp) / (2 * tp + fp + fn)
-
-
-def precision(tp, fp, tn, fn):
-    if tp + fp == 0:
-        return torch.tensor(torch.nan)
-    return (tp) / (tp + fp)
-
-
-def recall(tp, fp, tn, fn):
-    return (tp) / (tp + fn)
-
-
-def iou(tp: Tensor, fp: Tensor, tn: Tensor, fn: Tensor) -> Tensor:
-    """Compute IoU from statistics."""
-    return tp / (tp + fp + fn)
-
-
-def accuracy(tp: Tensor, fp: Tensor, tn: Tensor, fn: Tensor):
-    """Compute accuracy from statistics."""
-    return (tp + tn) / (tn + tp + fp + fn)
-
+from detectools.metrics.functionnals import match_boxes
 
 class DetectMetric(Metric):
     """Base class for custom detection metric with torchmetrics engine."""
 
     is_differentiable = None
     higher_is_better = True
     full_state_update: bool = False
@@ -293,15 +215,15 @@
     paradigm to provide stats based on classes masks (instead of objects).
     """
 
     def __init__(
         self,
         func: Callable,  # metric functionnal
         num_classes: int = 1,
-        name: str = "ClassifMetric",
+        name: str = "SegmentationMetric",
         **kwargs: Any,
     ):
         assert (
             Task.mode == "instance_segmentation"
         ), "lib mode must be instance_segmentation to use SemanticSegmentationMetric, please set mode by using Task.set_lib_mode() at the begining of script "
         # init from ClassifMetric and
         # redefine stat score num_classes for multiclass detection to include background as a class (+1 class)
@@ -397,8 +319,8 @@
         """Call each metric and merge outptu dicts."""
         metric_dict = {}
         for metric in self.metrics:
             subdict = metric(prediction, target)
             subdict = {f"{metric.name}_{key}": value for key, value in subdict}
             metric_dict.update(subdict)
 
-        return metric_dict
+        return metric_dict
```

### Comparing `detectools-0.1.5/src/detectools/utils/trainer.py` & `detectools-0.1.6/src/detectools/train/loss_aggregator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,63 @@
 from typing import Dict
 
 from torch import Tensor
 
 
 class Aggregator:
-    """Class to aggregate losses across batchs."""
+    """Aggregator aggregate losses across batchs.
+    
+    Attributes:
+    -----------
+    
+    Attributes:
+        iterations (``int``): Number of iterations.
+        losses (``Dict[str, Tensor]``): Dictionnary of epoch losses (over iterations).
+    
+    Methods:
+    ----------
+        """
+
+    iterations: int
+    losses: dict
 
     def __init__(self):
         self.iterations = 0
         self.losses: dict = None
 
     def update(self, batch_losses: Dict[str, Tensor]):
         """Update internal loss dict with new losses.
 
         Args:
-            batch_losses (Dict[str, Tensor]): Dict of losses.
+            batch_losses (``Dict[str, Tensor]``): Dict of losses.
         """
 
         for key, value in self.losses.items():
             self.losses[key] = value + batch_losses[key]
 
     def __call__(self, batch_losses: Dict[str, Tensor], batch_size: int):
-        """Either create or update internal loss dict.
+        """Update internal loss dict.
 
         Args:
-            batch_losses (Dict[str, Tensor]): Dict of losses.
-            batch_size (int): batch size.
+            batch_losses (``Dict[str, Tensor]``): Dict of losses.
+            batch_size (``int``): Batch size.
         """
 
         if self.losses:
             self.update(batch_losses)
         else:
             self.losses = batch_losses
 
         self.iterations += 1 * batch_size
 
     def compute(self) -> Dict[str, Tensor]:
-        """Return loss dict with values divided by iterations (Mean accross samples)."""
+        """Return loss dict with values divided by iterations (Mean accross samples).
+
+        Returns:
+            ``Dict[str, Tensor]``:
+                - Losses over iterations.
+        """
 
         out_dict = {
             key: (value / self.iterations) for key, value in self.losses.items()
         }
         return out_dict
```

### Comparing `detectools-0.1.5/src/detectools/utils/visualisation.py` & `detectools-0.1.6/src/detectools/visualisation.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from detectools.formats import BaseFormat, BaseAnnotation, SegmentationAnnotation, SegmentationFormat
 from torch import Tensor
 from torchvision.transforms.v2 import ConvertBoundingBoxFormat
 from torchvision.utils import draw_bounding_boxes, draw_segmentation_masks
 import random as rd
 
 
-def draw_object(image: Tensor, obj: BaseAnnotation, classes: List[str] = [], colors: List[Tuple[int, int, int]]=COLORS,  color_objects: bool=False) -> Tensor:
-    """Draw bounding boxe & mask to image.
+def draw_object(image: Tensor, obj: BaseAnnotation, classes: List[str] = [], colors: List[Tuple[int, int, int]]=COLORS) -> Tensor:
+    """Draw bounding boxe & mask from Annotation to image.
 
     Args:
-        image (Tensor): Tensor image (uint8 & RGB)
-        obj (Union[Annotation]): Annotation to draw.
-        classes ( List[str]) : Names of classes to draw.  Defaults to [].
-        colors (List[Tuple[int, int, int]]): List of colors for visualisations.
-        color_objects (bool): If True a random color is applied to each object instead of one color/label.
+        image (``Tensor``): Tensor image (uint8 & RGB).
+        obj (``BaseAnnotation``): Annotation to draw.
+        classes (``List[str]``, **optional**): Names of classes to draw, cif no list passed classes names are not displayed. Defaults to [].
+        colors (``List[Tuple[int, int, int]]``, **optional**): List of RGB colors for visualisations. Defaults to COLORS.
 
     Returns:
-        Tensor: Image with object box drawed on.
+        ``Tensor``:
+            - Image with annotation drawed.
     """
     # convert box for torch drawing bb
     format_converter = ConvertBoundingBoxFormat("XYXY")
     # wrap in object data in list
     boxe = format_converter(obj.boxe)
     color = [colors[obj.label]]
     label = obj.label.item()
@@ -45,23 +45,23 @@
     return image
 
 
 def draw_objects(image: Tensor, objects: BaseFormat, classes: List[str] = [], colors: List[Tuple[int, int, int]]=COLORS, color_objects: bool=False):
     """Draw all bounding boxes of an object on image.
 
     Args:
-        image (Tensor): Tensor image (uint8 & RGB)
-        objects (DetectionTarget): DetectionTargets to draw.
-        classes (List[str], optional): Names of classes to draw. Defaults to [].
-        colors (List[Tuple[int, int, int]]): List of colors for visualisations.
-        color_objects (bool): If True a random color is applied to each object instead of one color/label.
-
+        image (``Tensor``): Tensor image (uint8 & RGB).
+        obj (``BaseAnnotation``): Annotation to draw.
+        classes (``List[str]``, **optional**): Names of classes to draw, if no list passed classes names are not displayed. Defaults to [].
+        colors (``List[Tuple[int, int, int]]``, **optional**): List of RGB colors for visualisations. Defaults to COLORS.
+        color_objects (``bool``, **optional**): If True one random color/object, if False one color/class. Defaults to False.
 
     Returns:
-        Tensor: Image with objects boxes drawed on.
+        ``Tensor``:
+            - Image with annotations drawed.
     """
     # convert boxes format
     labels, boxes = objects.get("labels", "boxes")
     format_converter = ConvertBoundingBoxFormat("XYXY")
     boxes = format_converter(boxes)
     # either write class names if passed or labels.
     if classes:
@@ -80,15 +80,15 @@
         colors = [colors[rd.randint(0, len(colors)-1)] for label in labels]
     else:
         colors = [colors[label] for label in labels]
     # draw objects on image
     image = draw_bounding_boxes(image, boxes, upstring, colors, width=6)
 
     if isinstance(objects, SegmentationFormat) and objects.size != 0:
-        image.to("cpu") # limit GPU memory usage by switching to CPU
+        image.to("cpu") # limit GPU memory usage by switching to CPU
         objects.set_device("cpu")
         masks = objects.get("masks").to_binary_masks()
         image = draw_segmentation_masks(image, masks.bool(), colors=colors, alpha=0.5)
 
     return image
 
 
@@ -98,21 +98,23 @@
     classes: List[str] = [],
     colors: List[Tuple[int, int, int]]=COLORS,
     color_objects: bool = False
 ) -> Tensor:
     """Draw boxe(s) on image from DetectionTarget or DetectionObject.
 
     Args:
-        image (Tensor): _description_
-        objects (Union[DetectionTarget, DetectionObject]): _description_
-        classes (List[str], optional): _description_. Defaults to [].
-        colors (List[Tuple[int, int, int]]): List of colors for visualisations.
-        color_objects (bool): If True a random color is applied to each object instead of one color/label.
+        image (``Tensor``): Image (RGB & uint8).
+        target (``Union[BaseFormat, SegmentationFormat]``): Target as BaseFormat or Annotation.
+        classes (``List[str]``, **optional**): Names of classes to draw, if no list passed classes names are not displayed. Defaults to [].
+        colors (``List[Tuple[int, int, int]]``, **optional**): List of RGB colors for visualisations. Defaults to COLORS.
+        color_objects (``bool``, **optional**): If True one random color/object, if False one color/class. Defaults to False.
+        
     Returns:
-        Tensor: Image with objects boxes drawed on.
+        ``Tensor``:
+            - Visaulisation of objects on RGB image.
     """
 
     if isinstance(target, BaseAnnotation):
         image = draw_object(image, target, classes, colors)
 
     if isinstance(target, BaseFormat):
         if target.size > 0:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `detectools-0.1.5/src/detectools.egg-info/SOURCES.txt` & `detectools-0.1.6/src/detectools.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 LICENSE.txt
 README.md
 README_deployment.md
 pyproject.toml
 setup.py
 src/detectools/__init__.py
-src/detectools/augmentation.py
-src/detectools/dataset.py
-src/detectools/inference.py
-src/detectools/metrics.py
-src/detectools/trainer.py
+src/detectools/data_management.py
+src/detectools/visualisation.py
 src/detectools.egg-info/PKG-INFO
 src/detectools.egg-info/SOURCES.txt
 src/detectools.egg-info/dependency_links.txt
 src/detectools.egg-info/requires.txt
 src/detectools.egg-info/top_level.txt
+src/detectools/data/__init__.py
+src/detectools/data/augmentation.py
+src/detectools/data/dataset.py
 src/detectools/formats/__init__.py
 src/detectools/formats/base.py
+src/detectools/formats/detect_mask.py
 src/detectools/formats/detection_format.py
-src/detectools/formats/mask.py
+src/detectools/formats/interfaces.py
+src/detectools/formats/mask_utils.py
 src/detectools/formats/segmentation_format.py
+src/detectools/inference/__init__.py
+src/detectools/inference/engine.py
+src/detectools/inference/predictor.py
+src/detectools/metrics/__init__.py
+src/detectools/metrics/available_metrics.py
+src/detectools/metrics/base.py
+src/detectools/metrics/functionnals.py
 src/detectools/models/__init__.py
 src/detectools/models/base.py
 src/detectools/models/mask2former.py
 src/detectools/models/yolo.py
 src/detectools/models/yolov8_seg.py
+src/detectools/train/__init__.py
+src/detectools/train/loss_aggregator.py
+src/detectools/train/trainer.py
 src/detectools/utils/__init__.py
-src/detectools/utils/data_management.py
-src/detectools/utils/inference.py
-src/detectools/utils/mask_utils.py
-src/detectools/utils/metrics.py
-src/detectools/utils/trainer.py
-src/detectools/utils/visualisation.py
+src/detectools/utils/data.py
+src/detectools/utils/display.py
+src/detectools/utils/load_and_write.py
```

