# Comparing `tmp/lbmpy-1.3.3.tar.gz` & `tmp/lbmpy-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbmpy-1.3.3.tar", last modified: Sat Jan  6 16:05:07 2024, max compression
+gzip compressed data, was "lbmpy-1.3.4.tar", last modified: Wed May 15 07:47:00 2024, max compression
```

## Comparing `lbmpy-1.3.3.tar` & `lbmpy-1.3.4.tar`

### file list

```diff
@@ -1,127 +1,187 @@
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.616006 lbmpy-1.3.3/
--rw-r--r--   0 holzer     (502) staff       (20)      441 2024-01-06 15:48:19.000000 lbmpy-1.3.3/AUTHORS.txt
--rw-r--r--   0 holzer     (502) staff       (20)      281 2024-01-06 15:48:19.000000 lbmpy-1.3.3/CONTRIBUTING.md
--rw-r--r--   0 holzer     (502) staff       (20)    34913 2024-01-06 15:48:19.000000 lbmpy-1.3.3/COPYING.txt
--rw-r--r--   0 holzer     (502) staff       (20)      151 2024-01-06 15:48:19.000000 lbmpy-1.3.3/MANIFEST.in
--rw-r--r--   0 holzer     (502) staff       (20)     4960 2024-01-06 16:05:07.616082 lbmpy-1.3.3/PKG-INFO
--rw-r--r--   0 holzer     (502) staff       (20)     3840 2024-01-06 15:48:19.000000 lbmpy-1.3.3/README.md
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.616639 lbmpy-1.3.3/lbmpy/
--rw-r--r--   0 holzer     (502) staff       (20)     1625 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)      497 2024-01-06 16:05:07.616671 lbmpy-1.3.3/lbmpy/_version.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.604200 lbmpy-1.3.3/lbmpy/advanced_streaming/
--rw-r--r--   0 holzer     (502) staff       (20)      530 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/advanced_streaming/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     9867 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/advanced_streaming/communication.py
--rw-r--r--   0 holzer     (502) staff       (20)     7404 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/advanced_streaming/indexing.py
--rw-r--r--   0 holzer     (502) staff       (20)     4558 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/advanced_streaming/utility.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.604893 lbmpy-1.3.3/lbmpy/boundaries/
--rw-r--r--   0 holzer     (502) staff       (20)      615 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/boundaries/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     4807 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/boundaries/boundaries_in_kernel.py
--rw-r--r--   0 holzer     (502) staff       (20)    43335 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/boundaries/boundaryconditions.py
--rw-r--r--   0 holzer     (502) staff       (20)     9750 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/boundaries/boundaryhandling.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.605757 lbmpy-1.3.3/lbmpy/chapman_enskog/
--rw-r--r--   0 holzer     (502) staff       (20)      403 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/chapman_enskog/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    27639 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/chapman_enskog/chapman_enskog.py
--rw-r--r--   0 holzer     (502) staff       (20)     4846 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/chapman_enskog/chapman_enskog_higher_order.py
--rw-r--r--   0 holzer     (502) staff       (20)    14666 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/chapman_enskog/chapman_enskog_steady_state.py
--rw-r--r--   0 holzer     (502) staff       (20)     1154 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/chapman_enskog/derivative.py
--rw-r--r--   0 holzer     (502) staff       (20)     6620 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/continuous_distribution_measures.py
--rw-r--r--   0 holzer     (502) staff       (20)    47299 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/creationfunctions.py
--rw-r--r--   0 holzer     (502) staff       (20)     7942 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/cumulants.py
--rw-r--r--   0 holzer     (502) staff       (20)     4093 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/custom_code_nodes.py
--rw-r--r--   0 holzer     (502) staff       (20)     1681 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/db.py
--rw-r--r--   0 holzer     (502) staff       (20)     9618 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/enums.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.606592 lbmpy-1.3.3/lbmpy/equilibrium/
--rw-r--r--   0 holzer     (502) staff       (20)     1037 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/equilibrium/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    12418 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/equilibrium/abstract_equilibrium.py
--rw-r--r--   0 holzer     (502) staff       (20)    11897 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/equilibrium/continuous_hydro_maxwellian.py
--rw-r--r--   0 holzer     (502) staff       (20)     7081 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/equilibrium/discrete_hydro_maxwellian.py
--rw-r--r--   0 holzer     (502) staff       (20)     4334 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/equilibrium/generic_discrete_equilibrium.py
--rw-r--r--   0 holzer     (502) staff       (20)    13243 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/fieldaccess.py
--rw-r--r--   0 holzer     (502) staff       (20)     4297 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/fluctuatinglb.py
--rw-r--r--   0 holzer     (502) staff       (20)    25530 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/forcemodels.py
--rw-r--r--   0 holzer     (502) staff       (20)    11833 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/geometry.py
--rw-r--r--   0 holzer     (502) staff       (20)     2860 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/innerloopsplit.py
--rw-r--r--   0 holzer     (502) staff       (20)    22102 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/lbstep.py
--rw-r--r--   0 holzer     (502) staff       (20)    12921 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/macroscopic_value_kernels.py
--rw-r--r--   0 holzer     (502) staff       (20)     5813 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/max_domain_size_info.py
--rw-r--r--   0 holzer     (502) staff       (20)    11639 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/maxwellian_equilibrium.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.607553 lbmpy-1.3.3/lbmpy/methods/
--rw-r--r--   0 holzer     (502) staff       (20)     1400 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     5085 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/abstractlbmethod.py
--rw-r--r--   0 holzer     (502) staff       (20)    24119 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/conservedquantitycomputation.py
--rw-r--r--   0 holzer     (502) staff       (20)    42178 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/creationfunctions.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.608500 lbmpy-1.3.3/lbmpy/methods/cumulantbased/
--rw-r--r--   0 holzer     (502) staff       (20)      272 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/cumulantbased/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     1711 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/cumulantbased/cumulant_simplifications.py
--rw-r--r--   0 holzer     (502) staff       (20)    20343 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/cumulantbased/cumulantbasedmethod.py
--rw-r--r--   0 holzer     (502) staff       (20)    11391 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/cumulantbased/fourth_order_correction.py
--rw-r--r--   0 holzer     (502) staff       (20)     3918 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/cumulantbased/galilean_correction.py
--rw-r--r--   0 holzer     (502) staff       (20)     9813 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/default_moment_sets.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.609436 lbmpy-1.3.3/lbmpy/methods/momentbased/
--rw-r--r--   0 holzer     (502) staff       (20)      206 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/momentbased/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    19775 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/momentbased/centralmomentbasedmethod.py
--rw-r--r--   0 holzer     (502) staff       (20)    14484 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/momentbased/entropic.py
--rw-r--r--   0 holzer     (502) staff       (20)    20410 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/momentbased/momentbasedmethod.py
--rw-r--r--   0 holzer     (502) staff       (20)    16613 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/methods/momentbased/momentbasedsimplifications.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.610507 lbmpy-1.3.3/lbmpy/moment_transforms/
--rw-r--r--   0 holzer     (502) staff       (20)     1601 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/moment_transforms/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     6494 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/moment_transforms/abstractmomenttransform.py
--rw-r--r--   0 holzer     (502) staff       (20)    51672 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/moment_transforms/centralmomenttransforms.py
--rw-r--r--   0 holzer     (502) staff       (20)     9516 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/moment_transforms/cumulanttransforms.py
--rw-r--r--   0 holzer     (502) staff       (20)    21505 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/moment_transforms/rawmomenttransforms.py
--rw-r--r--   0 holzer     (502) staff       (20)    33288 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/moments.py
--rw-r--r--   0 holzer     (502) staff       (20)     3532 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/non_newtonian_models.py
--rw-r--r--   0 holzer     (502) staff       (20)     9642 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/oldroydb.py
--rw-r--r--   0 holzer     (502) staff       (20)    12414 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/parameterization.py
--rw-r--r--   0 holzer     (502) staff       (20)     4400 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/partially_saturated_cells.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.613925 lbmpy-1.3.3/lbmpy/phasefield/
--rw-r--r--   0 holzer     (502) staff       (20)        0 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    16242 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/analytical.py
--rw-r--r--   0 holzer     (502) staff       (20)     1881 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/cahn_hilliard_lbm.py
--rw-r--r--   0 holzer     (502) staff       (20)     5916 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/contact_angle_circle_fitting.py
--rw-r--r--   0 holzer     (502) staff       (20)     4102 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/eos.py
--rw-r--r--   0 holzer     (502) staff       (20)     7387 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/experiments1D.py
--rw-r--r--   0 holzer     (502) staff       (20)     4153 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/experiments2D.py
--rw-r--r--   0 holzer     (502) staff       (20)     1460 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/fd_stencils.py
--rw-r--r--   0 holzer     (502) staff       (20)     2581 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/high_density_ratio_model.py
--rw-r--r--   0 holzer     (502) staff       (20)     6205 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/kerneleqs.py
--rw-r--r--   0 holzer     (502) staff       (20)    12474 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/n_phase_boyer.py
--rw-r--r--   0 holzer     (502) staff       (20)    10740 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/nphase_nestler.py
--rw-r--r--   0 holzer     (502) staff       (20)    16274 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/phasefieldstep.py
--rw-r--r--   0 holzer     (502) staff       (20)     8719 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/phasefieldstep_direct.py
--rw-r--r--   0 holzer     (502) staff       (20)     7950 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/post_processing.py
--rw-r--r--   0 holzer     (502) staff       (20)     4197 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/scenarios.py
--rw-r--r--   0 holzer     (502) staff       (20)   299145 2024-01-06 16:05:07.000000 lbmpy-1.3.3/lbmpy/phasefield/simplex_projection.c
--rw-r--r--   0 holzer     (502) staff       (20)     3286 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield/simplex_projection.pyx
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.615126 lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/
--rw-r--r--   0 holzer     (502) staff       (20)        0 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     3499 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/analytical.py
--rw-r--r--   0 holzer     (502) staff       (20)     3021 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/contact_angle.py
--rw-r--r--   0 holzer     (502) staff       (20)     4122 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/derivatives.py
--rw-r--r--   0 holzer     (502) staff       (20)    18998 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/kernel_equations.py
--rw-r--r--   0 holzer     (502) staff       (20)     5679 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/numerical_solver.py
--rw-r--r--   0 holzer     (502) staff       (20)    19092 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/parameter_calculation.py
--rw-r--r--   0 holzer     (502) staff       (20)     7451 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/plot.py
--rw-r--r--   0 holzer     (502) staff       (20)      787 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/postprocessing.py
--rw-r--r--   0 holzer     (502) staff       (20)     4696 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/quadratic_equilibrium_construction.py
--rw-r--r--   0 holzer     (502) staff       (20)     2852 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/relaxationrates.py
--rw-r--r--   0 holzer     (502) staff       (20)     9095 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/scenarios.py
--rw-r--r--   0 holzer     (502) staff       (20)      601 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/session.py
--rw-r--r--   0 holzer     (502) staff       (20)     4111 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/simplificationfactory.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.615843 lbmpy-1.3.3/lbmpy/sparse/
--rw-r--r--   0 holzer     (502) staff       (20)      452 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/sparse/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    10642 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/sparse/mapping.py
--rw-r--r--   0 holzer     (502) staff       (20)     3945 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/sparse/update_rule_sparse.py
--rw-r--r--   0 holzer     (502) staff       (20)    12074 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/stencils.py
--rw-r--r--   0 holzer     (502) staff       (20)     3214 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/turbulence_models.py
--rw-r--r--   0 holzer     (502) staff       (20)     7158 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/updatekernels.py
--rw-r--r--   0 holzer     (502) staff       (20)     1371 2024-01-06 15:48:19.000000 lbmpy-1.3.3/lbmpy/utils.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 16:05:07.603514 lbmpy-1.3.3/lbmpy.egg-info/
--rw-r--r--   0 holzer     (502) staff       (20)     4960 2024-01-06 16:05:07.000000 lbmpy-1.3.3/lbmpy.egg-info/PKG-INFO
--rw-r--r--   0 holzer     (502) staff       (20)     3680 2024-01-06 16:05:07.000000 lbmpy-1.3.3/lbmpy.egg-info/SOURCES.txt
--rw-r--r--   0 holzer     (502) staff       (20)        1 2024-01-06 16:05:07.000000 lbmpy-1.3.3/lbmpy.egg-info/dependency_links.txt
--rw-r--r--   0 holzer     (502) staff       (20)      322 2024-01-06 16:05:07.000000 lbmpy-1.3.3/lbmpy.egg-info/requires.txt
--rw-r--r--   0 holzer     (502) staff       (20)        6 2024-01-06 16:05:07.000000 lbmpy-1.3.3/lbmpy.egg-info/top_level.txt
--rw-r--r--   0 holzer     (502) staff       (20)      202 2024-01-06 16:05:07.616376 lbmpy-1.3.3/setup.cfg
--rw-r--r--   0 holzer     (502) staff       (20)     4026 2024-01-06 15:48:19.000000 lbmpy-1.3.3/setup.py
--rw-r--r--   0 holzer     (502) staff       (20)    70144 2024-01-06 15:48:19.000000 lbmpy-1.3.3/versioneer.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.348848 lbmpy-1.3.4/
+-rw-r--r--   0 holzer     (502) staff       (20)      441 2024-05-15 07:41:23.000000 lbmpy-1.3.4/AUTHORS.txt
+-rw-r--r--   0 holzer     (502) staff       (20)      117 2024-05-15 07:41:23.000000 lbmpy-1.3.4/CHANGELOG.md
+-rw-r--r--   0 holzer     (502) staff       (20)      281 2024-05-15 07:41:23.000000 lbmpy-1.3.4/CONTRIBUTING.md
+-rw-r--r--   0 holzer     (502) staff       (20)    34913 2024-05-15 07:41:23.000000 lbmpy-1.3.4/COPYING.txt
+-rw-r--r--   0 holzer     (502) staff       (20)       65 2024-05-15 07:41:23.000000 lbmpy-1.3.4/MANIFEST.in
+-rw-r--r--   0 holzer     (502) staff       (20)    45223 2024-05-15 07:47:00.348651 lbmpy-1.3.4/PKG-INFO
+-rw-r--r--   0 holzer     (502) staff       (20)     3840 2024-05-15 07:41:23.000000 lbmpy-1.3.4/README.md
+-rw-r--r--   0 holzer     (502) staff       (20)     2257 2024-05-15 07:41:23.000000 lbmpy-1.3.4/pyproject.toml
+-rw-r--r--   0 holzer     (502) staff       (20)       38 2024-05-15 07:47:00.348921 lbmpy-1.3.4/setup.cfg
+-rw-r--r--   0 holzer     (502) staff       (20)      661 2024-05-15 07:41:23.000000 lbmpy-1.3.4/setup.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.316488 lbmpy-1.3.4/src/
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.327532 lbmpy-1.3.4/src/lbmpy/
+-rw-r--r--   0 holzer     (502) staff       (20)     1698 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)      497 2024-05-15 07:47:00.349066 lbmpy-1.3.4/src/lbmpy/_version.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.328958 lbmpy-1.3.4/src/lbmpy/advanced_streaming/
+-rw-r--r--   0 holzer     (502) staff       (20)      530 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/advanced_streaming/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9868 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/advanced_streaming/communication.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7404 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/advanced_streaming/indexing.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4558 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/advanced_streaming/utility.py
+-rw-r--r--   0 holzer     (502) staff       (20)      789 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/analytical_solutions.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.329758 lbmpy-1.3.4/src/lbmpy/boundaries/
+-rw-r--r--   0 holzer     (502) staff       (20)      851 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/boundaries/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4807 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/boundaries/boundaries_in_kernel.py
+-rw-r--r--   0 holzer     (502) staff       (20)    57519 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/boundaries/boundaryconditions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9750 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/boundaries/boundaryhandling.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7476 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/boundaries/wall_function_models.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.330539 lbmpy-1.3.4/src/lbmpy/chapman_enskog/
+-rw-r--r--   0 holzer     (502) staff       (20)      403 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/chapman_enskog/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    27639 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/chapman_enskog/chapman_enskog.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4846 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/chapman_enskog/chapman_enskog_higher_order.py
+-rw-r--r--   0 holzer     (502) staff       (20)    14666 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/chapman_enskog/chapman_enskog_steady_state.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1154 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/chapman_enskog/derivative.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6620 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/continuous_distribution_measures.py
+-rw-r--r--   0 holzer     (502) staff       (20)    47937 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/creationfunctions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7942 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/cumulants.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3892 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/custom_code_nodes.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1719 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/db.py
+-rw-r--r--   0 holzer     (502) staff       (20)    10000 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/enums.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.331285 lbmpy-1.3.4/src/lbmpy/equilibrium/
+-rw-r--r--   0 holzer     (502) staff       (20)     1037 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/equilibrium/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12418 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/equilibrium/abstract_equilibrium.py
+-rw-r--r--   0 holzer     (502) staff       (20)    11897 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/equilibrium/continuous_hydro_maxwellian.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7081 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/equilibrium/discrete_hydro_maxwellian.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4334 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/equilibrium/generic_discrete_equilibrium.py
+-rw-r--r--   0 holzer     (502) staff       (20)    13243 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/fieldaccess.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3764 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/flow_statistics.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4297 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/fluctuatinglb.py
+-rw-r--r--   0 holzer     (502) staff       (20)    25530 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/forcemodels.py
+-rw-r--r--   0 holzer     (502) staff       (20)    11833 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/geometry.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2860 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/innerloopsplit.py
+-rw-r--r--   0 holzer     (502) staff       (20)    22188 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/lbstep.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12921 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/macroscopic_value_kernels.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5813 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/max_domain_size_info.py
+-rw-r--r--   0 holzer     (502) staff       (20)    11680 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/maxwellian_equilibrium.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.332119 lbmpy-1.3.4/src/lbmpy/methods/
+-rw-r--r--   0 holzer     (502) staff       (20)     1400 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5085 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/abstractlbmethod.py
+-rw-r--r--   0 holzer     (502) staff       (20)    24119 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/conservedquantitycomputation.py
+-rw-r--r--   0 holzer     (502) staff       (20)    42178 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/creationfunctions.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.332884 lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/
+-rw-r--r--   0 holzer     (502) staff       (20)      272 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1711 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/cumulant_simplifications.py
+-rw-r--r--   0 holzer     (502) staff       (20)    20343 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/cumulantbasedmethod.py
+-rw-r--r--   0 holzer     (502) staff       (20)    11391 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/fourth_order_correction.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3918 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/galilean_correction.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9813 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/default_moment_sets.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.333665 lbmpy-1.3.4/src/lbmpy/methods/momentbased/
+-rw-r--r--   0 holzer     (502) staff       (20)      206 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/momentbased/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    19775 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/momentbased/centralmomentbasedmethod.py
+-rw-r--r--   0 holzer     (502) staff       (20)    14484 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/momentbased/entropic.py
+-rw-r--r--   0 holzer     (502) staff       (20)    20410 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/momentbased/momentbasedmethod.py
+-rw-r--r--   0 holzer     (502) staff       (20)    16613 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/methods/momentbased/momentbasedsimplifications.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.334508 lbmpy-1.3.4/src/lbmpy/moment_transforms/
+-rw-r--r--   0 holzer     (502) staff       (20)     1601 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/moment_transforms/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6494 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/moment_transforms/abstractmomenttransform.py
+-rw-r--r--   0 holzer     (502) staff       (20)    51672 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/moment_transforms/centralmomenttransforms.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9516 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/moment_transforms/cumulanttransforms.py
+-rw-r--r--   0 holzer     (502) staff       (20)    21505 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/moment_transforms/rawmomenttransforms.py
+-rw-r--r--   0 holzer     (502) staff       (20)    33288 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/moments.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3532 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/non_newtonian_models.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9579 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/oldroydb.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12414 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/parameterization.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4400 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/partially_saturated_cells.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.337016 lbmpy-1.3.4/src/lbmpy/phasefield/
+-rw-r--r--   0 holzer     (502) staff       (20)        0 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    16242 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/analytical.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1881 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/cahn_hilliard_lbm.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5916 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/contact_angle_circle_fitting.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4102 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/eos.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7387 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/experiments1D.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4153 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/experiments2D.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1460 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/fd_stencils.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2581 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/high_density_ratio_model.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6205 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/kerneleqs.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12474 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/n_phase_boyer.py
+-rw-r--r--   0 holzer     (502) staff       (20)    10625 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/nphase_nestler.py
+-rw-r--r--   0 holzer     (502) staff       (20)    16274 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/phasefieldstep.py
+-rw-r--r--   0 holzer     (502) staff       (20)     8719 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/phasefieldstep_direct.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7950 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/post_processing.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4197 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield/scenarios.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.338241 lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/
+-rw-r--r--   0 holzer     (502) staff       (20)        0 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3499 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/analytical.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3021 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/contact_angle.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4122 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/derivatives.py
+-rw-r--r--   0 holzer     (502) staff       (20)    18998 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/kernel_equations.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5679 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/numerical_solver.py
+-rw-r--r--   0 holzer     (502) staff       (20)    19092 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/parameter_calculation.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7451 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/plot.py
+-rw-r--r--   0 holzer     (502) staff       (20)      787 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/postprocessing.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4696 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/quadratic_equilibrium_construction.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2852 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/relaxationrates.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9095 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/scenarios.py
+-rw-r--r--   0 holzer     (502) staff       (20)      601 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/session.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4111 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/simplificationfactory.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.338749 lbmpy-1.3.4/src/lbmpy/sparse/
+-rw-r--r--   0 holzer     (502) staff       (20)      452 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/sparse/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    10642 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/sparse/mapping.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3945 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/sparse/update_rule_sparse.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12602 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/stencils.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7631 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/turbulence_models.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7158 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/updatekernels.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1371 2024-05-15 07:41:23.000000 lbmpy-1.3.4/src/lbmpy/utils.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.328347 lbmpy-1.3.4/src/lbmpy.egg-info/
+-rw-r--r--   0 holzer     (502) staff       (20)    45223 2024-05-15 07:47:00.000000 lbmpy-1.3.4/src/lbmpy.egg-info/PKG-INFO
+-rw-r--r--   0 holzer     (502) staff       (20)     5881 2024-05-15 07:47:00.000000 lbmpy-1.3.4/src/lbmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 holzer     (502) staff       (20)        1 2024-05-15 07:47:00.000000 lbmpy-1.3.4/src/lbmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 holzer     (502) staff       (20)      459 2024-05-15 07:47:00.000000 lbmpy-1.3.4/src/lbmpy.egg-info/requires.txt
+-rw-r--r--   0 holzer     (502) staff       (20)        6 2024-05-15 07:47:00.000000 lbmpy-1.3.4/src/lbmpy.egg-info/top_level.txt
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:47:00.348384 lbmpy-1.3.4/tests/
+-rw-r--r--   0 holzer     (502) staff       (20)    18681 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_boundary_handling.py
+-rw-r--r--   0 holzer     (502) staff       (20)      651 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_builtin_periodicity.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4609 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_central_moment.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2216 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_central_moment_equivalences.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3839 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_central_moment_transform.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9413 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_chapman_enskog.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6508 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_conserved_quantity_relaxation_invariance.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2353 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_cpu_gpu_equivalence.py
+-rw-r--r--   0 holzer     (502) staff       (20)      930 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_cumulant_equivalences.py
+-rw-r--r--   0 holzer     (502) staff       (20)      665 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_cumulant_methods.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1324 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_cumulant_transform.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3072 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_cumulants.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2025 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_density_velocity_input.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6367 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_diffusion.py
+-rw-r--r--   0 holzer     (502) staff       (20)      935 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_entropic.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5593 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_extrapolation_outflow.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1921 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_float_kernel.py
+-rw-r--r--   0 holzer     (502) staff       (20)    14853 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_fluctuating_lb.py
+-rw-r--r--   0 holzer     (502) staff       (20)    19015 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_force.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1181 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_force_on_boundary.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2961 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_free_slip.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2436 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_geometry_setup_serial.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1003 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_gpu_block_size_limiting.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1811 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_html_output.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5687 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_hydro_maxwellian_class.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5721 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_interpolation_boundaries.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1752 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_json_serializer.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4571 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_lbstep.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6985 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_lees_edwards.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4470 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_macroscopic_value_kernels.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5858 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_maxwellian_equilibrium.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1586 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_moment_transform_api.py
+-rw-r--r--   0 holzer     (502) staff       (20)    10353 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_momentbased_equivalences.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6187 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_momentbased_methods_equilibrium.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3213 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_moments.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1344 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_mrt_simplifications.py
+-rwxr-xr-x   0 holzer     (502) staff       (20)    11064 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_oldroydb.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1528 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_plot.py
+-rw-r--r--   0 holzer     (502) staff       (20)      971 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_poisuille_channel.py
+-rw-r--r--   0 holzer     (502) staff       (20)      562 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_postprocessing.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1384 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_quicktests.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1591 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_relaxation_rate.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2177 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_scaling_widget.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7348 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_shear_flow.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2922 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_shifted_transforms.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1638 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_simple_equilibrium_conservation.py
+-rw-r--r--   0 holzer     (502) staff       (20)      899 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_smagorinsky.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4178 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_split_optimization.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3678 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_srt_trt_simplifications.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3158 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_stencils.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1569 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_update_kernel.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3691 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_vectorization.py
+-rw-r--r--   0 holzer     (502) staff       (20)      270 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_version_string.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5360 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_wall_function_bounce.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1592 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_weights.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2586 2024-05-15 07:41:23.000000 lbmpy-1.3.4/tests/test_zero_centering.py
```

### Comparing `lbmpy-1.3.3/COPYING.txt` & `lbmpy-1.3.4/COPYING.txt`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/PKG-INFO` & `lbmpy-1.3.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: lbmpy
-Version: 1.3.3
-Summary: Code Generation for Lattice Boltzmann Methods
-Home-page: https://i10git.cs.fau.de/pycodegen/lbmpy/
-Author: Martin Bauer, Markus Holzer, Frederik Hennig
-Author-email: cs10-codegen@fau.de
-License: AGPLv3
-Project-URL: Bug Tracker, https://i10git.cs.fau.de/pycodegen/lbmpy/-/issues
-Project-URL: Documentation, https://pycodegen.pages.i10git.cs.fau.de/lbmpy/
-Project-URL: Source Code, https://i10git.cs.fau.de/pycodegen/lbmpy
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Jupyter
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: gpu
-Provides-Extra: opencl
-Provides-Extra: alltrafos
-Provides-Extra: interactive
-Provides-Extra: doc
-Provides-Extra: phasefield
-License-File: COPYING.txt
-License-File: AUTHORS.txt
-
 lbmpy
 =====
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mabau/lbmpy/master?filepath=doc%2Fnotebooks)
 [![Docs](https://img.shields.io/badge/read-the_docs-brightgreen.svg)](http://pycodegen.pages.i10git.cs.fau.de/lbmpy)
 [![pipeline status](https://i10git.cs.fau.de/pycodegen/lbmpy/badges/master/pipeline.svg)](https://i10git.cs.fau.de/pycodegen/lbmpy/commits/master)
 [![coverage report](https://i10git.cs.fau.de/pycodegen/lbmpy/badges/master/coverage.svg)](http://pycodegen.pages.i10git.cs.fau.de/lbmpy/coverage_report)
```

