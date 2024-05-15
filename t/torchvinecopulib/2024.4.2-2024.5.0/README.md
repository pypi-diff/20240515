# Comparing `tmp/torchvinecopulib-2024.4.2.tar.gz` & `tmp/torchvinecopulib-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchvinecopulib-2024.4.2.tar", max compression
+gzip compressed data, was "torchvinecopulib-2024.5.0.tar", max compression
```

## Comparing `torchvinecopulib-2024.4.2.tar` & `torchvinecopulib-2024.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35593 2024-04-27 07:17:40.868884 torchvinecopulib-2024.4.2/LICENSE
--rw-r--r--   0        0        0     1670 2024-04-30 03:11:55.068293 torchvinecopulib-2024.4.2/pyproject.toml
--rw-r--r--   0        0        0     5672 2024-04-30 07:21:24.864497 torchvinecopulib-2024.4.2/README.md
--rw-r--r--   0        0        0       97 2024-04-30 03:35:06.539336 torchvinecopulib-2024.4.2/torchvinecopulib/__init__.py
--rw-r--r--   0        0        0      529 2024-04-30 03:28:39.037386 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/__init__.py
--rw-r--r--   0        0        0     9267 2024-04-27 07:17:41.246247 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_abc.py
--rw-r--r--   0        0        0     1357 2024-04-27 07:17:41.252249 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_archimedean.py
--rw-r--r--   0        0        0     1949 2024-04-27 07:17:41.256246 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_clayton.py
--rw-r--r--   0        0        0     8300 2024-04-27 07:17:41.260276 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_data_bcp.py
--rw-r--r--   0        0        0      414 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_elliptical.py
--rw-r--r--   0        0        0     4869 2024-04-30 03:54:31.509330 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_factory_bcp.py
--rw-r--r--   0        0        0     2881 2024-04-30 02:54:11.474705 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_frank.py
--rw-r--r--   0        0        0     1676 2024-04-27 07:17:41.276252 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_gaussian.py
--rw-r--r--   0        0        0     2438 2024-04-30 02:54:59.026533 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_gumbel.py
--rw-r--r--   0        0        0     1353 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_independent.py
--rw-r--r--   0        0        0     3133 2024-04-30 02:55:12.338411 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_joe.py
--rw-r--r--   0        0        0     3170 2024-04-27 07:17:41.289787 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_studentt.py
--rw-r--r--   0        0        0    28939 2024-04-30 04:02:06.809730 torchvinecopulib-2024.4.2/torchvinecopulib/util/__init__.py
--rw-r--r--   0        0        0      207 2024-04-30 07:05:31.177262 torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/__init__.py
--rw-r--r--   0        0        0    33968 2024-04-30 07:38:57.742190 torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/_data_vcp.py
--rw-r--r--   0        0        0    26154 2024-04-30 07:39:09.083590 torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/_factory_vcp.py
--rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 torchvinecopulib-2024.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35593 2024-04-27 07:17:40.868884 torchvinecopulib-2024.5.0/LICENSE
+-rw-r--r--   0        0        0     1670 2024-05-04 08:08:23.668568 torchvinecopulib-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5905 2024-05-04 08:08:23.668568 torchvinecopulib-2024.5.0/README.md
+-rw-r--r--   0        0        0       97 2024-04-30 03:35:06.539336 torchvinecopulib-2024.5.0/torchvinecopulib/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-30 03:28:39.037386 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/__init__.py
+-rw-r--r--   0        0        0     9267 2024-04-27 07:17:41.246247 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_abc.py
+-rw-r--r--   0        0        0     1357 2024-04-27 07:17:41.252249 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_archimedean.py
+-rw-r--r--   0        0        0     1949 2024-04-27 07:17:41.256246 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_clayton.py
+-rw-r--r--   0        0        0     8300 2024-04-27 07:17:41.260276 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_data_bcp.py
+-rw-r--r--   0        0        0      414 2024-03-24 13:54:38.000000 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_elliptical.py
+-rw-r--r--   0        0        0     4870 2024-05-13 03:29:54.000000 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_factory_bcp.py
+-rw-r--r--   0        0        0     2881 2024-04-30 02:54:11.474705 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_frank.py
+-rw-r--r--   0        0        0     1676 2024-04-27 07:17:41.276252 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_gaussian.py
+-rw-r--r--   0        0        0     2438 2024-04-30 02:54:59.026533 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_gumbel.py
+-rw-r--r--   0        0        0     1353 2024-03-24 13:54:38.000000 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_independent.py
+-rw-r--r--   0        0        0     3133 2024-04-30 02:55:12.338411 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_joe.py
+-rw-r--r--   0        0        0     3170 2024-05-06 08:36:25.110870 torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_studentt.py
+-rw-r--r--   0        0        0    29074 2024-05-04 10:14:22.282715 torchvinecopulib-2024.5.0/torchvinecopulib/util/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-30 07:05:31.177262 torchvinecopulib-2024.5.0/torchvinecopulib/vinecop/__init__.py
+-rw-r--r--   0        0        0    34005 2024-05-08 08:30:03.178162 torchvinecopulib-2024.5.0/torchvinecopulib/vinecop/_data_vcp.py
+-rw-r--r--   0        0        0    26154 2024-04-30 07:39:09.083590 torchvinecopulib-2024.5.0/torchvinecopulib/vinecop/_factory_vcp.py
+-rw-r--r--   0        0        0     7045 1970-01-01 00:00:00.000000 torchvinecopulib-2024.5.0/PKG-INFO
```

### Comparing `torchvinecopulib-2024.4.2/LICENSE` & `torchvinecopulib-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/pyproject.toml` & `torchvinecopulib-2024.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 package-mode = true
 license = "GNU GPLv3"
 name = "torchvinecopulib"
