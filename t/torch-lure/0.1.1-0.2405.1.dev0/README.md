# Comparing `tmp/torch_lure-0.1.1.tar.gz` & `tmp/torch_lure-0.2405.1.dev0.tar.gz`

## Comparing `torch_lure-0.1.1.tar` & `torch_lure-0.2405.1.dev0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 torch_lure-0.1.1/.python-version
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/__init__.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/noise_schedulers.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/optim.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/utils.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/functional/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/modules/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 torch_lure-0.1.1/.gitignore
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 torch_lure-0.1.1/README.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 torch_lure-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 torch_lure-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/.python-version
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/src/torch_lure/__init__.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/src/torch_lure/noise_schedulers.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/src/torch_lure/optim.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/src/torch_lure/utils.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/src/torch_lure/datasets/__init__.py
+-rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/src/torch_lure/datasets/minari_ext.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/src/torch_lure/functional/__init__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/src/torch_lure/modules/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/.gitignore
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/README.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev0/PKG-INFO
```

### Comparing `torch_lure-0.1.1/src/torch_lure/noise_schedulers.py` & `torch_lure-0.2405.1.dev0/src/torch_lure/noise_schedulers.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.1.1/src/torch_lure/utils.py` & `torch_lure-0.2405.1.dev0/src/torch_lure/utils.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.1.1/src/torch_lure/functional/__init__.py` & `torch_lure-0.2405.1.dev0/src/torch_lure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.1.1/src/torch_lure/modules/__init__.py` & `torch_lure-0.2405.1.dev0/src/torch_lure/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.1.1/README.md` & `torch_lure-0.2405.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `torch_lure-0.1.1/PKG-INFO` & `torch_lure-0.2405.1.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.3
 Name: torch-lure
-Version: 0.1.1
+Version: 0.2405.1.dev0
 Project-URL: Homepage, https://github.com/fuyutarow/torch-lure
 Project-URL: Repository, https://github.com/fuyutarow/torch-lure
 Author-email: fuyutarow <fuyutarow@gmail.com>
 Keywords: pytorch
 Requires-Python: >=3.8
+Requires-Dist: gymnasium>=0.29.1
+Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: sophia-opt>=0.2.2
 Requires-Dist: torch>=2.1
 Description-Content-Type: text/markdown
 
 # Torch Lure
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.3 Name: torch-lure Version: 0.1.1 Project-URL: Homepage,
-https://github.com/fuyutarow/torch-lure Project-URL: Repository, https://
-github.com/fuyutarow/torch-lure Author-email: fuyutarow
+Metadata-Version: 2.3 Name: torch-lure Version: 0.2405.1.dev0 Project-URL:
+Homepage, https://github.com/fuyutarow/torch-lure Project-URL: Repository,
+https://github.com/fuyutarow/torch-lure Author-email: fuyutarow
 gmail.com> Keywords: pytorch Requires-Python: >=3.8 Requires-Dist:
-numpy>=1.26.4 Requires-Dist: sophia-opt>=0.2.2 Requires-Dist: torch>=2.1
-Description-Content-Type: text/markdown # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]```sh pip
-install torch-lure ``` # Usage ```py import torch_lure as lure # Optimizers
-lure.SophiaG(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x)
-lure.TanhExp() lure.quantile_loss(y_pred, y_target, quantile=0.5)
-lure.QuantileLoss(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise
-Scheduler lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02,
-num_timesteps=1000) lure.CosineNoiseScheduler(max_beta=0.999, s=0.008,
-num_timesteps=1000): ```
+gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28 Requires-Dist: numpy>=1.26.4
+Requires-Dist: sophia-opt>=0.2.2 Requires-Dist: torch>=2.1 Description-Content-
+Type: text/markdown # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]```sh pip install torch-lure ``` #
+Usage ```py import torch_lure as lure # Optimizers lure.SophiaG(lr=1e-3,
+weight_decay=0.2) # Functions lure.tanh_exp(x) lure.TanhExp()
+lure.quantile_loss(y_pred, y_target, quantile=0.5) lure.QuantileLoss
+(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise Scheduler
+lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
+lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000): ```
```