### Comparing `lbmpy-1.3.3/lbmpy/advanced_streaming/__init__.py` & `lbmpy-1.3.4/src/lbmpy/advanced_streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/advanced_streaming/communication.py` & `lbmpy-1.3.4/src/lbmpy/advanced_streaming/communication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import itertools
 from pystencils import CreateKernelConfig, Field, Assignment, AssignmentCollection
 from pystencils.slicing import shift_slice, get_slice_before_ghost_layer, normalize_slice
-from lbmpy.advanced_streaming.utility import is_inplace, get_accessor, numeric_index,\
+from lbmpy.advanced_streaming.utility import is_inplace, get_accessor, numeric_index, \
     Timestep, get_timesteps, numeric_offsets
 from pystencils.datahandling import SerialDataHandling
 from pystencils.enums import Target
 from itertools import chain
 
 
 class LBMPeriodicityHandling:
```

### Comparing `lbmpy-1.3.3/lbmpy/advanced_streaming/indexing.py` & `lbmpy-1.3.4/src/lbmpy/advanced_streaming/indexing.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/advanced_streaming/utility.py` & `lbmpy-1.3.4/src/lbmpy/advanced_streaming/utility.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/boundaries/__init__.py` & `lbmpy-1.3.4/src/lbmpy/boundaries/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from lbmpy.boundaries.boundaryconditions import (
-    UBB, FixedDensity, DiffusionDirichlet, SimpleExtrapolationOutflow,
+    UBB, FixedDensity, DiffusionDirichlet, SimpleExtrapolationOutflow, WallFunctionBounce,
     ExtrapolationOutflow, NeumannByCopy, NoSlip, NoSlipLinearBouzidi, QuadraticBounceBack, StreamInConstant, FreeSlip)
 from lbmpy.boundaries.boundaryhandling import LatticeBoltzmannBoundaryHandling
