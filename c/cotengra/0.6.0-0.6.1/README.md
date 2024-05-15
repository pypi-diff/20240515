# Comparing `tmp/cotengra-0.6.0.tar.gz` & `tmp/cotengra-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cotengra-0.6.0.tar", last modified: Wed Apr 10 21:37:57 2024, max compression
+gzip compressed data, was "cotengra-0.6.1.tar", last modified: Wed May 15 21:37:34 2024, max compression
```

## Comparing `cotengra-0.6.0.tar` & `cotengra-0.6.1.tar`

### file list

```diff
@@ -1,126 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.783739 cotengra-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-10 21:37:46.000000 cotengra-0.6.0/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.743739 cotengra-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.747739 cotengra-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-10 21:37:46.000000 cotengra-0.6.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-10 21:37:46.000000 cotengra-0.6.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-10 21:37:46.000000 cotengra-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-10 21:37:46.000000 cotengra-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 21:37:46.000000 cotengra-0.6.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-10 21:37:46.000000 cotengra-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-10 21:37:46.000000 cotengra-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-10 21:37:57.783739 cotengra-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-10 21:37:46.000000 cotengra-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.743739 cotengra-0.6.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.747739 cotengra-0.6.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-10 21:37:46.000000 cotengra-0.6.0/ci/requirements/py-base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-10 21:37:46.000000 cotengra-0.6.0/ci/requirements/py-mac.yml
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-10 21:37:46.000000 cotengra-0.6.0/ci/requirements/py-no-oe.yml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-10 21:37:46.000000 cotengra-0.6.0/ci/requirements/py-win.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.751739 cotengra-0.6.0/cotengra/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 21:37:57.000000 cotengra-0.6.0/cotengra/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    28858 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)   132344 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.751739 cotengra-0.6.0/cotengra/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/experimental/path_compressed_branchbound.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/experimental/path_compressed_mcts.py
--rw-r--r--   0 runner    (1001) docker     (127)    28097 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/hypergraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.755739 cotengra-0.6.0/cotengra/hyperoptimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/hyperoptimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41240 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/hyperoptimizers/hyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/hyperoptimizers/hyper_baytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/hyperoptimizers/hyper_choco.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/hyperoptimizers/hyper_nevergrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/hyperoptimizers/hyper_optuna.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/hyperoptimizers/hyper_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/hyperoptimizers/hyper_skopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    33080 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/oe.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.755739 cotengra-0.6.0/cotengra/pathfinders/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.755739 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/cut_kKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/cut_rKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/km1_kKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/km1_rKaHyPar_sea20.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.759739 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/old/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/old/cut_kKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/old/cut_rKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/old/km1_kKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/old/km1_rKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)    35878 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/path_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12996 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/path_compressed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/path_flowcutter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/path_greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/path_igraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/path_kahypar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/path_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/path_quickbb.py
--rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/path_simulated_annealing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/pathfinders/treedecomp.py
--rw-r--r--   0 runner    (1001) docker     (127)    51499 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    48584 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/schematic.py
--rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    14666 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)    41181 2024-04-10 21:37:46.000000 cotengra-0.6.0/cotengra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.779739 cotengra-0.6.0/cotengra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-10 21:37:57.000000 cotengra-0.6.0/cotengra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-10 21:37:57.000000 cotengra-0.6.0/cotengra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:37:57.000000 cotengra-0.6.0/cotengra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 21:37:57.000000 cotengra-0.6.0/cotengra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 21:37:57.000000 cotengra-0.6.0/cotengra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.759739 cotengra-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.763739 cotengra-0.6.0/docs/_pygments/
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/_pygments/_pygments_dark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/_pygments/_pygments_light.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.763739 cotengra-0.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/_static/logo-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    22713 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/_static/logo-full.png
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/_static/my-styles.css
--rw-r--r--   0 runner    (1001) docker     (127)    18274 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    77146 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)   596952 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/contraction.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.767739 cotengra-0.6.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)  2748603 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/examples/ex_compressed_contraction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   871844 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/examples/ex_large_output_lazy.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   318454 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/high-level-interface.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/index_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)   324466 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/trees.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1311527 2024-04-10 21:37:46.000000 cotengra-0.6.0/docs/visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.779739 cotengra-0.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)  1627407 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/Example - Reproducing 2005.06787.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1635278 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/Example - Reproducing 2103-03074.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1892297 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/Quantum Circuit Example Old.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1598303 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/Quantum Circuit Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    42045 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/circuit_n53_m10_s0_e0_pABCDCDAB.qsim
--rw-r--r--   0 runner    (1001) docker     (127)    50412 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/circuit_n53_m12_s0_e0_pABCDCDAB.qsim
--rw-r--r--   0 runner    (1001) docker     (127)    83874 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/circuit_n53_m20_s0_e0_pABCDCDAB.qsim
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/ex_jax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/ex_mpi_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-10 21:37:46.000000 cotengra-0.6.0/examples/ex_mpi_spmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-10 21:37:46.000000 cotengra-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:37:57.783739 cotengra-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-10 21:37:46.000000 cotengra-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.779739 cotengra-0.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)    28953 2024-04-10 21:37:46.000000 cotengra-0.6.0/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:57.779739 cotengra-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:37:46.000000 cotengra-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-10 21:37:46.000000 cotengra-0.6.0/tests/test_compressed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-10 21:37:46.000000 cotengra-0.6.0/tests/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-10 21:37:46.000000 cotengra-0.6.0/tests/test_hypergraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-10 21:37:46.000000 cotengra-0.6.0/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-04-10 21:37:46.000000 cotengra-0.6.0/tests/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-10 21:37:46.000000 cotengra-0.6.0/tests/test_paths_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 21:37:46.000000 cotengra-0.6.0/tests/test_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-10 21:37:46.000000 cotengra-0.6.0/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.467719 cotengra-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-15 21:37:22.000000 cotengra-0.6.1/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.427719 cotengra-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.431719 cotengra-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-15 21:37:22.000000 cotengra-0.6.1/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 21:37:22.000000 cotengra-0.6.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-15 21:37:22.000000 cotengra-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 21:37:22.000000 cotengra-0.6.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 21:37:22.000000 cotengra-0.6.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-15 21:37:22.000000 cotengra-0.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 21:37:22.000000 cotengra-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-15 21:37:34.467719 cotengra-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-15 21:37:22.000000 cotengra-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.427719 cotengra-0.6.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.435719 cotengra-0.6.1/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 21:37:22.000000 cotengra-0.6.1/ci/requirements/py-base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 21:37:22.000000 cotengra-0.6.1/ci/requirements/py-mac.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-15 21:37:22.000000 cotengra-0.6.1/ci/requirements/py-no-oe.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 21:37:22.000000 cotengra-0.6.1/ci/requirements/py-win.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.435719 cotengra-0.6.1/cotengra/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28858 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132859 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/core_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.439719 cotengra-0.6.1/cotengra/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/experimental/path_compressed_branchbound.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/experimental/path_compressed_mcts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28097 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hypergraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.439719 cotengra-0.6.1/cotengra/hyperoptimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41260 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_baytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_choco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_nevergrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_skopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33562 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/oe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.439719 cotengra-0.6.1/cotengra/pathfinders/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.443719 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/cut_kKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/cut_rKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/km1_kKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/km1_rKaHyPar_sea20.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.443719 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/cut_kKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/cut_rKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/km1_kKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/km1_rKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    48385 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12996 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_compressed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_compressed_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_flowcutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_igraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_kahypar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_quickbb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_simulated_annealing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/treedecomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51499 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48584 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/schematic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28660 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.463719 cotengra-0.6.1/cotengra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.447719 cotengra-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.447719 cotengra-0.6.1/docs/_pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_pygments/_pygments_dark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_pygments/_pygments_light.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.447719 cotengra-0.6.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_static/logo-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    22713 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_static/logo-full.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_static/my-styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    77146 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   596952 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/contraction.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.451719 cotengra-0.6.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)  2748603 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/examples/ex_compressed_contraction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   871844 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/examples/ex_large_output_lazy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   318454 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/high-level-interface.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/index_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)   324466 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/trees.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1311527 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.463719 cotengra-0.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)  1627407 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/Example - Reproducing 2005.06787.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1635278 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/Example - Reproducing 2103-03074.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1892297 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/Quantum Circuit Example Old.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1598303 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/Quantum Circuit Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    42045 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/circuit_n53_m10_s0_e0_pABCDCDAB.qsim
+-rw-r--r--   0 runner    (1001) docker     (127)    50412 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/circuit_n53_m12_s0_e0_pABCDCDAB.qsim
+-rw-r--r--   0 runner    (1001) docker     (127)    83874 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/circuit_n53_m20_s0_e0_pABCDCDAB.qsim
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/ex_jax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/ex_mpi_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/ex_mpi_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-15 21:37:22.000000 cotengra-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:37:34.467719 cotengra-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-15 21:37:22.000000 cotengra-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.463719 cotengra-0.6.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    28953 2024-05-15 21:37:22.000000 cotengra-0.6.1/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.463719 cotengra-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_compressed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_hypergraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_paths_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_tree.py
```

### Comparing `cotengra-0.6.0/.github/workflows/pypi-release.yml` & `cotengra-0.6.1/.github/workflows/pypi-release.yml`

 * *Files 17% similar despite different names*

```diff
@@ -8,85 +8,108 @@
       - 'v*'
 
 jobs:
   build-artifacts:
     runs-on: ubuntu-latest
     if: github.repository == 'jcmgray/cotengra'
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
-          python-version: 3.8
+          python-version: "3.12"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install build twine
+
       - name: Build tarball and wheels
         run: |
           git clean -xdf
           git restore -SW .
           python -m build
