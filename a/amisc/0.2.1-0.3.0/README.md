# Comparing `tmp/amisc-0.2.1.tar.gz` & `tmp/amisc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amisc-0.2.1.tar", last modified: Tue Jan 30 16:53:28 2024, max compression
+gzip compressed data, was "amisc-0.3.0.tar", last modified: Tue May 14 23:06:28 2024, max compression
```

## Comparing `amisc-0.2.1.tar` & `amisc-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2024-01-30 16:53:14.395595 amisc-0.2.1/LICENSE
--rw-r--r--   0        0        0     2904 2024-01-30 16:53:14.395595 amisc-0.2.1/docs/README.md
--rw-r--r--   0        0        0     1904 2024-01-30 16:53:28.799402 amisc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      587 2024-01-30 16:53:14.399595 amisc-0.2.1/src/amisc/__init__.py
--rw-r--r--   0        0        0    50209 2024-01-30 16:53:14.399595 amisc-0.2.1/src/amisc/component.py
--rw-r--r--   0        0        0    11579 2024-01-30 16:53:14.399595 amisc-0.2.1/src/amisc/examples/models.py
--rw-r--r--   0        0        0     2112 2024-01-30 16:53:14.399595 amisc-0.2.1/src/amisc/examples/tutorial.py
--rw-r--r--   0        0        0    38513 2024-01-30 16:53:14.399595 amisc-0.2.1/src/amisc/interpolator.py
--rw-r--r--   0        0        0    12424 2024-01-30 16:53:14.399595 amisc-0.2.1/src/amisc/rv.py
--rw-r--r--   0        0        0    79289 2024-01-30 16:53:14.399595 amisc-0.2.1/src/amisc/system.py
--rw-r--r--   0        0        0     3140 2024-01-30 16:53:14.399595 amisc-0.2.1/src/amisc/utils.py
--rw-r--r--   0        0        0        0 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      318 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     4400 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/test_component.py
--rw-r--r--   0        0        0     1983 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/test_convergence.py
--rw-r--r--   0        0        0     7151 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/test_interpolator.py
--rw-r--r--   0        0        0     2205 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/test_loading.py
--rw-r--r--   0        0        0       95 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/test_package.py
--rw-r--r--   0        0        0      664 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/test_rv.py
--rw-r--r--   0        0        0    13763 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/test_system.py
--rw-r--r--   0        0        0      183 2024-01-30 16:53:14.399595 amisc-0.2.1/tests/test_utils.py
--rw-r--r--   0        0        0    44541 1970-01-01 00:00:00.000000 amisc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-14 23:06:11.147476 amisc-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2904 2024-05-14 23:06:11.147476 amisc-0.3.0/docs/README.md
+-rw-r--r--   0        0        0     1925 2024-05-14 23:06:28.691406 amisc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      587 2024-05-14 23:06:11.151476 amisc-0.3.0/src/amisc/__init__.py
+-rw-r--r--   0        0        0    51534 2024-05-14 23:06:11.151476 amisc-0.3.0/src/amisc/component.py
+-rw-r--r--   0        0        0    11579 2024-05-14 23:06:11.151476 amisc-0.3.0/src/amisc/examples/models.py
+-rw-r--r--   0        0        0     2112 2024-05-14 23:06:11.151476 amisc-0.3.0/src/amisc/examples/tutorial.py
+-rw-r--r--   0        0        0    38513 2024-05-14 23:06:11.151476 amisc-0.3.0/src/amisc/interpolator.py
+-rw-r--r--   0        0        0    12424 2024-05-14 23:06:11.151476 amisc-0.3.0/src/amisc/rv.py
+-rw-r--r--   0        0        0    79571 2024-05-14 23:06:11.151476 amisc-0.3.0/src/amisc/system.py
+-rw-r--r--   0        0        0     3140 2024-05-14 23:06:11.151476 amisc-0.3.0/src/amisc/utils.py
+-rw-r--r--   0        0        0        0 2024-05-14 23:06:11.151476 amisc-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      318 2024-05-14 23:06:11.151476 amisc-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     4400 2024-05-14 23:06:11.151476 amisc-0.3.0/tests/test_component.py
+-rw-r--r--   0        0        0     1983 2024-05-14 23:06:11.151476 amisc-0.3.0/tests/test_convergence.py
+-rw-r--r--   0        0        0     7151 2024-05-14 23:06:11.151476 amisc-0.3.0/tests/test_interpolator.py
+-rw-r--r--   0        0        0     2205 2024-05-14 23:06:11.155476 amisc-0.3.0/tests/test_loading.py
+-rw-r--r--   0        0        0       95 2024-05-14 23:06:11.155476 amisc-0.3.0/tests/test_package.py
+-rw-r--r--   0        0        0      664 2024-05-14 23:06:11.155476 amisc-0.3.0/tests/test_rv.py
+-rw-r--r--   0        0        0    13763 2024-05-14 23:06:11.155476 amisc-0.3.0/tests/test_system.py
+-rw-r--r--   0        0        0      183 2024-05-14 23:06:11.155476 amisc-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0    44570 1970-01-01 00:00:00.000000 amisc-0.3.0/PKG-INFO
```

### Comparing `amisc-0.2.1/LICENSE` & `amisc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/docs/README.md` & `amisc-0.3.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/pyproject.toml` & `amisc-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "numpy>=1.26.2",
     "scikit-learn>=1.3.2",
     "networkx>=3.2.1",
     "dill>=0.3.7",
     "scipy>=1.11.4",
     "matplotlib>=3.8.2",
     "uqtils>=0.1.0",
