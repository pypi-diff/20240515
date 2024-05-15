# Comparing `tmp/langvae-0.2.4.tar.gz` & `tmp/langvae-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langvae-0.2.4.tar", last modified: Tue May 14 20:00:41 2024, max compression
+gzip compressed data, was "langvae-0.2.5.tar", last modified: Wed May 15 07:23:39 2024, max compression
```

## Comparing `langvae-0.2.4.tar` & `langvae-0.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:00:41.334981 langvae-0.2.4/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 langvae-0.2.4/LICENSE
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:00:41.334330 langvae-0.2.4/LangVAE.egg-info/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3642 2024-05-14 20:00:41.000000 langvae-0.2.4/LangVAE.egg-info/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      857 2024-05-14 20:00:41.000000 langvae-0.2.4/LangVAE.egg-info/SOURCES.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-14 20:00:41.000000 langvae-0.2.4/LangVAE.egg-info/dependency_links.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       34 2024-05-14 20:00:41.000000 langvae-0.2.4/LangVAE.egg-info/requires.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        8 2024-05-14 20:00:41.000000 langvae-0.2.4/LangVAE.egg-info/top_level.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3642 2024-05-14 20:00:41.334706 langvae-0.2.4/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2906 2024-05-14 13:36:08.000000 langvae-0.2.4/README.md
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:00:41.327710 langvae-0.2.4/langvae/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       62 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:00:41.331008 langvae-0.2.4/langvae/arch/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-26 18:39:44.000000 langvae-0.2.4/langvae/arch/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2687 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/arch/cvae.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     7486 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/arch/vae.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:00:41.331437 langvae-0.2.4/langvae/data_conversion/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-12 01:44:56.000000 langvae-0.2.4/langvae/data_conversion/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     6052 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/data_conversion/tokenization.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:00:41.332152 langvae-0.2.4/langvae/decoders/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       94 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/decoders/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     5246 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/decoders/sentence.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3614 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/decoders/sentence_annotated.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:00:41.332930 langvae-0.2.4/langvae/encoders/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       94 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/encoders/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2548 2024-02-08 19:30:25.000000 langvae-0.2.4/langvae/encoders/sentence.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3041 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/encoders/sentence_annotated.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:00:41.333447 langvae-0.2.4/langvae/pipelines/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       52 2024-03-18 10:49:43.000000 langvae-0.2.4/langvae/pipelines/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4668 2024-03-18 10:49:43.000000 langvae-0.2.4/langvae/pipelines/lang_training.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-14 20:00:41.334032 langvae-0.2.4/langvae/trainers/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      111 2024-03-18 10:49:43.000000 langvae-0.2.4/langvae/trainers/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4055 2024-05-14 12:28:12.000000 langvae-0.2.4/langvae/trainers/cyclical_schedule_kl.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      693 2024-05-14 13:57:07.000000 langvae-0.2.4/pyproject.toml
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       33 2024-05-14 19:59:00.000000 langvae-0.2.4/requirements.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-14 20:00:41.335050 langvae-0.2.4/setup.cfg
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      889 2024-05-14 13:57:07.000000 langvae-0.2.4/setup.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.888749 langvae-0.2.5/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 langvae-0.2.5/LICENSE
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.888059 langvae-0.2.5/LangVAE.egg-info/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3642 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      857 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/SOURCES.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/dependency_links.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       34 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/requires.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        8 2024-05-15 07:23:39.000000 langvae-0.2.5/LangVAE.egg-info/top_level.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3642 2024-05-15 07:23:39.888419 langvae-0.2.5/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2906 2024-05-14 13:36:08.000000 langvae-0.2.5/README.md
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.880791 langvae-0.2.5/langvae/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       62 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.883539 langvae-0.2.5/langvae/arch/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-26 18:39:44.000000 langvae-0.2.5/langvae/arch/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2687 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/arch/cvae.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     9372 2024-05-15 00:19:05.000000 langvae-0.2.5/langvae/arch/vae.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.884340 langvae-0.2.5/langvae/data_conversion/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-12 01:44:56.000000 langvae-0.2.5/langvae/data_conversion/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     6052 2024-05-15 01:16:04.000000 langvae-0.2.5/langvae/data_conversion/tokenization.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.885438 langvae-0.2.5/langvae/decoders/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       94 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/decoders/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     5246 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/decoders/sentence.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3614 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/decoders/sentence_annotated.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.886378 langvae-0.2.5/langvae/encoders/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       94 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/encoders/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2548 2024-02-08 19:30:25.000000 langvae-0.2.5/langvae/encoders/sentence.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3041 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/encoders/sentence_annotated.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.886991 langvae-0.2.5/langvae/pipelines/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       52 2024-03-18 10:49:43.000000 langvae-0.2.5/langvae/pipelines/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4668 2024-03-18 10:49:43.000000 langvae-0.2.5/langvae/pipelines/lang_training.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:23:39.887704 langvae-0.2.5/langvae/trainers/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      111 2024-03-18 10:49:43.000000 langvae-0.2.5/langvae/trainers/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4055 2024-05-14 12:28:12.000000 langvae-0.2.5/langvae/trainers/cyclical_schedule_kl.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      693 2024-05-15 07:22:19.000000 langvae-0.2.5/pyproject.toml
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       33 2024-05-14 19:59:00.000000 langvae-0.2.5/requirements.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-15 07:23:39.888823 langvae-0.2.5/setup.cfg
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      889 2024-05-15 07:22:19.000000 langvae-0.2.5/setup.py
```

### Comparing `langvae-0.2.4/LICENSE` & `langvae-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/LangVAE.egg-info/PKG-INFO` & `langvae-0.2.5/LangVAE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langvae
-Version: 0.2.4
+Version: 0.2.5
 Summary: LangVAE: Large Language VAEs made simple
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/LangVAE
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/LangVAE/issues
 Keywords: vae,llm,generative,nlp
