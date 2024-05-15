# Comparing `tmp/solid_dmft-3.2.1.tar.gz` & `tmp/solid_dmft-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solid_dmft-3.2.1.tar", last modified: Mon Sep 25 20:05:46 2023, max compression
+gzip compressed data, was "solid_dmft-3.2.2.tar", last modified: Wed May 15 15:20:35 2024, max compression
```

## Comparing `solid_dmft-3.2.1.tar` & `solid_dmft-3.2.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 20:05:46.521285 solid_dmft-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    35147 2023-09-25 20:05:29.000000 solid_dmft-3.2.1/COPYING.txt
--rw-r--r--   0 root         (0) root         (0)      885 2023-09-25 20:05:29.000000 solid_dmft-3.2.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      227 2023-09-25 20:05:35.000000 solid_dmft-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3643 2023-09-25 20:05:46.521285 solid_dmft-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2796 2023-09-25 20:05:29.000000 solid_dmft-3.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)      973 2023-09-25 20:05:35.000000 solid_dmft-3.2.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 20:05:46.509285 solid_dmft-3.2.1/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 20:05:46.513285 solid_dmft-3.2.1/python/solid_dmft/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14897 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/csc_flow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 20:05:46.517285 solid_dmft-3.2.1/python/solid_dmft/dft_managers/
--rw-r--r--   0 root         (0) root         (0)     1146 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dft_managers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5494 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dft_managers/mpi_helpers.py
--rw-r--r--   0 root         (0) root         (0)     7302 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dft_managers/qe_manager.py
--rw-r--r--   0 root         (0) root         (0)     7980 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dft_managers/vasp_manager.py
--rwxr-xr-x   0 root         (0) root         (0)    36932 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_cycle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 20:05:46.517285 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/
--rw-r--r--   0 root         (0) root         (0)     1179 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6014 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/afm_mapping.py
--rw-r--r--   0 root         (0) root         (0)    12110 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/convergence.py
--rw-r--r--   0 root         (0) root         (0)     8953 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/formatter.py
--rw-r--r--   0 root         (0) root         (0)    10088 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/greens_functions_mixer.py
--rwxr-xr-x   0 root         (0) root         (0)    22700 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/initial_self_energies.py
--rw-r--r--   0 root         (0) root         (0)    24491 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/interaction_hamiltonian.py
--rw-r--r--   0 root         (0) root         (0)     2068 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/legendre_filter.py
--rwxr-xr-x   0 root         (0) root         (0)    18548 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py
--rw-r--r--   0 root         (0) root         (0)    24521 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/observables.py
--rw-r--r--   0 root         (0) root         (0)     7298 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/results_to_archive.py
--rwxr-xr-x   0 root         (0) root         (0)    57100 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/dmft_tools/solver.py
--rw-r--r--   0 root         (0) root         (0)     5028 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 20:05:46.521285 solid_dmft-3.2.1/python/solid_dmft/postprocessing/
--rw-r--r--   0 root         (0) root         (0)     1143 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/postprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9176 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py
--rw-r--r--   0 root         (0) root         (0)    16115 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/postprocessing/maxent_gf_imp.py
--rw-r--r--   0 root         (0) root         (0)    12338 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/postprocessing/maxent_gf_latt.py
--rw-r--r--   0 root         (0) root         (0)    17196 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/postprocessing/maxent_sigma.py
--rw-r--r--   0 root         (0) root         (0)    38595 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/postprocessing/plot_correlated_bands.py
--rwxr-xr-x   0 root         (0) root         (0)    71238 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/read_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 20:05:46.521285 solid_dmft-3.2.1/python/solid_dmft/util/
--rw-r--r--   0 root         (0) root         (0)     1178 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6808 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/util/symmetrize_gamma_file.py
--rw-r--r--   0 root         (0) root         (0)     4940 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/util/update_dmft_config.py
--rw-r--r--   0 root         (0) root         (0)     3814 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/util/update_results_h5.py
--rw-r--r--   0 root         (0) root         (0)     4727 2023-09-25 20:05:30.000000 solid_dmft-3.2.1/python/solid_dmft/util/write_kslice_to_h5.py
--rw-r--r--   0 root         (0) root         (0)     1392 2023-09-25 20:05:38.000000 solid_dmft-3.2.1/python/solid_dmft/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 20:05:46.513285 solid_dmft-3.2.1/python/solid_dmft.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3643 2023-09-25 20:05:46.000000 solid_dmft-3.2.1/python/solid_dmft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1828 2023-09-25 20:05:46.000000 solid_dmft-3.2.1/python/solid_dmft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-25 20:05:46.000000 solid_dmft-3.2.1/python/solid_dmft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-09-25 20:05:46.000000 solid_dmft-3.2.1/python/solid_dmft.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-09-25 20:05:46.000000 solid_dmft-3.2.1/python/solid_dmft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-09-25 20:05:46.000000 solid_dmft-3.2.1/python/solid_dmft.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-25 20:05:46.521285 solid_dmft-3.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:20:35.570828 solid_dmft-3.2.2/
+-rw-r--r--   0 root         (0) root         (0)    35147 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/COPYING.txt
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-15 15:20:33.000000 solid_dmft-3.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3591 2024-05-15 15:20:35.570828 solid_dmft-3.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      937 2024-05-15 15:20:33.000000 solid_dmft-3.2.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:20:35.558828 solid_dmft-3.2.2/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:20:35.562828 solid_dmft-3.2.2/python/solid_dmft/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14897 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/csc_flow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:20:35.562828 solid_dmft-3.2.2/python/solid_dmft/dft_managers/
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dft_managers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5494 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dft_managers/mpi_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dft_managers/qe_manager.py
+-rw-r--r--   0 root         (0) root         (0)     7980 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dft_managers/vasp_manager.py
+-rwxr-xr-x   0 root         (0) root         (0)    36937 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_cycle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:20:35.566828 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6014 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/afm_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    12110 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/convergence.py
+-rw-r--r--   0 root         (0) root         (0)     8953 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/formatter.py
+-rw-r--r--   0 root         (0) root         (0)    10088 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/greens_functions_mixer.py
+-rwxr-xr-x   0 root         (0) root         (0)    22700 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/initial_self_energies.py
+-rw-r--r--   0 root         (0) root         (0)    24491 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/interaction_hamiltonian.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/legendre_filter.py
+-rwxr-xr-x   0 root         (0) root         (0)    18548 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/matheval.py
+-rw-r--r--   0 root         (0) root         (0)    24521 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/observables.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/results_to_archive.py
+-rwxr-xr-x   0 root         (0) root         (0)    57627 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/dmft_tools/solver.py
+-rw-r--r--   0 root         (0) root         (0)     5064 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:20:35.570828 solid_dmft-3.2.2/python/solid_dmft/postprocessing/
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/postprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py
+-rw-r--r--   0 root         (0) root         (0)    16115 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/postprocessing/maxent_gf_imp.py
+-rw-r--r--   0 root         (0) root         (0)    12338 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/postprocessing/maxent_gf_latt.py
+-rw-r--r--   0 root         (0) root         (0)    17196 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/postprocessing/maxent_sigma.py
+-rw-r--r--   0 root         (0) root         (0)    38731 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/postprocessing/plot_correlated_bands.py
+-rwxr-xr-x   0 root         (0) root         (0)    71594 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/read_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:20:35.570828 solid_dmft-3.2.2/python/solid_dmft/util/
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6808 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/util/symmetrize_gamma_file.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/util/update_dmft_config.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/util/update_results_h5.py
+-rw-r--r--   0 root         (0) root         (0)     4727 2024-05-15 15:20:28.000000 solid_dmft-3.2.2/python/solid_dmft/util/write_kslice_to_h5.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-05-15 15:20:33.000000 solid_dmft-3.2.2/python/solid_dmft/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:20:35.570828 solid_dmft-3.2.2/python/solid_dmft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3591 2024-05-15 15:20:35.000000 solid_dmft-3.2.2/python/solid_dmft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1869 2024-05-15 15:20:35.000000 solid_dmft-3.2.2/python/solid_dmft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 15:20:35.000000 solid_dmft-3.2.2/python/solid_dmft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-15 15:20:35.000000 solid_dmft-3.2.2/python/solid_dmft.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-15 15:20:35.000000 solid_dmft-3.2.2/python/solid_dmft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-15 15:20:35.000000 solid_dmft-3.2.2/python/solid_dmft.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 15:20:35.570828 solid_dmft-3.2.2/setup.cfg
```

### Comparing `solid_dmft-3.2.1/COPYING.txt` & `solid_dmft-3.2.2/COPYING.txt`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/LICENSE.txt` & `solid_dmft-3.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/PKG-INFO` & `solid_dmft-3.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solid_dmft
-Version: 3.2.1
+Version: 3.2.2
 Summary: solid_dmft: a versatile python wrapper to perform DFT+DMFT calculations utilizing the TRIQS software library
 Author-email: Alexander Hampel <ahampel@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/solid_dmft
 Project-URL: Bug Tracker, https://github.com/triqs/solid_dmft/issues
 Project-URL: Paper, https://doi.org/10.21105/joss.04623
 Keywords: DMFT,DFT,triqs
 Classifier: Programming Language :: Python :: 3
@@ -13,16 +13,14 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: COPYING.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pytest
-Requires-Dist: scikit-image
-Requires-Dist: argparse
 
 ![logo_soliDMFT](https://raw.githubusercontent.com/triqs/solid_dmft/unstable/doc/logos/logo_solid_dmft.png)
 
 ![CI](https://github.com/triqs/solid_dmft/actions/workflows/build.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/solid_dmft.svg)](https://badge.fury.io/py/solid_dmft)
 [![status](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922/status.svg)](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922)
```