-version = "2024.4.2"
+version = "2024.5.0"
 description = "yet another vine copula library for PyTorch."
 authors = ["Tuoyuan Cheng <cty120120@gmail.com>"]
 maintainers = ["Xiaosheng You <e1204754@u.nus.edu>"]
 readme = "README.md"
 # homepage = ""
 repository = "https://github.com/TY-Cheng/torchvinecopulib"
 documentation = "https://ty-cheng.github.io/torchvinecopulib/"
```

### Comparing `torchvinecopulib-2024.4.2/README.md` & `torchvinecopulib-2024.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # TorchVineCopuLib
 
-[![Python package](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml)
-![Static Badge](https://img.shields.io/badge/Python-%203.10%7C3.11%7C3.12-blue)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e8a7a7448b2043d9bbefafc5a3ec14f7)](https://app.codacy.com/gh/TY-Cheng/torchvinecopulib/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e8a7a7448b2043d9bbefafc5a3ec14f7)](https://app.codacy.com?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![Python package](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml)
 [![Deploy Docs](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml)
+
+![Static Badge](https://img.shields.io/badge/Python-%203.10%7C3.11%7C3.12-blue)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![PyPI - Version](https://img.shields.io/pypi/v/torchvinecopulib?style=flat)
 [![DOI](https://zenodo.org/badge/768037665.svg)](https://zenodo.org/doi/10.5281/zenodo.10836953)
 
 
 Yet another vine copula package, using [PyTorch](https://pytorch.org/get-started/locally/).
 
@@ -52,17 +54,17 @@
 ```
 
 By `pip` from `./dist/*.whl` or `./dist/*.tar.gz` in this repo.
 Need to use proper file name.
 
 ```bash
 # inside project root folder
-pip install ./dist/torchvinecopulib-2024.4.2-py3-none-any.whl
+pip install ./dist/torchvinecopulib-2024.5.0-py3-none-any.whl
 # or
-pip install ./dist/torchvinecopulib-2024.4.2.tar.gz
+pip install ./dist/torchvinecopulib-2024.5.0.tar.gz
 ```
 
 ## Examples
 
 Visit the `./examples/` folder for `.ipynb` Jupyter notebooks.
 
 ## Documentation
```

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/__init__.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_abc.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_abc.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_archimedean.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_archimedean.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_clayton.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_clayton.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_data_bcp.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_data_bcp.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_factory_bcp.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_factory_bcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ) -> DataBiCop:
     """factory method to make a bivariate copula dataclass object, fitted from observations
 
     :param obs_bcp: bivariate copula obs, of shape (num_obs, 2) with values in [0, 1]
     :type obs_bcp: torch.Tensor
     :param tau: Kendall's tau of the observations, defaults to None for the function to estimate
     :type tau: float, optional
-    :param thresh_trunc: threshold of Kendall's tau independence test, below which we reject independent bicop, defaults to 0.1
+    :param thresh_trunc: threshold of Kendall's tau independence test, below which we reject independent bicop, defaults to 0.05
     :type thresh_trunc: float, optional
     :param mtd_fit: parameter estimation method, either 'itau' (inverse of tau) or
         'mle' (maximum likelihood estimation); defaults to "itau"
     :type mtd_fit: str, optional
     :param mtd_mle: optimization method for mle as used by scipy.optimize.minimize, defaults to "COBYLA"
     :type mtd_mle: str, optional
     :param mtd_sel: model selection criterion, either 'aic' or 'bic'; defaults to "aic"
```

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_frank.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_frank.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_gaussian.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_gaussian.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_gumbel.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_gumbel.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_independent.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_independent.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_joe.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_joe.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_studentt.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/bicop/_studentt.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/util/__init__.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 from enum import Enum
 from functools import partial
+from itertools import product
 
 import torch
-from scipy.stats import t, kendalltau
+from scipy.stats import kendalltau, t
 
 __all__ = [
     "ENUM_FUNC_BIDEP",
     "kendall_tau",
     "mutual_info",
     "ferreira_tail_dep_coeff",
     "chatterjee_xi",
@@ -152,57 +153,58 @@
         torch.as_tensor([xy_sum(m) for m in range(1, M + 1)]).sum(dim=0).max().item()
     ) / (M * (1.0 + n) * (1.0 + M + 4.0 * n))
 
 
 def wasserstein_dist_ind(
     x: torch.Tensor,
     y: torch.Tensor,
-    reg: float = 0.1,
     p: int = 2,
+    reg: float = 0.1,
+    num_step: int = 50,
     seed: int = 0,
-    num_sim: int = 2,
 ) -> float:
-    """Wasserstein distance from bicop obs to indep bicop simulations, by ot.sinkhorn2 (averaged for each observation).
+    """Wasserstein distance from bicop obs to indep bicop, by ot.sinkhorn2 (averaged for each observation).
 
     :param x: copula obs of shape (n,1)
     :type x: torch.Tensor
     :param y: copula obs of shape (n,1)
     :type y: torch.Tensor
+    :param p: p-norm to calculate distance between each vector pair, defaults to 2
+    :type p: int, optional
     :param reg: regularization strength, defaults to 0.1
     :type reg: float, optional
-    :param p: p-norm distance to calculate between each vector pair, defaults to 2
-    :type p: int, optional
-    :param seed: random seed for torch.manual_seed() in indep bicop simulations, defaults to 0
+    :param num_step: number of steps in the independent bivariate copula grid, defaults to 50
+    :type num_step: int, optional
+    :param seed: random seed for torch.manual_seed(), defaults to 0
     :type seed: int, optional
-    :return: Wasserstein distance from bicop obs to indep bicop simulations
+    :return: Wasserstein distance from bicop obs to indep bicop
     :rtype: float
     """
     from ot import sinkhorn2
 
     torch.manual_seed(seed=seed)
-    X_s = torch.hstack([x, y])
-    num_obs = x.shape[0]
-    a, b = (
-        torch.ones(size=(num_obs, 1), device=x.device, dtype=x.dtype) / num_obs,
-        torch.ones(size=(num_obs, 1), device=x.device, dtype=x.dtype) / num_obs,
-    )
-    return (
-        sum(
-            (
-                sinkhorn2(
-                    a=a,
-                    b=b,
-                    M=torch.cdist(X_s, torch.rand_like(X_s), p=p),
-                    reg=reg,
-                ).item()
-                for _ in range(num_sim)
-            )
-        )
-        / num_sim
-    )
+    return sinkhorn2(
+        a=torch.ones_like(x) / x.shape[0],
+        b=torch.ones(size=(num_step**2, 1), device=x.device, dtype=x.dtype) / num_step**2,
+        M=torch.cdist(
+            x1=torch.hstack([x, y]),
+            x2=torch.as_tensor(
+                (
+                    *product(
+                        torch.linspace(0, 1, num_step),
+                        torch.linspace(0, 1, num_step),
+                    ),
+                ),
+                device=x.device,
+                dtype=x.dtype,
+            ),
+            p=p,
+        ),
+        reg=reg,
+    ).item()
 
 
 class ENUM_FUNC_BIDEP(Enum):
     """an enum class for bivariate dependence measures"""
 
     chatterjee_xi = partial(chatterjee_xi)
     ferreira_tail_dep_coeff = partial(ferreira_tail_dep_coeff)
```

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/_data_vcp.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/vinecop/_data_vcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,14 +331,15 @@
         else:
             return fig, ax, G
 
     def draw_dag(
         self,
         tpl_first_vs: tuple = tuple(),
         tpl_sim: tuple = tuple(),
+        title: str = "Vine Copula, Obs and BiCop",
         font_size_vertex: int = 8,
         f_path: Path = None,
         fig_size: tuple = None,
     ) -> tuple:
         """draw the directed acyclic graph (DAG) of the vine copula, with pseudo observations and bicops as nodes.
         The source nodes in simulation workflow are highlighted in yellow.
 
@@ -359,15 +360,15 @@
         :rtype: tuple
         """
         import matplotlib.pyplot as plt
         import networkx as nx
 
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=fig_size)
         ax.set_title(
-            label="Vine Copula, Obs and BiCop",
+            label=title,
             fontsize=font_size_vertex + 1,
         )
         G = nx.DiGraph()
         pos_obs = {}
         pos_bcp = {}
         dct_label = {}
         for lv in self.dct_tree:
@@ -466,14 +467,15 @@
             ax=ax,
             edge_color="gray",
             width=0.5,
             style="--",
             alpha=0.8,
         )
         fig.tight_layout()
+        plt.box(False)
         plt.draw_if_interactive()
         if f_path:
             fig.savefig(fname=f_path, bbox_inches="tight")
             return fig, ax, G, f_path
         else:
             return fig, ax, G
 
@@ -587,25 +589,25 @@
 
         return res
 
     def rosenblatt_transform(
         self,
         obs_mvcp: torch.Tensor,
         tpl_sim: tuple = tuple(),
-    ) -> torch.Tensor:
+    ) -> dict:
         """Rosenblatt transformation, from the multivariate copula (with dependence)
         to the uniform multivariate copula (independent), using constructed vine copula
 
         :param obs_mvcp: observation of the multivariate copula, of shape (num_obs, num_dim)
         :type obs_mvcp: torch.Tensor
         :param tpl_sim: tuple of vertices (read from right to left) in a full simulation workflow,
             gives flexibility to experienced users, defaults to tuple()
         :type tpl_sim: tuple, optional
         :return: ideally independent uniform multivariate copula, of shape (num_obs, num_dim)
-        :rtype: torch.Tensor
+        :rtype: dict
         """
         num_dim = self.num_dim
         if not tpl_sim:
             tpl_sim = self.tpl_sim
         tpl_sim_v_s_cond = tuple(
             (v, frozenset(tpl_sim[idx + 1 :])) for idx, v in enumerate(tpl_sim)
         )
```

### Comparing `torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/_factory_vcp.py` & `torchvinecopulib-2024.5.0/torchvinecopulib/vinecop/_factory_vcp.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.2/PKG-INFO` & `torchvinecopulib-2024.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchvinecopulib
-Version: 2024.4.2
+Version: 2024.5.0
 Summary: yet another vine copula library for PyTorch.
 Home-page: https://github.com/TY-Cheng/torchvinecopulib
 License: GNU GPLv3
 Keywords: vine copula,copula,torch
 Author: Tuoyuan Cheng
 Author-email: cty120120@gmail.com
 Maintainer: Xiaosheng You
@@ -26,18 +26,20 @@
 Project-URL: Bug Tracker, https://github.com/TY-Cheng/torchvinecopulib/issues/new
 Project-URL: Documentation, https://ty-cheng.github.io/torchvinecopulib/
 Project-URL: Repository, https://github.com/TY-Cheng/torchvinecopulib
 Description-Content-Type: text/markdown
 
 # TorchVineCopuLib
 
-[![Python package](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml)
-![Static Badge](https://img.shields.io/badge/Python-%203.10%7C3.11%7C3.12-blue)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e8a7a7448b2043d9bbefafc5a3ec14f7)](https://app.codacy.com/gh/TY-Cheng/torchvinecopulib/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e8a7a7448b2043d9bbefafc5a3ec14f7)](https://app.codacy.com?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![Python package](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml)
 [![Deploy Docs](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml)
+
+![Static Badge](https://img.shields.io/badge/Python-%203.10%7C3.11%7C3.12-blue)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![PyPI - Version](https://img.shields.io/pypi/v/torchvinecopulib?style=flat)
 [![DOI](https://zenodo.org/badge/768037665.svg)](https://zenodo.org/doi/10.5281/zenodo.10836953)
 
 
 Yet another vine copula package, using [PyTorch](https://pytorch.org/get-started/locally/).
 
@@ -82,17 +84,17 @@
 ```
 
 By `pip` from `./dist/*.whl` or `./dist/*.tar.gz` in this repo.
 Need to use proper file name.
 
 ```bash
 # inside project root folder
-pip install ./dist/torchvinecopulib-2024.4.2-py3-none-any.whl
+pip install ./dist/torchvinecopulib-2024.5.0-py3-none-any.whl
 # or
-pip install ./dist/torchvinecopulib-2024.4.2.tar.gz
+pip install ./dist/torchvinecopulib-2024.5.0.tar.gz
 ```
 
 ## Examples
 
 Visit the `./examples/` folder for `.ipynb` Jupyter notebooks.
 
 ## Documentation
```