+from lbmpy.boundaries.wall_function_models import MoninObukhovSimilarityTheory, LogLaw, MuskerLaw, SpaldingsLaw
 
-__all__ = ['NoSlip', 'NoSlipLinearBouzidi', 'QuadraticBounceBack', 'FreeSlip',
+__all__ = ['NoSlip', 'NoSlipLinearBouzidi', 'QuadraticBounceBack', 'FreeSlip', 'WallFunctionBounce',
            'UBB', 'FixedDensity',
            'SimpleExtrapolationOutflow', 'ExtrapolationOutflow',
            'DiffusionDirichlet', 'NeumannByCopy', 'StreamInConstant',
-           'LatticeBoltzmannBoundaryHandling']
+           'LatticeBoltzmannBoundaryHandling',
+           'MoninObukhovSimilarityTheory', 'LogLaw', 'MuskerLaw', 'SpaldingsLaw']
```

### Comparing `lbmpy-1.3.3/lbmpy/boundaries/boundaries_in_kernel.py` & `lbmpy-1.3.4/src/lbmpy/boundaries/boundaries_in_kernel.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/boundaries/boundaryconditions.py` & `lbmpy-1.3.4/src/lbmpy/boundaries/boundaryconditions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+from enum import Enum, auto
 from warnings import warn
 
 from pystencils import Assignment, Field
 from pystencils.simp.assignment_collection import AssignmentCollection
 from pystencils.stencil import offset_to_direction_string, direction_string_to_offset, inverse_direction
 from pystencils.sympyextensions import get_symmetric_part, simplify_by_equality, scalar_product
 from pystencils.typing import create_type, TypedSymbol
@@ -10,14 +11,15 @@
 from lbmpy.advanced_streaming.utility import AccessPdfValues, Timestep
 from lbmpy.custom_code_nodes import (NeighbourOffsetArrays, MirroredStencilDirections, LbmWeightInfo,
                                      TranslationArraysNode)
 from lbmpy.maxwellian_equilibrium import discrete_equilibrium
 from lbmpy.simplificationfactory import create_simplification_strategy
 
 import sympy as sp
+import numpy as np
 
 
 class LbBoundary(abc.ABC):
     """Base class that all boundaries should derive from.
 
     Args:
         name: optional name of the boundary.
@@ -93,17 +95,21 @@
         return self.__dict__ == other.__dict__
 
 
 # end class Boundary
 
 
 class NoSlip(LbBoundary):
-    """
+    r"""
     No-Slip, (half-way) simple bounce back boundary condition, enforcing zero velocity at obstacle.
-    Extended for use with any streaming pattern.
+    Populations leaving the boundary node :math:`\mathbf{x}_b` at time :math:`t` are reflected
+    back with :math:`\mathbf{c}_{\overline{i}} = -\mathbf{c}_{i}`
+
+    .. math ::
+        f_{\overline{i}}(\mathbf{x}_b, t + \Delta t) = f^{\star}_{i}(\mathbf{x}_b, t)
 
     Args:
         name: optional name of the boundary.
     """
 
     def __init__(self, name=None):
         """Set an optional name here, to mark boundaries, for example for force evaluations"""
@@ -236,27 +242,28 @@
         inv_directions = [str(stencil.index(inverse_direction(direction))) for direction in stencil]
         dtype = self.inv_dir_symbol.dtype
         name = self.inv_dir_symbol.name
         inverse_dir_node = TranslationArraysNode([(dtype, name, inv_directions), ], {self.inv_dir_symbol})
         return [LbmWeightInfo(lb_method, self.data_type), inverse_dir_node, NeighbourOffsetArrays(lb_method.stencil)]
 
     @staticmethod
-    def get_equilibrium(v, u, rho, drho, weight, compressible, deviation_only):
+    def get_equilibrium(v, u, rho, drho, weight, compressible, zero_centered):
         rho_background = sp.Integer(1)
 
         result = discrete_equilibrium(v, u, rho, weight,
                                       order=2, c_s_sq=sp.Rational(1, 3), compressible=compressible)
-        if deviation_only:
+        if zero_centered:
             shift = discrete_equilibrium(v, [0] * len(u), rho_background, weight,
                                          order=0, c_s_sq=sp.Rational(1, 3), compressible=False)
             result = simplify_by_equality(result - shift, rho, drho, rho_background)
 
         return result
 
     def __call__(self, f_out, f_in, dir_symbol, inv_dir, lb_method, index_field):
