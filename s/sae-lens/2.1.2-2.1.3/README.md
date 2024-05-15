# Comparing `tmp/sae_lens-2.1.2.tar.gz` & `tmp/sae_lens-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-2.1.2.tar", max compression
+gzip compressed data, was "sae_lens-2.1.3.tar", max compression
```

## Comparing `sae_lens-2.1.2.tar` & `sae_lens-2.1.3.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1069 2024-05-13 19:17:01.966214 sae_lens-2.1.2/LICENSE
--rw-r--r--   0        0        0     3381 2024-05-13 19:17:01.966214 sae_lens-2.1.2/README.md
--rw-r--r--   0        0        0     2041 2024-05-13 19:17:03.306225 sae_lens-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      939 2024-05-13 19:17:03.306225 sae_lens-2.1.2/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    17062 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20134 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     1164 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0        0 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     6844 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0        0 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    20594 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     6065 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0    15343 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/config.py
--rw-r--r--   0        0        0     6711 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     4377 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1280 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     5040 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8403 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2424 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    20000 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     1932 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    18456 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    30701 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0      423 2024-05-13 19:17:01.978214 sae_lens-2.1.2/sae_lens/training/utils.py
--rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-15 20:51:54.662037 sae_lens-2.1.3/LICENSE
+-rw-r--r--   0        0        0     3381 2024-05-15 20:51:54.662037 sae_lens-2.1.3/README.md
+-rw-r--r--   0        0        0     2041 2024-05-15 20:51:56.206061 sae_lens-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1098 2024-05-15 20:51:56.206061 sae_lens-2.1.3/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    17062 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20134 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     1164 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0        0 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     2674 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     6844 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0        0 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    20340 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     4052 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/batching.py
+-rw-r--r--   0        0        0     6065 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0    16237 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/config.py
+-rw-r--r--   0        0        0     8229 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     4377 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1280 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     5574 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     5401 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/pretokenize_runner.py
+-rw-r--r--   0        0        0     8403 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2424 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    20000 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     1932 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    18456 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    31427 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0      423 2024-05-15 20:51:54.674038 sae_lens-2.1.3/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-2.1.3/PKG-INFO
```

### Comparing `sae_lens-2.1.2/LICENSE` & `sae_lens-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/README.md` & `sae_lens-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/pyproject.toml` & `sae_lens-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "2.1.2"
+version = "2.1.3"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `sae_lens-2.1.2/sae_lens/__init__.py` & `sae_lens-2.1.3/sae_lens/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-__version__ = "2.1.2"
+__version__ = "2.1.3"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import CacheActivationsRunner
-from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
+from .training.config import (
+    CacheActivationsRunnerConfig,
+    LanguageModelSAERunnerConfig,
+    PretokenizeRunnerConfig,
+)
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
+from .training.pretokenize_runner import pretokenize_runner
 from .training.sae_group import SparseAutoencoderDictionary
 from .training.session_loader import LMSparseAutoencoderSessionloader
 from .training.sparse_autoencoder import SparseAutoencoder
 from .training.train_sae_on_language_model import train_sae_group_on_language_model
 
 __all__ = [
     "LanguageModelSAERunnerConfig",
     "CacheActivationsRunnerConfig",
     "LMSparseAutoencoderSessionloader",
+    "PretokenizeRunnerConfig",
     "SparseAutoencoder",
     "SparseAutoencoderDictionary",
     "run_evals",
     "language_model_sae_runner",
+    "pretokenize_runner",
     "CacheActivationsRunner",
     "ActivationsStore",
     "train_sae_group_on_language_model",
 ]
```

### Comparing `sae_lens-2.1.2/sae_lens/analysis/dashboard_runner.py` & `sae_lens-2.1.3/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/analysis/feature_statistics.py` & `sae_lens-2.1.3/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-2.1.3/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-2.1.3/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/analysis/tsea.py` & `sae_lens-2.1.3/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/pretrained_saes.yaml` & `sae_lens-2.1.3/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-2.1.3/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-2.1.3/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-2.1.3/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/activations_store.py` & `sae_lens-2.1.3/sae_lens/training/activations_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,16 @@
         self.device = device
         self.dtype = dtype
         self.cached_activations_path = cached_activations_path
 
         self.n_dataset_processed = 0
         self.iterable_dataset = iter(self.dataset)
 