+
       - name: Check built artifacts
         run: |
           python -m twine check --strict dist/*
           pwd
           if [ -f dist/cotengra-0.0.0.tar.gz ]; then
             echo "❌ INVALID VERSION NUMBER"
             exit 1
           else
             echo "✅ Looks good"
           fi
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: releases
           path: dist
 
   test-built-dist:
     needs: build-artifacts
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
-          python-version: 3.8
-      - uses: actions/download-artifact@v3
+          python-version: "3.12"
+      - uses: actions/download-artifact@v4
         with:
           name: releases
           path: dist
       - name: List contents of built dist
         run: |
           ls -ltrh
           ls -ltrh dist
+
       - name: Verify the built dist/wheel is valid
         if: github.event_name == 'push'
         run: |
           python -m pip install --upgrade pip
           python -m pip install dist/cotengra*.whl
+
+  upload-to-test-pypi:
+    needs: test-built-dist
+    if: github.event_name == 'push'
+    runs-on: ubuntu-latest
+
+    environment:
+      name: pypi
+      url: https://test.pypi.org/p/cotengra
+    permissions:
+      id-token: write
+
+    steps:
+      - uses: actions/download-artifact@v4
+        with:
+          name: releases
+          path: dist
       - name: Publish package to TestPyPI
         if: github.event_name == 'push'
-        uses: pypa/gh-action-pypi-publish@release/v1
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
-          user: __token__
-          password: ${{ secrets.TESTPYPI_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
           verbose: true
 
 
   upload-to-pypi:
     needs: test-built-dist
     if: github.event_name == 'release'
     runs-on: ubuntu-latest
+
+    environment:
+      name: pypi
+      url: https://pypi.org/p/cotengra
+    permissions:
+      id-token: write
+
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: releases
           path: dist
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
-          user: __token__
-          password: ${{ secrets.PYPI_TOKEN }}
-          verbose: true
+          verbose: true
```

### Comparing `cotengra-0.6.0/.github/workflows/test.yml` & `cotengra-0.6.1/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -40,8 +40,10 @@
           python=${{ matrix.python-version }}
         cache-environment: true
 
     - name: Test with pytest
       run: pytest --cov=cotengra tests/ --cov-report=xml tests
 
     - name: Report to codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `cotengra-0.6.0/.gitignore` & `cotengra-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/LICENSE.md` & `cotengra-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/PKG-INFO` & `cotengra-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: cotengra
-Version: 0.6.0
+Version: 0.6.1
 Summary: Hyper optimized contraction trees for large tensor networks and einsums.
 Home-page: https://github.com/jcmgray/cotengra
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/cotengra/issues
 Project-URL: Source, https://github.com/jcmgray/cotengra/
 Keywords: tensor network contraction graph hypergraph partition einsum
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: autoray
 Provides-Extra: recommended
-Requires-Dist: cotengrust; extra == "recommended"
+Requires-Dist: cotengrust>=0.1.3; extra == "recommended"
 Requires-Dist: cytoolz; extra == "recommended"
 Requires-Dist: kahypar; extra == "recommended"
 Requires-Dist: networkx; extra == "recommended"
 Requires-Dist: numpy; extra == "recommended"
 Requires-Dist: opt_einsum; extra == "recommended"
 Requires-Dist: optuna; extra == "recommended"
 Requires-Dist: ray; extra == "recommended"
```

### Comparing `cotengra-0.6.0/README.md` & `cotengra-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/__init__.py` & `cotengra-0.6.1/cotengra/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-"""Hyper optimized contraction trees for large tensor networks and einsums.
-"""
+"""Hyper optimized contraction trees for large tensor networks and einsums."""
+
 try:
     # -- Distribution mode --
     # import from _version.py generated by setuptools_scm during release
     from ._version import version as __version__
 except ImportError:
     # -- Source mode --
     try:
         # use setuptools_scm to get the current version from src using git
-        from setuptools_scm import get_version as _gv
         from pathlib import Path as _Path
 
+        from setuptools_scm import get_version as _gv
+
         __version__ = _gv(_Path(__file__).parent.parent)
     except ImportError:
         # setuptools_scm is not available, use a default version
         __version__ = "0.0.0+unknown"
 
 import functools
 
 from . import utils
 from .core import (
     ContractionTree,
     ContractionTreeCompressed,
+)
+from .core_multi import (
     ContractionTreeMulti,
 )
 from .hypergraph import (
     HyperGraph,
     get_hypergraph,
 )
 from .hyperoptimizers import (
@@ -54,22 +57,23 @@
     einsum,
     einsum_expression,
     einsum_tree,
     register_preset,
 )
 from .pathfinders import (
     path_basic,
-    path_greedy,
+    path_compressed_greedy,
     path_igraph,
     path_kahypar,
     path_labels,
 )
 from .pathfinders.path_basic import (
     GreedyOptimizer,
     OptimalOptimizer,
+    RandomGreedyOptimizer,
 )
 from .pathfinders.path_flowcutter import (
     FlowCutterOptimizer,
     optimize_flowcutter,
 )
 from .pathfinders.path_quickbb import QuickBBOptimizer, optimize_quickbb
 from .plot import (
@@ -159,15 +163,15 @@
     "list_hyper_functions",
     "optimal_optimize",
     "optimal_outer_optimize",
     "OptimalOptimizer",
     "optimize_flowcutter",
     "optimize_quickbb",
     "path_basic",
-    "path_greedy",
+    "path_compressed_greedy",
     "path_igraph",
     "path_kahypar",
     "path_labels",
     "plot_contractions_alt",
     "plot_contractions",
     "plot_scatter_alt",
     "plot_scatter",
@@ -177,14 +181,15 @@
     "plot_tree_span",
     "plot_tree_tent",
     "plot_tree",
     "plot_trials_alt",
     "plot_trials",
     "QuasiRandOptimizer",
     "QuickBBOptimizer",
+    "RandomGreedyOptimizer",
     "register_preset",
     "ReusableHyperCompressedOptimizer",
     "ReusableHyperOptimizer",
     "SliceFinder",
     "UniformOptimizer",
     "utils",
 )
@@ -194,14 +199,21 @@
 
 
 def hyper_optimize(inputs, output, size_dict, memory_limit=None, **opts):
     optimizer = HyperOptimizer(**opts)
     return optimizer(inputs, output, size_dict, memory_limit)
 
 
+def random_greedy_optimize(
+    inputs, output, size_dict, memory_limit=None, **opts
+):
+    optimizer = RandomGreedyOptimizer(**opts)
+    return optimizer(inputs, output, size_dict)
+
+
 try:
     register_preset(
         "hyper",
         hyper_optimize,
     )
     register_preset(
         "hyper-256",
@@ -239,14 +251,22 @@
         functools.partial(hyper_optimize, methods=["spinglass"]),
     )
     register_preset(
         "hyper-betweenness",
         functools.partial(hyper_optimize, methods=["betweenness"]),
     )
     register_preset(
+        "random-greedy",
+        random_greedy_optimize,
+    )
+    register_preset(
+        "random-greedy-128",
+        functools.partial(random_greedy_optimize, max_repeats=128),
+    )
+    register_preset(
         "flowcutter-2",
         functools.partial(optimize_flowcutter, max_time=2),
     )
     register_preset(
         "flowcutter-10",
         functools.partial(optimize_flowcutter, max_time=10),
     )
@@ -264,18 +284,18 @@
     )
     register_preset(
         "quickbb-60",
         functools.partial(optimize_quickbb, max_time=60),
     )
     register_preset(
         "greedy-compressed",
-        path_greedy.greedy_compressed,
+        path_compressed_greedy.greedy_compressed,
         compressed=True,
     )
     register_preset(
         "greedy-span",
-        path_greedy.greedy_span,
+        path_compressed_greedy.greedy_span,
         compressed=True,
     )
 except KeyError:
     # KeyError: if reloading cotengra e.g. library entries already registered
     pass
```

### Comparing `cotengra-0.6.0/cotengra/contract.py` & `cotengra-0.6.1/cotengra/contract.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/core.py` & `cotengra-0.6.1/cotengra/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -871,15 +871,15 @@
     def get_centrality(self, node):
         try:
             return self.info[node]["centrality"]
         except KeyError:
             self.compute_centralities()
             return self.info[node]["centrality"]
 
-    def total_flops(self, dtype=None):
+    def total_flops(self, dtype=None, log=None):
         """Sum the flops contribution from every node in the tree.
 
         Parameters
         ----------
         dtype : {'float', 'complex', None}, optional
             Scale the answer depending on the assumed data type.
         """
@@ -891,47 +891,54 @@
             for node, _, _ in self.traverse():
                 self._flops += self.get_flops(node)
 
             self._track_flops = True
             C = self.multiplicity * self._flops
 
         if dtype is None:
-            return C
+            pass
+        elif "float" in dtype:
+            C *= 2
+        elif "complex" in dtype:
+            C *= 4
+        else:
+            raise ValueError(f"Unknown dtype {dtype}")
 
-        if "float" in dtype:
-            return 2 * C
+        if log is not None:
+            C = math.log(C, log)
 
-        if "complex" in dtype:
-            return 8 * C
+        return C
 
     def total_write(self):
         """Sum the total amount of memory that will be created and operated on."""
         if not self._track_write:
             self._write = 0
             for node, _, _ in self.traverse():
                 self._write += self.get_size(node)
 
             self._track_write = True
 
         return self.multiplicity * self._write
 
-    def total_cost(self, factor=DEFAULT_COMBO_FACTOR, combine=sum, log=None):
+    def combo_cost(self, factor=DEFAULT_COMBO_FACTOR, combine=sum, log=None):
         t = 0
         for p in self.children:
             f = self.get_flops(p)
             w = self.get_size(p)
             t += combine((f, factor * w))
 
         t *= self.multiplicity
 
         if log is not None:
             t = math.log(t, log)
 
         return t
 
+    total_cost = combo_cost
+
     def max_size(self, log=None):
         """The size of the largest intermediate tensor."""
         if self.N == 1:
             return self.get_size(self.root)
 
         if not self._track_size:
             self._sizes = MaxCounter()
@@ -1007,18 +1014,15 @@
         in any single contraction, which will match the scaling assuming that
         all dimensions are equal.
         """
         return max(len(self.get_involved(node)) for node in self.info)
 
     def contraction_cost(self, log=None):
         """Get the total number of scalar operations ~ time complexity."""
-        C = float(self.total_flops(dtype=None))
-        if log is not None:
-            C = math.log(C, log)
-        return C
+        return self.total_flops(dtype=None, log=log)
 
     def contraction_width(self, log=2):
         """Get log2 of the size of the largest tensor."""
         return self.max_size(log=log)
 
     def compressed_contract_stats(
         self,
@@ -1068,50 +1072,64 @@
 
     def total_flops_compressed(
         self,
         chi=None,
         order="surface_order",
         compress_late=None,
         dtype=None,
+        log=None,
     ):
         """Estimate the total flops for a compressed contraction of this tree
         with maximum bond size ``chi``. This includes basic estimates of the
         ops to perform contractions, QRs and SVDs.
         """
         if dtype is not None:
             raise ValueError(
                 "Can only estimate cost in terms of "
                 "number of abstract scalar ops."
             )
 
-        return self.compressed_contract_stats(
+        F = self.compressed_contract_stats(
             chi=chi,
             order=order,
             compress_late=compress_late,
         ).flops
 
+        if log is not None:
+            F = math.log(F, log)
+
+        return F
+
+    contraction_cost_compressed = total_flops_compressed
+
     def total_write_compressed(
         self,
         chi=None,
         order="surface_order",
         compress_late=None,
         accel="auto",
+        log=None,
     ):
         """Compute the total size of all intermediate tensors when a
         compressed contraction is performed with maximum bond size ``chi``,
         ordered by ``order``. This is relevant maybe for time complexity and
         e.g. autodiff space complexity (since every intermediate is kept).
         """
-        return self.compressed_contract_stats(
+        W = self.compressed_contract_stats(
             chi=chi,
             order=order,
             compress_late=compress_late,
         ).write
 
-    def total_cost_compressed(
+        if log is not None:
+            W = math.log(W, log)
+
+        return W
+
+    def combo_cost_compressed(
         self,
         chi=None,
         order="surface_order",
         compress_late=None,
         factor=None,
         log=None,
     ):
@@ -1119,33 +1137,39 @@
             factor = self.get_default_combo_factor()
 
         C = self.total_flops_compressed(
             chi=chi, order=order, compress_late=compress_late
         ) + factor * self.total_write_compressed(
             chi=chi, order=order, compress_late=compress_late
         )
+
         if log is not None:
             C = math.log(C, log)
+
         return C
 
+    total_cost_compressed = combo_cost_compressed
+
     def max_size_compressed(
         self, chi=None, order="surface_order", compress_late=None, log=None
     ):
         """Compute the maximum sized tensor produced when a compressed
         contraction is performed with maximum bond size ``chi``, ordered by
         ``order``. This is close to the ideal space complexity if only
         tensors that are being directly operated on are kept in memory.
         """
         S = self.compressed_contract_stats(
             chi=chi,
             order=order,
             compress_late=compress_late,
         ).max_size
+
         if log is not None:
             S = math.log(S, log)
+
         return S
 
     def peak_size_compressed(
         self,
         chi=None,
         order="surface_order",
         compress_late=None,
@@ -1158,29 +1182,37 @@
         not swapping intermediates in and out of memory.
         """
         P = self.compressed_contract_stats(
             chi=chi,
             order=order,
             compress_late=compress_late,
         ).peak_size
+
         if log is not None:
             P = math.log(P, log)
-        return P
 
-    contraction_cost_compressed = total_cost_compressed
+        return P
 
     def contraction_width_compressed(
         self, chi=None, order="surface_order", compress_late=None, log=2
     ):
         """Compute log2 of the maximum sized tensor produced when a compressed
         contraction is performed with maximum bond size ``chi``, ordered by
         ``order``.
         """
         return self.max_size_compressed(chi, order, compress_late, log=log)
 
+    def _update_tracked(self, node):
+        if self._track_flops:
+            self._flops += self.get_flops(node)
+        if self._track_write:
+            self._write += self.get_size(node)
+        if self._track_size:
+            self._sizes.add(self.get_size(node))
+
     def contract_nodes_pair(
         self,
         x,
         y,
         legs=None,
         cost=None,
         size=None,
@@ -1246,20 +1278,15 @@
         if legs is not None:
             self.info[parent]["legs"] = legs
         if cost is not None:
             self.info[parent]["flops"] = cost
         if size is not None:
             self.info[parent]["size"] = size
 
-        if self._track_flops:
-            self._flops += self.get_flops(parent)
-        if self._track_write:
-            self._write += self.get_size(parent)
-        if self._track_size:
-            self._sizes.add(self.get_size(parent))
+        self._update_tracked(parent)
 
         return parent
 
     def contract_nodes(
         self,
         nodes,
         optimize="auto-hq",
@@ -2494,14 +2521,15 @@
         ssa_path = opt.ssa_path
         # ssa_path = opt(self.inputs, self.output, self.size_dict)
         rtree = self.__class__.from_path(
             self.inputs,
             self.output,
             self.size_dict,
             ssa_path=ssa_path,
+            objective=minimize,
         )
         if inplace:
             self.set_state_from(rtree)
             rtree = self
         rtree.set_surface_order_from_path(ssa_path)
         rtree.contraction_cores.clear()
         return rtree
@@ -3515,43 +3543,43 @@
     @functools.wraps(plot_hypergraph)
     def plot_hypergraph(self, **kwargs):
         hg = self.get_hypergraph(accel=False)
         hg.plot(**kwargs)
 
     def describe(self, info="normal", join=" "):
         """Return a string describing the contraction tree."""
-        stats = self.contract_stats()
+        self.contract_stats()
         if info == "normal":
             return join.join(
                 (
-                    f"log10[FLOPs]={math.log10(stats['flops']):.4g}",
-                    f"log2[SIZE]={math.log2(stats['size']):.4g}",
+                    f"log10[FLOPs]={self.total_flops(log=10):.2f}",
+                    f"log2[SIZE]={self.max_size(log=2):.2f}",
                 )
             )
 
         elif info == "full":
             s = [
-                f"log10[FLOPS]={self.contraction_cost(log=10):.4g}",
-                f"log10[COMBO]={self.total_cost(log=10):.4g}",
-                f"log2[SIZE]={self.contraction_width(log=2):.4g}",
-                f"log2[PEAK]={self.peak_size(log=2):.4g}",
+                f"log10[FLOPS]={self.total_flops(log=10):.2f}",
+                f"log10[COMBO]={self.combo_cost(log=10):.2f}",
+                f"log2[SIZE]={self.max_size(log=2):.2f}",
+                f"log2[PEAK]={self.peak_size(log=2):.2f}",
             ]
             if self.sliced_inds:
-                s.append(f"NSLICES={self.multiplicity:.4g}")
+                s.append(f"NSLICES={self.multiplicity:.2f}")
             return join.join(s)
 
         elif info == "concise":
             s = [
-                f"F={self.contraction_cost(log=10):.4g}",
-                f"C={self.total_cost(log=10):.4g}",
-                f"S={self.contraction_width(log=2):.4g}",
-                f"P={self.peak_size(log=2):.4g}",
+                f"F={self.total_flops(log=10):.2f}",
+                f"C={self.combo_cost(log=10):.2f}",
+                f"S={self.max_size(log=2):.2f}",
+                f"P={self.peak_size(log=2):.2f}",
             ]
             if self.sliced_inds:
-                s.append(f"$={self.multiplicity:.4g}")
+                s.append(f"$={self.multiplicity:.2f}")
             return join.join(s)
 
     def __repr__(self):
         if self.is_complete():
             return f"<{self.__class__.__name__}(N={self.N})>"
         else:
             s = "<{}(N={}, branches={}, complete={})>"
@@ -3643,35 +3671,37 @@
         objective = self.get_default_objective()
         try:
             chi = objective.chi
         except AttributeError:
             chi = "auto"
 
         if chi == "auto":
-            chi = max(self.size_dict.values())**2
+            chi = max(self.size_dict.values()) ** 2
 
         return chi
 
     def get_default_compress_late(self):
         objective = self.get_default_objective()
         try:
             return objective.compress_late
         except AttributeError:
             return False
 
     total_flops = ContractionTree.total_flops_compressed
     total_write = ContractionTree.total_write_compressed
+    combo_cost = ContractionTree.combo_cost_compressed
     total_cost = ContractionTree.total_cost_compressed
     max_size = ContractionTree.max_size_compressed
     peak_size = ContractionTree.peak_size_compressed
     contraction_cost = ContractionTree.contraction_cost_compressed
     contraction_width = ContractionTree.contraction_width_compressed
 
     total_flops_exact = ContractionTree.total_flops
     total_write_exact = ContractionTree.total_write
+    combo_cost_exact = ContractionTree.combo_cost
     total_cost_exact = ContractionTree.total_cost
     max_size_exact = ContractionTree.max_size
     peak_size_exact = ContractionTree.peak_size
 
     def get_contractor(self, *_, **__):
         raise NotImplementedError(
             "`cotengra` doesn't implement compressed contraction itself. "
```

### Comparing `cotengra-0.6.0/cotengra/experimental/path_compressed_branchbound.py` & `cotengra-0.6.1/cotengra/experimental/path_compressed_branchbound.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/experimental/path_compressed_mcts.py` & `cotengra-0.6.1/cotengra/experimental/path_compressed_mcts.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/hypergraph.py` & `cotengra-0.6.1/cotengra/hypergraph.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/hyperoptimizers/hyper.py` & `cotengra-0.6.1/cotengra/hyperoptimizers/hyper.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import time
 import warnings
 from math import log2, log10
 
 from ..core import (
     ContractionTree,
     ContractionTreeCompressed,
-    ContractionTreeMulti,
 )
+from ..core_multi import ContractionTreeMulti
 from ..oe import PathOptimizer
 from ..parallel import get_n_workers, parse_parallel_arg, should_nest, submit
 from ..plot import plot_scatter, plot_scatter_alt, plot_trials, plot_trials_alt
 from ..scoring import get_score_fn
 from ..utils import BadTrial, DiskDict, get_rng
 
 
@@ -322,16 +322,16 @@
 
 
 def progress_description(best, info="concise"):
     try:
         return best["tree"].describe(info=info)
     except KeyError:
         return (
-            f"log10[FLOPs]={log10(best['flops']):.4g} "
-            f"log2[SIZE]={log2(best['size']):.4g}"
+            f"log10[FLOPs]={log10(best['flops']):.2f} "
+            f"log2[SIZE]={log2(best['size']):.2f}"
         )
 
 
 class HyperOptimizer(PathOptimizer):
     """A path optimizer that samples a series of contraction trees
     while optimizing the hyper parameters used to generate them.
```

### Comparing `cotengra-0.6.0/cotengra/hyperoptimizers/hyper_baytune.py` & `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_baytune.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/hyperoptimizers/hyper_choco.py` & `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_choco.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/hyperoptimizers/hyper_nevergrad.py` & `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_nevergrad.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/hyperoptimizers/hyper_optuna.py` & `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_optuna.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/hyperoptimizers/hyper_random.py` & `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_random.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/hyperoptimizers/hyper_skopt.py` & `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_skopt.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/interface.py` & `cotengra-0.6.1/cotengra/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,17 +535,26 @@
         term = tuple(inputs[0])
         output = tuple(output)
 
         if term == output:
             # 'contraction' is a no-op
 
             def fn(*arrays, backend=None):
+                # this is surprisingly complicated 'to do nothing', since we
+                # have to respect potential backend conversion
+                x = arrays[0]
                 if backend is None:
-                    return arrays[0]
-                return ar.do("array", arrays[0], like=backend)
+                    # haven't requested a specific backend, just return
+                    return x
+                elif backend == ar.infer_backend(x):
+                    # requested backend is the same as the input, just return
+                    return x
+                else:
+                    # requested backend is different, convert
+                    return ar.do("array", arrays[0], like=backend)
 
         elif len(term) == len(output):
             # 'contraction' is just a transposition
             perm = tuple(map(term.index, output))
 
             def fn(*arrays, backend=None):
                 return ar.do("transpose", arrays[0], perm, like=backend)
```

### Comparing `cotengra-0.6.0/cotengra/oe.py` & `cotengra-0.6.1/cotengra/oe.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/parallel.py` & `cotengra-0.6.1/cotengra/parallel.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,32 +9,51 @@
 import collections
 
 
 _AUTO_BACKEND = None
 _DEFAULT_BACKEND = "concurrent.futures"
 
 
+@functools.lru_cache(None)
+def choose_default_num_workers():
+    import os
+
+    if "COTENGRA_NUM_WORKERS" in os.environ:
+        return int(os.environ["COTENGRA_NUM_WORKERS"])
+
+    if "OMP_NUM_THREADS" in os.environ:
+        return int(os.environ["OMP_NUM_THREADS"])
+
+    return os.cpu_count()
+
+
 def get_pool(n_workers=None, maybe_create=False, backend=None):
     """Get a parallel pool."""
-
     if backend is None:
         backend = _DEFAULT_BACKEND
 
+    if backend == "dask":
+        return _get_pool_dask(n_workers=n_workers, maybe_create=maybe_create)
+
+    if backend == "ray":
+        return _get_pool_ray(n_workers=n_workers, maybe_create=maybe_create)
+
+    # above backends are distributed, don't specify n_workers
+    if n_workers is None:
+        n_workers = choose_default_num_workers()
+
     if backend == "loky":
         get_reusable_executor = get_loky_get_reusable_executor()
         return get_reusable_executor(max_workers=n_workers)
 
     if backend == "concurrent.futures":
-        return _get_pool_cf(n_workers=n_workers)
-
-    if backend == "dask":
-        return _get_pool_dask(n_workers=n_workers, maybe_create=maybe_create)
+        return _get_process_pool_cf(n_workers=n_workers)
 
-    if backend == "ray":
-        return _get_pool_ray(n_workers=n_workers, maybe_create=maybe_create)
+    if backend == "threads":
+        return _get_thread_pool_cf(n_workers=n_workers)
 
 
 @functools.lru_cache(None)
 def _infer_backed_cached(pool_class):
     if pool_class.__name__ == "RayExecutor":
         return "ray"
 
@@ -114,14 +133,17 @@
 
     if parallel == "loky":
         return get_pool(maybe_create=True, backend="loky")
 
     if parallel == "concurrent.futures":
         return get_pool(maybe_create=True, backend="concurrent.futures")
 
+    if parallel == "threads":
+        return get_pool(maybe_create=True, backend="threads")
+
     if parallel == "dask":
         _AUTO_BACKEND = "dask"
         return get_pool(maybe_create=True, backend="dask")
 
     if parallel == "ray":
         _AUTO_BACKEND = "ray"
         return get_pool(maybe_create=True, backend="ray")
@@ -215,24 +237,62 @@
             self._pool.shutdown()
             self._pool = None
 
     def __del__(self):
         self.shutdown()
 
 
-PoolHandler = CachedProcessPoolExecutor()
+ProcessPoolHandler = CachedProcessPoolExecutor()
 
 
 @atexit.register
 def _shutdown_cached_process_pool():
-    PoolHandler.shutdown()
+    ProcessPoolHandler.shutdown()
+
+
+def _get_process_pool_cf(n_workers=None):
+    return ProcessPoolHandler(n_workers)
+
+
+class CachedThreadPoolExecutor:
+    def __init__(self):
+        self._pool = None
+        self._n_workers = -1
+
+    def __call__(self, n_workers=None):
+        if n_workers != self._n_workers:
+            from concurrent.futures import ThreadPoolExecutor
+
+            self.shutdown()
+            self._pool = ThreadPoolExecutor(n_workers)
+            self._n_workers = n_workers
+        return self._pool
+
+    def is_initialized(self):
+        return self._pool is not None
+
+    def shutdown(self):
+        if self._pool is not None:
+            self._pool.shutdown()
+            self._pool = None
+
+    def __del__(self):
+        self.shutdown()
+
+
+ThreadPoolHandler = CachedThreadPoolExecutor()
+
+
+@atexit.register
+def _shutdown_cached_thread_pool():
+    ThreadPoolHandler.shutdown()
 
 
-def _get_pool_cf(n_workers=None):
-    return PoolHandler(n_workers)
+def _get_thread_pool_cf(n_workers=None):
+    return ThreadPoolHandler(n_workers)
 
 
 # ---------------------------------- DASK ----------------------------------- #
 
 
 def _get_pool_dask(n_workers=None, maybe_create=False):
     """Maybe get an existing or create a new dask.distrbuted client.
```

### Comparing `cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/cut_kKaHyPar_sea20.ini` & `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/cut_kKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/cut_rKaHyPar_sea20.ini` & `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/cut_rKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/km1_kKaHyPar_sea20.ini` & `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/km1_kKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/km1_rKaHyPar_sea20.ini` & `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/km1_rKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/old/cut_kKaHyPar_sea20.ini` & `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/cut_kKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/old/cut_rKaHyPar_sea20.ini` & `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/cut_rKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/old/km1_kKaHyPar_sea20.ini` & `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/km1_kKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/kahypar_profiles/old/km1_rKaHyPar_sea20.ini` & `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/km1_rKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/path_basic.py` & `cotengra-0.6.1/cotengra/pathfinders/path_basic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-"""Basic optimization routines.
-"""
+"""Basic optimization routines."""
+
 import math
 import heapq
 import bisect
 import functools
 import itertools
 
 from ..oe import PathOptimizer
-from ..utils import GumbelBatchedGenerator
+from ..utils import get_rng, GumbelBatchedGenerator
+from ..parallel import parse_parallel_arg, get_n_workers
+
 
 def is_simplifiable(legs, appearances):
     """Check if ``legs`` contains any diag (repeated) or reduced (appears
     nowhere else) indices.
     """
     prev_ix = None
     for ix, ix_cnt in legs:
@@ -92,14 +94,27 @@
     """Compute the size of a term."""
     size = 1
     for ix, _ in legs:
         size *= sizes[ix]
     return size
 
 
+def compute_flops(ilegs, jlegs, sizes):
+    """Compute the flops cost of contracting two terms."""
+    seen = set()
+    flops = 1
+    for ix, _ in ilegs:
+        seen.add(ix)
+        flops *= sizes[ix]
+    for ix, _ in jlegs:
+        if ix not in seen:
+            flops *= sizes[ix]
+    return flops
+
+
 def compute_con_cost_flops(
     temp_legs,
     appearances,
     sizes,
     iscore,
     jscore,
 ):
@@ -268,15 +283,35 @@
 
 
 class ContractionProcessor:
     """A helper class for combining bottom up simplifications, greedy, and
     optimal contraction path optimization.
     """
 
-    def __init__(self, inputs, output, size_dict):
+    __slots__ = (
+        "nodes",
+        "edges",
+        "indmap",
+        "appearances",
+        "sizes",
+        "ssa",
+        "ssa_path",
+        "track_flops",
+        "flops",
+        "flops_limit",
+    )
+
+    def __init__(
+        self,
+        inputs,
+        output,
+        size_dict,
+        track_flops=False,
+        flops_limit=float("inf"),
+    ):
         self.nodes = {}
         self.edges = {}
         self.indmap = {}
         self.appearances = []
         self.sizes = []
         c = 0
 
@@ -301,14 +336,31 @@
             self.nodes[i] = tuple(legs)
 
         for ind in output:
             self.appearances[self.indmap[ind]] += 1
 
         self.ssa = len(self.nodes)
         self.ssa_path = []
+        self.track_flops = track_flops
+        self.flops = 0
+        self.flops_limit = flops_limit
+
+    def copy(self):
+        new = ContractionProcessor.__new__(ContractionProcessor)
+        new.nodes = self.nodes.copy()
+        new.edges = {k: v.copy() for k, v in self.edges.items()}
+        new.indmap = self.indmap  # never mutated
+        new.appearances = self.appearances  # never mutated
+        new.sizes = self.sizes  # never mutated
+        new.ssa = self.ssa
+        new.ssa_path = self.ssa_path.copy()
+        new.track_flops = self.track_flops
+        new.flops = self.flops
+        new.flops_limit = self.flops_limit
+        return new
 
     def neighbors(self, i):
         """Get all neighbors of node ``i``."""
         # only want to yield each neighbor once and not i itself
         for ix, _ in self.nodes[i]:
             for j in self.edges[ix]:
                 if j != i:
@@ -360,21 +412,27 @@
         for node, legs in self.nodes.items():
             for ix, _ in legs:
                 assert node in self.edges[ix]
         for ix, ix_nodes in self.edges.items():
             for node in ix_nodes:
                 assert ix in {jx for jx, _ in self.nodes[node]}
 
-    def contract_nodes(self, i, j):
+    def contract_nodes(self, i, j, new_legs=None):
         """Contract the nodes ``i`` and ``j``, adding a new node to the graph
         and returning its index.
         """
         ilegs = self.pop_node(i)
         jlegs = self.pop_node(j)
-        new_legs = compute_contracted(ilegs, jlegs, self.appearances)
+
+        if self.track_flops:
+            self.flops += compute_flops(ilegs, jlegs, self.sizes)
+
+        if new_legs is None:
+            new_legs = compute_contracted(ilegs, jlegs, self.appearances)
+
         k = self.add_node(new_legs)
         self.ssa_path.append((i, j))
         return k
 
     def simplify_batch(self):
         """Find any indices that appear in all terms and remove them, since
         they simply add an constant factor to the cost of the contraction, but
@@ -475,33 +533,30 @@
     def optimize_greedy(
         self,
         costmod=1.0,
         temperature=0.0,
         seed=None,
     ):
         """ """
-
         if temperature == 0.0:
 
             def local_score(sa, sb, sab):
-                return sab - costmod * (sa + sb)
+                return sab / costmod - (sa + sb) * costmod
 
         else:
             gmblgen = GumbelBatchedGenerator(seed)
 
             def local_score(sa, sb, sab):
-                score = sab - costmod * (sa + sb)
+                score = sab / costmod - (sa + sb) * costmod
                 if score > 0:
                     return math.log(score) - temperature * gmblgen()
                 elif score < 0:
                     return -math.log(-score) - temperature * gmblgen()
                 else:
-                    return - temperature * gmblgen()
-
-                # return sab - costmod * (sa + sb) - temperature * gmblgen()
+                    return -temperature * gmblgen()
 
         node_sizes = {}
         for i, ilegs in self.nodes.items():
             node_sizes[i] = compute_size(ilegs, self.sizes)
 
         queue = []
         contractions = {}
@@ -522,31 +577,37 @@
         while queue:
             _, c0 = heapq.heappop(queue)
             i, j, ksize, klegs = contractions.pop(c0)
             if (i not in self.nodes) or (j not in self.nodes):
                 # one of nodes already contracted
                 continue
 
-            self.pop_node(i)
-            self.pop_node(j)
-            k = self.add_node(klegs)
-            self.ssa_path.append((i, j))
+            k = self.contract_nodes(i, j, new_legs=klegs)
+
+            if (
+                self.track_flops and (self.flops >= self.flops_limit)
+            ):
+                # shortcut - stop early and return failed
+                return False
+
             node_sizes[k] = ksize
 
             for l in self.neighbors(k):
                 lsize = node_sizes[l]
                 mlegs = compute_contracted(
                     klegs, self.nodes[l], self.appearances
                 )
                 msize = compute_size(mlegs, self.sizes)
                 score = local_score(ksize, lsize, msize)
                 heapq.heappush(queue, (score, c))
                 contractions[c] = (k, l, msize, mlegs)
                 c += 1
 
+        return True
+
     def optimize_optimal_connected(
         self,
         where,
         minimize="flops",
         cost_cap=2,
         search_outer=False,
     ):
@@ -743,16 +804,15 @@
         ids.append(ssa)
         path.append(con)
         ssa += 1
     return path
 
 
 def is_ssa_path(path, nterms):
-    """Check if an explicitly given path is in 'static single assignment' form.
-    """
+    """Check if an explicitly given path is in 'static single assignment' form."""
     seen = set()
     # we reverse as more likely to see high id and shortcut
     for con in reversed(path):
         for i in con:
             if (nterms is not None) and (i >= nterms):
                 # indices beyond nterms -> ssa
                 return True
@@ -815,15 +875,15 @@
         The indices of the output tensor.
     size_dict : dict[str, int]
         A dictionary mapping indices to their dimension.
     costmod : float, optional
         When assessing local greedy scores how much to weight the size of the
         tensors removed compared to the size of the tensor added::
 
-            score = size_ab - costmod * (size_a + size_b)
+            score = size_ab / costmod - (size_a + size_b) * costmod
 
         This can be a useful hyper-parameter to tune.
     temperature : float, optional
         When asessing local greedy scores, how much to randomly perturb the
         score. This is implemented as::
 
             score -> sign(score) * log(|score|) - temperature * gumbel()
@@ -859,14 +919,147 @@
     # handle disconnected subgraphs
     cp.optimize_remaining_by_size()
     if use_ssa:
         return cp.ssa_path
     return ssa_to_linear(cp.ssa_path, len(inputs))
 
 
+def optimize_random_greedy_track_flops(
+    inputs,
+    output,
+    size_dict,
+    ntrials=1,
+    costmod=(0.1, 4.0),
+    temperature=(0.001, 1.0),
+    seed=None,
+    simplify=True,
+    use_ssa=False,
+):
+    """Perform a batch of random greedy optimizations, simulteneously tracking
+    the best contraction path in terms of flops, so as to avoid constructing a
+    separate contraction tree.
+
+    Parameters
+    ----------
+    inputs : tuple[tuple[str]]
+        The indices of each input tensor.
+    output : tuple[str]
+        The indices of the output tensor.
+    size_dict : dict[str, int]
+        A dictionary mapping indices to their dimension.
+    ntrials : int, optional
+        The number of random greedy trials to perform. The default is 1.
+    costmod : (float, float), optional
+        When assessing local greedy scores how much to weight the size of the
+        tensors removed compared to the size of the tensor added::
+
+            score = size_ab / costmod - (size_a + size_b) * costmod
+
+        It is sampled uniformly from the given range.
+    temperature : (float, float), optional
+        When asessing local greedy scores, how much to randomly perturb the
+        score. This is implemented as::
+
+            score -> sign(score) * log(|score|) - temperature * gumbel()
+
+        which implements boltzmann sampling. It is sampled log-uniformly from
+        the given range.
+    seed : int, optional
+        The seed for the random number generator.
+    simplify : bool, optional
+        Whether to perform simplifications before optimizing. These are:
+
+            - ignore any indices that appear in all terms
+            - combine any repeated indices within a single term
+            - reduce any non-output indices that only appear on a single term
+            - combine any scalar terms
+            - combine any tensors with matching indices (hadamard products)
+
+        Such simpifications may be required in the general case for the proper
+        functioning of the core optimization, but may be skipped if the input
+        indices are already in a simplified form.
+    use_ssa : bool, optional
+        Whether to return the contraction path in 'single static assignment'
+        (SSA) format (i.e. as if each intermediate is appended to the list of
+        inputs, without removals). This can be quicker and easier to work with
+        than the 'linear recycled' format that `numpy` and `opt_einsum` use.
+
+    Returns
+    -------
+    path : list[list[int]]
+        The best contraction path, given as a sequence of pairs of node
+        indices.
+    flops : float
+        The flops (/ contraction cost / number of multiplications), of the best
+        contraction path, given log10.
+    """
+    rng = get_rng(seed)
+    best_path = None
+    best_flops = float("inf")
+
+    # create initial processor and simplify only once
+    cp0 = ContractionProcessor(inputs, output, size_dict, track_flops=True)
+    if simplify:
+        cp0.simplify()
+
+    if isinstance(costmod, float):
+        # constant
+
+        def _next_costmod():
+            return costmod
+
+    else:
+        # uniformly sample
+
+        def _next_costmod():
+            return rng.uniform(*costmod)
+
+    if isinstance(temperature, float):
+        # constant
+
+        def _next_temperature():
+            return temperature
+
+    else:
+        # log-uniformly sample
+        logtempmin, logtempmax = map(math.log, temperature)
+
+        def _next_temperature():
+            return math.exp(rng.uniform(logtempmin, logtempmax))
+
+    for _ in range(ntrials):
+        cp = cp0.copy()
+        success = cp.optimize_greedy(
+            costmod=_next_costmod(),
+            temperature=_next_temperature(),
+            seed=rng,
+        )
+
+        if not success:
+            # optimization hit the flops limit
+            continue
+
+        # handle disconnected subgraphs
+        cp.optimize_remaining_by_size()
+
+        if cp.flops < best_flops:
+            best_path = cp.ssa_path
+            best_flops = cp.flops
+            # enable even earlier stopping
+            cp0.flops_limit = best_flops
+
+    # for consistency with cotengrust / easier comparison
+    best_flops = math.log10(best_flops)
+
+    if not use_ssa:
+        best_path = ssa_to_linear(best_path, len(inputs))
+
+    return best_path, best_flops
+
+
 def optimize_optimal(
     inputs,
     output,
     size_dict,
     minimize="flops",
     cost_cap=2,
     search_outer=False,
@@ -946,46 +1139,62 @@
     # handle disconnected subgraphs
     cp.optimize_remaining_by_size()
     if use_ssa:
         return cp.ssa_path
     return ssa_to_linear(cp.ssa_path, len(inputs))
 
 
+class EnsureInputsOutputAreSequence:
+    def __init__(self, f):
+        self.f = f
 
-def ensure_inputs_output_are_sequence(f):
-
-    def wrapped(inputs, output, *args, **kwargs):
+    def __call__(self, inputs, output, *args, **kwargs):
         if not isinstance(inputs[0], (tuple, list)):
             inputs = tuple(map(tuple, inputs))
         if not isinstance(output, (tuple, list)):
             output = tuple(output)
-        return f(inputs, output, *args, **kwargs)
-
-    return wrapped
-
+        return self.f(inputs, output, *args, **kwargs)
 
 
 @functools.lru_cache()
 def get_optimize_greedy(accel="auto"):
     if accel == "auto":
         import importlib.util
 
         accel = importlib.util.find_spec("cotengrust") is not None
 
     if accel is True:
         from cotengrust import optimize_greedy as f
 
-        return ensure_inputs_output_are_sequence(f)
+        return EnsureInputsOutputAreSequence(f)
 
     if accel is False:
         return optimize_greedy
 
     raise ValueError(f"Unrecognized value for `accel`: {accel}.")
 
 
+@functools.lru_cache()
+def get_optimize_random_greedy_track_flops(accel="auto"):
+    if accel == "auto":
+        import importlib.util
+
+        accel = importlib.util.find_spec("cotengrust") is not None
+
+    if accel is True:
+        from cotengrust import optimize_random_greedy_track_flops as f
+
+        return EnsureInputsOutputAreSequence(f)
+
+    if accel is False:
+        return optimize_random_greedy_track_flops
+
+    raise ValueError(f"Unrecognized value for `accel`: {accel}.")
+
+
 class GreedyOptimizer(PathOptimizer):
     """Class interface to the greedy optimizer which can be instantiated with
     default options.
     """
 
     __slots__ = (
         "costmod",
@@ -1039,25 +1248,199 @@
             output,
             size_dict,
             use_ssa=False,
             **self.maybe_update_defaults(**kwargs),
         )
 
 
+class RandomGreedyOptimizer(PathOptimizer):
+    """Lightweight random greedy optimizer, that eschews hyper parameter
+    tuning and contraction tree construction. This is a stateful optimizer
+    that should not be re-used on different contractions.
+
+    Parameters
+    ----------
+    max_repeats : int, optional
+        The number of random greedy trials to perform.
+    costmod : (float, float), optional
+        When assessing local greedy scores how much to weight the size of the
+        tensors removed compared to the size of the tensor added::
+
+            score = size_ab / costmod - (size_a + size_b) * costmod
+
+        It is sampled uniformly from the given range.
+    temperature : (float, float), optional
+        When asessing local greedy scores, how much to randomly perturb the
+        score. This is implemented as::
+
+            score -> sign(score) * log(|score|) - temperature * gumbel()
+
+        which implements boltzmann sampling. It is sampled log-uniformly from
+        the given range.
+    seed : int, optional
+        The seed for the random number generator. Note that deterministic
+        behavior is only guaranteed within the python or rust backend
+        (the `accel` parameter) and parallel settings.
+    simplify : bool, optional
+        Whether to perform simplifications before optimizing. These are:
+
+            - ignore any indices that appear in all terms
+            - combine any repeated indices within a single term
+            - reduce any non-output indices that only appear on a single term
+            - combine any scalar terms
+            - combine any tensors with matching indices (hadamard products)
+
+        Such simpifications may be required in the general case for the proper
+        functioning of the core optimization, but may be skipped if the input
+        indices are already in a simplified form.
+    accel : bool or str, optional
+        Whether to use the accelerated `cotengrust` backend. If "auto" the
+        backend is used if available.
+    parallel : bool or str, optional
+        Whether to use parallel processing. If "auto" the default is to use
+        threads if the accelerated backend is not used, and processes if it is.
+
+    Attributes
+    ----------
+    best_ssa_path : list[list[int]]
+        The best contraction path found so far.
+    best_flops : float
+        The flops (/ contraction cost / number of multiplications) of the best
+        contraction path found so far.
+    """
+
+    def __init__(
+        self,
+        max_repeats=32,
+        costmod=(0.1, 4.0),
+        temperature=(0.001, 1.0),
+        seed=None,
+        simplify=True,
+        accel="auto",
+        parallel="auto",
+    ):
+        self.max_repeats = max_repeats
+
+        # for cotengrust, ensure these are always ranges
+        if isinstance(costmod, float):
+            self.costmod = (costmod, costmod)
+        else:
+            self.costmod = tuple(costmod)
+
+        if isinstance(temperature, float):
+            self.temperature = (temperature, temperature)
+        else:
+            self.temperature = tuple(temperature)
+
+        self.simplify = simplify
+        self.rng = get_rng(seed)
+        self.best_ssa_path = None
+        self.best_flops = float("inf")
+        self._optimize_fn = get_optimize_random_greedy_track_flops(accel)
+
+        if (parallel == "auto") and (
+            self._optimize_fn is not optimize_random_greedy_track_flops
+        ):
+            # using accelerated fn, so default to threads
+            parallel = "threads"
+        self._pool = parse_parallel_arg(parallel)
+        if self._pool is not None:
+            self._nworkers = get_n_workers(self._pool)
+        else:
+            self._nworkers = 1
+
+    def maybe_update_defaults(self, **kwargs):
+        # allow overriding of defaults
+        opts = {
+            "costmod": self.costmod,
+            "temperature": self.temperature,
+            "simplify": self.simplify,
+        }
+        opts.update(kwargs)
+        return opts
+
+    def ssa_path(self, inputs, output, size_dict, **kwargs):
+        if self._pool is None:
+            ssa_path, flops = self._optimize_fn(
+                inputs,
+                output,
+                size_dict,
+                use_ssa=True,
+                ntrials=self.max_repeats,
+                seed=self.rng.randint(0, 2**32 - 1),
+                **self.maybe_update_defaults(**kwargs),
+            )
+        else:
+            # XXX: just use small batchsize if can't find num_workers?
+            nbatches = self._nworkers
+            batchsize = self.max_repeats // nbatches
+            batchremainder = self.max_repeats % nbatches
+            each_ntrials = [
+                batchsize + (i < batchremainder) for i in range(nbatches)
+            ]
+
+            fs = [
+                self._pool.submit(
+                    self._optimize_fn,
+                    inputs,
+                    output,
+                    size_dict,
+                    use_ssa=True,
+                    ntrials=ntrials,
+                    seed=self.rng.randint(0, 2**32 - 1),
+                    **self.maybe_update_defaults(**kwargs),
+                )
+                for ntrials in each_ntrials
+                if (ntrials > 0)
+            ]
+            ssa_path, flops = min((f.result() for f in fs), key=lambda x: x[1])
+
+        if flops < self.best_flops:
+            self.best_ssa_path = ssa_path
+            self.best_flops = flops
+
+        return self.best_ssa_path
+
+    def search(self, inputs, output, size_dict, **kwargs):
+        from ..core import ContractionTree
+
+        return ContractionTree.from_path(
+            inputs,
+            output,
+            size_dict,
+            ssa_path=self.ssa_path(
+                inputs,
+                output,
+                size_dict,
+                **self.maybe_update_defaults(**kwargs),
+            ),
+        )
+
+    def __call__(self, inputs, output, size_dict, **kwargs):
+        return ssa_to_linear(
+            self.ssa_path(
+                inputs,
+                output,
+                size_dict,
+                **self.maybe_update_defaults(**kwargs),
+            ),
+        )
+
+
 @functools.lru_cache()
 def get_optimize_optimal(accel="auto"):
     if accel == "auto":
         import importlib.util
 
         accel = importlib.util.find_spec("cotengrust") is not None
 
     if accel is True:
         from cotengrust import optimize_optimal as f
 
-        return ensure_inputs_output_are_sequence(f)
+        return EnsureInputsOutputAreSequence(f)
 
     if accel is False:
         return optimize_optimal
 
     raise ValueError(f"Unrecognized value for `accel`: {accel}.")
```

### Comparing `cotengra-0.6.0/cotengra/pathfinders/path_compressed.py` & `cotengra-0.6.1/cotengra/pathfinders/path_compressed.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/path_flowcutter.py` & `cotengra-0.6.1/cotengra/pathfinders/path_flowcutter.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/path_greedy.py` & `cotengra-0.6.1/cotengra/pathfinders/path_compressed_greedy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,81 +1,23 @@
-"""Greedy contraction tree finders.
-"""
+"""Greedy contraction tree finders."""
+
 import collections
-import functools
 import heapq
 import itertools
 import math
 
 from ..core import (
     ContractionTree,
     ContractionTreeCompressed,
     get_hypergraph,
-    jitter_dict,
 )
 from ..hyperoptimizers.hyper import register_hyper_function
 from ..utils import BadTrial, GumbelBatchedGenerator, get_rng, oset
-from .path_basic import get_optimize_greedy, ssa_to_linear
-
-ssa_greedy_optimize = functools.partial(get_optimize_greedy(), use_ssa=True)
-
-# ------------------------------ GREEDY HYPER ------------------------------- #
-
-
-def trial_greedy(
-    inputs,
-    output,
-    size_dict,
-    random_strength=0.0,
-    temperature=0.0,
-    costmod=1.0,
-):
-    if random_strength != 0.0:
-        # don't supply randomized sizes to actual contraction tree
-        greedy_size_dict = jitter_dict(size_dict, random_strength)
-    else:
-        greedy_size_dict = size_dict
-
-    ssa_path = ssa_greedy_optimize(
-        inputs,
-        output,
-        greedy_size_dict,
-        temperature=temperature,
-        costmod=costmod,
-    )
-
-    return ContractionTree.from_path(
-        inputs, output, size_dict, ssa_path=ssa_path
-    )
-
-
-register_hyper_function(
-    name="greedy",
-    ssa_func=trial_greedy,
-    space={
-        "random_strength": {"type": "FLOAT_EXP", "min": 0.001, "max": 1.0},
-        "temperature": {"type": "FLOAT_EXP", "min": 0.001, "max": 1.0},
-        "costmod": {"type": "FLOAT", "min": 0.0, "max": 50.0},
-    },
-)
-
-# greedy but don't explore costmod or add index size noise
-# -> better for a small number of runs
-register_hyper_function(
-    name="random-greedy",
-    ssa_func=trial_greedy,
-    space={
-        "temperature": {"type": "FLOAT_EXP", "min": 0.001, "max": 0.01},
-    },
-    constants={
-        "costmod": 1.0,
-        "random_strength": 0.0,
-    },
-)
-
+from .path_basic import ssa_to_linear
+from .path_greedy import ssa_greedy_optimize
 
 # --------------------------------------------------------------------------- #
 
 
 def _binary_combine(func, x, y):
     if func == "sum":
         return x + y
@@ -528,7 +470,24 @@
         "coeff_next_centrality": {"type": "FLOAT", "min": -1, "max": 1},
         "weight_bonds": {"type": "BOOL"},
         "temperature": {"type": "FLOAT", "min": -1.0, "max": 1.0},
         "distance_p": {"type": "FLOAT", "min": -5.0, "max": 5.0},
         "distance_steal": {"type": "STRING", "options": ["", "abs", "rel"]},
     },
 )
+
+register_hyper_function(
+    name="greedy-span-max",
+    ssa_func=trial_greedy_span,
+    space={
+        "score_perm": {"type": "STRING", "options": _allowed_perms},
+        "coeff_connectivity": {"type": "INT", "min": 0, "max": 1},
+        "coeff_ndim": {"type": "INT", "min": -1, "max": 1},
+        "coeff_distance": {"type": "INT", "min": -1, "max": 1},
+        "coeff_next_centrality": {"type": "FLOAT", "min": -1, "max": 1},
+        "weight_bonds": {"type": "BOOL"},
+        "temperature": {"type": "FLOAT", "min": -1.0, "max": 1.0},
+        "distance_p": {"type": "FLOAT", "min": -5.0, "max": 5.0},
+        "distance_steal": {"type": "STRING", "options": ["", "abs", "rel"]},
+    },
+    constants={"start": "max"},
+)
```

### Comparing `cotengra-0.6.0/cotengra/pathfinders/path_igraph.py` & `cotengra-0.6.1/cotengra/pathfinders/path_igraph.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/path_kahypar.py` & `cotengra-0.6.1/cotengra/pathfinders/path_kahypar.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/path_labels.py` & `cotengra-0.6.1/cotengra/pathfinders/path_labels.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/path_quickbb.py` & `cotengra-0.6.1/cotengra/pathfinders/path_quickbb.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/pathfinders/path_simulated_annealing.py` & `cotengra-0.6.1/cotengra/pathfinders/path_simulated_annealing.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
                 )
                 proposed_score = scorer.score_local(
                     flops=[new_cost0, new_cost1],
                     size=[new_size0, new_size1],
                 )
 
                 dE = proposed_score - current_score
-                accept = (dE < 0) or (math.log(rng.random()) < -dE / temp)
+                accept = (dE <= 0) or (math.log(rng.random()) < -dE / temp)
 
                 if accept:
                     tree._remove_node(p)
                     tree._remove_node(x)
 
                     tree.contract_nodes_pair(
                         tree.contract_nodes_pair(
@@ -356,29 +356,34 @@
 
         if progbar:
             pbar.update()
 
     return tree
 
 
+def _do_anneal(tree, *args, **kwargs):
+    return tree.simulated_anneal(*args, **kwargs)
+
+
 def parallel_temper_tree(
     tree_or_trees,
     tfinal=0.01,
     tstart=1,
     tsteps=50,
     num_trees=8,
     numiter=50,
-    minimize="flops",
+    minimize=None,
     target_size=None,
     slice_mode="drift",
     parallel_slice_mode="temperature",
     swappiness=1.0,
     max_time=None,
     seed=None,
     parallel="auto",
+    info=None,
     progbar=False,
     inplace=False,
 ):
     """Perform parallel tempering optimization of a contraction tree. This
     anneals ``num_trees`` different trees at a range of temperatures between
     ``tfinal`` and ``tstart``. After each step, trees are exchanged between
     neighboring temperatures according to the Metropolis-Hastings criterion.
@@ -431,15 +436,19 @@
         tree_or_trees = tuple(tree_or_trees)
         num_trees = max(num_trees, len(tree_or_trees))
         initial_trees = itertools.cycle(tree_or_trees)
     else:
         initial_trees = itertools.repeat(tree_or_trees)
         tree_or_trees = (tree_or_trees,)
 
-    scorer = get_score_fn(minimize)
+    if minimize is None:
+        scorer = tree_or_trees[0].get_default_objective()
+    else:
+        scorer = get_score_fn(minimize)
+
     rng = get_rng(seed)
 
     if progbar:
         import tqdm
 
         pbar = tqdm.tqdm(total=tsteps)
         pbar.set_description(_describe_tree(tree_or_trees[0]))
@@ -512,27 +521,27 @@
             minimize=minimize,
             slice_mode=slice_mode,
             seed=rng.randrange(0, 2**32),
         )
 
         if pool is None:
             trees = [
-                t.simulated_anneal(
-                    tfinal=temp, tstart=temp, target_size=tsz, **sa_opts
+                _do_anneal(
+                    t, tfinal=temp, tstart=temp, target_size=tsz, **sa_opts
                 )
                 for t, temp, tsz in args
             ]
             scores = [_score_tree(scorer, t, target_size) for t in trees]
 
         else:
             # submit in smaller steps for scatter pools?
             trees = [
                 submit(
                     pool,
-                    simulated_anneal_tree,
+                    _do_anneal,
                     t,
                     tfinal=temp,
                     tstart=temp,
                     target_size=tsz,
                     **sa_opts,
                 )
                 for t, temp, tsz in args
@@ -577,14 +586,17 @@
                 else:
                     desc = _describe_tree(best_tree)
                 pbar.set_description(f"nswap: {nswap} " + desc, refresh=False)
 
         if progbar:
             pbar.update()
 
+        if info is not None:
+            info.setdefault("scores", []).append(scores)
+
         if (max_time is not None) and (time.time() > max_time):
             break
 
     if is_scatter_pool:
         best_tree = best_tree.result()
         maybe_rejoin_pool(is_worker, pool)
```

### Comparing `cotengra-0.6.0/cotengra/pathfinders/treedecomp.py` & `cotengra-0.6.1/cotengra/pathfinders/treedecomp.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/plot.py` & `cotengra-0.6.1/cotengra/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             besty,
             color=(0, 0.7, 0.3, 0.5),
             zorder=10,
         )
         ax.text(
             bestx[-1],
             besty[-1],
-            f"{besty[-1]:.4g}",
+            f"{besty[-1]:.2f}",
             ha="left",
             va="center",
             color=(0, 0.7, 0.3),
             fontsize=8,
         )
 
     ax.grid(True, color=(0.5, 0.5, 0.5), which="major", alpha=0.1)
```

### Comparing `cotengra-0.6.0/cotengra/presets.py` & `cotengra-0.6.1/cotengra/presets.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/schematic.py` & `cotengra-0.6.1/cotengra/schematic.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/cotengra/scoring.py` & `cotengra-0.6.1/cotengra/scoring.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Objects for defining and customizing the target cost of a contraction.
-"""
+"""Objects for defining and customizing the target cost of a contraction."""
+
 import re
 import math
 import functools
 
 # the default weighting for comparing flops vs mops
 DEFAULT_COMBO_FACTOR = 64
 
@@ -274,17 +274,15 @@
         )
 
     def get_dynamic_programming_minimize(self):
         return f"combo-{self.factor}"
 
     def __call__(self, trial):
         ensure_basic_quantities_are_computed(trial)
-        return (
-            math.log2(trial["flops"] + self.factor * trial["write"])
-        )
+        return math.log2(trial["flops"] + self.factor * trial["write"])
 
 
 class LimitObjective(ExactObjective):
     """Objective that scores based on a maximum of either estimated floating
     point operations or the total write, weighted by some factor:
 
     .. math::
@@ -328,15 +326,15 @@
         )
 
     def get_dynamic_programming_minimize(self):
         return f"limit-{self.factor}"
 
     def __call__(self, trial):
         tree = trial["tree"]
-        return math.log2(tree.total_cost(factor=self.factor, combine=max))
+        return math.log2(tree.combo_cost(factor=self.factor, combine=max))
 
 
 # --------------------- compressed contraction scoring ---------------------- #
 
 
 class CompressedStatsTracker:
     __slots__ = (
@@ -434,22 +432,32 @@
     def combo_score(self):
         return math.log2(self.flops + DEFAULT_COMBO_FACTOR * self.write + 1)
 
     @property
     def score(self):
         raise NotImplementedError
 
-    def __repr__(self):
+    def describe(self, join=" "):
+        F = math.log10(max(1, self.flops))
+        C = math.log10(
+            max(
+                1,
+                self.flops
+                + getattr(self, "factor", DEFAULT_COMBO_FACTOR) * self.write,
+            )
+        )
+        S = math.log2(max(1, self.max_size))
+        P = math.log2(max(1, self.peak_size))
+        return join.join((
+            f"F={F:.2f}", f"C={C:.2f}", f"S={S:.2f}", f"P={P:.2f}"
+        ))
+
+    def __repr__(self):\
         return (
-            f"<{self.__class__.__name__}("
-            f"F={math.log10(max(1, self.flops)):.4g}, "
-            f"W={math.log10(max(1, self.write)):.4g}, "
-            f"S={math.log2(max(1, self.max_size)):.4g}, "
-            f"P={math.log2(max(1, self.peak_size)):.4g}"
-            f")>"
+            f"<{self.__class__.__name__}({self.describe(join=', ')})>"
         )
 
 
 class CompressedStatsTrackerSize(CompressedStatsTracker):
     __slots__ = CompressedStatsTracker.__slots__ + ("secondary_weight",)
 
     def __init__(self, hg, chi, secondary_weight=1e-3):
@@ -863,7 +871,80 @@
 def get_score_fn(minimize):
     if isinstance(minimize, str):
         return _get_score_fn_str_cached(minimize)
     if callable(minimize):
         # custom objective function
         return minimize
     raise TypeError("minimize must be a string or callable.")
+# ----------------------- multi-contraction scoring ------------------------- #
+
+
+class MultiObjective(Objective):
+
+    __slots__ = ("num_configs",)
+
+    def __init__(self, num_configs):
+        self.num_configs = num_configs
+
+    def compute_mult(self, dims):
+        raise NotImplementedError
+
+    def estimate_node_mult(self, tree, node):
+        return self.compute_mult([
+            tree.size_dict[ix] for ix in tree.get_node_var_inds(node)
+        ])
+
+    def estimate_node_cache_mult(self, tree, node, sliced_ind_ordering):
+        node_var_inds = tree.get_node_var_inds(node)
+
+        # indices which are the first 'k' in the sliced ordering
+        non_heavy_inds = [
+            ix
+            for ix in tree.get_node_var_inds(node)
+            if ix not in sliced_ind_ordering[: len(node_var_inds)]
+        ]
+
+        # each of these cycles 'out of sync' and thus must be kept
+        return self.compute_mult([tree.size_dict[ix] for ix in non_heavy_inds])
+
+
+class MultiObjectiveDense(MultiObjective):
+    """Number of intermediate configurations is expected to scale as if all
+    configurations are present.
+    """
+    __slots__ = ("num_configs",)
+
+    def compute_mult(self, dims):
+        return math.prod(dims)
+
+
+def expected_coupons(num_sub, num_total):
+    """If we draw a random 'coupon` which can take `num_sub` different values
+    `num_total` times, how many unique coupons will we expect?
+    """
+    return num_sub * (1 - (1 - 1 / num_sub) ** num_total)
+
+
+class MultiObjectiveUniform(MultiObjective):
+    """Number of intermediate configurations is expected to scale as if all
+    configurations are randomly draw from a uniform distribution.
+    """
+    __slots__ = ("num_configs",)
+
+    def compute_mult(self, dims):
+        return expected_coupons(math.prod(dims), self.num_configs)
+
+
+class MultiObjectiveLinear(MultiObjective):
+    """Number of intermediate configurations is expected to scale linearly with
+    respect to number of variable indices (e.g. VMC like 'locally connected'
+    configurations).
+    """
+    __slots__ = ("num_configs", "coeff")
+
+    def __init__(self, num_configs, coeff=1):
+        self.coeff = coeff
+        super().__init__(num_configs=num_configs)
+
+    def compute_mult(self, dims):
+        return min(self.coeff * len(dims), self.num_configs)
+
```

### Comparing `cotengra-0.6.0/cotengra/slicer.py` & `cotengra-0.6.1/cotengra/slicer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-"""Functionality for identifying indices to sliced.
-"""
+"""Functionality for identifying indices to sliced."""
+
 import collections
 from math import log
 
 from .core import ContractionTree
 from .plot import plot_slicings, plot_slicings_alt
 from .scoring import get_score_fn
-from .utils import MaxCounter, compute_size_by_dict, get_rng, oset
+from .utils import MaxCounter, get_rng
+
+IDX_INVOLVED = 0
+IDX_LEGS = 1
+IDX_SIZE = 2
+IDX_FLOPS = 3
 
 
 class ContractionCosts:
     """A simplified struct for tracking the contraction costs of a path only.
 
     Parameters
     ----------
@@ -39,56 +44,81 @@
         self,
         contractions,
         size_dict,
         nslices=1,
         original_flops=None,
     ):
         self.size_dict = dict(size_dict)
-        self.contractions = tuple(contractions)
+        self.contractions = list(contractions)
 
         self._flops = 0
         self._sizes = MaxCounter()
         self._flop_reductions = collections.defaultdict(lambda: 0)
         self._write_reductions = collections.defaultdict(lambda: 0)
         self._where = collections.defaultdict(set)
 
         for i, c in enumerate(self.contractions):
-            self._flops += c["flops"]
-            self._sizes.add(c["size"])
+            self._flops += c[IDX_FLOPS]
+            self._sizes.add(c[IDX_SIZE])
 
-            for ix in c["involved"].union(c["legs"]):
+            for ix in c[IDX_INVOLVED]:
                 d = self.size_dict[ix]
-                self._flop_reductions[ix] += int((1 - 1 / d) * c["flops"])
+                self._flop_reductions[ix] += c[IDX_FLOPS] - c[IDX_FLOPS] // d
                 self._where[ix].add(i)
-                if ix in c["legs"]:
-                    self._write_reductions[ix] += int((1 - 1 / d) * c["size"])
+                if ix in c[IDX_LEGS]:
+                    self._write_reductions[ix] += c[IDX_SIZE] - c[IDX_SIZE] // d
 
         self.nslices = nslices
         if original_flops is None:
             original_flops = self._flops
         self.original_flops = original_flops
 
     def _set_state_from(self, other):
         """Copy all internal structure from another ``ContractionCosts``."""
         self.size_dict = other.size_dict.copy()
-        self.contractions = tuple(c.copy() for c in other.contractions)
+        self.contractions = other.contractions.copy()
         self.nslices = other.nslices
         self.original_flops = other.original_flops
         self._flops = other._flops
         self._sizes = other._sizes.copy()
         self._flop_reductions = other._flop_reductions.copy()
         self._write_reductions = other._write_reductions.copy()
         self._where = other._where.copy()
 
     def copy(self):
         """Get a copy of this ``ContractionCosts``."""
         new = object.__new__(ContractionCosts)
         new._set_state_from(self)
         return new
 
+    @classmethod
+    def from_contraction_tree(cls, contraction_tree, **kwargs):
+        """Generate a set of contraction costs from a ``ContractionTree``
+        object.
+        """
+        size_dict = contraction_tree.size_dict
+        contractions = (
+            (
+                set(contraction_tree.get_involved(node)),
+                set(contraction_tree.get_legs(node)),
+                contraction_tree.get_size(node),
+                contraction_tree.get_flops(node),
+            )
+            for node in contraction_tree.info
+            # ignore leaf nodes
+            if len(node) != 1
+        )
+        return cls(contractions, size_dict, **kwargs)
+
+    @classmethod
+    def from_info(cls, info, **kwargs):
+        """Generate a set of contraction costs from a ``PathInfo`` object."""
+        tree = ContractionTree.from_info(info)
+        return cls.from_contraction_tree(tree, **kwargs)
+
     @property
     def size(self):
         return self._sizes.max()
 
     @property
     def flops(self):
         return self._flops
@@ -97,105 +127,66 @@
     def total_flops(self):
         return self.nslices * self.flops
 
     @property
     def overhead(self):
         return self.total_flops / self.original_flops
 
-    @classmethod
-    def from_info(cls, info, **kwargs):
-        """Generate a set of contraction costs from a ``PathInfo`` object."""
-        cs = []
-        size_dict = info.size_dict
-
-        # add all the input 'contractions'
-        for term in info.input_subscripts.split(","):
-            cs.append(
-                {
-                    "involved": oset(),
-                    "legs": oset(term),
-                    "size": compute_size_by_dict(term, size_dict),
-                    "flops": 0,
-                }
-            )
-
-        for c in info.contraction_list:
-            eq = c[2]
-            lhs, rhs = eq.split("->")
-            legs = oset(rhs)
-            involved = oset.union(*map(oset, lhs.split(",")))
-
-            cs.append(
-                {
-                    "involved": involved,
-                    "legs": legs,
-                    "size": compute_size_by_dict(legs, size_dict),
-                    "flops": compute_size_by_dict(involved, size_dict),
-                }
-            )
-
-        return cls(cs, size_dict)
-
-    @classmethod
-    def from_contraction_tree(cls, contraction_tree, **kwargs):
-        """Generate a set of contraction costs from a ``ContractionTree``
-        object.
-        """
-        size_dict = contraction_tree.size_dict
-        cs = (
-            {
-                "involved": oset(contraction_tree.get_involved(node)),
-                "legs": oset(contraction_tree.get_legs(node)),
-                "size": contraction_tree.get_size(node),
-                "flops": contraction_tree.get_flops(node),
-            }
-            for node in contraction_tree.info
-        )
-        return cls(cs, size_dict, **kwargs)
-
     def remove(self, ix, inplace=False):
         """ """
         cost = self if inplace else self.copy()
 
         d = cost.size_dict[ix]
         cost.nslices *= d
-        ix_s = oset([ix])
 
-        for i in cost._where[ix]:
-            c = cost.contractions[i]
+        for i in cost._where.pop(ix):
 
-            # update the potential flops reductions of other inds
-            for oix in c["involved"]:
-                di = cost.size_dict[oix]
-                cost._flop_reductions[oix] -= int(
-                    (1 - 1 / di) * c["flops"] * (1 - 1 / d)
-                )
+            old_involved, old_legs, old_size, old_flops = cost.contractions[i]
 
             # update the actual flops reduction
-            old_flops = c["flops"]
             new_flops = old_flops // d
             cost._flops += new_flops - old_flops
-            c["flops"] = new_flops
-            c["involved"] = c["involved"].difference(ix_s)
+            new_involved = old_involved.copy()
+            new_involved.discard(ix)
 
-            # update the tensor sizes
-            if ix in c["legs"]:
-                # update the potential size reductions of other inds
-                for oix in c["legs"]:
-                    di = cost.size_dict[oix]
-                    cost._write_reductions[oix] -= int(
-                        (1 - 1 / di) * c["size"] * (1 - 1 / d)
-                    )
+            # update the potential flops reductions of other inds
+            for oix in new_involved:
+                di = cost.size_dict[oix]
+                old_flops_reduction = old_flops - old_flops // di
+                new_flops_reduction = old_flops_reduction // d
+                cost._flop_reductions[oix] += (
+                    new_flops_reduction - old_flops_reduction
+                )
 
-                old_size = c["size"]
+            # update the tensor sizes
+            if ix in old_legs:
                 new_size = old_size // d
                 cost._sizes.discard(old_size)
                 cost._sizes.add(new_size)
-                c["size"] = new_size
-                c["legs"] = c["legs"].difference(ix_s)
+                new_legs = old_legs.copy()
+                new_legs.discard(ix)
+
+                # update the potential size reductions of other inds
+                for oix in new_legs:
+                    di = cost.size_dict[oix]
+                    old_size_reduction = old_size - old_size // di
+                    new_size_reduction = old_size_reduction // d
+                    cost._write_reductions[oix] -= (
+                        old_size_reduction - new_size_reduction
+                    )
+            else:
+                new_size = old_size
+                new_legs = old_legs
+
+            cost.contractions[i] = (
+                new_involved,
+                new_legs,
+                new_size,
+                new_flops,
+            )
 
         del cost.size_dict[ix]
         del cost._flop_reductions[ix]
         del cost._write_reductions[ix]
 
         return cost
 
@@ -372,17 +363,19 @@
         )
 
         while not already_satisfied:
             ix = max(
                 cost.size_dict,
                 key=lambda ix:
                 # the base score
-                self.minimize.score_slice_index(cost, ix) -
+                self.minimize.score_slice_index(cost, ix)
+                -
                 # a smudge that replicates boltzmann sampling
-                temperature * log(-log(self.rng.random())) -
+                temperature * log(-log(self.rng.random()))
+                -
                 # penalize forbidden (outer) indices
                 (0 if ix not in self.forbidden else float("inf")),
             )
             if ix in self.forbidden:
                 raise RuntimeError("Ran out of valid indices to slice.")
 
             next_ix_sl = ix_sl | frozenset([ix])
```

### Comparing `cotengra-0.6.0/cotengra/utils.py` & `cotengra-0.6.1/cotengra/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -749,20 +749,25 @@
         #> 'Ŕ'
 
         get_symbol(20000)
         #> '京'
 
     """
     if i < 52:
+        # use a-z, A-Z first
         return _einsum_symbols_base[i]
-    elif i >= 55296:
+
+    # then proceed from 'À'
+    i += 140
+
+    if i >= 55296:
         # Skip chr(57343) - chr(55296) as surrogates
-        return chr(i + 2048)
-    else:
-        return chr(i + 140)
+        i += 2048
+
+    return chr(i)
 
 
 def get_symbol_map(inputs):
     """Get a mapping of arbitrary hashable 'indices' to single unicode symbols,
     matching the canonicalization of the expression.
     """
     symbol_map = {}
```

### Comparing `cotengra-0.6.0/cotengra.egg-info/PKG-INFO` & `cotengra-0.6.1/cotengra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: cotengra
-Version: 0.6.0
+Version: 0.6.1
 Summary: Hyper optimized contraction trees for large tensor networks and einsums.
 Home-page: https://github.com/jcmgray/cotengra
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/cotengra/issues
 Project-URL: Source, https://github.com/jcmgray/cotengra/
 Keywords: tensor network contraction graph hypergraph partition einsum
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: autoray
 Provides-Extra: recommended
-Requires-Dist: cotengrust; extra == "recommended"
+Requires-Dist: cotengrust>=0.1.3; extra == "recommended"
 Requires-Dist: cytoolz; extra == "recommended"
 Requires-Dist: kahypar; extra == "recommended"
 Requires-Dist: networkx; extra == "recommended"
 Requires-Dist: numpy; extra == "recommended"
 Requires-Dist: opt_einsum; extra == "recommended"
 Requires-Dist: optuna; extra == "recommended"
 Requires-Dist: ray; extra == "recommended"
```

### Comparing `cotengra-0.6.0/cotengra.egg-info/SOURCES.txt` & `cotengra-0.6.1/cotengra.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ci/requirements/py-no-oe.yml
 ci/requirements/py-win.yml
 cotengra/.gitattributes
 cotengra/__init__.py
 cotengra/_version.py
 cotengra/contract.py
 cotengra/core.py
+cotengra/core_multi.py
 cotengra/hypergraph.py
 cotengra/interface.py
 cotengra/oe.py
 cotengra/parallel.py
 cotengra/plot.py
 cotengra/presets.py
 cotengra/schematic.py
@@ -43,14 +44,15 @@
 cotengra/hyperoptimizers/hyper_nevergrad.py
 cotengra/hyperoptimizers/hyper_optuna.py
 cotengra/hyperoptimizers/hyper_random.py
 cotengra/hyperoptimizers/hyper_skopt.py
 cotengra/pathfinders/__init__.py
 cotengra/pathfinders/path_basic.py
 cotengra/pathfinders/path_compressed.py
+cotengra/pathfinders/path_compressed_greedy.py
 cotengra/pathfinders/path_flowcutter.py
 cotengra/pathfinders/path_greedy.py
 cotengra/pathfinders/path_igraph.py
 cotengra/pathfinders/path_kahypar.py
 cotengra/pathfinders/path_labels.py
 cotengra/pathfinders/path_quickbb.py
 cotengra/pathfinders/path_simulated_annealing.py
```

### Comparing `cotengra-0.6.0/docs/Makefile` & `cotengra-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/_pygments/_pygments_dark.py` & `cotengra-0.6.1/docs/_pygments/_pygments_dark.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/_pygments/_pygments_light.py` & `cotengra-0.6.1/docs/_pygments/_pygments_light.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/_static/logo-favicon.ico` & `cotengra-0.6.1/docs/_static/logo-favicon.ico`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/_static/logo-full.png` & `cotengra-0.6.1/docs/_static/logo-full.png`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/_static/my-styles.css` & `cotengra-0.6.1/docs/_static/my-styles.css`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/advanced.ipynb` & `cotengra-0.6.1/docs/advanced.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9790598290598291%*

 * *Differences: {"'cells'": "{28: {'source': {insert: [(9, '- `parallel=pool` - supply your own "*

 * *            "`concurrent.futures.ProcessPoolExecutor` compatible pool\\n'), (10, '\\n'), (11, 'For "*

 * *            'non-distributed pools the default number of workers is computed, in order of '*

 * *            "preference, as:\\n'), (12, '\\n'), (13, '1. `COTENGRA_NUM_WORKERS` environment "*

 * *            "variable\\n'), (14, '2. `OMP_NUM_THREADS` environment variable\\n'), (15, '3. "*

 * *            '`os.cpu_count()`\\n\'), (56, \'```\\n […]*

```diff
@@ -405,14 +405,21 @@
                 "`cotengra` can fairly naturally parallelize over the trials of the hyper \n",
                 "optimization, and does so by default `HyperOptimizer(parallel='auto')`.\n",
                 "The basic `parallel` options are:\n",
                 "\n",
                 "- `parallel=False` - no parallelization\n",
                 "- `parallel=True` - alias for using default parallelization and number of workers\n",
                 "- `parallel=X:int` - alias for using default parallelization but specify number of workers\n",
+                "- `parallel=pool` - supply your own `concurrent.futures.ProcessPoolExecutor` compatible pool\n",
+                "\n",
+                "For non-distributed pools the default number of workers is computed, in order of preference, as:\n",
+                "\n",
+                "1. `COTENGRA_NUM_WORKERS` environment variable\n",
+                "2. `OMP_NUM_THREADS` environment variable\n",
+                "3. `os.cpu_count()`\n",
                 "\n",
                 "### `parallel='concurrent.futures'` \n",
                 "\n",
                 "The default parallelization is the python [standard library](https://docs.python.org/3/library/concurrent.futures.html).\n",
                 "A cached `ProcessPoolExecutor` is used.\n",
                 "    \n",
                 "### `parallel='loky'` \n",
@@ -445,15 +452,22 @@
                 "   sampling and reporting trials to the underlying optimizer\n",
                 "2. If the underlying optimizer cannot suggest trials quickly enough, or the pre\n",
                 "   dispatch is not large enough, workers can become idle.\n",
                 "\n",
                 "Consider using `optlib='nevergrad'` or `optlib='random'` if you are optimizing\n",
                 "with many tens or more workers to avoid being bottlenecked by the default Bayesian \n",
                 "optimization for example.\n",
-                "```"
+                "```\n",
+                "\n",
+                "### `parallel='threads'` \n",
+                "\n",
+                "You can specify a `ThreadPoolExecutor` for parallelization, but this is only\n",
+                "useful tasks where the underlying driver releases the GIL, e.g. \n",
+                "[`RandomGreedyOptimizer`](cotengra.pathfinders.path_basic.RandomGreedyOptimizer),\n",
+                "with `accel=True`, where threads are used by default."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "78ac17b8",
             "metadata": {},
             "source": [
@@ -483,14 +497,103 @@
                 "conditions and continue.\n",
                 "\n",
                 "```{hint}\n",
                 "The [`ReusableHyperOptimizer`](cotengra.core.ReusableHyperOptimizer) on the \n",
                 "other hand only runs once.\n",
                 "```"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "e47a6e6f",
+            "metadata": {},
+            "source": [
+                "## Large graphs - `RandomGreedyOptimizer`\n",
+                "\n",
+                "The `HyperOptimizer` can handle medium sizes of graph (up to 1000s of tensors), but the hyper-optimization and explicit `ContractionTree` construction of every trial can become slow for very large contractions. An alternative more suited to very lightweight path finding that can handle 10,000s of tensors is the [`RandomGreedyOptimizer`](cotengra.pathfinders.path_basic.RandomGreedyOptimizer). This only samples random greedy paths whilst simultaneously calculating each flops score, thus avoiding the heavier machinery of the hyper optimizer. Moreover, the core function [`optimize_random_greedy_track_flops`](cotengra.pathfinders.path_basic.optimize_random_greedy_track_flops) has an accelerated rust counterpart in [cotengrust](https://github.com/jcmgray/cotengrust), that is both faster and allows threaded parallelization."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "7d2fe2ce",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "inputs, output, _, size_dict = ctg.utils.lattice_equation([100, 100])\n",
+                "\n",
+                "opt = ctg.RandomGreedyOptimizer(\n",
+                "    max_repeats=32,\n",
+                "    temperature=(0.01, 0.1),  # sample a range\n",
+                "    seed=42,\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "39ecfb61",
+            "metadata": {},
+            "source": [
+                "It has the same call methods as all `cotengra` optimizers:\n",
+                "\n",
+                "- `path = opt(inputs, output, size_dict)`: return the best contraction path\n",
+                "- `ssa_path = opt.ssa_path(inputs, output, size_dict)`: return the best contraction path in SSA format\n",
+                "- `tree = opt.search(inputs, output, size_dict)`: return the best `ContractionTree`\n",
+                "\n",
+                "The marginally cheapest of these is the SSA format:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "06d097cd",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "CPU times: user 3.21 s, sys: 58 ms, total: 3.26 s\n",
+                        "Wall time: 613 ms\n"
+                    ]
+                }
+            ],
+            "source": [
+                "%%time\n",
+                "ssa_path = opt.ssa_path(inputs, output, size_dict)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "f0040ef5",
+            "metadata": {},
+            "source": [
+                "Once the optimizer has been run, the corresponding flops (log10) can be retrieved with:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "395c2b80",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "65.02261352539062"
+                        ]
+                    },
+                    "execution_count": 13,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "opt.best_flops"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `cotengra-0.6.0/docs/basics.ipynb` & `cotengra-0.6.1/docs/basics.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/changelog.md` & `cotengra-0.6.1/docs/changelog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## v0.6.1 (unreleased)
+
+**Breaking changes**
+
+- The number of workers initialized (for non-distributed pools) is now set to, in order of preference, 1. the environment variable `COTENGRA_NUM_WORKERS`, 2. the environment variable `OMP_NUM_THREADS`, or 3. `os.cpu_count()`.
+
+**Enhancements**
+
+- add [RandomGreedyOptimizer](cotengra.pathfinders.path_basic.RandomGreedyOptimizer) which is a lightweight and performant randomized greedy optimizer, eschewing both hyper parameter tuning and full contraction tree construction, making it suitable for very large contractions (10,000s of tensors+).
+- add [optimize_random_greedy_track_flops](cotengra.pathfinders.path_basic.optimize_random_greedy_track_flops) which runs N trials of (random) greedy path optimization, whilst computing the FLOP count simultaneously. This or its accelerated rust counterpart in `cotengrust` is the driver for the above optimizer.
+- add `parallel="threads"` backend, and make it the default for `RandomGreedyOptimizer` when `cotengrust` is present, since its version of `optimize_random_greedy_track_flops` releases the GIL.
+- significantly improve both the speed and memory usage of [`SliceFinder`](cotengra.slicer.SliceFinder)
+- alias `tree.total_cost()` to `tree.combo_cost()`
+
+
 ## v0.6.0 (2024-04-10)
 
 **Bug fixes**
 
 - all input node legs and pre-processing steps are now calculated lazily,
   allowing slicing of indices including those 'simplified' away {issue}`31`.
 - make [`tree.peak_size`](cotengra.ContractionTree.peak_size) more accurate,
@@ -44,15 +59,15 @@
   propagating a random number generator, to help determinism.
 - set ``autojit="auto"`` for contractions, which by default turns on jit for
   `backend="jax"` only.
 - add [`tree.describe`](cotengra.ContractionTree.describe) for a various levels
   of information about a tree, e.g. `tree.describe("full")` and
   `tree.describe("concise")`.
 - add [ctg.GreedyOptimizer](cotengra.pathfinders.path_basic.GreedyOptimizer)
-  and [ctg.OptimalOptimizer](cotengra.pathfinders.path_optimal.OptimalOptimizer)
+  and [ctg.OptimalOptimizer](cotengra.pathfinders.path_basic.OptimalOptimizer)
   to the top namespace.
 - add [ContractionTree.benchmark](cotengra.ContractionTree.benchmark) for
   for automatically assessing hardware performance vs theoretical cost.
 - contraction trees now have a `get_default_objective` method to return the
   objective function they were optimized with, for simpler further refinement
   or scoring, where it is now picked up automatically.
 - change the default 'sub' optimizer on divisive partition building algorithms
```

### Comparing `cotengra-0.6.0/docs/conf.py` & `cotengra-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/contraction.ipynb` & `cotengra-0.6.1/docs/contraction.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/examples/ex_compressed_contraction.ipynb` & `cotengra-0.6.1/docs/examples/ex_compressed_contraction.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/examples/ex_large_output_lazy.ipynb` & `cotengra-0.6.1/docs/examples/ex_large_output_lazy.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/high-level-interface.ipynb` & `cotengra-0.6.1/docs/high-level-interface.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/index.md` & `cotengra-0.6.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/installation.md` & `cotengra-0.6.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/make.bat` & `cotengra-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/trees.ipynb` & `cotengra-0.6.1/docs/trees.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/docs/visualization.ipynb` & `cotengra-0.6.1/docs/visualization.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/Example - Reproducing 2005.06787.ipynb` & `cotengra-0.6.1/examples/Example - Reproducing 2005.06787.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/Example - Reproducing 2103-03074.ipynb` & `cotengra-0.6.1/examples/Example - Reproducing 2103-03074.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/Quantum Circuit Example Old.ipynb` & `cotengra-0.6.1/examples/Quantum Circuit Example Old.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/Quantum Circuit Example.ipynb` & `cotengra-0.6.1/examples/Quantum Circuit Example.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/circuit_n53_m10_s0_e0_pABCDCDAB.qsim` & `cotengra-0.6.1/examples/circuit_n53_m10_s0_e0_pABCDCDAB.qsim`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/circuit_n53_m12_s0_e0_pABCDCDAB.qsim` & `cotengra-0.6.1/examples/circuit_n53_m12_s0_e0_pABCDCDAB.qsim`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/circuit_n53_m20_s0_e0_pABCDCDAB.qsim` & `cotengra-0.6.1/examples/circuit_n53_m20_s0_e0_pABCDCDAB.qsim`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/ex_jax.py` & `cotengra-0.6.1/examples/ex_jax.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/ex_mpi_executor.py` & `cotengra-0.6.1/examples/ex_mpi_executor.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/examples/ex_mpi_spmd.py` & `cotengra-0.6.1/examples/ex_mpi_spmd.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/pyproject.toml` & `cotengra-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/setup.py` & `cotengra-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     packages=find_packages(exclude=["docs", "tests"]),
     include_package_data=True,
     install_requires=[
         "autoray",
     ],
     extras_require={
         "recommended": [
-            "cotengrust",
+            "cotengrust>=0.1.3",
             "cytoolz",
             "kahypar",
             "networkx",
             "numpy",
             "opt_einsum",
             "optuna",
             "ray",
@@ -72,10 +72,11 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords="tensor network contraction graph hypergraph partition einsum",
 )
```

### Comparing `cotengra-0.6.0/src/lib.rs` & `cotengra-0.6.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/tests/test_compressed.py` & `cotengra-0.6.1/tests/test_compressed.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,11 +63,11 @@
     chi = 16
     minimize = ctg.scoring.CompressedPeakObjective(chi)
     inputs, output, _, size_dict = ctg.utils.lattice_equation([16, 16])
     tree = ctg.array_contract_tree(
         inputs,
         output,
         size_dict,
-        optimize=ctg.path_greedy.GreedyCompressed(chi),
+        optimize=ctg.path_compressed_greedy.GreedyCompressed(chi),
     )
     tree_wr = tree.windowed_reconfigure(minimize, order_only=order_only)
     assert tree_wr.peak_size(chi) < tree.peak_size(chi)
```

### Comparing `cotengra-0.6.0/tests/test_compute.py` & `cotengra-0.6.1/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/tests/test_hypergraph.py` & `cotengra-0.6.1/tests/test_hypergraph.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/tests/test_interface.py` & `cotengra-0.6.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/tests/test_optimizers.py` & `cotengra-0.6.1/tests/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/tests/test_paths_basic.py` & `cotengra-0.6.1/tests/test_paths_basic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import pytest
 import numpy as np
+import pytest
 from numpy.testing import assert_allclose
+
 import cotengra as ctg
 import cotengra.pathfinders.path_basic as pb
 
-
 # these are taken from opt_einsum
 test_case_eqs = [
     # Test scalar-like operations
     "a,->a",
     "ab,->ab",
     ",ab,->ab",
     ",,->",
@@ -97,17 +97,15 @@
     size_dict = ctg.utils.make_rand_size_dict_from_inputs(inputs)
     arrays = ctg.utils.make_arrays_from_inputs(inputs, size_dict)
     expected = np.einsum(eq, *arrays, optimize=True)
 
     path = {
         "greedy": pb.optimize_greedy,
         "optimal": pb.optimize_optimal,
-    }[
-        which
-    ](inputs, output, size_dict)
+    }[which](inputs, output, size_dict)
     tree = ctg.ContractionTree.from_path(inputs, output, size_dict, path=path)
     assert_allclose(tree.contract(arrays), expected)
 
 
 @pytest.mark.parametrize("seed", range(10))
 @pytest.mark.parametrize("which", ["greedy", "optimal"])
 def test_basic_rand(seed, which):
@@ -122,39 +120,66 @@
         seed=seed,
     )
     eq = ctg.utils.inputs_output_to_eq(inputs, output)
 
     path = {
         "greedy": pb.optimize_greedy,
         "optimal": pb.optimize_optimal,
-    }[
-        which
-    ](inputs, output, size_dict)
+    }[which](inputs, output, size_dict)
 
     tree = ctg.ContractionTree.from_path(inputs, output, size_dict, path=path)
     arrays = [np.random.randn(*s) for s in shapes]
     assert_allclose(
         tree.contract(arrays), np.einsum(eq, *arrays, optimize=True)
     )
 
 
+@pytest.mark.parametrize("seed", range(3))
+def test_random_greedy_track_flops(seed):
+    inputs, output, _, size_dict = ctg.utils.lattice_equation(
+        [4, 5],
+        d_min=2,
+        d_max=3,
+        seed=seed,
+    )
+    opt = ctg.RandomGreedyOptimizer(
+        max_repeats=2,
+        temperature=0.1,
+        seed=seed,
+        accel=False,
+        parallel=False,
+    )
+    path = opt(inputs, output, size_dict)
+    tree = ctg.ContractionTree.from_path(inputs, output, size_dict, path=path)
+    assert tree.contraction_cost(log=10) == pytest.approx(opt.best_flops)
+    # check deterministic
+    opt2 = ctg.RandomGreedyOptimizer(
+        max_repeats=2,
+        temperature=0.1,
+        seed=seed,
+        accel=False,
+        parallel=False,
+    )
+    opt2(inputs, output, size_dict)
+    assert opt.best_ssa_path == opt2.best_ssa_path
+    assert opt.best_flops == opt2.best_flops
+
+
 @pytest.mark.parametrize("seed", range(10))
 @pytest.mark.parametrize("which", ["greedy", "optimal"])
 def test_basic_perverse(seed, which):
     inputs, output, shapes, size_dict = ctg.utils.perverse_equation(
         10, seed=seed
     )
     eq = ctg.utils.inputs_output_to_eq(inputs, output)
     print(eq)
     path = {
         "greedy": pb.optimize_greedy,
         "optimal": pb.optimize_optimal,
-    }[
-        which
-    ](inputs, output, size_dict)
+    }[which](inputs, output, size_dict)
     tree = ctg.ContractionTree.from_path(inputs, output, size_dict, path=path)
     arrays = [np.random.randn(*s) for s in shapes]
     assert_allclose(
         tree.contract(arrays), np.einsum(eq, *arrays, optimize=True)
     )
```

### Comparing `cotengra-0.6.0/tests/test_slicer.py` & `cotengra-0.6.1/tests/test_slicer.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.0/tests/test_tree.py` & `cotengra-0.6.1/tests/test_tree.py`

 * *Files identical despite different names*