```

### Comparing `langvae-0.2.4/LangVAE.egg-info/SOURCES.txt` & `langvae-0.2.5/LangVAE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/PKG-INFO` & `langvae-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langvae
-Version: 0.2.4
+Version: 0.2.5
 Summary: LangVAE: Large Language VAEs made simple
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/LangVAE
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/LangVAE/issues
 Keywords: vae,llm,generative,nlp
```

### Comparing `langvae-0.2.4/README.md` & `langvae-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/langvae/arch/cvae.py` & `langvae-0.2.5/langvae/arch/cvae.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/langvae/arch/vae.py` & `langvae-0.2.5/langvae/arch/vae.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+import sys
+import os
+import pickle
 import numpy as np
 import torch
 import torch.nn.functional as F
 from typing import Tuple, List, Optional
+from copy import deepcopy
 
 from pythae.trainers import BaseTrainerConfig
 from pythae.models.nn import BaseEncoder, BaseDecoder
+from pythae.models.base.base_config import BaseAEConfig, EnvironmentConfig
 from torch import Tensor
 from pythae.models.vae import VAE, VAEConfig
 from pythae.trainers.training_callbacks import TrainingCallback
 
 
 @torch.jit.script
 def vae_nll_loss(recon_x: Tensor,
@@ -174,7 +179,46 @@
         """
         self.device = "cpu"
         self.encoder.device = "cpu"
         self.decoder.device = "cpu"
         self.encoder.debug = False
         self.decoder.debug = False
         super().push_to_hf_hub(hf_hub_path)
+
+    def save(self, dir_path: str):
+        """Method to save the model at a specific location. It saves, the model weights as a
+        ``models.pt`` file along with the model config as a ``model_config.json`` file. If the
+        model to save used custom encoder (resp. decoder) provided by the user, these are also
+        saved as ``decoder.pkl`` (resp. ``decoder.pkl``).
+
+        Args:
+            dir_path (str): The path where the model should be saved. If the path
+                path does not exist a folder will be created at the provided location.
+        """
+
+        env_spec = EnvironmentConfig(
+            python_version=f"{sys.version_info[0]}.{sys.version_info[1]}"
+        )
+        model_dict = {"model_state_dict": deepcopy(self.state_dict())}
+
+        if not os.path.exists(dir_path):
+            try:
+                os.makedirs(dir_path)
+
+            except FileNotFoundError as e:
+                raise e
+
+        env_spec.save_json(dir_path, "environment")
+        self.model_config.save_json(dir_path, "model_config")
+
+        # only save .pkl if custom architecture provided
+        if not self.model_config.uses_default_encoder:
+            with open(os.path.join(dir_path, "encoder.pkl"), "wb") as fp:
+                # cloudpickle.register_pickle_by_value(inspect.getmodule(self.encoder))
+                pickle.dump(self.encoder, fp, pickle.DEFAULT_PROTOCOL)
+
+        if not self.model_config.uses_default_decoder:
+            with open(os.path.join(dir_path, "decoder.pkl"), "wb") as fp:
+                # cloudpickle.register_pickle_by_value(inspect.getmodule(self.decoder))
+                pickle.dump(self.decoder, fp, pickle.DEFAULT_PROTOCOL)
+
+        torch.save(model_dict, os.path.join(dir_path, "model.pt"))
```

### Comparing `langvae-0.2.4/langvae/data_conversion/tokenization.py` & `langvae-0.2.5/langvae/data_conversion/tokenization.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/langvae/decoders/sentence.py` & `langvae-0.2.5/langvae/decoders/sentence.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/langvae/decoders/sentence_annotated.py` & `langvae-0.2.5/langvae/decoders/sentence_annotated.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/langvae/encoders/sentence.py` & `langvae-0.2.5/langvae/encoders/sentence.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/langvae/encoders/sentence_annotated.py` & `langvae-0.2.5/langvae/encoders/sentence_annotated.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/langvae/pipelines/lang_training.py` & `langvae-0.2.5/langvae/pipelines/lang_training.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/langvae/trainers/cyclical_schedule_kl.py` & `langvae-0.2.5/langvae/trainers/cyclical_schedule_kl.py`

 * *Files identical despite different names*

### Comparing `langvae-0.2.4/pyproject.toml` & `langvae-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "langvae"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Danilo S. Carvalho", email="danilo.carvalho@manchester.ac.uk" }
 ]
 description = "LangVAE: Large Language VAEs made simple"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `langvae-0.2.4/setup.py` & `langvae-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = [str(x).strip() for x in all_reqs]
 
     return install_requires
 
 
 setup(
     name='LangVAE',
-    version='0.2.4',
+    version='0.2.5',
     packages=[
         'langvae',
         'langvae.arch',
         'langvae.decoders',
         'langvae.encoders',
         'langvae.data_conversion',
         'langvae.pipelines',
```