+    "joblib>=1.3.2",
 ]
 requires-python = ">=3.11"
 readme = "docs/README.md"
 keywords = [
     "surrogates",
     "multidisciplinary",
     "multifidelity",
@@ -29,15 +30,15 @@
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Intended Audience :: Science/Research",
 ]
-version = "0.2.1"
+version = "0.3.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Repository = "https://github.com/eckelsjd/amisc.git"
 Documentation = "https://eckelsjd.github.io/amisc"
```

### Comparing `amisc-0.2.1/src/amisc/__init__.py` & `amisc-0.3.0/src/amisc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 - License - GNU GPLv3
 """
 import numpy as np
 
 from amisc.interpolator import BaseInterpolator
 from amisc.rv import BaseRV
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 
 # Custom types that are used frequently
 IndexSet = list[tuple[tuple, tuple]]
 MiscTree = dict[str: dict[str: float | BaseInterpolator]]
 InterpResults = BaseInterpolator | tuple[list[int | tuple | str], np.ndarray, BaseInterpolator]
 IndicesRV = list[int | str | BaseRV] | int | str | BaseRV
```

### Comparing `amisc-0.2.1/src/amisc/component.py` & `amisc-0.3.0/src/amisc/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 """
 import itertools
 import copy
 import ast
 from pathlib import Path
 from abc import ABC, abstractmethod
 from concurrent.futures import Executor, ALL_COMPLETED, wait
+import tempfile
+import os
 
 import numpy as np
 from sklearn.linear_model import Ridge
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import MaxAbsScaler
+from joblib import delayed
 
 from amisc.utils import get_logger
 from amisc.rv import BaseRV
 from amisc import IndexSet, MiscTree, InterpResults
 from amisc.interpolator import BaseInterpolator, LagrangeInterpolator
 
 
