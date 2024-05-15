# Comparing `tmp/keras_vision-0.4.4.tar.gz` & `tmp/keras_vision-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_vision-0.4.4.tar", last modified: Tue May  7 20:45:48 2024, max compression
+gzip compressed data, was "keras_vision-0.4.5.tar", last modified: Wed May 15 15:36:53 2024, max compression
```

## Comparing `keras_vision-0.4.4.tar` & `keras_vision-0.4.5.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 20:45:48.011488 keras_vision-0.4.4/
--rw-rw-rw-   0        0        0     1455 2024-05-07 20:45:48.009487 keras_vision-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-05-03 19:13:27.000000 keras_vision-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 20:45:47.982475 keras_vision-0.4.4/keras_vision/
-drwxrwxrwx   0        0        0        0 2024-05-07 20:45:48.006472 keras_vision-0.4.4/keras_vision/MobileViT_v1/
--rw-rw-rw-   0        0        0      501 2024-05-03 18:35:52.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/__init__.py
--rw-rw-rw-   0        0        0     4662 2024-05-07 20:24:40.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/base_layers.py
--rw-rw-rw-   0        0        0     2428 2024-05-03 18:38:07.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/configs.py
--rw-rw-rw-   0        0        0     6418 2024-05-07 20:28:52.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/extras.py
--rw-rw-rw-   0        0        0     8177 2024-05-07 11:37:39.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/mobile_vit_v1.py
--rw-rw-rw-   0        0        0    10286 2024-05-07 20:32:59.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
--rw-rw-rw-   0        0        0     2529 2024-05-03 18:37:13.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
--rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/utils.py
--rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras_vision-0.4.4/keras_vision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 20:45:48.008478 keras_vision-0.4.4/keras_vision.egg-info/
--rw-rw-rw-   0        0        0     1455 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       58 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1322 2024-05-07 20:45:09.000000 keras_vision-0.4.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 20:45:48.012472 keras_vision-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1832 2024-05-07 20:35:22.000000 keras_vision-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:36:53.904659 keras_vision-0.4.5/
+-rw-rw-rw-   0        0        0     2018 2024-05-15 15:36:53.903658 keras_vision-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      979 2024-05-11 16:07:47.000000 keras_vision-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 15:36:53.884117 keras_vision-0.4.5/keras_vision/
+drwxrwxrwx   0        0        0        0 2024-05-15 15:36:53.901656 keras_vision-0.4.5/keras_vision/MobileViT_v1/
+-rw-rw-rw-   0        0        0      501 2024-05-15 15:26:13.000000 keras_vision-0.4.5/keras_vision/MobileViT_v1/__init__.py
+-rw-rw-rw-   0        0        0     4662 2024-05-14 19:55:24.000000 keras_vision-0.4.5/keras_vision/MobileViT_v1/base_layers.py
+-rw-rw-rw-   0        0        0     2428 2024-05-03 18:38:07.000000 keras_vision-0.4.5/keras_vision/MobileViT_v1/configs.py
+-rw-rw-rw-   0        0        0     8673 2024-05-15 15:26:00.000000 keras_vision-0.4.5/keras_vision/MobileViT_v1/mobile_vit_v1.py
+-rw-rw-rw-   0        0        0    10867 2024-05-15 15:21:45.000000 keras_vision-0.4.5/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
+-rw-rw-rw-   0        0        0     2545 2024-05-14 19:55:08.000000 keras_vision-0.4.5/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
+-rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras_vision-0.4.5/keras_vision/MobileViT_v1/utils.py
+-rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras_vision-0.4.5/keras_vision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:36:53.902651 keras_vision-0.4.5/keras_vision.egg-info/
+-rw-rw-rw-   0        0        0     2018 2024-05-15 15:36:53.000000 keras_vision-0.4.5/keras_vision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2024-05-15 15:36:53.000000 keras_vision-0.4.5/keras_vision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 15:36:53.000000 keras_vision-0.4.5/keras_vision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-15 15:36:53.000000 keras_vision-0.4.5/keras_vision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       58 2024-05-15 15:36:53.000000 keras_vision-0.4.5/keras_vision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1331 2024-05-15 15:24:11.000000 keras_vision-0.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 15:36:53.904659 keras_vision-0.4.5/setup.cfg
```

### Comparing `keras_vision-0.4.4/PKG-INFO` & `keras_vision-0.4.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.4.4
+Version: 0.4.5
 Summary: Building Vision models in Keras3 for framework-agnostic training and inference.