### Comparing `solid_dmft-3.2.1/README.md` & `solid_dmft-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/pyproject.toml` & `solid_dmft-3.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 
 [project]
 name = "solid_dmft"
-version = "3.2.1"
+version = "3.2.2"
 authors = [
   { name="Alexander Hampel", email="ahampel@flatironinstitute.org" }
 ]
 description = "solid_dmft: a versatile python wrapper to perform DFT+DMFT calculations utilizing the TRIQS software library"
 readme = "README.md"
 keywords = ["DMFT", "DFT", "triqs"]
 requires-python = ">=3.7"
@@ -19,17 +19,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy",
     "scipy",
-    "pytest",
-    "scikit-image",
-    "argparse"
+    "pytest"
 ]
 
 [project.urls]
 "Homepage" = "https://triqs.github.io/solid_dmft"
 "Bug Tracker" = "https://github.com/triqs/solid_dmft/issues"
 "Paper" = "https://doi.org/10.21105/joss.04623"
```

### Comparing `solid_dmft-3.2.1/python/solid_dmft/__init__.py` & `solid_dmft-3.2.2/python/solid_dmft/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/csc_flow.py` & `solid_dmft-3.2.2/python/solid_dmft/csc_flow.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dft_managers/__init__.py` & `solid_dmft-3.2.2/python/solid_dmft/dft_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dft_managers/mpi_helpers.py` & `solid_dmft-3.2.2/python/solid_dmft/dft_managers/mpi_helpers.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dft_managers/qe_manager.py` & `solid_dmft-3.2.2/python/solid_dmft/dft_managers/qe_manager.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dft_managers/vasp_manager.py` & `solid_dmft-3.2.2/python/solid_dmft/dft_managers/vasp_manager.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_cycle.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_cycle.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,15 +656,15 @@
             # copy the self energy instead of solving it explicitly
             solvers = afm_mapping.apply(general_params, solver_params, icrsh, sum_k.gf_struct_solver[icrsh], solvers)
         else:
             # Solve the impurity problem for this shell
             mpi.report('\nSolving the impurity problem for shell {} ...'.format(icrsh))
             mpi.barrier()
             start_time = timer()