+        omega = self.relaxation_rate
         inv = sp.IndexedBase(self.inv_dir_symbol, shape=(1,))[dir_symbol]
         weight_info = LbmWeightInfo(lb_method, data_type=self.data_type)
         weight_of_direction = weight_info.weight_of_direction
         pdf_field_accesses = [f_out(i) for i in range(len(lb_method.stencil))]
 
         pdf_symbols = [sp.Symbol(f"pdf_{i}") for i in range(len(lb_method.stencil))]
         f_xf = sp.Symbol("f_xf")
@@ -264,15 +271,15 @@
         q = sp.Symbol("q")
         feq = sp.Symbol("f_eq")
         weight = sp.Symbol("w")
         weight_inv = sp.Symbol("w_inv")
         v = [TypedSymbol(f"c_{i}", self.data_type) for i in range(lb_method.stencil.D)]
         v_inv = [TypedSymbol(f"c_inv_{i}", self.data_type) for i in range(lb_method.stencil.D)]
         one = sp.Float(1.0)
-        two = sp.Float(2.0)
+        half = sp.Rational(1, 2)
 
         subexpressions = [Assignment(pdf_symbols[i], pdf) for i, pdf in enumerate(pdf_field_accesses)]
         subexpressions.append(Assignment(f_xf, f_out(dir_symbol)))
         subexpressions.append(Assignment(f_xf_inv, f_out(inv_dir[dir_symbol])))
         subexpressions.append(Assignment(q, index_field[0]('q')))
         subexpressions.append(Assignment(weight, weight_of_direction(dir_symbol, lb_method)))
         subexpressions.append(Assignment(weight_inv, weight_of_direction(inv, lb_method)))
@@ -286,32 +293,27 @@
             subexpressions.append(Assignment(v_inv[i], offset[i]))
 
         cqc = lb_method.conserved_quantity_computation
         rho = cqc.density_symbol
         drho = cqc.density_deviation_symbol
         u = sp.Matrix(cqc.velocity_symbols)
         compressible = cqc.compressible
-        deviation_only = lb_method.equilibrium_distribution.deviation_only
+        zero_centered = cqc.zero_centered_pdfs
 
         cqe = cqc.equilibrium_input_equations_from_pdfs(pdf_symbols, False)
         subexpressions.append(cqe.all_assignments)
 
-        eq_dir = self.get_equilibrium(v, u, rho, drho, weight, compressible, deviation_only)
-        eq_inv = self.get_equilibrium(v_inv, u, rho, drho, weight_inv, compressible, deviation_only)
+        eq_dir = self.get_equilibrium(v, u, rho, drho, weight, compressible, zero_centered)
+        eq_inv = self.get_equilibrium(v_inv, u, rho, drho, weight_inv, compressible, zero_centered)
 
         subexpressions.append(Assignment(feq, eq_dir + eq_inv))
 
-        # equation E.4 first summand
-        e41 = (f_xf_inv - f_xf) / two
-        # equation E.4 second summand
-        e42 = (f_xf_inv + f_xf - self.relaxation_rate * feq) / (two - two * self.relaxation_rate)
-        # equation E.3
-        fw = ((one - q) * (e41 + e42)) + q * f_xf_inv
-        # equation E.1
-        result = (one / (q + one)) * fw + (q / (q + one)) * f_xf
+        t1 = (f_xf - f_xf_inv + (f_xf + f_xf_inv - feq * omega) / (one - omega))
+        t2 = (q * (f_xf + f_xf_inv)) / (one + q)
+        result = (one - q) / (one + q) * t1 * half + t2
 
         boundary_assignments = [Assignment(f_in(inv_dir[dir_symbol]), result)]
         return AssignmentCollection(boundary_assignments, subexpressions=subexpressions)
 
 
 # end class QuadraticBounceBack
 
@@ -440,30 +442,275 @@
 
         return Assignment(f_in.center(inv_dir[dir_symbol]), f_out[tangential_offset](mirrored_direction))
 
 
 # end class FreeSlip
 
 
+class WallFunctionBounce(LbBoundary):
+    """
+    Wall function based on the bounce back idea, cf. :cite:`Han2021`. Its implementation is extended to the D3Q27
+    stencil, whereas different weights of the drag distribution are proposed.
+
+    Args:
+        lb_method: LB method which is used for the simulation
+        pdfs: Symbolic representation of the particle distribution functions.
+        normal_direction: Normal direction of the wall. Currently, only straight and axis-aligned walls are supported.
+        wall_function_model: Wall function that is used to retrieve the wall stress :math:`tau_w` during the simulation.
+                             See :class:`lbmpy.boundaries.wall_treatment.WallFunctionModel` for more details
+        mean_velocity: Optional field or field access for the mean velocity. As wall functions are typically defined
+                       in terms of the mean velocity, it is recommended to provide this variable. Per default, the
+                       instantaneous velocity obtained from pdfs is used for the wall function.
+        sampling_shift: Optional sampling shift for the velocity sampling. Can be provided as symbolic variable or
+                        integer. In both cases, the user must assure that the sampling shift is at least 1, as sampling
+                        in boundary cells is not physical. Per default, a sampling shift of 1 is employed which
+                        corresponds to a sampling in the first fluid cell normal to the wall. For lower friction
+                        Reynolds numbers, choosing a sampling shift >1 has shown to improve the results for higher
+                        resolutions.
+                        Mutually exclusive with the Maronga sampling shift.
+        maronga_sampling_shift: Optionally, apply a correction factor to the wall shear stress proposed by Maronga et
+                                al. :cite:`Maronga2020`. Has only been tested and validated for the MOST wall function.
+                                No guarantee is given that it also works with other wall functions.
+                                Mutually exclusive with the standard sampling shift.
+        dt: time discretisation. Usually one in LB units
+        dy: space discretisation. Usually one in LB units
+        y: distance from the wall
+        target_friction_velocity: A target friction velocity can be given if an estimate is known a priori. This target
+                                  friction velocity will be used as initial guess for implicit wall functions to ensure
+                                  convergence of the Newton algorithm.
+        weight_method: The extension of the WFB to a D3Q27 stencil is non-unique. Different weights can be chosen to
+                       define the drag distribution onto the pdfs. Per default, weights corresponding to the weights
+                       in the D3Q27 stencil are chosen.
+        name: Optional name of the boundary.
+        data_type: Floating-point precision. Per default, double.
+    """
+
+    class WeightMethod(Enum):
+        LATTICE_WEIGHT = auto(),
+        GEOMETRIC_WEIGHT = auto()
+
+    def __init__(self, lb_method, pdfs, normal_direction, wall_function_model,
+                 mean_velocity=None, sampling_shift=1, maronga_sampling_shift=None,
+                 dt=1, dy=1, y=0.5,
+                 target_friction_velocity=None,
+                 weight_method=WeightMethod.LATTICE_WEIGHT,
+                 name=None, data_type='double'):
+        """Set an optional name here, to mark boundaries, for example for force evaluations"""
+        self.stencil = lb_method.stencil
+        if not (self.stencil.Q == 19 or self.stencil.Q == 27):
+            raise ValueError("WFB boundary is currently only defined for D3Q19 and D3Q27 stencils.")
+        self.pdfs = pdfs
+
+        self.wall_function_model = wall_function_model
+
+        if mean_velocity:
+            if isinstance(mean_velocity, Field):
+                self.mean_velocity = mean_velocity.center_vector
+            elif isinstance(mean_velocity, Field.Access):
+                self.mean_velocity = mean_velocity.field.neighbor_vector(mean_velocity.offsets)
+            else:
+                raise ValueError("Mean velocity field has to be a pystencils Field or Field.Access")
+        else:
+            self.mean_velocity = None
+
+        if not isinstance(sampling_shift, int):
+            self.sampling_shift = TypedSymbol(sampling_shift.name, np.uint32)
+        else:
+            assert sampling_shift >= 1, "The sampling shift must be greater than 1."
+            self.sampling_shift = sampling_shift
+
+        if maronga_sampling_shift:
+            assert self.mean_velocity, "Mean velocity field must be provided when using the Maronga correction"
+            if not isinstance(maronga_sampling_shift, int):
+                self.maronga_sampling_shift = TypedSymbol(maronga_sampling_shift.name, np.uint32)
+            else:
+                assert maronga_sampling_shift >= 1, "The Maronga sampling shift must be greater than 1."
+                self.maronga_sampling_shift = maronga_sampling_shift
+        else:
+            self.maronga_sampling_shift = None
+
+        if (self.sampling_shift != 1) and self.maronga_sampling_shift:
+            raise ValueError("Both sampling shift and Maronga offset are set. This is currently not supported.")
+
+        self.dt = dt
+        self.dy = dy
+        self.y = y
+        self.data_type = data_type
+
+        self.target_friction_velocity = target_friction_velocity
+
+        self.weight_method = weight_method
+
+        if len(normal_direction) - normal_direction.count(0) != 1:
+            raise ValueError("Only normal directions for straight walls are supported for example (0, 1, 0) for "
+                             "a WallFunctionBounce applied to the southern boundary of the domain")
+
+        self.mirror_axis = normal_direction.index(*[direction for direction in normal_direction if direction != 0])
+
+        self.normal_direction = normal_direction
+        assert all([n in [-1, 0, 1] for n in self.normal_direction]), \
+            "Only -1, 0 and 1 allowed for defining the normal direction"
+        tangential_component = [int(not n) for n in self.normal_direction]
+        self.normal_axis = tangential_component.index(0)
+        self.tangential_axis = [0, 1, 2]
+        self.tangential_axis.remove(self.normal_axis)
+
+        self.dim = self.stencil.D
+
+        if name is None:
+            name = f"WFB : {offset_to_direction_string([-x for x in normal_direction])}"
+
+        super(WallFunctionBounce, self).__init__(name)
+
+    def get_additional_code_nodes(self, lb_method):
+        return [MirroredStencilDirections(self.stencil, self.mirror_axis),
+                NeighbourOffsetArrays(lb_method.stencil)]
+
+    def __call__(self, f_out, f_in, dir_symbol, inv_dir, lb_method, index_field):
+        # needed symbols for offsets and indices
+        # neighbour offset symbols are basically the stencil directions defined in stencils.py:L130ff.
+        neighbor_offset = NeighbourOffsetArrays.neighbour_offset(dir_symbol, lb_method.stencil)
+        tangential_offset = tuple(offset + normal for offset, normal in zip(neighbor_offset, self.normal_direction))
+        mirrored_stencil_symbol = MirroredStencilDirections._mirrored_symbol(self.mirror_axis)
+        mirrored_direction = inv_dir[sp.IndexedBase(mirrored_stencil_symbol, shape=(1,))[dir_symbol]]
+
+        name_base = "f_in_inv_offsets_"
+        offset_array_symbols = [TypedSymbol(name_base + d, mirrored_stencil_symbol.dtype) for d in ['x', 'y', 'z']]
+        mirrored_offset = sp.IndexedBase(mirrored_stencil_symbol, shape=(1,))[dir_symbol]
+        offsets = tuple(sp.IndexedBase(s, shape=(1,))[mirrored_offset] for s in offset_array_symbols)
+
+        # needed symbols in the Assignments
+        u_m = sp.Symbol("u_m")
+        tau_w = sp.Symbol("tau_w")
+        wall_stress = sp.symbols("tau_w_x tau_w_y tau_w_z")
+
+        # if the mean velocity field is not given, or the Maronga correction is applied, density and velocity values
+        # will be calculated from pdfs
+        cqc = lb_method.conserved_quantity_computation
+
+        result = []
+        if (not self.mean_velocity) or self.maronga_sampling_shift:
+            pdf_center_vector = sp.Matrix([0] * self.stencil.Q)
+
+            for i in range(self.stencil.Q):
+                pdf_center_vector[i] = self.pdfs[offsets[0] + self.normal_direction[0],
+                                                 offsets[1] + self.normal_direction[1],
+                                                 offsets[2] + self.normal_direction[2]](i)
+
+            eq_equations = cqc.equilibrium_input_equations_from_pdfs(pdf_center_vector)
+            result.append(eq_equations.all_assignments)
+
+        # sample velocity which will be used in the wall stress calculation
+        if self.mean_velocity:
+            if self.maronga_sampling_shift:
+                u_for_tau_wall = tuple(u_mean_i.get_shifted(
+                    self.maronga_sampling_shift * self.normal_direction[0],
+                    self.maronga_sampling_shift * self.normal_direction[1],
+                    self.maronga_sampling_shift * self.normal_direction[2]
+                ) for u_mean_i in self.mean_velocity)
+            else:
+                u_for_tau_wall = tuple(u_mean_i.get_shifted(
+                    self.sampling_shift * self.normal_direction[0],
+                    self.sampling_shift * self.normal_direction[1],
+                    self.sampling_shift * self.normal_direction[2]
+                ) for u_mean_i in self.mean_velocity)
+
+            rho_for_tau_wall = sp.Float(1)
+        else:
+            rho_for_tau_wall = cqc.density_symbol
+            u_for_tau_wall = cqc.velocity_symbols
+
+        # calculate Maronga factor in case of correction
+        maronga_fix = sp.Symbol("maronga_fix")
+        if self.maronga_sampling_shift:
+            inst_first_cell_vel = cqc.velocity_symbols
+            mean_first_cell_vel = tuple(u_mean_i.get_shifted(*self.normal_direction) for u_mean_i in self.mean_velocity)
+
+            mag_inst_vel_first_cell = sp.sqrt(sum([inst_first_cell_vel[i] ** 2 for i in self.tangential_axis]))
+            mag_mean_vel_first_cell = sp.sqrt(sum([mean_first_cell_vel[i] ** 2 for i in self.tangential_axis]))
+
+            result.append(Assignment(maronga_fix, mag_inst_vel_first_cell / mag_mean_vel_first_cell))
+        else:
+            maronga_fix = 1
+
+        # store which direction is tangential component (only those are used for the wall shear stress)
+        red_u_mag = sp.sqrt(sum([u_for_tau_wall[i]**2 for i in self.tangential_axis]))
+
+        u_mag = Assignment(u_m, red_u_mag)
+        result.append(u_mag)
+
+        wall_distance = self.maronga_sampling_shift if self.maronga_sampling_shift else self.sampling_shift
+
+        # using wall function model
+        wall_law_assignments = self.wall_function_model.shear_stress_assignments(
+            density_symbol=rho_for_tau_wall, velocity_symbol=u_m, shear_stress_symbol=tau_w,
+            wall_distance=(wall_distance - sp.Rational(1, 2) * self.dy),
+            u_tau_target=self.target_friction_velocity)
+        result.append(wall_law_assignments)
+
+        # calculate wall stress components and use them to calculate the drag
+        for i in self.tangential_axis:
+            result.append(Assignment(wall_stress[i], - u_for_tau_wall[i] / u_m * tau_w * maronga_fix))
+
+        weight, inv_weight_sq = sp.symbols("wfb_weight inverse_weight_squared")
+
+        if self.stencil.Q == 19:
+            result.append(Assignment(weight, sp.Rational(1, 2)))
+        elif self.stencil.Q == 27:
+            result.append(Assignment(inv_weight_sq, sum([neighbor_offset[i]**2 for i in self.tangential_axis])))
+            a, b = sp.symbols("wfb_a wfb_b")
+
+            if self.weight_method == self.WeightMethod.LATTICE_WEIGHT:
+                res_ab = sp.solve([2 * a + 4 * b - 1, a - 4 * b], [a, b])  # lattice weight scaling
+            elif self.weight_method == self.WeightMethod.GEOMETRIC_WEIGHT:
+                res_ab = sp.solve([2 * a + 4 * b - 1, a - sp.sqrt(2) * b], [a, b])  # geometric scaling
+            else:
+                raise ValueError("Unknown weighting method for the WFB D3Q27 extension. Currently, only lattice "
+                                 "weights and geometric weights are supported.")
+
+            result.append(Assignment(weight, sp.Piecewise((sp.Float(0), sp.Equality(inv_weight_sq, 0)),
+                                                          (res_ab[a], sp.Equality(inv_weight_sq, 1)),
+                                                          (res_ab[b], True))))
+
+        factor = self.dt / self.dy * weight
+        drag = sum([neighbor_offset[i] * factor * wall_stress[i] for i in self.tangential_axis])
+
+        result.append(Assignment(f_in.center(inv_dir[dir_symbol]), f_out[tangential_offset](mirrored_direction) - drag))
+
+        return result
+
+# end class WallFunctionBounce
+
+
 class UBB(LbBoundary):