-Home-page: https://github.com/veb-101/keras-vision
-Author: Vaibhav Singh
 Author-email: Vaibhav Singh <vaibhav.singh.3001@gmail.com>
 Project-URL: Homepage, https://github.com/veb-101/keras-vision
 Keywords: keras3,tensorflow,Jax,PyTorch,Vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,17 +15,28 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: keras>=3.3.3
+Requires-Dist: numpy
 
-Porting all models from everywhere to Keras for leveraging multi-backend support.
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/keras-vision)](https://www.python.org/)  [![PyPI version](https://badge.fury.io/py/keras-vision.svg)](https://badge.fury.io/py/keras-vision) [![Keras](https://img.shields.io/badge/Keras%203.x-%23D00000.svg?logo=Keras&logoColor=white)](https://github.com/keras-team/keras/releases)
+
+Porting all models from everywhere to Keras to leverage multi-backend support.
 
 Cause why not?🤷🏻‍♂️
 
+**Installation:**
+
+1. Option 1: Install from PyPI: `pip install -U keras-vision`
+
+2. Option 2: Install the latest updates present in the repository: `pip install git+https://github.com/veb-101/keras-vision.git`
+
+**Usage:** Please refer to the `examples` folder
+
 ### Updates
 
 1. [2024-05-04] Converted MobileViT to Keras 3 and released weights of all 3 variants.
    1. Jax backend currently not working, I'm working on a fix.
    2. Release: <https://github.com/veb-101/keras-vision/releases/tag/v0.4>
```

### Comparing `keras_vision-0.4.4/keras_vision/MobileViT_v1/base_layers.py` & `keras_vision-0.4.5/keras_vision/MobileViT_v1/base_layers.py`

 * *Files identical despite different names*

### Comparing `keras_vision-0.4.4/keras_vision/MobileViT_v1/configs.py` & `keras_vision-0.4.5/keras_vision/MobileViT_v1/configs.py`

 * *Files identical despite different names*

### Comparing `keras_vision-0.4.4/keras_vision/MobileViT_v1/mobile_vit_v1.py` & `keras_vision-0.4.5/keras_vision/MobileViT_v1/mobile_vit_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,46 @@
+import os
 import warnings
 from typing import Optional
 
-
+import numpy as np
 import keras.ops as kops
 from keras import Model, Input
 from keras.layers import GlobalAveragePooling2D, Dropout, Dense
 from keras.utils import get_file
 
 from .configs import get_mobile_vit_v1_configs
 from .base_layers import ConvLayer, InvertedResidualBlock
+
 from .mobile_vit_v1_block import MobileViT_v1_Block
 
 VERSION = 0.4
 WEIGHTS_URL = "https://github.com/veb-101/keras-vision/releases/download/v{version}/keras_MobileVIT_v1_model_{model_type}.weights.h5"
 
 
 def MobileViT_v1(
     configs,
-    dropout: float = 0.1,
-    linear_drop: float = 0.0,
+    linear_drop: float = 0.1,
     attention_drop: float = 0.0,
+    dropout: float = 0.0,
     num_classes: int | None = 1000,
     input_shape: tuple[int, int, int] = (256, 256, 3),
     model_name: str = f"MobileViT_v1-S",
 ):
     """
     Arguments
     --------
 
         configs: A dataclass instance with model information such as per layer output channels, transformer embedding dimensions, transformer repeats, IR expansion factor
-
-        num_classes: (int)   Number of output classes
-
+        num_classes: (int) Number of output classes
         input_shape: (tuple) Input shape -> H, W, C
-
-        model_type: (str)   Model to create
-
-        linear_drop: (float) Dropout rate for Dense layers
-
+        model_type: (str) Model to create
+        linear_drop: (float) Dropout rate used for MHSA output and Transformer Dense block
         attention_drop: (float) Dropout rate for the attention matrix
-
+        dropout: (float) Additional Dropout rate used in Transformer Dense block.
     """
 
     input_layer = Input(shape=input_shape)
 
     # Block 1
     out = ConvLayer(
         num_filters=configs.block_1_1_dims,
@@ -179,17 +176,19 @@
         include_top: (bool) Whether to include the classification layers
         pretrained: (bool) Whether to load pretrained weights
         cache_dir: (str) Local directory to cache the downloaded weights
         updates: (dict) a key-value pair indicating the changes to be made to the base model.
 
     Additional arguments:
     ---------------------
-        linear_drop: (float) Dropout rate for Dense layers
+        linear_drop: (float) Dropout rate used for MHSA output and Transformer Dense block
         attention_drop: (float) Dropout rate for the attention matrix
+        dropout: (float) Additional Dropout rate used in Transformer Dense block.
     """
+
     model_type = model_type.upper()
     if model_type not in ("S", "XS", "XXS"):
         raise ValueError("Bad Input. 'model_type' should be one of ['S', 'XS', 'XXS']")
 
     updated_configs = get_mobile_vit_v1_configs(model_type, updates=updates)
 
     # Build the base model
@@ -197,16 +196,23 @@
         configs=updated_configs,
         num_classes=num_classes if include_top else None,
         input_shape=input_shape,
         model_name=f"MobileViT_v1-{model_type}",
         **kwargs,
     )
 
-    if pretrained:
+    # Initialize parameters of MobileViT block.
+    if None in input_shape:
+        dummy_input_shape = (1, 256, 256, 3)
+    else:
+        dummy_input_shape = (1,) + input_shape
+
+    model(np.random.randn(*dummy_input_shape), training=False)
 
+    if pretrained:
         weights_path = get_file(
             fname=f"keras_MobileVIT_v1_model_{model_type}.weights.h5",
             origin=WEIGHTS_URL.format(version=VERSION, model_type=model_type),
             cache_subdir="models",
             hash_algorithm="auto",
             extract=False,
             archive_format="auto",
```

### Comparing `keras_vision-0.4.4/keras_vision/MobileViT_v1/mobile_vit_v1_block.py` & `keras_vision-0.4.5/keras_vision/MobileViT_v1/mobile_vit_v1_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from typing import Union
-
 import keras
 import keras.ops as kops
 from keras.layers import Layer, Dropout, Dense, LayerNormalization, Concatenate
 
 from .base_layers import ConvLayer
 from .multihead_self_attention_2D import MultiHeadSelfAttention as MHSA
+from math import ceil
 
 
 class Transformer(Layer):
     def __init__(
         self,
         num_heads: int = 4,
         embedding_dim: int = 90,
         qkv_bias: bool = True,
         mlp_ratio: float = 2.0,
-        dropout: float = 0.1,
-        linear_drop: float = 0.0,
+        dropout: float = 0.0,
+        linear_drop: float = 0.1,
         attention_drop: float = 0.0,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.num_heads = num_heads
         self.embedding_dim = embedding_dim
         self.qkv_bias = qkv_bias
@@ -32,29 +31,29 @@
         self.norm_1 = LayerNormalization(epsilon=1e-5)
 
         self.attn = MHSA(
             num_heads=self.num_heads,
             embedding_dim=self.embedding_dim,
             qkv_bias=self.qkv_bias,
             attention_drop=self.attention_drop,
-            linear_drop=dropout,
+            linear_drop=self.linear_drop,
         )
         self.norm_2 = LayerNormalization(epsilon=1e-5)
 
         hidden_features = int(self.embedding_dim * self.mlp_ratio)
 
         self.mlp_block_0 = Dense(hidden_features, activation="swish")
-        self.mlp_block_1 = Dropout(self.linear_drop)
-        self.mlp_block_2 = Dense(embedding_dim)
-        self.mlp_block_3 = Dropout(dropout)
+        self.mlp_block_1 = Dropout(self.dropout)
+        self.mlp_block_2 = Dense(self.embedding_dim)
+        self.mlp_block_3 = Dropout(self.linear_drop)
 
     def build(self, input_shape):
         super().build(input_shape)
 
-    def call(self, x):
+    def call(self, x, training=False):
         x = x + self.attn(self.norm_1(x))
 
         mlp_block_out = self.mlp_block_0(self.norm_2(x))
         mlp_block_out = self.mlp_block_1(mlp_block_out)
         mlp_block_out = self.mlp_block_2(mlp_block_out)
         mlp_block_out = self.mlp_block_3(mlp_block_out)
 
@@ -79,35 +78,35 @@
 
 
 class MobileViT_v1_Block(Layer):
     def __init__(
         self,
         out_filters: int = 64,
         embedding_dim: int = 90,
-        patch_size: Union[int, tuple] = 2,
+        patch_size: int = 2,
         transformer_repeats: int = 2,
         num_heads: int = 4,
-        dropout: float = 0.1,
+        linear_drop: float = 0.1,
         attention_drop: float = 0.0,
-        linear_drop: float = 0.0,
+        dropout: float = 0.0,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.out_filters = out_filters
         self.embedding_dim = embedding_dim
         self.patch_size = patch_size
         self.transformer_repeats = transformer_repeats
         self.num_heads = num_heads
         self.dropout = dropout
         self.attention_drop = attention_drop
         self.linear_drop = linear_drop
 
         self.patch_size_h, self.patch_size_w = patch_size if isinstance(self.patch_size, tuple) else (self.patch_size, self.patch_size)
-        self.patch_size_h, self.patch_size_w = kops.cast(self.patch_size_h, dtype="int32"), kops.cast(self.patch_size_w, dtype="int32")
+        self.patch_area = self.patch_size_h * self.patch_size_w
 
         # # local_feature_extractor 1 and 2
         self.local_rep_layer_1 = ConvLayer(num_filters=self.out_filters, kernel_size=3, strides=1, use_bn=True, use_activation=True)
         self.local_rep_layer_2 = ConvLayer(num_filters=self.embedding_dim, kernel_size=1, strides=1, use_bn=False, use_activation=False, use_bias=False)
 
         self.transformer_layers = [
             Transformer(
@@ -126,23 +125,26 @@
         self.local_features_3 = ConvLayer(num_filters=self.out_filters, kernel_size=1, strides=1, use_bn=True, use_activation=True)
         self.concat = Concatenate(axis=-1)
         self.fuse_local_global = ConvLayer(num_filters=self.out_filters, kernel_size=3, strides=1, use_bn=True, use_activation=True)
 
     def build(self, input_shape):
         super().build(input_shape)
 
-    def call(self, x):
+    def compute_output_shape(self, input_shape):
+        shape = input_shape
+        return (shape[0], shape[1], shape[2], self.out_filters)
+
+    def call(self, x, training=False):
         # Local Representation
         local_representation = self.local_rep_layer_1(x)
         local_representation = self.local_rep_layer_2(local_representation)
 
         # Transformer as Convolution Steps
         # --------------------------------
         # # Unfolding
-
         unfolded, info_dict = self.unfolding(local_representation)
 
         # # Infomation sharing/mixing --> global representation
         for layer in self.transformer_layers:
             unfolded = layer(unfolded)
 
         global_representation = self.transformer_layer_norm(unfolded)
@@ -173,47 +175,58 @@
             [9, 10, 11, 12],            [5, 7, 13, 15],
             [13, 14, 15, 16],           [6, 8, 14, 16]
         ]                            ]
         """
 
         # Initially convert channel-last to channel-first for processing
         shape = kops.shape(x)
-        batch_size, orig_h, orig_w, D = shape[0], shape[1], shape[2], shape[3]
+        batch_size = shape[0]
+        orig_h, orig_w, D = x.shape[1], x.shape[2], x.shape[3]
 
-        patch_area = self.patch_size_w * self.patch_size_h
+        h_ceil = ceil(orig_h / self.patch_size_h)
+        w_ceil = ceil(orig_w / self.patch_size_w)
 
-        orig_h, orig_w = kops.cast(orig_h, dtype="int32"), kops.cast(orig_w, dtype="int32")
-        num_patches_h = orig_h // self.patch_size_h
-        num_patches_w = orig_w // self.patch_size_w
-        num_patches = kops.cast(num_patches_h * num_patches_w, dtype="int32")
+        new_h = h_ceil * self.patch_size_h
+        new_w = w_ceil * self.patch_size_w
 
-        # Handle dynamic shape multiplication
-        dynamic_shape_mul = kops.prod([batch_size, num_patches_h])
+        # Condition to decide if resizing is necessary
+        resize_required = (new_h != orig_h) or (new_w != orig_w)
+
+        if resize_required:
+            x = kops.image.resize(x, (new_h, new_w))
+            num_patches_h = new_h // self.patch_size_h
+            num_patches_w = new_w // self.patch_size_w
+            num_patches = num_patches_h * num_patches_w
+        else:
+            num_patches_h = orig_h // self.patch_size_h
+            num_patches_w = orig_w // self.patch_size_w
+            num_patches = num_patches_h * num_patches_w
 
         # [B, H, W, D] --> [B*nh, ph, nw, pw*D]
-        reshaped_fm = kops.reshape(x, (dynamic_shape_mul, self.patch_size_h, num_patches_w, self.patch_size_w * D))
+        reshaped_fm = kops.reshape(x, (batch_size * num_patches_h, self.patch_size_h, num_patches_w, self.patch_size_w * D))
 
         # [B * n_h, p_h, n_w, p_w*D] --> [B * n_h, n_w, p_h, p_w * D]
         transposed_fm = kops.transpose(reshaped_fm, axes=[0, 2, 1, 3])
 
         # [B * n_h, n_w, p_h, p_w * D] --> [B, N, P, D] where P = p_h * p_w and N = n_h * n_w
-        reshaped_fm = kops.reshape(transposed_fm, (batch_size, num_patches, patch_area, D))
+        reshaped_fm = kops.reshape(transposed_fm, (batch_size, num_patches, self.patch_area, D))
 
         # [B, N, P, D] --> [B, P, N, D]
         transposed_fm = kops.transpose(reshaped_fm, axes=[0, 2, 1, 3])
 
         # [B, P, N, D] -> [BP, N, D]
-        patches = kops.reshape(transposed_fm, [batch_size * patch_area, num_patches, D])
+        patches = kops.reshape(transposed_fm, [batch_size * self.patch_area, num_patches, D])
 
         info_dict = {
             "batch_size": batch_size,
-            "total_patches": num_patches,
+            "orig_size": (orig_h, orig_w),
+            "resize": resize_required,
             "num_patches_h": num_patches_h,
             "num_patches_w": num_patches_w,
-            "patch_area": patch_area,
+            "total_patches": num_patches,
         }
 
         return patches, info_dict
 
     def folding(self, x, info_dict):
         """
         ### Notations (wrt paper) ###
@@ -226,31 +239,34 @@
         # Get shape parameters for further processing
         shape = kops.shape(x)
         D = shape[2]
         batch_size = info_dict["batch_size"]
         num_patches = info_dict["total_patches"]
         num_patch_h = info_dict["num_patches_h"]
         num_patch_w = info_dict["num_patches_w"]
-        patch_area = info_dict["patch_area"]
+        resize_required = info_dict["resize"]
 
         # Reshape to [BP, N, D] -> [B, P, N, D]
-        x = kops.reshape(x, [batch_size, patch_area, num_patches, D])
+        x = kops.reshape(x, [batch_size, self.patch_area, num_patches, D])
 
         # [B, P, N D] --> [B, N, P, D]
         x = kops.transpose(x, (0, 2, 1, 3))
 
         # [B, N, P, D] --> [B *n_h, n_w, p_h, p_w * D]
         x = kops.reshape(x, (batch_size * num_patch_h, num_patch_w, self.patch_size_h, self.patch_size_w * D))
 
         # [B *n_h, n_w, p_h, p_w * D] --> [B * n_h, p_h, n_w, p_w * D]
         x = kops.transpose(x, (0, 2, 1, 3))
 
         # [B * n_h, p_h, n_w, p_w * D] --> [B, n_h * p_h, n_w, p_w, D] --> [B, H, W, C]
         x = kops.reshape(x, (batch_size, num_patch_h * self.patch_size_h, num_patch_w * self.patch_size_w, D))
 
+        if resize_required:
+            x = kops.image.resize(x, info_dict["orig_size"])
+
         return x
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "out_filters": self.out_filters,
```

### Comparing `keras_vision-0.4.4/keras_vision/MobileViT_v1/multihead_self_attention_2D.py` & `keras_vision-0.4.5/keras_vision/MobileViT_v1/multihead_self_attention_2D.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     def split_heads(self, x, batch_size):
         # Split the last dimension into (num_heads, projection_dim)
         x = kops.reshape(x, (batch_size, -1, self.num_heads, self.projection_dim))
         # Transpose to shape (batch_size, num_heads, seq_len, projection_dim)
         return kops.transpose(x, axes=(0, 2, 1, 3))
 
-    def call(self, x):
+    def call(self, x, training=False):
         batch_size = kops.shape(x)[0]
 
         # Project and reshape to (batch_size, seq_len, 3, num_heads, projection_dim)
         qkv = self.qkv(x)
         qkv = kops.reshape(qkv, (batch_size, -1, 3, self.num_heads, self.projection_dim))
         qkv = kops.transpose(qkv, axes=(0, 2, 1, 3, 4))
         q, k, v = qkv[:, 0], qkv[:, 1], qkv[:, 2]
```

### Comparing `keras_vision-0.4.4/keras_vision/MobileViT_v1/utils.py` & `keras_vision-0.4.5/keras_vision/MobileViT_v1/utils.py`

 * *Files identical despite different names*

### Comparing `keras_vision-0.4.4/keras_vision.egg-info/PKG-INFO` & `keras_vision-0.4.5/keras_vision.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.4.4
+Version: 0.4.5
 Summary: Building Vision models in Keras3 for framework-agnostic training and inference.
-Home-page: https://github.com/veb-101/keras-vision
-Author: Vaibhav Singh
 Author-email: Vaibhav Singh <vaibhav.singh.3001@gmail.com>
 Project-URL: Homepage, https://github.com/veb-101/keras-vision
 Keywords: keras3,tensorflow,Jax,PyTorch,Vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,17 +15,28 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: keras>=3.3.3
+Requires-Dist: numpy
 
-Porting all models from everywhere to Keras for leveraging multi-backend support.
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/keras-vision)](https://www.python.org/)  [![PyPI version](https://badge.fury.io/py/keras-vision.svg)](https://badge.fury.io/py/keras-vision) [![Keras](https://img.shields.io/badge/Keras%203.x-%23D00000.svg?logo=Keras&logoColor=white)](https://github.com/keras-team/keras/releases)
+
+Porting all models from everywhere to Keras to leverage multi-backend support.
 
 Cause why not?🤷🏻‍♂️
 
+**Installation:**
+
+1. Option 1: Install from PyPI: `pip install -U keras-vision`
+
+2. Option 2: Install the latest updates present in the repository: `pip install git+https://github.com/veb-101/keras-vision.git`
+
+**Usage:** Please refer to the `examples` folder
+
 ### Updates
 
 1. [2024-05-04] Converted MobileViT to Keras 3 and released weights of all 3 variants.
    1. Jax backend currently not working, I'm working on a fix.
    2. Release: <https://github.com/veb-101/keras-vision/releases/tag/v0.4>
```

### Comparing `keras_vision-0.4.4/keras_vision.egg-info/SOURCES.txt` & `keras_vision-0.4.5/keras_vision.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 README.md
 pyproject.toml
-setup.py
 keras_vision/__init__.py
 keras_vision.egg-info/PKG-INFO
 keras_vision.egg-info/SOURCES.txt
 keras_vision.egg-info/dependency_links.txt
 keras_vision.egg-info/requires.txt
 keras_vision.egg-info/top_level.txt
 keras_vision/MobileViT_v1/__init__.py
 keras_vision/MobileViT_v1/base_layers.py
 keras_vision/MobileViT_v1/configs.py
-keras_vision/MobileViT_v1/extras.py
 keras_vision/MobileViT_v1/mobile_vit_v1.py
 keras_vision/MobileViT_v1/mobile_vit_v1_block.py
 keras_vision/MobileViT_v1/multihead_self_attention_2D.py
 keras_vision/MobileViT_v1/utils.py
```

### Comparing `keras_vision-0.4.4/pyproject.toml` & `keras_vision-0.4.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "keras-vision"
-version = "0.4.4"
+version = "0.4.5"
 description = "Building Vision models in Keras3 for framework-agnostic training and inference."
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.10"
 
 authors = [{ name = "Vaibhav Singh", email = "vaibhav.singh.3001@gmail.com" }]
 
 urls = { "Homepage" = "https://github.com/veb-101/keras-vision" }
@@ -26,12 +26,12 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 keywords = ["keras3", "tensorflow", "Jax", "PyTorch", "Vision"]
 
-dependencies = ["keras>=3.3.3"]
+dependencies = ["keras>=3.3.3", "numpy"]
 
 [tool.setuptools.packages.find]
 # In your `setup.py`, you had `find_packages()`. This line achieves the same.
 where = ["."]
```