@@ -233,41 +236,55 @@
         for alpha, beta in list(self.candidate_set):
             # Temporarily add a candidate index to active set
             self.index_set.append((alpha, beta))
             yield alpha, beta
             del self.index_set[-1]
 
     def predict(self, x: np.ndarray | float, use_model: str | tuple = None, model_dir: str | Path = None,
-                training: bool = False, index_set: IndexSet = None) -> np.ndarray:
+                training: bool = False, index_set: IndexSet = None, ppool=None) -> np.ndarray:
         """Evaluate the MISC approximation at new points `x`.
 
         !!! Note
             By default this will predict the MISC surrogate approximation. However, for convenience you can also specify
             `use_model` to call the underlying function instead.
 
         :param x: `(..., x_dim)` the points to be interpolated, must be within input domain for accuracy
         :param use_model: 'best'=high-fidelity, 'worst'=low-fidelity, tuple=a specific `alpha`, None=surrogate (default)
         :param model_dir: directory to save output files if `use_model` is specified, ignored otherwise
         :param training: if `True`, then only compute with the active index set, otherwise use all candidates as well
         :param index_set: a list of concatenated $(\\alpha, \\beta)$ to override `self.index_set` if given, else ignore
+        :param ppool: a joblib `Parallel` pool to loop over multi-indices in parallel
         :returns y: `(..., y_dim)` the surrogate approximation of the function (or the function itself if `use_model`)
         """
         x = np.atleast_1d(x)
         if use_model is not None:
             return self._bypass_surrogate(x, use_model, model_dir)
 
         index_set, misc_coeff = self._combination(index_set, training)  # Choose the correct index set and misc_coeff
 
-        y = np.zeros(x.shape[:-1] + (self.ydim,), dtype=x.dtype)
-        for alpha, beta in index_set:
+        def run_batch(alpha, beta, y):
             comb_coeff = misc_coeff[str(alpha)][str(beta)]
             if np.abs(comb_coeff) > 0:
                 func = self.surrogates[str(alpha)][str(beta)]
                 y += int(comb_coeff) * func(x)
 