-    """Velocity bounce back boundary condition, enforcing specified velocity at obstacle
+    r"""Velocity bounce back boundary condition, enforcing specified velocity at obstacle. Furthermore, a density
+        at the wall can be implied. The boundary condition is implemented with the following formula:
+
+    .. math ::
+        f_{\overline{i}}(\mathbf{x}_b, t + \Delta t) = f^{\star}_{i}(\mathbf{x}_b, t) -
+        2 w_{i} \rho_{w} \frac{\mathbf{c}_i \cdot \mathbf{u}_w}{c_s^2}
+
 
     Args:
-        velocity: can either be a constant, an access into a field, or a callback function.
-                  The callback functions gets a numpy record array with members, 'x','y','z', 'dir' (direction)
-                  and 'velocity' which has to be set to the desired velocity of the corresponding link
+        velocity: Prescribe the fluid velocity :math:`\mathbf{u}_w` at the wall.
+                  Can either be a constant, an access into a field, or a callback function.
+                  The callback functions gets a numpy record array with members, ``x``, ``y``, ``z``, ``dir``
+                  (direction) and ``velocity`` which has to be set to the desired velocity of the corresponding link
+        density: Prescribe the fluid density :math:`\rho_{w}` at the wall. If not prescribed the density is
+                 calculated from the PDFs at the wall. The density can only be set constant.
         adapt_velocity_to_force: adapts the velocity to the correct equilibrium when the lattice Boltzmann method holds
                                  a forcing term. If no forcing term is set and adapt_velocity_to_force is set to True
                                  it has no effect.
         dim: number of spatial dimensions
         name: optional name of the boundary.
     """
 
-    def __init__(self, velocity, adapt_velocity_to_force=False, dim=None, name=None, data_type='double'):
+    def __init__(self, velocity, density=None, adapt_velocity_to_force=False, dim=None, name=None, data_type='double'):
         self._velocity = velocity
+        self._density = density
         self._adaptVelocityToForce = adapt_velocity_to_force
         if callable(self._velocity) and not dim:
             raise ValueError("When using a velocity callback the dimension has to be specified with the dim parameter")
         elif not callable(self._velocity):
             dim = len(velocity)
         self.dim = dim
         self.data_type = data_type
@@ -535,15 +782,18 @@
         # provide a new quantity density, which is constant in case of incompressible models
         if lb_method.conserved_quantity_computation.compressible:
             cqc = lb_method.conserved_quantity_computation
             density_symbol = sp.Symbol("rho")
             pdf_field_accesses = [f_out(i) for i in range(len(lb_method.stencil))]
             density_equations = cqc.output_equations_from_pdfs(pdf_field_accesses, {'density': density_symbol})
             density_symbol = lb_method.conserved_quantity_computation.density_symbol
-            result = density_equations.all_assignments
+            if self._density:
+                result = [Assignment(density_symbol, self._density)]
+            else:
+                result = density_equations.all_assignments
             result += [Assignment(f_in(inv_dir[dir_symbol]),
                                   f_out(dir_symbol) - vel_term * density_symbol)]
             return result
         else:
             return [Assignment(f_in(inv_dir[dir_symbol]),
                                f_out(dir_symbol) - vel_term)]
 
@@ -748,15 +998,20 @@
         return AssignmentCollection(boundary_assignments, subexpressions=subexpressions)
 
 
 # end class ExtrapolationOutflow
 
 
 class FixedDensity(LbBoundary):
-    """Boundary condition that fixes the density/pressure at the obstacle.
+    r"""Boundary condition for prescribing a density at the wall. Through :math:`p = c_s^2 \rho` this boundary condition
+        can also function as a pressure boundary condition.
+
+    .. math ::
+        f_{\overline{i}}(\mathbf{x}_b, t + \Delta t) = - f^{\star}_{i}(\mathbf{x}_b, t) +
+        2 w_{i} \rho_{w} (1 + \frac{(\mathbf{c}_i \cdot \mathbf{u}_w)^2}{2c_s^4} + \frac{\mathbf{u}_w^2}{2c_s^2})
 
     Args:
         density: value of the density which should be set.
         name: optional name of the boundary.
     """
 
     def __init__(self, density, name=None):
@@ -808,16 +1063,17 @@
 
 class DiffusionDirichlet(LbBoundary):
     """Concentration boundary which is used for concentration or thermal boundary conditions of convection-diffusion
     equation Base on https://doi.org/10.1103/PhysRevE.85.016701.
 
     Args:
         concentration: can either be a constant, an access into a field, or a callback function.
-                       The callback functions gets a numpy record array with members, 'x','y','z', 'dir' (direction)
-                       and 'concentration' which has to be set to the desired velocity of the corresponding link
+                       The callback functions gets a numpy record array with members, ``x``, ``y``, ``z``, ``dir``
+                       (direction) and ``concentration`` which has to be set to the desired
+                       velocity of the corresponding link
         velocity_field: if velocity field is given the boundary value is approximated by using the discrete equilibrium.
         name: optional name of the boundary.
         data_type: data type of the concentration value. default is double
     """
 
     def __init__(self, concentration, velocity_field=None, name=None, data_type='double'):
         if name is None:
```

### Comparing `lbmpy-1.3.3/lbmpy/boundaries/boundaryhandling.py` & `lbmpy-1.3.4/src/lbmpy/boundaries/boundaryhandling.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/chapman_enskog/chapman_enskog.py` & `lbmpy-1.3.4/src/lbmpy/chapman_enskog/chapman_enskog.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/chapman_enskog/chapman_enskog_higher_order.py` & `lbmpy-1.3.4/src/lbmpy/chapman_enskog/chapman_enskog_higher_order.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/chapman_enskog/chapman_enskog_steady_state.py` & `lbmpy-1.3.4/src/lbmpy/chapman_enskog/chapman_enskog_steady_state.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/chapman_enskog/derivative.py` & `lbmpy-1.3.4/src/lbmpy/chapman_enskog/derivative.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/continuous_distribution_measures.py` & `lbmpy-1.3.4/src/lbmpy/continuous_distribution_measures.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/creationfunctions.py` & `lbmpy-1.3.4/src/lbmpy/creationfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 The third data class determines hardware optimisation. This means that contrary to the `LBMOptimisation` class,
 it acts on the level of the abstract syntax tree. Thus, it is independent of the assignments and the LBM
 and belongs to pystencils, not lbmpy. This can be found in the pystencils module as
 'pystencils.kernelcreation.CreateKernelConfig'. With this class, for example, the target (CPU, GPU etc.)
 of the generated code is specified.
 
 1. *Method*:
-         the method defines the collision process. Currently there are two big categories:
+         the method defines the collision process. Currently, there are two big categories:
          moment and cumulant based methods. A method defines how each moment or cumulant is relaxed by
          storing the equilibrium value and the relaxation rate for each moment/cumulant.
 2. *Collision/Update Rule*:
          Methods can generate a "collision rule" which is an equation collection that define the
          post collision values as a function of the pre-collision values. On these equation collection
          simplifications are applied to reduce the number of floating point operations.
-         At this stage an entropic optimization step can also be added to determine one relaxation rate by an
+         At this stage an entropic optimisation step can also be added to determine one relaxation rate by an
          entropy condition.
          Then a streaming rule is added which transforms the collision rule into an update rule.
          The streaming step depends on the pdf storage (source/destination, AABB pattern, EsoTwist).
          Currently only the simple source/destination  pattern is supported.
 3. *AST*:
         The abstract syntax tree describes the structure of the kernel, including loops and conditionals.
-        The ast can be modified e.g. to add OpenMP pragmas, reorder loops or apply other optimizations.
+        The ast can be modified, e.g., to add OpenMP pragmas, reorder loops or apply other optimisations.
 4. *Function*:
         This step compiles the AST into an executable function, either for CPU or GPUs. This function
         behaves like a normal Python function and runs one LBM time step.
 
 Each stage (apart from *Function*) also adds its result to the given `LBMConfig` object. The `LBMConfig`
 thus coalesces all information defining the LBM kernel.
 
@@ -59,30 +59,30 @@
 from warnings import warn, filterwarnings
 
 import lbmpy.moment_transforms
 import pystencils.astnodes
 import sympy as sp
 import sympy.core.numbers
 
-from lbmpy.enums import Stencil, Method, ForceModel, CollisionSpace
+from lbmpy.enums import Stencil, Method, ForceModel, CollisionSpace, SubgridScaleModel
 import lbmpy.forcemodels as forcemodels
 from lbmpy.fieldaccess import CollideOnlyInplaceAccessor, PdfFieldAccessor, PeriodicTwoFieldsAccessor
 from lbmpy.fluctuatinglb import add_fluctuations_to_collision_rule
 from lbmpy.partially_saturated_cells import add_psm_to_collision_rule, PSMConfig
 from lbmpy.non_newtonian_models import add_cassons_model, CassonsParameters
 from lbmpy.methods import (create_mrt_orthogonal, create_mrt_raw, create_central_moment,
                            create_srt, create_trt, create_trt_kbc)
 from lbmpy.methods.creationfunctions import CollisionSpaceInfo
 from lbmpy.methods.creationfunctions import (
     create_with_monomial_cumulants, create_cumulant, create_with_default_polynomial_cumulants)
 from lbmpy.methods.momentbased.entropic import add_entropy_condition, add_iterative_entropy_condition
 from lbmpy.relaxationrates import relaxation_rate_from_magic_number
 from lbmpy.simplificationfactory import create_simplification_strategy
 from lbmpy.stencils import LBStencil
-from lbmpy.turbulence_models import add_smagorinsky_model
+from lbmpy.turbulence_models import add_sgs_model
 from lbmpy.updatekernels import create_lbm_kernel, create_stream_pull_with_output_kernel
 from lbmpy.advanced_streaming.utility import Timestep, get_accessor
 from pystencils import CreateKernelConfig, create_kernel
 from pystencils.astnodes import Conditional, Block
 from pystencils.cache import disk_cache_no_fallback
 from pystencils.node_collection import NodeCollection
 from pystencils.typing import collate_types
@@ -141,15 +141,15 @@
     """
     Governs the storage format of populations. If `False`, the discrete particle distribution vector is stored in its
     absolute form. If `True`, instead, only the distribution's deviation from its rest state (typically given by the
     lattice weights) is stored.
     """
     delta_equilibrium: bool = None
     """
-    Determines whether or not the (continuous or discrete, see `continuous_equilibrium`) maxwellian equilibrium is
+    Determines whether or not the (continuous or discrete, see `continuous_equilibrium`) Maxwellian equilibrium is
     expressed in its absolute form, or only by its deviation from the rest state (typically given by the reference
     density and zero velocity). This parameter is only effective if `zero_centered` is set to `True`. Then, if
     `delta_equilibrium` is `False`, the rest state must be reintroduced to the populations during collision. Otherwise,
     if `delta_equilibrium` is `True`, the collision equations can be derived using only the deviations from the rest 
     state.
 
     If `None` is passed to `delta_equilibrium`, its value will be chosen automatically, depending on the value of
@@ -171,15 +171,15 @@
     Affects only orthogonal MRT methods. If set to True a weighted Gram-Schmidt procedure is used to orthogonalise 
     the moments.
     """
     nested_moments: List[List] = None
     """
     A list of lists of modes, grouped by common relaxation times. This is usually used in
     conjunction with `lbmpy.methods.default_moment_sets.mrt_orthogonal_modes_literature`.
-    If this argument is not provided, Gram-Schmidt orthogonalization of the default modes is performed.
+    If this argument is not provided, Gram-Schmidt orthogonalisation of the default modes is performed.
     """
 
     force_model: Union[lbmpy.forcemodels.AbstractForceModel, ForceModel] = None
     """
     Force model to determine how forcing terms enter the collision rule.
     Possibilities are defined in :class: `lbmpy.enums.ForceModel`
     """
@@ -235,20 +235,25 @@
     For moment methods the entropy optimum can be calculated in closed form.
     For cumulant methods this is not possible, in that case it is computed using Newton iterations.
     This parameter can be used to force Newton iterations and specify how many should be done
     """
     omega_output_field: Field = None
     """
     A pystencils Field can be passed here, where the calculated free relaxation rate of
-    an entropic or Smagorinsky method is written to
+    an entropic or subgrid-scale method is written to
     """
-    smagorinsky: Union[float, bool] = False
+    eddy_viscosity_field: Field = None
     """
-    set to Smagorinsky constant to activate turbulence model, ``omega_output_field`` can be set to
-    write out adapted relaxation rates. If set to `True`, 0.12 is used as default smagorinsky constant.
+    A pystencils Field can be passed here, where the eddy-viscosity of a subgrid-scale model is written.
+    """
+    subgrid_scale_model: Union[SubgridScaleModel, tuple[SubgridScaleModel, float], tuple[SubgridScaleModel, int]] = None
+    """
+    Choose a subgrid-scale model (SGS) for large-eddy simulations. ``omega_output_field`` can be set to
+    write out adapted relaxation rates. Either provide just the SGS and use the default model constants or provide a
+    tuple of the SGS and its corresponding model constant.
     """
     cassons: CassonsParameters = False
     """
     Adds the Cassons model according to https://doi.org/10.1007/s10955-005-8415-x
     The parameters are set with the ``CassonsParameters`` dataclass.
     """
     fluctuating: dict = False
@@ -698,34 +703,43 @@
         cumulant_limiter = 1e6 if lbm_config.fourth_order_correction is True else lbm_config.fourth_order_correction
         collision_rule = add_fourth_order_correction(collision_rule=collision_rule,
                                                      shear_relaxation_rate=lbm_config.relaxation_rates[0],
                                                      bulk_relaxation_rate=lbm_config.relaxation_rates[1],
                                                      limiter=cumulant_limiter)
 
     if lbm_config.entropic:
-        if lbm_config.smagorinsky or lbm_config.cassons:
-            raise ValueError("Choose either entropic, smagorinsky or cassons")
+        if lbm_config.subgrid_scale_model or lbm_config.cassons:
+            raise ValueError("Choose either entropic, subgrid-scale or cassons")
         if lbm_config.entropic_newton_iterations:
             if isinstance(lbm_config.entropic_newton_iterations, bool):
                 iterations = 3
             else:
                 iterations = lbm_config.entropic_newton_iterations
             collision_rule = add_iterative_entropy_condition(collision_rule, newton_iterations=iterations,
                                                              omega_output_field=lbm_config.omega_output_field)
         else:
             collision_rule = add_entropy_condition(collision_rule, omega_output_field=lbm_config.omega_output_field)
 
-    elif lbm_config.smagorinsky:
+    elif lbm_config.subgrid_scale_model:
         if lbm_config.cassons:
-            raise ValueError("Cassons model can not be combined with Smagorinsky model")
-        smagorinsky_constant = 0.12 if lbm_config.smagorinsky is True else lbm_config.smagorinsky
-        collision_rule = add_smagorinsky_model(collision_rule, smagorinsky_constant,
-                                               omega_output_field=lbm_config.omega_output_field)
-        if 'split_groups' in collision_rule.simplification_hints:
-            collision_rule.simplification_hints['split_groups'][0].append(sp.Symbol("smagorinsky_omega"))
+            raise ValueError("Cassons model can not be combined with a subgrid-scale model")
+
+        model_constant = None
+        sgs_model = lbm_config.subgrid_scale_model
+
+        if isinstance(lbm_config.subgrid_scale_model, tuple):
+            sgs_model = lbm_config.subgrid_scale_model[0]
+            model_constant = lbm_config.subgrid_scale_model[1]
+
+        collision_rule = add_sgs_model(collision_rule=collision_rule, subgrid_scale_model=sgs_model,
+                                       model_constant=model_constant, omega_output_field=lbm_config.omega_output_field,
+                                       eddy_viscosity_field=lbm_config.eddy_viscosity_field)
+
+    if 'split_groups' in collision_rule.simplification_hints:
+        collision_rule.simplification_hints['split_groups'][0].append(sp.Symbol("sgs_omega"))
 
     elif lbm_config.cassons:
         collision_rule = add_cassons_model(collision_rule, parameter=lbm_config.cassons,
                                            omega_output_field=lbm_config.omega_output_field)
 
     if lbm_config.output:
         output_eqs = cqc.output_equations_from_pdfs(lb_method.pre_collision_pdf_symbols, lbm_config.output)
```

### Comparing `lbmpy-1.3.3/lbmpy/cumulants.py` & `lbmpy-1.3.4/src/lbmpy/cumulants.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/custom_code_nodes.py` & `lbmpy-1.3.4/src/lbmpy/custom_code_nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,24 +60,19 @@
         super(MirroredStencilDirections, self).__init__(code, symbols_read=set(),
                                                         symbols_defined={mirrored_stencil_symbol})
 
 
 class LbmWeightInfo(CustomCodeNode):
     def __init__(self, lb_method, data_type='double'):
         self.weights_symbol = TypedSymbol("weights", data_type)
-        data_type_string = "double" if self.weights_symbol.dtype.numpy_dtype == np.float64 else "float"
 
-        weights = [str(w.evalf(17)) for w in lb_method.weights]
-        if data_type_string == "float":
-            weights = "f, ".join(weights)
-            weights += "f"  # suffix for the last element
-        else:
-            weights = ", ".join(weights)
+        weights = [f"(({self.weights_symbol.dtype.c_name})({str(w.evalf(17))}))" for w in lb_method.weights]
+        weights = ", ".join(weights)
         w_sym = self.weights_symbol
-        code = f"const {data_type_string} {w_sym.name} [] = {{{ weights }}};\n"
+        code = f"const {self.weights_symbol.dtype.c_name} {w_sym.name} [] = {{{ weights }}};\n"
         super(LbmWeightInfo, self).__init__(code, symbols_read=set(), symbols_defined={w_sym})
 
     def weight_of_direction(self, dir_idx, lb_method=None):
         if isinstance(sp.sympify(dir_idx), sp.Integer):
             return lb_method.weights[dir_idx].evalf(17)
         else:
             return sp.IndexedBase(self.weights_symbol, shape=(1,))[dir_idx]
```

### Comparing `lbmpy-1.3.3/lbmpy/db.py` & `lbmpy-1.3.4/src/lbmpy/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 import six
 import inspect
 
 from pystencils.runhelper.db import PystencilsJsonEncoder
 from pystencils.simp import SimplificationStrategy
-from lbmpy import LBStencil, Method, CollisionSpace
+from lbmpy import LBStencil, Method, CollisionSpace, SubgridScaleModel
 from lbmpy.creationfunctions import LBMConfig, LBMOptimisation
 from lbmpy.methods import CollisionSpaceInfo
 from lbmpy.forcemodels import AbstractForceModel
 from lbmpy.non_newtonian_models import CassonsParameters
 
 
 class LbmpyJsonEncoder(PystencilsJsonEncoder):
 
     def default(self, obj):
         if isinstance(obj, (LBMConfig, LBMOptimisation, CollisionSpaceInfo, CassonsParameters)):
             return obj.__dict__
-        if isinstance(obj, (LBStencil, Method, CollisionSpace)):
+        if isinstance(obj, (LBStencil, Method, CollisionSpace, SubgridScaleModel)):
             return obj.name
         if isinstance(obj, AbstractForceModel):
             return obj.__class__.__name__
         if isinstance(obj, SimplificationStrategy):
             return obj.__str__()
         if inspect.isclass(obj):
             return obj.__name__
```

### Comparing `lbmpy-1.3.3/lbmpy/enums.py` & `lbmpy-1.3.4/src/lbmpy/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,9 +215,24 @@
     """
     SHANCHEN = auto()
     """
     See :class:`lbmpy.forcemodels.ShanChen`
     """
     CENTRALMOMENT = auto()
     """
-    See :class:`lbmpy.forcemodels`
+    See :class:`lbmpy.forcemodels.CentralMoment`
+    """
+
+
+class SubgridScaleModel(Enum):
+    """
+    The SubgridScaleModel enumeration defines which subgrid-scale model (SGS) is used to perform
+    Large-Eddy-Simulations (LES).
+    """
+    SMAGORINSKY = auto()
+    """
+    See :func:`lbmpy.turbulence_models.add_smagorinsky_model`
+    """
+    QR = auto()
+    """
+    See :func:`lbmpy.turbulence_models.add_qr_model`
     """