+        self.estimated_norm_scaling_factor = 1.0
+
         # Check if dataset is tokenized
         dataset_sample = next(self.iterable_dataset)
 
         # check if it's tokenized
         if "tokens" in dataset_sample.keys():
             self.is_dataset_tokenized = True
             self.tokens_column = "tokens"
@@ -171,14 +173,17 @@
             assert (
                 n_activations_on_disk >= self.total_training_tokens
             ), f"Only {n_activations_on_disk/1e6:.1f}M activations on disk, but total_training_tokens is {self.total_training_tokens/1e6:.1f}M."
 
     def apply_norm_scaling_factor(self, activations: torch.Tensor) -> torch.Tensor:
         return activations * self.estimated_norm_scaling_factor
 
+    def unscale(self, activations: torch.Tensor) -> torch.Tensor:
+        return activations / self.estimated_norm_scaling_factor
+
     def get_norm_scaling_factor(self, activations: torch.Tensor) -> torch.Tensor:
         return (self.d_in**0.5) / activations.norm(dim=-1).mean()
 
     @property
     def storage_buffer(self) -> torch.Tensor:
         if self._storage_buffer is None:
             self._storage_buffer = self.get_buffer(self.n_batches_in_buffer // 2)
@@ -382,26 +387,16 @@
             # pbar.update(1)
 
         new_buffer = new_buffer.reshape(-1, num_layers, d_in)
         new_buffer = new_buffer[torch.randperm(new_buffer.shape[0])]
 
         # every buffer should be normalized:
         if self.normalize_activations:
-            try:
-                # check if we've already estimated the norm scaling factor
-                assert self.estimated_norm_scaling_factor is not None
-            except AttributeError:
-                # if we haven't estimated it yet, do so.
-                assert (
-                    new_buffer.shape[0] > 3e5
-                ), "Warning: Storage buffer is too small to calculate norm scaling factor and expect it to be reliable."
-                self.estimated_norm_scaling_factor = self.get_norm_scaling_factor(
-                    new_buffer
-                )
-
+            if self.estimated_norm_scaling_factor == 1:
+                print("WARNING: no normalisation is being applied, scaling factor = 1")
             new_buffer = self.apply_norm_scaling_factor(new_buffer)
 
         return new_buffer
 
     def save_buffer(self, buffer: torch.Tensor, path: str):
         """
         Used by cached activations runner to save a buffer to disk.
```

### Comparing `sae_lens-2.1.2/sae_lens/training/cache_activations_runner.py` & `sae_lens-2.1.3/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/config.py` & `sae_lens-2.1.3/sae_lens/training/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from dataclasses import dataclass, field
-from typing import Any, Optional, cast
+from typing import Any, Literal, Optional, cast
 
 import torch
 import wandb
 
 from sae_lens import __version__
 
 DTYPE_MAP = {
@@ -405,7 +405,36 @@
     hook_point: str,
     hook_point_head_index: int | None,
 ) -> str:
     path = f"activations/{dataset_path.replace('/', '_')}/{model_name.replace('/', '_')}/{hook_point}"
     if hook_point_head_index is not None:
         path += f"_{hook_point_head_index}"
     return path
+
+
+@dataclass
+class PretokenizeRunnerConfig:
+    tokenizer_name: str = "gpt2"
+    dataset_path: str = "NeelNanda/c4-10k"
+    split: str | None = "train"
+    data_files: list[str] | None = None
+    data_dir: str | None = None
+    num_proc: int = 4
+    context_size: int = 128
+    column_name: str = "text"
+    shuffle: bool = True
+    seed: int | None = None
+    streaming: bool = False
+
+    # special tokens
+    begin_batch_token: int | Literal["bos", "eos", "sep"] | None = "bos"
+    begin_sequence_token: int | Literal["bos", "eos", "sep"] | None = None
+    sequence_separator_token: int | Literal["bos", "eos", "sep"] | None = "eos"
+
+    # if saving locally, set save_path
+    save_path: str | None = None
+
+    # if saving to huggingface, set hf_repo_id
+    hf_repo_id: str | None = None
+    hf_num_shards: int = 64
+    hf_revision: str = "main"
+    hf_is_private_repo: bool = False
```

### Comparing `sae_lens-2.1.2/sae_lens/training/geometric_median.py` & `sae_lens-2.1.3/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/lm_runner.py` & `sae_lens-2.1.3/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/load_model.py` & `sae_lens-2.1.3/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/optim.py` & `sae_lens-2.1.3/sae_lens/training/optim.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Took the LR scheduler from my previous work: https://github.com/jbloomAus/DecisionTransformerInterpretability/blob/ee55df35cdb92e81d689c72fb9dd5a7252893363/src/decision_transformer/utils.py#L425
 """
 
+from typing import Any
+
 import torch.optim as optim
 import torch.optim.lr_scheduler as lr_scheduler
 
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
 #  Constant
@@ -136,7 +138,21 @@
             self.sparse_autoencoder.l1_coefficient = self.final_l1_value * (
                 (1 + step) / self.l1_warmup_steps
             )  # type: ignore
         else:
             self.sparse_autoencoder.l1_coefficient = self.final_l1_value  # type: ignore
 
         self.current_step += 1
+
+    def state_dict(self):
+        """State dict for serializing as part of an SAETrainContext."""
+        return {
+            "l1_warmup_steps": self.l1_warmup_steps,
+            "total_steps": self.total_steps,
+            "final_l1_value": self.final_l1_value,
+            "current_step": self.current_step,
+        }
+
+    def load_state_dict(self, state_dict: dict[str, Any]):
+        """Loads all state apart from attached SAE."""
+        for k in state_dict:
+            setattr(self, k, state_dict[k])
```

### Comparing `sae_lens-2.1.2/sae_lens/training/sae_group.py` & `sae_lens-2.1.3/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/session_loader.py` & `sae_lens-2.1.3/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/sparse_autoencoder.py` & `sae_lens-2.1.3/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/toy_model_runner.py` & `sae_lens-2.1.3/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/toy_models.py` & `sae_lens-2.1.3/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-2.1.3/sae_lens/training/train_sae_on_language_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,14 +274,28 @@
         raise InterruptedException()
 
     try:
         # signal handlers (if preempted)
         signal.signal(signal.SIGINT, interrupt_callback)
         signal.signal(signal.SIGTERM, interrupt_callback)
 
+        # Estimate norm scaling factor if necessary
+        # TODO(tomMcGrath): this is a bodge and should be moved back inside a class
+        if activation_store.normalize_activations:
+            print("Estimating activation norm")
+            n_batches_for_norm_estimate = int(1e3)
+            norms_per_batch = []
+            for _ in tqdm(range(n_batches_for_norm_estimate)):
+                acts = activation_store.next_batch()
+                norms_per_batch.append(acts.norm(dim=-1).mean().item())
+            mean_norm = np.mean(norms_per_batch)
+            scaling_factor = np.sqrt(activation_store.d_in) / mean_norm
+            activation_store.estimated_norm_scaling_factor = scaling_factor
+
+        # Train loop
         while training_run_state.n_training_tokens < total_training_tokens:
             # Do a training step.
             layer_acts = activation_store.next_batch()
             training_run_state.n_training_tokens += batch_size
 
             mse_losses: list[torch.Tensor] = []
             l1_losses: list[torch.Tensor] = []
```

### Comparing `sae_lens-2.1.2/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-2.1.3/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.2/PKG-INFO` & `sae_lens-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 2.1.2
+Version: 2.1.3
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

