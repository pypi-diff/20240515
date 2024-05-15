# Comparing `tmp/alphafold3-0.0.4.tar.gz` & `tmp/alphafold3-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphafold3-0.0.4.tar", max compression
+gzip compressed data, was "alphafold3-0.0.6.tar", max compression
```

## Comparing `alphafold3-0.0.4.tar` & `alphafold3-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1074 2024-05-08 16:55:43.323225 alphafold3-0.0.4/LICENSE
--rw-r--r--   0        0        0     3885 2024-05-09 20:34:50.011249 alphafold3-0.0.4/README.md
--rw-r--r--   0        0        0      169 2024-05-09 20:33:55.539381 alphafold3-0.0.4/alphafold3/__init__.py
--rw-r--r--   0        0        0     4196 2024-05-08 17:23:47.690079 alphafold3-0.0.4/alphafold3/constants.py
--rw-r--r--   0        0        0     5314 2024-05-09 19:20:59.867782 alphafold3-0.0.4/alphafold3/diffusion.py
--rw-r--r--   0        0        0     4007 2024-05-09 20:42:14.235905 alphafold3-0.0.4/alphafold3/model.py
--rw-r--r--   0        0        0    16667 2024-05-09 20:42:14.555185 alphafold3-0.0.4/alphafold3/pairformer.py
--rw-r--r--   0        0        0     1364 2024-05-09 20:48:57.627865 alphafold3-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4674 1970-01-01 00:00:00.000000 alphafold3-0.0.4/setup.py
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 alphafold3-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-08 16:55:43.323225 alphafold3-0.0.6/LICENSE
+-rw-r--r--   0        0        0     8736 2024-05-15 01:22:42.640855 alphafold3-0.0.6/README.md
+-rw-r--r--   0        0        0      225 2024-05-10 08:58:21.425325 alphafold3-0.0.6/alphafold3/__init__.py
+-rw-r--r--   0        0        0     4196 2024-05-08 17:23:47.690079 alphafold3-0.0.6/alphafold3/constants.py
+-rw-r--r--   0        0        0     5449 2024-05-10 08:58:21.426043 alphafold3-0.0.6/alphafold3/diffusion.py
+-rw-r--r--   0        0        0     4896 2024-05-15 01:22:42.641740 alphafold3-0.0.6/alphafold3/model.py
+-rw-r--r--   0        0        0    16667 2024-05-09 20:42:14.555185 alphafold3-0.0.6/alphafold3/pairformer.py
+-rw-r--r--   0        0        0     2751 2024-05-15 01:22:42.653241 alphafold3-0.0.6/alphafold3/template_embedder.py
+-rw-r--r--   0        0        0     1349 2024-05-15 01:22:52.978561 alphafold3-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9624 1970-01-01 00:00:00.000000 alphafold3-0.0.6/setup.py
+-rw-r--r--   0        0        0     9679 1970-01-01 00:00:00.000000 alphafold3-0.0.6/PKG-INFO
```

### Comparing `alphafold3-0.0.4/LICENSE` & `alphafold3-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3-0.0.4/alphafold3/constants.py` & `alphafold3-0.0.6/alphafold3/constants.py`

 * *Files identical despite different names*

### Comparing `alphafold3-0.0.4/alphafold3/diffusion.py` & `alphafold3-0.0.6/alphafold3/diffusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,17 +129,22 @@
             x (Tensor): Input tensor.
             ground_truth (Tensor): Ground truth tensor.
 
         Returns:
             Tuple[Tensor, Tensor]: Output tensor and loss tensor.
 
         """
-        for layer in self.layers:
-            x, loss = layer(x, ground_truth)
-        return x, loss
+        if ground_truth is True:
+            for layer in self.layers:
+                x = layer(x, ground_truth)
+            return x
+        else:
+            for layer in self.layers:
+                x = layer(x)
+            return x
 
 
 # # Example usage
 # if __name__ == "__main__":
 #     model = GeneticDiffusionModuleBlock(
 #         channels=3, training=True
 #     )  # Assuming 3D coordinates
```

### Comparing `alphafold3-0.0.4/alphafold3/model.py` & `alphafold3-0.0.6/alphafold3/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import torch
 from torch import Tensor, nn
 
 from alphafold3.diffusion import GeneticDiffusion
 from alphafold3.pairformer import PairFormer
+from einops import rearrange
 
 # structure module
 
 
 class AlphaFold3(nn.Module):
     """
     AlphaFold3 model implementation.
@@ -59,19 +59,22 @@
             global_column_attn=global_column_attn,
             depth=pair_former_depth,
         )
 
         # Diffusion module
         self.diffuser = GeneticDiffusion(
             channels=dim,
-            num_diffusion_steps=1000,
+            num_diffusion_steps=num_diffusion_steps,
             training=False,
             depth=diffusion_depth,
         )
 
+        # Norm
+        self.norm = nn.Layernorm(dim)
+
     def forward(
         self,
         pair_representation: Tensor,
         single_representation: Tensor,
         return_loss: bool = False,
         ground_truth: Tensor = None,
         return_confidence: bool = False,
@@ -97,28 +100,47 @@
         # TODO: Input
         # TODO: Template
         # TODO: MSA
 
         b, n, n_two, dim = pair_representation.shape
         b_two, n_two, dim_two = single_representation.shape
 
-        # Concat
-        x = torch.cat(
-            [pair_representation, single_representation], dim=1
+        # Transforming the tensor into 4d for concatenation
+        single_representation = single_representation.unsqueeze(2)
+        print(single_representation.shape)
+        z, j, y, d = single_representation.shape
+        single_representation = rearrange(
+            single_representation, "b n s d -> b n d s"
+        )
+        single_representation = nn.Linear(y, n)(single_representation)
+        print(single_representation.shape)
+        single_representation = rearrange(
+            single_representation, "b n d s -> b n s d"
         )
+        print(single_representation.shape)
+
+        # # Concat
+        # x = torch.cat(
+        #     [pair_representation, single_representation], dim=1
+        # )
+        pair_representation = self.norm(pair_representation)
+        single_representation = self.norm(single_representation)
 
         # Apply the 48 blocks of PairFormer
-        x = self.pairformer(x)
+        x, m = self.pairformer(
+            pair_representation, single_representation
+        )
         print(x.shape)
+        print(m.shape)
 
         # Add the embeddings to the recycle bins
         # recyle_bins.append(x)
 
         # Diffusion
-        x = self.diffuser(x, ground_truth)
+        x = self.diffuser(x)
 
         # If return_confidence is True, return the confidence
         if return_confidence is True:
             x = self.confidence_projection(x)
             return x
 
         # If return_loss is True, return the loss
```

### Comparing `alphafold3-0.0.4/alphafold3/pairformer.py` & `alphafold3-0.0.6/alphafold3/pairformer.py`

 * *Files identical despite different names*

### Comparing `alphafold3-0.0.4/pyproject.toml` & `alphafold3-0.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "alphafold3"
-version = "0.0.4"
+version = "0.0.6"
 description = "Paper - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/AlphaFold3"
 documentation = "https://github.com/kyegomez/AlphaFold3"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/AlphaFold3"
@@ -22,15 +22,14 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 zetascale = "*"
 torch = "*"
 einops = "*"
-openfold = "*"
 
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.6"
 types-toml = "^0.10.8.1"
 types-redis = "^4.3.21.6"
 types-pytz = "^2023.3.0.0"
```