```

### Comparing `lbmpy-1.3.3/lbmpy/equilibrium/__init__.py` & `lbmpy-1.3.4/src/lbmpy/equilibrium/__init__.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/equilibrium/abstract_equilibrium.py` & `lbmpy-1.3.4/src/lbmpy/equilibrium/abstract_equilibrium.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/equilibrium/continuous_hydro_maxwellian.py` & `lbmpy-1.3.4/src/lbmpy/equilibrium/continuous_hydro_maxwellian.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/equilibrium/discrete_hydro_maxwellian.py` & `lbmpy-1.3.4/src/lbmpy/equilibrium/discrete_hydro_maxwellian.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/equilibrium/generic_discrete_equilibrium.py` & `lbmpy-1.3.4/src/lbmpy/equilibrium/generic_discrete_equilibrium.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/fieldaccess.py` & `lbmpy-1.3.4/src/lbmpy/fieldaccess.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/fluctuatinglb.py` & `lbmpy-1.3.4/src/lbmpy/fluctuatinglb.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/forcemodels.py` & `lbmpy-1.3.4/src/lbmpy/forcemodels.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/geometry.py` & `lbmpy-1.3.4/src/lbmpy/geometry.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/innerloopsplit.py` & `lbmpy-1.3.4/src/lbmpy/innerloopsplit.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/lbstep.py` & `lbmpy-1.3.4/src/lbmpy/lbstep.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,17 @@
                 raise ValueError("Specify either domain_size or data_handling")
             data_handling = create_data_handling(domain_size,
                                                  default_ghost_layers=1,
                                                  periodicity=periodicity,
                                                  default_target=target,
                                                  parallel=False)
 
+        if lbm_config:
+            method_parameters['stencil'] = lbm_config.stencil
+
         if 'stencil' not in method_parameters:
             method_parameters['stencil'] = LBStencil(Stencil.D2Q9) \
                 if data_handling.dim == 2 else LBStencil(Stencil.D3Q27)
 
         lbm_config, lbm_optimisation, config = update_with_default_parameters(method_parameters, optimization,
                                                                               lbm_config, lbm_optimisation, config)
