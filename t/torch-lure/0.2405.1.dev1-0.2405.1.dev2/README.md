# Comparing `tmp/torch_lure-0.2405.1.dev1.tar.gz` & `tmp/torch_lure-0.2405.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "torch_lure-0.2405.1.dev2.tar", last modified: Wed May 15 15:57:03 2024, max compression
```

## Comparing `torch_lure-0.2405.1.dev1.tar` & `torch_lure-0.2405.1.dev2.tar`

### file list

```diff
@@ -1,13 +1,24 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/.python-version
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/src/torch_lure/__init__.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/src/torch_lure/noise_schedulers.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/src/torch_lure/optim.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/src/torch_lure/utils.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/src/torch_lure/datasets/__init__.py
--rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/src/torch_lure/datasets/minari_ext.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/src/torch_lure/functional/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/src/torch_lure/modules/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/.gitignore
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/README.md
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 torch_lure-0.2405.1.dev1/PKG-INFO
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 15:57:03.553635 torch_lure-0.2405.1.dev2/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torch_lure-0.2405.1.dev2/.gitignore
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torch_lure-0.2405.1.dev2/.python-version
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1254 2024-05-15 15:57:03.553635 torch_lure-0.2405.1.dev2/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      787 2024-05-15 15:14:40.000000 torch_lure-0.2405.1.dev2/README.md
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1021 2024-05-15 15:56:24.000000 torch_lure-0.2405.1.dev2/pyproject.toml
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-15 15:57:03.553635 torch_lure-0.2405.1.dev2/setup.cfg
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      940 2024-05-15 15:25:50.000000 torch_lure-0.2405.1.dev2/setup.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 15:57:03.543635 torch_lure-0.2405.1.dev2/src/
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 15:57:03.543635 torch_lure-0.2405.1.dev2/src/torch_lure/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      179 2024-05-15 15:20:27.000000 torch_lure-0.2405.1.dev2/src/torch_lure/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 15:57:03.543635 torch_lure-0.2405.1.dev2/src/torch_lure/functional/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torch_lure-0.2405.1.dev2/src/torch_lure/functional/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 15:57:03.543635 torch_lure-0.2405.1.dev2/src/torch_lure/modules/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torch_lure-0.2405.1.dev2/src/torch_lure/modules/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torch_lure-0.2405.1.dev2/src/torch_lure/noise_schedulers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torch_lure-0.2405.1.dev2/src/torch_lure/optim.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torch_lure-0.2405.1.dev2/src/torch_lure/utils.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 15:57:03.553635 torch_lure-0.2405.1.dev2/torch_lure.egg-info/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1254 2024-05-15 15:57:03.000000 torch_lure-0.2405.1.dev2/torch_lure.egg-info/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      412 2024-05-15 15:57:03.000000 torch_lure-0.2405.1.dev2/torch_lure.egg-info/SOURCES.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-15 15:57:03.000000 torch_lure-0.2405.1.dev2/torch_lure.egg-info/dependency_links.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       73 2024-05-15 15:57:03.000000 torch_lure-0.2405.1.dev2/torch_lure.egg-info/requires.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-15 15:57:03.000000 torch_lure-0.2405.1.dev2/torch_lure.egg-info/top_level.txt
```

### Comparing `torch_lure-0.2405.1.dev1/src/torch_lure/noise_schedulers.py` & `torch_lure-0.2405.1.dev2/src/torch_lure/noise_schedulers.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.2405.1.dev1/src/torch_lure/utils.py` & `torch_lure-0.2405.1.dev2/src/torch_lure/utils.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.2405.1.dev1/src/torch_lure/functional/__init__.py` & `torch_lure-0.2405.1.dev2/src/torch_lure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.2405.1.dev1/src/torch_lure/modules/__init__.py` & `torch_lure-0.2405.1.dev2/src/torch_lure/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.2405.1.dev1/README.md` & `torch_lure-0.2405.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `torch_lure-0.2405.1.dev1/pyproject.toml` & `torch_lure-0.2405.1.dev2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+
+[build-system]
+requires = ["setuptools>=61.0.0", "setuptools_scm", "wheel"]
+build-backend = "setuptools.build_meta"
+
+
 [project]
 name = "torch-lure"
-version = "0.2405.1-dev.1"
+dynamic = ["version"]
 description = ""
 authors = [
     { name = "fuyutarow", email = "fuyutarow@gmail.com" }
 ]
 dependencies = [
     "torch>=2.1",
     "numpy>=1.26.4",
@@ -13,26 +19,28 @@
     "gymnasium>=0.29.1",
     "jax>=0.4.28",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 keywords = ["pytorch"]
 
+
 [project.urls]
 Homepage = "https://github.com/fuyutarow/torch-lure"
 Repository = "https://github.com/fuyutarow/torch-lure"
 
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
 [tool.rye]
 managed = true
-dev-dependencies = []
-
-[tool.hatch.metadata]
-allow-direct-references = true
+dev-dependencies = [
+    "setuptools>=69.5.1",
+    "setuptools_scm>=8.1.0",
+    "wheel>=0.43.0",
+]
 
-[tool.hatch.build.targets.wheel]
-packages = ["src/torch_lure"]
 
+[tool.setuptools_scm]
+write_to = "src/torch_lure/_version.py"
+version_scheme = "post-release"
+local_scheme = "dirty-tag"
 
+[tool.setuptools.packages.find]
+include = ["src/torch_lure", "src/torch_lure.*"]
```