-            solvers[icrsh].solve()
+            solvers[icrsh].solve(it=it)
             mpi.barrier()
             mpi.report('Actual time for solver: {:.2f} s'.format(timer() - start_time))
 
         # some printout of the obtained density matrices and some basic checks from the unsymmetrized solver output
         density_shell[icrsh] = np.real(solvers[icrsh].G_freq_unsym.total_density())
         density_tot += density_shell[icrsh]*shell_multiplicity[icrsh]
         density_mat_unsym[icrsh] = solvers[icrsh].G_freq_unsym.density()
```

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/__init__.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/afm_mapping.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/afm_mapping.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/convergence.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/convergence.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/formatter.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/formatter.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/greens_functions_mixer.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/greens_functions_mixer.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/initial_self_energies.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/initial_self_energies.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/interaction_hamiltonian.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/interaction_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/legendre_filter.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/legendre_filter.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/observables.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/observables.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/results_to_archive.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/results_to_archive.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/dmft_tools/solver.py` & `solid_dmft-3.2.2/python/solid_dmft/dmft_tools/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from triqs.gf.tools import inverse, make_zero_tail
 from triqs.gf.descriptors import Fourier
 from triqs.operators import c_dag, c, Operator
 import triqs.utility.mpi as mpi
 from h5 import HDFArchive
 
 from . import legendre_filter
+from .matheval import MathExpr
 
 def get_n_orbitals(sum_k):
     """
     determines the number of orbitals within the
     solver block structure.
 
     Parameters
@@ -104,15 +105,15 @@
     Handles all solid_dmft solver objects and contains TRIQS solver instance.
 
     Attributes
     ----------
 
     Methods
     -------
-    solve(self)
+    solve(self, **kwargs)
         solve impurity problem
     '''
 
     def __init__(self, general_params, solver_params, advanced_params, sum_k, icrsh, h_int, iteration_offset, solver_struct_ftps):
         r'''
         Initialisation of the solver instance with h_int for impurity "icrsh" based on soliDMFT parameters.
 
@@ -136,14 +137,18 @@
         self.solver_params = solver_params
         self.advanced_params = advanced_params
         self.sum_k = sum_k
         self.icrsh = icrsh
         self.h_int = h_int
         self.iteration_offset = iteration_offset
         self.solver_struct_ftps = solver_struct_ftps
+        if solver_params.get("random_seed") is None:
+            self.random_seed_generator = None
+        else:
+            self.random_seed_generator = MathExpr(solver_params["random_seed"])
 
         # initialize solver object, options are cthyb
         if self.general_params['solver_type'] == 'cthyb':
             from triqs_cthyb.version import triqs_cthyb_hash, version
 
             # sets up necessary GF objects on ImFreq
             self._init_ImFreq_objects()
@@ -332,19 +337,24 @@
                                                                  mesh=MeshReFreq(n_w=self.n_w, window=self.general_params['w_range'])
                                                                  )
 
     # ********************************************************************
     # solver-specific solve() command
     # ********************************************************************
 
-    def solve(self):
+    def solve(self, **kwargs):
         r'''
         solve impurity problem with current solver
         '''
 
+        if self.random_seed_generator is None:
+            random_seed = {}
+        else:
+            random_seed = { "random_seed": int(self.random_seed_generator(it=kwargs["it"], rank=mpi.rank)) }
+
         if self.general_params['solver_type'] == 'cthyb':
 
             if self.general_params['cthyb_delta_interface']:
                 mpi.report('\n Using the delta interface for cthyb passing Delta(tau) and Hloc0 directly.')
                  # prepare solver input
                 sumk_eal = self.sum_k.eff_atomic_levels()[self.icrsh]
                 solver_eal = self.sum_k.block_structure.convert_matrix(sumk_eal, space_from='sumk', ish_from=self.sum_k.inequiv_to_corr[self.icrsh])
@@ -383,15 +393,15 @@
                         archive['DMFT_input/solver'].create_group('it_-1')
                     archive['DMFT_input/solver/it_-1'][f'S_{self.icrsh}'] = self.triqs_solver
                     archive['DMFT_input/solver/it_-1'][f'solve_params_{self.icrsh}'] = self.solver_params
                     archive['DMFT_input/solver/it_-1']['mpi_size'] = mpi.size
 
             # Solve the impurity problem for icrsh shell
             # *************************************
-            self.triqs_solver.solve(h_int=self.h_int, **self.solver_params)
+            self.triqs_solver.solve(h_int=self.h_int, **{ **self.solver_params, **random_seed })
             # *************************************
 
             # call postprocessing
             self._cthyb_postprocessing()
 
         elif self.general_params['solver_type'] == 'ctint':
             # fill G0_freq from sum_k to solver
@@ -399,15 +409,15 @@
 
             if self.general_params['h_int_type'] == 'dynamic':
                 for b1, b2 in product(self.sum_k.gf_struct_solver_dict[self.icrsh].keys(), repeat=2):
                     self.triqs_solver.D0_iw[b1,b2] << self.U_iw[self.icrsh]
 
             # Solve the impurity problem for icrsh shell
             # *************************************
-            self.triqs_solver.solve(h_int=self.h_int, **self.solver_params)
+            self.triqs_solver.solve(h_int=self.h_int, **{ **self.solver_params, **random_seed })
             # *************************************
 
             # call postprocessing
             self._ctint_postprocessing()
 
         elif self.general_params['solver_type'] == 'hubbardI':
             # fill G0_freq from sum_k to solver
@@ -573,15 +583,15 @@
 
         elif self.general_params['solver_type'] == 'inchworm':
             # fill Delta_time from Delta_freq sum_k to solver
             self.triqs_solver.Delta_tau << make_gf_from_fourier(self.Delta_freq).real
 
             # Solve the impurity problem for icrsh shell
             # *************************************
-            self.triqs_solver.solve(h_int=self.h_int, **self.solver_params)
+            self.triqs_solver.solve(h_int=self.h_int, **{ **self.solver_params, **random_seed })
             # *************************************
 
             # call postprocessing
             self._inchworm_postprocessing()
 
         if self.general_params['solver_type'] == 'ctseg':
             # fill G0_freq from sum_k to solver
@@ -590,15 +600,15 @@
 
             if self.general_params['h_int_type'] == 'dynamic':
                 for b1, b2 in product(self.sum_k.gf_struct_solver_dict[self.icrsh].keys(), repeat=2):
                     self.triqs_solver.D0_iw[b1+"|"+b2] << self.U_iw[self.icrsh]
 
             # Solve the impurity problem for icrsh shell
             # *************************************
-            self.triqs_solver.solve(h_int=self.h_int, **self.solver_params)
+            self.triqs_solver.solve(h_int=self.h_int, **{ **self.solver_params, **random_seed })
             # *************************************
 
             # call postprocessing
             self._ctseg_postprocessing()
 
         return
 
@@ -697,15 +707,15 @@
                                       n_iw=self.general_params['n_iw'], force_real=self.solver_params['force_real'],
                                       symmetries=[self._make_spin_equal],
                                       dc_U= self.general_params['U'][self.icrsh],
                                       dc_J= self.general_params['J'][self.icrsh]
                                       )
 
         def _interface_hartree_dc(hartree_instance, general_params, advanced_params, icrsh):
-            """ Modifies in-place class attributes to infercace with options in solid_dmft 
+            """ Modifies in-place class attributes to infercace with options in solid_dmft
                 for the moment supports only DC-relevant parameters
 
             Parameters
             ----------
                 general_params : dict
                     solid_dmft general parameter dictionary
                 advanced_params : dict
```