```

### Comparing `lbmpy-1.3.3/lbmpy/macroscopic_value_kernels.py` & `lbmpy-1.3.4/src/lbmpy/macroscopic_value_kernels.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/max_domain_size_info.py` & `lbmpy-1.3.4/src/lbmpy/max_domain_size_info.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/maxwellian_equilibrium.py` & `lbmpy-1.3.4/src/lbmpy/maxwellian_equilibrium.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     res = [discrete_equilibrium(e_q, u, rho, w_q, order, c_s_sq, compressible) for w_q, e_q in zip(weights, stencil)]
     return tuple(res)
 
 
 def discrete_equilibrium(v=sp.symbols("v_:3"), u=sp.symbols("u_:3"), rho=sp.Symbol("rho"), weight=sp.Symbol("w"),
                          order=2, c_s_sq=sp.Symbol("c_s") ** 2, compressible=True):
     """
-    Returns the common discrete LBM equilibrium as a list of sympy expressions
+    Returns the common discrete LBM equilibrium depending on the mesoscopic velocity and the directional lattice weight
 
     Args:
         v: symbols for mesoscopic velocity
         u: symbols for macroscopic velocity
         rho: sympy symbol for the density
         weight: symbol for stencil weights
         order: highest order of velocity terms (for hydrodynamics order 2 is sufficient)
```

### Comparing `lbmpy-1.3.3/lbmpy/methods/__init__.py` & `lbmpy-1.3.4/src/lbmpy/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/abstractlbmethod.py` & `lbmpy-1.3.4/src/lbmpy/methods/abstractlbmethod.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/conservedquantitycomputation.py` & `lbmpy-1.3.4/src/lbmpy/methods/conservedquantitycomputation.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/creationfunctions.py` & `lbmpy-1.3.4/src/lbmpy/methods/creationfunctions.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/cumulantbased/cumulant_simplifications.py` & `lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/cumulant_simplifications.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/cumulantbased/cumulantbasedmethod.py` & `lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/cumulantbasedmethod.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/cumulantbased/fourth_order_correction.py` & `lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/fourth_order_correction.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/cumulantbased/galilean_correction.py` & `lbmpy-1.3.4/src/lbmpy/methods/cumulantbased/galilean_correction.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/default_moment_sets.py` & `lbmpy-1.3.4/src/lbmpy/methods/default_moment_sets.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/momentbased/centralmomentbasedmethod.py` & `lbmpy-1.3.4/src/lbmpy/methods/momentbased/centralmomentbasedmethod.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/momentbased/entropic.py` & `lbmpy-1.3.4/src/lbmpy/methods/momentbased/entropic.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/momentbased/momentbasedmethod.py` & `lbmpy-1.3.4/src/lbmpy/methods/momentbased/momentbasedmethod.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/methods/momentbased/momentbasedsimplifications.py` & `lbmpy-1.3.4/src/lbmpy/methods/momentbased/momentbasedsimplifications.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/moment_transforms/__init__.py` & `lbmpy-1.3.4/src/lbmpy/moment_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/moment_transforms/abstractmomenttransform.py` & `lbmpy-1.3.4/src/lbmpy/moment_transforms/abstractmomenttransform.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/moment_transforms/centralmomenttransforms.py` & `lbmpy-1.3.4/src/lbmpy/moment_transforms/centralmomenttransforms.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/moment_transforms/cumulanttransforms.py` & `lbmpy-1.3.4/src/lbmpy/moment_transforms/cumulanttransforms.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/moment_transforms/rawmomenttransforms.py` & `lbmpy-1.3.4/src/lbmpy/moment_transforms/rawmomenttransforms.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/moments.py` & `lbmpy-1.3.4/src/lbmpy/moments.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/non_newtonian_models.py` & `lbmpy-1.3.4/src/lbmpy/non_newtonian_models.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/oldroydb.py` & `lbmpy-1.3.4/src/lbmpy/oldroydb.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,98 +9,98 @@
 class OldroydB:
     def __init__(self, dim, u, tau, F, tauflux, tauface, lambda_p, eta_p, vof=True):
         assert not ps.FieldType.is_staggered(u)
         assert not ps.FieldType.is_staggered(tau)
         assert not ps.FieldType.is_staggered(F)
         assert ps.FieldType.is_staggered(tauflux)
         assert ps.FieldType.is_staggered(tauface)
-        
+
         self.dim = dim
         self.u = u
         self.tau = tau
         self.F = F
         self.tauflux = tauflux
         self.tauface_field = tauface
         self.lambda_p = lambda_p
         self.eta_p = eta_p
-        
+
         full_stencil = ["C"] + self.tauflux.staggered_stencil + \
             list(map(inverse_direction_string, self.tauflux.staggered_stencil))
         self.stencil = tuple(map(lambda d: tuple(ps.stencil.direction_string_to_offset(d, self.dim)), full_stencil))
         full_stencil = ["C"] + self.tauface_field.staggered_stencil + \
             list(map(inverse_direction_string, self.tauface_field.staggered_stencil))
         self.force_stencil = tuple(map(lambda d: tuple(ps.stencil.direction_string_to_offset(d, self.dim)),
                                    full_stencil))
-        
+
         self.disc = ps.fd.FVM1stOrder(self.tau, self._flux(), self._source())
         if vof:
             self.vof = ps.fd.VOF(self.tauflux, self.u, self.tau)
         else:
             self.vof = None
-    
+
     def _flux(self):
         return [self.tau.center_vector.applyfunc(lambda t: t * self.u.center_vector[i]) for i in range(self.dim)]
-    
+
     def _source(self):
         gradu = sp.Matrix([[ps.fd.diff(self.u.center_vector[j], i) for j in range(self.dim)] for i in range(self.dim)])
         gamma = gradu + gradu.transpose()
         return self.tau.center_vector * gradu + gradu.transpose() * self.tau.center_vector + \
             (self.eta_p * gamma - self.tau.center_vector) / self.lambda_p
-    
+
     def tauface(self):
         return ps.AssignmentCollection([ps.Assignment(self.tauface_field.staggered_vector_access(d),
                                         (self.tau.center_vector + self.tau.neighbor_vector(d)) / 2)
                                         for d in self.tauface_field.staggered_stencil])
-    
+
     def force(self):
         full_stencil = self.tauface_field.staggered_stencil + \
             list(map(inverse_direction_string, self.tauface_field.staggered_stencil))
         dtau = sp.Matrix([sum([sum([
                           self.tauface_field.staggered_access(d, (i, j)) * direction_string_to_offset(d)[i]
                           for i in range(self.dim)]) / sp.Matrix(direction_string_to_offset(d)).norm()
                          for d in full_stencil]) for j in range(self.dim)])
         A0 = sum([sp.Matrix(direction_string_to_offset(d)).norm() for d in full_stencil])
         return ps.AssignmentCollection(ps.Assignment(self.F.center_vector, dtau / A0 * 2 * self.dim))
-    
+
     def flux(self):
         if self.vof is not None:
             return self.vof
         else:
             return self.disc.discrete_flux(self.tauflux)
-    
+
     def continuity(self):
         cont = self.disc.discrete_continuity(self.tauflux)
         tau_copy = sp.Matrix(self.dim, self.dim, lambda i, j: sp.Symbol("tau_old_%d_%d" % (i, j)))
         tau_subs = {self.tau.center_vector[i, j]: tau_copy[i, j] for i in range(self.dim) for j in range(self.dim)}
         return [ps.Assignment(tau_copy[i, j], self.tau.center_vector[i, j])
                 for i in range(self.dim) for j in range(self.dim)] + \
                [ps.Assignment(a.lhs, a.rhs.subs(tau_subs)) for a in cont]
 
 
 class Flux(Boundary):
     inner_or_boundary = True  # call the boundary condition with the fluid cell
     single_link = False  # needs to be called for all directional fluxes
-    
+
     def __init__(self, stencil, value=None):
         self.stencil = stencil
         self.value = value
 
     def __call__(self, field, direction_symbol, **kwargs):
         assert ps.FieldType.is_staggered(field)
-        
+
         assert all([s == 0 for s in self.stencil[0]])
         accesses = [field.staggered_vector_access(ps.stencil.offset_to_direction_string(d))
                     for d in self.stencil[1:]]
         conds = [sp.Equality(direction_symbol, d + 1) for d in range(len(accesses))]
-        
+
         if self.value is None:
             val = sp.Matrix(np.zeros(accesses[0].shape, dtype=int))
         else:
             val = self.value
-        
+
         # use conditional
         conditional = None
         for a, c, d in zip(accesses, conds, self.stencil[1:]):
             d = ps.stencil.offset_to_direction_string(d)
             assignments = []
             for i in range(len(a)):
                 fac = 1
@@ -114,15 +114,15 @@
                                                       conditional)
         return [conditional]
 
     def __hash__(self):
         return hash((Flux, self.stencil, self.value))
 
     def __eq__(self, other):
-        return type(other) == Flux and other.stencil == self.stencil and self.value == other.value
+        return type(other) is Flux and other.stencil == self.stencil and self.value == other.value
 
 
 class Extrapolation(Boundary):
     inner_or_boundary = True  # call the boundary condition with the fluid cell
     single_link = False  # needs to be called for all directional fluxes
 
     def __init__(self, stencil, src_field, order):
@@ -135,20 +135,20 @@
         elif order == 2:
             self.weights = (sp.Rational(15, 8), - sp.Rational(10, 8), sp.Rational(3, 8))
         else:
             raise NotImplementedError("weights are not known for extrapolation orders > 2")
 
     def __call__(self, field, direction_symbol, **kwargs):
         assert ps.FieldType.is_staggered(field)
-        
+
         assert all([s == 0 for s in self.stencil[0]])
         accesses = [field.staggered_vector_access(ps.stencil.offset_to_direction_string(d))
                     for d in self.stencil[1:]]
         conds = [sp.Equality(direction_symbol, d + 1) for d in range(len(accesses))]
-        
+
         # use conditional
         conditional = None
         for a, c, o in zip(accesses, conds, self.stencil[1:]):
             assignments = []
             src = [self.src.neighbor_vector(tuple([-1 * n * i for i in o])) for n in range(len(self.weights))]
             interp = self.weights[0] * src[0]
             for i in range(1, len(self.weights)):
@@ -165,45 +165,46 @@
                                                       conditional)
         return [conditional]
 
     def __hash__(self):
         return hash((Extrapolation, self.stencil, self.src, self.weights))
 
     def __eq__(self, other):
-        return type(other) == Extrapolation and other.stencil == self.stencil and \
+        return type(other) is Extrapolation and other.stencil == self.stencil and \
             other.src == self.src and other.weights == self.weights
 
 
 class ForceOnBoundary(Boundary):
     inner_or_boundary = False  # call the boundary condition with the boundary cell
     single_link = False  # needs to be called for all directional fluxes
-    
-    def __init__(self, stencil, force_field):
+
+    def __init__(self, stencil, force_field, name=None):
         self.stencil = stencil
         self.force_field = force_field
-        
+        super(ForceOnBoundary).__init__(name)
+
         assert not ps.FieldType.is_staggered(force_field)
 
     def __call__(self, face_stress_field, direction_symbol, **kwargs):
         assert ps.FieldType.is_staggered(face_stress_field)
-        
+
         assert all([s == 0 for s in self.stencil[0]])
         accesses = [face_stress_field.staggered_vector_access(ps.stencil.offset_to_direction_string(d))
                     for d in self.stencil[1:]]
         conds = [sp.Equality(direction_symbol, d + 1) for d in range(len(accesses))]
-        
+
         # use conditional
         conditional = None
         for a, c, o in zip(accesses, conds, self.stencil[1:]):
             assignments = ps.Assignment(self.force_field.center_vector,
                                         self.force_field.center_vector + 1 * a.transpose() * sp.Matrix(o))
             conditional = ps.astnodes.Conditional(ps.data_types.type_all_numbers(c, "int"),
                                                   ps.astnodes.Block(assignments),
                                                   conditional)
         return [conditional]
 
     def __hash__(self):
         return hash((ForceOnBoundary, self.stencil, self.force_field))
 
     def __eq__(self, other):
-        return type(other) == ForceOnBoundary and other.stencil == self.stencil and \
+        return type(other) is ForceOnBoundary and other.stencil == self.stencil and \
             other.force_field == self.force_field
```

### Comparing `lbmpy-1.3.3/lbmpy/parameterization.py` & `lbmpy-1.3.4/src/lbmpy/parameterization.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/partially_saturated_cells.py` & `lbmpy-1.3.4/src/lbmpy/partially_saturated_cells.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/analytical.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/analytical.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/cahn_hilliard_lbm.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/cahn_hilliard_lbm.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/contact_angle_circle_fitting.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/contact_angle_circle_fitting.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/eos.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/eos.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/experiments1D.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/experiments1D.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/experiments2D.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/experiments2D.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/fd_stencils.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/fd_stencils.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/high_density_ratio_model.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/high_density_ratio_model.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/kerneleqs.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/kerneleqs.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/n_phase_boyer.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/n_phase_boyer.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/nphase_nestler.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/nphase_nestler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 try:
     import pyximport
 
     pyximport.install(language_level=3)
     from lbmpy.phasefield.simplex_projection import simplex_projection_2d  # NOQA
 except ImportError:
-    try:
-        from lbmpy.phasefield.simplex_projection import simplex_projection_2d  # NOQA
-    except ImportError:
-        raise ImportError("neither pyximport nor binary module simplex_projection_2d available.")
+    raise ImportError("pyximport not available. Please install Cython to use simplex_projection_2d.")
 
 import sympy as sp
 
 from lbmpy.creationfunctions import create_lb_update_rule, LBMConfig, LBMOptimisation
 from lbmpy.enums import Stencil
 from lbmpy.macroscopic_value_kernels import pdf_initialization_assignments
 from lbmpy.phasefield.analytical import chemical_potentials_from_free_energy, force_from_phi_and_mu
```

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/phasefieldstep.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/phasefieldstep.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/phasefieldstep_direct.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/phasefieldstep_direct.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/post_processing.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/post_processing.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield/scenarios.py` & `lbmpy-1.3.4/src/lbmpy/phasefield/scenarios.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/analytical.py` & `lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/analytical.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/contact_angle.py` & `lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/contact_angle.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/derivatives.py` & `lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/derivatives.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/kernel_equations.py` & `lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/kernel_equations.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/numerical_solver.py` & `lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/numerical_solver.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/phasefield_allen_cahn/parameter_calculation.py` & `lbmpy-1.3.4/src/lbmpy/phasefield_allen_cahn/parameter_calculation.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/plot.py` & `lbmpy-1.3.4/src/lbmpy/plot.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/postprocessing.py` & `lbmpy-1.3.4/src/lbmpy/postprocessing.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/quadratic_equilibrium_construction.py` & `lbmpy-1.3.4/src/lbmpy/quadratic_equilibrium_construction.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/relaxationrates.py` & `lbmpy-1.3.4/src/lbmpy/relaxationrates.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/scenarios.py` & `lbmpy-1.3.4/src/lbmpy/scenarios.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/session.py` & `lbmpy-1.3.4/src/lbmpy/session.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/simplificationfactory.py` & `lbmpy-1.3.4/src/lbmpy/simplificationfactory.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/sparse/mapping.py` & `lbmpy-1.3.4/src/lbmpy/sparse/mapping.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/sparse/update_rule_sparse.py` & `lbmpy-1.3.4/src/lbmpy/sparse/update_rule_sparse.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/stencils.py` & `lbmpy-1.3.4/src/lbmpy/stencils.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,14 +242,21 @@
             'lehmann': ((0, 0, 0),
                         (1, 0, 0), (-1, 0, 0), (0, 1, 0), (0, -1, 0), (0, 0, 1), (0, 0, -1),
                         (1, 1, 0), (-1, -1, 0), (1, 0, 1), (-1, 0, -1),
                         (0, 1, 1), (0, -1, -1), (1, -1, 0), (-1, 1, 0),
                         (1, 0, -1), (-1, 0, 1), (0, 1, -1), (0, -1, 1),
                         (1, 1, 1), (-1, -1, -1), (1, 1, -1), (-1, -1, 1), (1, -1, 1), (-1, 1, -1), (-1, 1, 1),
                         (1, -1, -1)),
+            'braunschweig': ((0, 0, 0),
+                             (1, 0, 0), (-1, 0, 0), (0, 1, 0), (0, -1, 0), (0, 0, 1), (0, 0, -1),
+                             (1, 1, 0), (-1, -1, 0), (1, -1, 0), (-1, 1, 0),
+                             (1, 0, 1), (-1, 0, -1), (1, 0, -1), (-1, 0, 1),
+                             (0, 1, 1), (0, -1, -1), (0, 1, -1), (0, -1, 1),
+                             (1, 1, 1), (-1, 1, 1), (1, -1, 1), (-1, -1, 1), (1, 1, -1), (-1, 1, -1), (1, -1, -1),
+                             (-1, -1, -1)),
         }
     }
     try:
         return predefined_stencils[stencil][ordering]
     except KeyError:
         err_msg = ""
         for stencil, ordering_names in predefined_stencils.items():
```

### Comparing `lbmpy-1.3.3/lbmpy/updatekernels.py` & `lbmpy-1.3.4/src/lbmpy/updatekernels.py`

 * *Files identical despite different names*

### Comparing `lbmpy-1.3.3/lbmpy/utils.py` & `lbmpy-1.3.4/src/lbmpy/utils.py`

 * *Files identical despite different names*