### Comparing `torch_lure-0.2405.1.dev1/PKG-INFO` & `torch_lure-0.2405.1.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: torch-lure
-Version: 0.2405.1.dev1
+Version: 0.2405.1.dev2
+Author-email: fuyutarow <fuyutarow@gmail.com>
 Project-URL: Homepage, https://github.com/fuyutarow/torch-lure
 Project-URL: Repository, https://github.com/fuyutarow/torch-lure
-Author-email: fuyutarow <fuyutarow@gmail.com>
 Keywords: pytorch
 Requires-Python: >=3.8
-Requires-Dist: gymnasium>=0.29.1
-Requires-Dist: jax>=0.4.28
+Description-Content-Type: text/markdown
+Requires-Dist: torch>=2.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: sophia-opt>=0.2.2
-Requires-Dist: torch>=2.1
-Description-Content-Type: text/markdown
+Requires-Dist: gymnasium>=0.29.1
+Requires-Dist: jax>=0.4.28
 
 # Torch Lure
 
 
 <a href="https://www.youtube.com/watch?v=wCzCOYCfY9g" target="_blank">
   <img src="http://img.youtube.com/vi/wCzCOYCfY9g/maxresdefault.jpg" alt="Chandelure" style="width: 100%;">
 </a>
@@ -47,8 +47,8 @@
 lure.QuantileLoss(quantile=0.5)
 
 lure.RMSNrom(dim=256, eps=1e-6)
 
 # Noise Scheduler
 lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
 lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000):
-```
+```
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.3 Name: torch-lure Version: 0.2405.1.dev1 Project-URL:
-Homepage, https://github.com/fuyutarow/torch-lure Project-URL: Repository,
-https://github.com/fuyutarow/torch-lure Author-email: fuyutarow
-gmail.com> Keywords: pytorch Requires-Python: >=3.8 Requires-Dist:
-gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28 Requires-Dist: numpy>=1.26.4
-Requires-Dist: sophia-opt>=0.2.2 Requires-Dist: torch>=2.1 Description-Content-
-Type: text/markdown # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install
-git+https://github.com/Farama-Foundation/
-Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip install
-torch-lure ``` # Usage ```py import torch_lure as lure # Optimizers
+Metadata-Version: 2.1 Name: torch-lure Version: 0.2405.1.dev2 Author-email:
+fuyutarow
+gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torch-lure
+Project-URL: Repository, https://github.com/fuyutarow/torch-lure Keywords:
+pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
+opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28 # Torch
+Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install git+https://github.com/Farama-
+Foundation/Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip
+install torch-lure ``` # Usage ```py import torch_lure as lure # Optimizers
 lure.SophiaG(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x)
 lure.TanhExp() lure.quantile_loss(y_pred, y_target, quantile=0.5)
 lure.QuantileLoss(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise
 Scheduler lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02,
 num_timesteps=1000) lure.CosineNoiseScheduler(max_beta=0.999, s=0.008,
 num_timesteps=1000): ```
```