+        if ppool is not None:
+            with tempfile.NamedTemporaryFile(suffix='.dat', mode='w+b', delete=False) as y_fd:
+                pass
+            y_ret = np.memmap(y_fd.name, dtype=x.dtype, mode='r+', shape=x.shape[:-1] + (self.ydim,))
+            res = ppool(delayed(run_batch)(alpha, beta, y_ret) for alpha, beta in index_set)
+            y = np.empty(y_ret.shape, dtype=x.dtype)
+            y[:] = y_ret[:]
+            del y_ret
+            os.unlink(y_fd.name)
+        else:
+            y = np.zeros(x.shape[:-1] + (self.ydim,), dtype=x.dtype)
+            for alpha, beta in index_set:
+                run_batch(alpha, beta, y)
+
         return y
 
     def grad(self, x: np.ndarray | float | list, training: bool = False, index_set: IndexSet = None) -> np.ndarray:
         """Evaluate the derivative/Jacobian of the MISC approximation at new points `x`.
 
         :param x: `(..., x_dim)` the evaluation points, must be within input domain for accuracy
         :param training: if `True`, then only compute with the active index set, otherwise use all candidates as well
@@ -593,33 +610,46 @@
         self.xi_map = dict()            # Maps alphas -> grid point coords -> interpolation points
         self.yi_map = dict()            # Maps alphas -> grid point coords -> interpolation function values
         self.yi_nan_map = dict()        # Maps alphas -> grid point coords -> interpolated yi values when yi=nan
         self.yi_files = dict()          # Maps alphas -> grid point coords -> model output files (optional)
         super().__init__(*args, **kwargs)
 
     # Override
-    def predict(self, x, use_model=None, model_dir=None, training=False, index_set=None):
+    def predict(self, x, use_model=None, model_dir=None, training=False, index_set=None, ppool=None):
         """Need to override `super()` to allow passing in interpolation grids `xi` and `yi`."""
         x = np.atleast_1d(x)
         if use_model is not None:
             return self._bypass_surrogate(x, use_model, model_dir)
 
         index_set, misc_coeff = self._combination(index_set, training)
 
-        y = np.zeros(x.shape[:-1] + (self.ydim,), dtype=x.dtype)
-        for alpha, beta in index_set:
+        def run_batch(alpha, beta, y):
             comb_coeff = misc_coeff[str(alpha)][str(beta)]
             if np.abs(comb_coeff) > 0:
                 # Gather the xi/yi interpolation points/qoi_ind for this sub tensor-product grid
                 interp = self.surrogates[str(alpha)][str(beta)]
                 xi, yi = self.get_tensor_grid(alpha, beta)
 
                 # Add this sub tensor-product grid to the MISC approximation
                 y += int(comb_coeff) * interp(x, xi=xi, yi=yi)
 
+        if ppool is not None:
+            with tempfile.NamedTemporaryFile(suffix='.dat', mode='w+b', delete=False) as y_fd:
+                pass
+            y_ret = np.memmap(y_fd.name, dtype=x.dtype, mode='r+', shape=x.shape[:-1] + (self.ydim,))
+            res = ppool(delayed(run_batch)(alpha, beta, y_ret) for alpha, beta in index_set)
+            y = np.empty(y_ret.shape, dtype=x.dtype)
+            y[:] = y_ret[:]
+            del y_ret
+            os.unlink(y_fd.name)
+        else:
+            y = np.zeros(x.shape[:-1] + (self.ydim,), dtype=x.dtype)
+            for alpha, beta in index_set:
+                run_batch(alpha, beta, y)
+
         return y
 
     # Override
     def grad(self, x, training=False, index_set=None):
         """Need to override `super()` to allow passing in interpolation grids `xi` and `yi`."""
         x = np.atleast_1d(x)
         index_set, misc_coeff = self._combination(index_set, training)  # Choose the correct index set and misc_coeff
```

### Comparing `amisc-0.2.1/src/amisc/examples/models.py` & `amisc-0.3.0/src/amisc/examples/models.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/src/amisc/examples/tutorial.py` & `amisc-0.3.0/src/amisc/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/src/amisc/interpolator.py` & `amisc-0.3.0/src/amisc/interpolator.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/src/amisc/rv.py` & `amisc-0.3.0/src/amisc/rv.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/src/amisc/system.py` & `amisc-0.3.0/src/amisc/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -760,15 +760,16 @@
             self.logger.info(f"No candidates left for refinement, iteration: {self.refine_level}")
             num_evals = 0
 
         return l2_star, node_star, alpha_star, beta_star, num_evals, cost_star
 
     def predict(self, x: np.ndarray | float, max_fpi_iter: int = 100, anderson_mem: int = 10, fpi_tol: float = 1e-10,
                 use_model: str | tuple | dict = None, model_dir: str | Path = None, verbose: bool = False,
-                training: bool = False, index_set: dict[str: IndexSet] = None, qoi_ind: IndicesRV = None) -> np.ndarray:
+                training: bool = False, index_set: dict[str: IndexSet] = None, qoi_ind: IndicesRV = None,
+                ppool=None) -> np.ndarray:
         """Evaluate the system surrogate at exogenous inputs `x`.
 
         !!! Warning
             You can use this function to predict outputs for your MD system using the full-order models rather than the
             surrogate, by specifying `use_model`. This is convenient because `SystemSurrogate` manages all the
             coupled information flow between models automatically. However, it is *highly* recommended to not use
             the full model if your system contains feedback loops. The FPI nonlinear solver would be infeasible using
@@ -781,14 +782,15 @@
         :param use_model: 'best'=highest-fidelity, 'worst'=lowest-fidelity, tuple=specific fidelity, None=surrogate,
                            specify a `dict` of the above to assign different model fidelities for diff components
         :param model_dir: directory to save model outputs if `use_model` is specified
         :param verbose: whether to print out iteration progress during execution
         :param training: whether to call the system surrogate in training or evaluation mode, ignored if `use_model`
         :param index_set: `dict(node=[indices])` to override default index set for a node (only useful for parallel)
         :param qoi_ind: list of qoi indices to return, defaults to returning all system `coupling_vars`