### Comparing `solid_dmft-3.2.1/python/solid_dmft/main.py` & `solid_dmft-3.2.2/python/solid_dmft/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,16 @@
             # Creates output directory if it does not exist
             if not os.path.exists(general_params['jobname']):
                 os.makedirs(general_params['jobname'])
 
             # Copies h5 archive and config file to subfolder if are not there
             for file in (general_params['seedname']+'.h5',
                          general_params['config_file']):
-                if not os.path.isfile(general_params['jobname']+'/'+file):
-                    shutil.copyfile(file, general_params['jobname']+'/'+file)
+                if not os.path.isfile(general_params['jobname']+'/'+os.path.basename(file)):
+                    shutil.copyfile(file, general_params['jobname']+'/'+os.path.basename(file))
         mpi.barrier()
 
         # Runs dmft_cycle
         dmft_cycle(general_params, solver_params, advanced_params,
                    dft_params, general_params['n_iter_dmft'])
 
     mpi.barrier()
```

### Comparing `solid_dmft-3.2.1/python/solid_dmft/postprocessing/__init__.py` & `solid_dmft-3.2.2/python/solid_dmft/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py` & `solid_dmft-3.2.2/python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py` & `solid_dmft-3.2.2/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/postprocessing/maxent_gf_imp.py` & `solid_dmft-3.2.2/python/solid_dmft/postprocessing/maxent_gf_imp.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/postprocessing/maxent_gf_latt.py` & `solid_dmft-3.2.2/python/solid_dmft/postprocessing/maxent_gf_latt.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/postprocessing/maxent_sigma.py` & `solid_dmft-3.2.2/python/solid_dmft/postprocessing/maxent_sigma.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/postprocessing/plot_correlated_bands.py` & `solid_dmft-3.2.2/python/solid_dmft/postprocessing/plot_correlated_bands.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,16 +174,14 @@
 
     sigma_interpolated = np.zeros((n_orb, n_orb, freq_dict['n_w']), dtype=complex)
 
     # interpolate sigma
     def interpolate_sigma(w_mesh, w_mesh_dmft, orb1, orb2): return np.interp(w_mesh, w_mesh_dmft, sigma_mat[:, orb1, orb2])
 
     for ct1, ct2 in itertools.product(range(n_orb), range(n_orb)):
-        if ct1 != ct2 and not SOC:
-            continue
         sigma_interpolated[ct1, ct2] = interpolate_sigma(w_mesh, w_mesh_dmft, ct1, ct2)
 
     return sigma_interpolated, mu_dmft, freq_dict
 
 
 def sigma_FL(n_orb, orbital_order, Sigma_0, Sigma_Z, freq_dict, eta=0.0, mu_dmft=None):
 
@@ -477,15 +475,15 @@
     band_char = {}
     # contour for each sheet
     for sheet in range(tb.n_orbitals):
         contours[sheet] = skimage.measure.find_contours(E_FS[sheet, :, :], 0.0)
 
     sheet_ct = 0
     for sheet in contours.keys():
-        for sec_per_sheet in range(np.shape(contours[sheet])[0]):
+        for sec_per_sheet in range(len(contours[sheet])):
             # once on 2D cubic mesh
             FS_kx_ky[sheet_ct] = np.vstack([_fract_ind_to_val(kx, contours[sheet][sec_per_sheet][:, 0]),
                                             _fract_ind_to_val(ky, contours[sheet][sec_per_sheet][:, 1]),
                                             kz*np.ones(len(contours[sheet][sec_per_sheet][:, 0]))]).T.reshape(-1, 3)
             # repeat on actual mesh for computing the weights
             ks_skimage = contours[sheet][sec_per_sheet]/(N_kxy-1)
             FS_kx_ky_prim[sheet_ct] = (+ np.einsum('i,j->ij', ks_skimage[:, 0], lower_right)
@@ -503,15 +501,15 @@
 
     return FS_kx_ky, band_char
 
 
 def _setup_plot_bands(ax, special_k, k_points_labels, freq_dict):
 
     ax.axhline(y=0, c='gray', ls='--', lw=0.8, zorder=0)
-    ax.set_ylabel(r'$\omega - \mu$ (eV)')
+    ax.set_ylabel(r'$\epsilon - \mu$ (eV)')
 #     ax.set_ylim(*freq_dict['window'])
     for ik in special_k:
         ax.axvline(x=ik, linewidth=0.7, color='k', zorder=0.5)
     ax.set_xticks(special_k)
     ax.set_xlim(special_k[0], special_k[-1])
     k_points_labels = [r'$\Gamma$' if k == 'G' else k for k in k_points_labels]
     ax.set_xticklabels(k_points_labels)
@@ -545,16 +543,18 @@
             kw_x, kw_y = np.meshgrid(tb_data['k_mesh'], freq_dict['w_mesh'])
 
             vmax = plot_dict['vmax'] if 'vmax' in plot_dict else np.max(alatt_k_w)
             vmin = plot_dict['vmin'] if 'vmin' in plot_dict else 0.0
 
             graph = ax.pcolormesh(kw_x, kw_y, alatt_k_w.T, cmap=plot_dict['colorscheme_alatt'],
                                   norm=Normalize(vmin=vmin, vmax=vmax), shading='gouraud')
-            colorbar = plt.colorbar(graph)
-            colorbar.set_label(r'$A(k, \omega)$')
+
+            if 'colorbar' not in plot_dict or plot_dict['colorbar']:
+                colorbar = plt.colorbar(graph)
+                colorbar.set_label(r'$A(k, \omega)$')
 
     if tb:
         # if projection is requested, _get_tb_bands() ran already
         if proj_on_orb[0] is not None:
             eps_nuk = tb_data['e_mat']
             evec_nuk = tb_data['e_vecs']
         else:
@@ -585,15 +585,15 @@
     if not color:
         ax.plot(freq_dict['w_mesh'], np.sum(alatt_k_w, axis=0)/alatt_k_w.shape[0], label=label)
     else:
         ax.plot(freq_dict['w_mesh'], np.sum(alatt_k_w, axis=0) /
                 alatt_k_w.shape[0], label=label, color=color)
 
     ax.axvline(x=0, c='gray', ls='--', zorder=0)
-    ax.set_xlabel(r'$\omega - \mu$ (eV)')
+    ax.set_xlabel(r'$\epsilon - \mu$ (eV)')
     ax.set_ylabel(r'A($\omega$)')
 
     ax.set_xlim(*freq_dict['window'])
 
     return
 
 def plot_kslice(fig, ax, alatt_k_w, tb_data, freq_dict, n_orb, tb_dict, tb=True, alatt=False, quarter=0, **plot_dict):
@@ -625,16 +625,18 @@
                     ax.contour(qx * kx/(n_kx-1), qy * ky/(n_ky-1), alatt_k_w[:, :, orb].T,
                                colors=np.array([eval('cm.'+plot_dict['colorscheme_qpbands'])(0.7)]), levels=1, zorder=2)
             else:
                 graph = ax.pcolormesh(qx * kx/(n_kx-1), qy * ky/(n_ky-1), alatt_k_w.T,
                                       cmap=plot_dict['colorscheme_kslice'],
                                       norm=Normalize(vmin=vmin, vmax=vmax),
                                       shading='gouraud')
-                #colorbar = plt.colorbar(graph)
-                #colorbar.set_label(r'$A(k, 0$)')
+
+            if 'colorbar' not in plot_dict or plot_dict['colorbar']:
+                colorbar = plt.colorbar(graph)
+                colorbar.set_label(r'$A(k, 0$)')
 
     if tb:
         FS_kx_ky, band_char = get_tb_kslice(tb_data['tb'], tb_data['mu_tb'], **tb_dict)
         for sheet in FS_kx_ky.keys():
             for k_on_sheet in range(FS_kx_ky[sheet].shape[0]):
                 if not proj_on_orb[0] is not None:
                     if isinstance(plot_dict['colorscheme_bands'], str):
@@ -857,14 +859,15 @@
             delta_sigma, freq_dict = sigma_FL(n_orb, orbital_order_to, specs['Sigma_0'], specs['Sigma_Z'], specs['w_mesh'], eta=eta, mu_dmft=mu_dmft)
             mu = mu_tb + mu_shift
         # else is from dmft or memory:
         else:
             delta_sigma, mu_dmft, freq_dict = _sigma_from_dmft(n_orb, orbital_order_to, with_sigma, **specs)
             mu = mu_dmft + mu_shift
 
+        freq_dict['sigma_upfolded'] = delta_sigma
         if add_mu_tb:
             print('Adding mu_tb to DMFT μ; assuming DMFT was run with subtracted dft μ.')
             mu += mu_tb
 
         print('μ={:2.4f} eV set for calculating A(k,ω)'.format(mu))
 
         assert n_orb == delta_sigma.shape[0] and n_orb == delta_sigma.shape[
```

### Comparing `solid_dmft-3.2.1/python/solid_dmft/read_config.py` & `solid_dmft-3.2.2/python/solid_dmft/read_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,17 @@
             magnetic field
 h_field_it : int, optional, default=0
             number of iterations the magnetic field is kept on
 sigma_mix : float, optional, default=1.0
             careful: Sigma mixing can break orbital symmetries, use G0 mixing
             mixing sigma with previous iteration sigma for better convergency. 1.0 means no mixing
 g0_mix : float, optional, default=1.0
-            mixing the weiss field G0 with previous iteration G0 for better convergency. 1.0 means no mixing
+            Mixing the weiss field G0 with previous iteration G0 for better convergency. 1.0 means no mixing.
+            Setting g0_mix to 0.0 with linear mixing can be used for statistic sampling when
+            restarting a calculation
 g0_mix_type : string, optional, default='linear'
             which type of mixing is used. Possible values are:
             linear: linear mixing
             broyden: broyden mixing
 broy_max_it : int, optional, default=1
             maximum number of iteration to be considered for broyden mixing
             1 corresponds to simple linear mixing
@@ -275,17 +277,20 @@
             number of start matsubara frequency to start with
 fit_max_n : int, optional
             number of highest matsubara frequency to fit
 fit_min_w : float, optional
             start matsubara frequency to start with
 fit_max_w : float, optional
             highest matsubara frequency to fit
-random_seed : int, optional default by triqs
+random_seed : str, optional default by triqs
             if specified the int will be used for random seeds! Careful, this will give the same random
             numbers on all mpi ranks
+            You can also pass a string that will convert the keywords it or rank on runtime, e.g.
+            34788 * it + 928374 * rank will convert each iteration the variables it and rank for the random
+            seed
 legendre_fit : bool, optional default= False
             filter noise of G(tau) with G_l, cutoff is taken from n_l
 loc_n_min : int, optional
             Restrict local Hilbert space to states with at least this number of particles
 loc_n_max : int, optional
             Restrict local Hilbert space to states with at most this number of particles
 
@@ -545,19 +550,19 @@
                                  'h_field_it': {'converter': int, 'used': True, 'default': 0},
 
                                  'afm_order': {'converter': BOOL_PARSER,
                                                'used': lambda params: params['general']['magnetic'],
                                                'default': False},
 
                                  'sigma_mix': {'converter': float,
-                                               'valid for': lambda x, params: x > 0 and (np.isclose(params['general']['g0_mix'], 1)
+                                               'valid for': lambda x, params: x >= 0 and (np.isclose(params['general']['g0_mix'], 1)
                                                                                          or np.isclose(x, 1)),
                                                'used': True, 'default': 1.0},
 
-                                 'g0_mix': {'converter': float, 'valid for': lambda x, _: x > 0,
+                                 'g0_mix': {'converter': float, 'valid for': lambda x, _: x >= 0,
                                                'used': True, 'default': 1.0},
 
                                  'g0_mix_type': {'valid for': lambda x, _: x in ('linear', 'broyden'),
                                                 'used': True, 'default': 'linear'},
 
                                  'broy_max_it': {'converter': int, 'valid for': lambda x, _: x >= 1 or x==-1 ,
                                                 'used': lambda params: params['general']['g0_mix_type'] == 'broyden', 'default': -1},
@@ -727,15 +732,15 @@
 
                                 'measure_pert_order': {'converter': BOOL_PARSER, 'default': False,
                                                        'used': lambda params: params['general']['solver_type'] in ['cthyb', 'ctint', 'ctseg']},
 
                                 'move_shift': {'converter': BOOL_PARSER, 'default': False,
                                                 'used': lambda params: params['general']['solver_type'] in ['cthyb']},
 
-                                'random_seed': {'converter': int, 'default': None,
+                                'random_seed': {'converter': str, 'default': None,
                                                 'used': lambda params: params['general']['solver_type'] in ['cthyb', 'ctint', 'ctseg']},
 
                                 'perform_tail_fit': {'converter': BOOL_PARSER,
                                                      'used': lambda params: params['general']['solver_type'] in ['cthyb']
                                                              and not params['solver']['measure_G_l'],
                                                      'default': False},
```

### Comparing `solid_dmft-3.2.1/python/solid_dmft/util/__init__.py` & `solid_dmft-3.2.2/python/solid_dmft/util/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/util/symmetrize_gamma_file.py` & `solid_dmft-3.2.2/python/solid_dmft/util/symmetrize_gamma_file.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/util/update_dmft_config.py` & `solid_dmft-3.2.2/python/solid_dmft/util/update_dmft_config.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/util/update_results_h5.py` & `solid_dmft-3.2.2/python/solid_dmft/util/update_results_h5.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/util/write_kslice_to_h5.py` & `solid_dmft-3.2.2/python/solid_dmft/util/write_kslice_to_h5.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.1/python/solid_dmft/version.py` & `solid_dmft-3.2.2/python/solid_dmft/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 # You should have received a copy of the GNU General Public License along with
 # solid_dmft (in the file COPYING.txt in this directory). If not, see
 # <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 
-version = "3.2.1"
-triqs_hash = "90c8f8c257be434bc4560f4bbc518905c4d226ea"
-solid_dmft_hash = ""
+version = "3.2.2"
+triqs_hash = "8216931d15230ad4ffd4acba3db651046c040d99"
+solid_dmft_hash = "90f23ef5222ddd232855e5a8d3440b8008359e65"
 
 def show_version():
   print("\nYou are using solid_dmft version %s\n"%version)
 
 def show_git_hash():
-  print("\nYou are using solid_dmft git hash %s based on triqs git hash %s\n"%("", triqs_hash))
+  print("\nYou are using solid_dmft git hash %s based on triqs git hash %s\n"%("90f23ef5222ddd232855e5a8d3440b8008359e65", triqs_hash))
```

### Comparing `solid_dmft-3.2.1/python/solid_dmft.egg-info/PKG-INFO` & `solid_dmft-3.2.2/python/solid_dmft.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: solid-dmft
-Version: 3.2.1
+Name: solid_dmft
+Version: 3.2.2
 Summary: solid_dmft: a versatile python wrapper to perform DFT+DMFT calculations utilizing the TRIQS software library
 Author-email: Alexander Hampel <ahampel@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/solid_dmft
 Project-URL: Bug Tracker, https://github.com/triqs/solid_dmft/issues
 Project-URL: Paper, https://doi.org/10.21105/joss.04623
 Keywords: DMFT,DFT,triqs
 Classifier: Programming Language :: Python :: 3
@@ -13,16 +13,14 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: COPYING.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pytest
-Requires-Dist: scikit-image
-Requires-Dist: argparse
 
 ![logo_soliDMFT](https://raw.githubusercontent.com/triqs/solid_dmft/unstable/doc/logos/logo_solid_dmft.png)
 
 ![CI](https://github.com/triqs/solid_dmft/actions/workflows/build.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/solid_dmft.svg)](https://badge.fury.io/py/solid_dmft)
 [![status](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922/status.svg)](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922)
```

### Comparing `solid_dmft-3.2.1/python/solid_dmft.egg-info/SOURCES.txt` & `solid_dmft-3.2.2/python/solid_dmft.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 python/solid_dmft/dmft_tools/convergence.py
 python/solid_dmft/dmft_tools/formatter.py
 python/solid_dmft/dmft_tools/greens_functions_mixer.py
 python/solid_dmft/dmft_tools/initial_self_energies.py
 python/solid_dmft/dmft_tools/interaction_hamiltonian.py
 python/solid_dmft/dmft_tools/legendre_filter.py
 python/solid_dmft/dmft_tools/manipulate_chemical_potential.py
+python/solid_dmft/dmft_tools/matheval.py
 python/solid_dmft/dmft_tools/observables.py
 python/solid_dmft/dmft_tools/results_to_archive.py
 python/solid_dmft/dmft_tools/solver.py
 python/solid_dmft/postprocessing/__init__.py
 python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py
 python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py
 python/solid_dmft/postprocessing/maxent_gf_imp.py
```