+        :param ppool: a joblib `Parallel` instance to pass to each component to loop over multi-indices in parallel
         :returns y: `(..., y_dim)` the surrogate approximation of the system QoIs
         """
         # Allocate space for all system outputs (just save all coupling vars)
         x = np.atleast_1d(x)
         ydim = len(self.coupling_vars)
         y = np.zeros(x.shape[:-1] + (ydim,), dtype=x.dtype)
         valid_idx = ~np.isnan(x[..., 0])  # Keep track of valid samples (set to False if FPI fails)
@@ -835,15 +837,16 @@
 
                 # Compute outputs
                 indices = index_set.get(scc[0], None) if index_set is not None else None
                 if model_dir is not None:
                     output_dir = Path(model_dir) / scc[0]
                     os.mkdir(output_dir)
                 comp_output = node_obj['surrogate'](comp_input[valid_idx, :], use_model=use_model.get(scc[0]),
-                                                    model_dir=output_dir, training=training, index_set=indices)
+                                                    model_dir=output_dir, training=training, index_set=indices,
+                                                    ppool=ppool)
                 for local_i, global_i in enumerate(node_obj['global_out']):
                     y[valid_idx, global_i] = comp_output[..., local_i]
                     is_computed[global_i] = True
                 node_obj['is_computed'] = True
 
                 if verbose:
                     self.logger.info(f"Component '{scc[0]}' completed. Runtime: {time.time() - t1} s")
@@ -886,15 +889,16 @@
                         exo_inputs = x[..., node_obj['exo_in']]
                         coupling_inputs = x_couple[..., node_obj['global_in']]
                         comp_input = np.concatenate((exo_inputs, coupling_inputs), axis=-1)     # (..., xdim)
 
                         # Compute component outputs (just don't do this FPI with the real models, please..)
                         indices = index_set.get(node, None) if index_set is not None else None
                         comp_output = node_obj['surrogate'](comp_input[valid_idx, :], use_model=use_model.get(node),
-                                                            model_dir=None, training=training, index_set=indices)
+                                                            model_dir=None, training=training, index_set=indices,
+                                                            ppool=ppool)
                         global_idx = node_obj['global_out']
                         for local_i, global_i in enumerate(global_idx):
                             x_couple_next[valid_idx, global_i] = comp_output[..., local_i]
                             # Can't splice valid_idx with global_idx for some reason, have to loop over global_idx here
 
                     # Compute residual and check end conditions
                     residual = np.expand_dims(x_couple_next[..., fpi_idx] - x_couple[..., fpi_idx], axis=-1)
```

### Comparing `amisc-0.2.1/src/amisc/utils.py` & `amisc-0.3.0/src/amisc/utils.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/tests/test_component.py` & `amisc-0.3.0/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/tests/test_convergence.py` & `amisc-0.3.0/tests/test_convergence.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/tests/test_interpolator.py` & `amisc-0.3.0/tests/test_interpolator.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/tests/test_loading.py` & `amisc-0.3.0/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/tests/test_rv.py` & `amisc-0.3.0/tests/test_rv.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/tests/test_system.py` & `amisc-0.3.0/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `amisc-0.2.1/PKG-INFO` & `amisc-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: amisc
-Version: 0.2.1
+Version: 0.3.0
 Summary: Adaptive multi-index stochastic collocation (surrogates) for metamodeling of multidisciplinary systems
-Keywords: surrogates multidisciplinary multifidelity adaptive collocation metamodeling
+Keywords: surrogates,multidisciplinary,multifidelity,adaptive,collocation,metamodeling
 Author-Email: Joshua Eckels <eckelsjd@umich.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -691,14 +691,15 @@
 Requires-Dist: numpy>=1.26.2
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: networkx>=3.2.1
 Requires-Dist: dill>=0.3.7
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: matplotlib>=3.8.2
 Requires-Dist: uqtils>=0.1.0
+Requires-Dist: joblib>=1.3.2
 Description-Content-Type: text/markdown
 
 ![Logo](https://raw.githubusercontent.com/eckelsjd/amisc/main/docs/assets/amisc_logo_text.svg)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
 [![PyPI](https://img.shields.io/pypi/v/amisc?logo=python&logoColor=%23cccccc)](https://pypi.org/project/amisc)
 [![Python 3.11](https://img.shields.io/badge/python-3.11+-blue.svg?logo=python&logoColor=cccccc)](https://www.python.org/downloads/)
 ![Commits](https://img.shields.io/github/commit-activity/m/eckelsjd/amisc?logo=github)
```

