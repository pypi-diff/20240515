# Comparing `tmp/pystencils-1.3.3.tar.gz` & `tmp/pystencils-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystencils-1.3.3.tar", last modified: Sat Jan  6 15:51:04 2024, max compression
+gzip compressed data, was "pystencils-1.3.4.tar", last modified: Wed May 15 07:44:25 2024, max compression
```

## Comparing `pystencils-1.3.3.tar` & `pystencils-1.3.4.tar`

### file list

```diff
@@ -1,124 +1,203 @@
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.692089 pystencils-1.3.3/
--rw-r--r--   0 holzer     (502) staff       (20)      502 2024-01-06 15:47:25.000000 pystencils-1.3.3/AUTHORS.txt
--rw-r--r--   0 holzer     (502) staff       (20)     3797 2024-01-06 15:47:25.000000 pystencils-1.3.3/CONTRIBUTING.md
--rw-r--r--   0 holzer     (502) staff       (20)    34523 2024-01-06 15:47:25.000000 pystencils-1.3.3/COPYING.txt
--rw-r--r--   0 holzer     (502) staff       (20)      169 2024-01-06 15:47:25.000000 pystencils-1.3.3/MANIFEST.in
--rw-r--r--   0 holzer     (502) staff       (20)     4822 2024-01-06 15:51:04.692163 pystencils-1.3.3/PKG-INFO
--rw-r--r--   0 holzer     (502) staff       (20)     3676 2024-01-06 15:47:25.000000 pystencils-1.3.3/README.md
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.692722 pystencils-1.3.3/pystencils/
--rw-r--r--   0 holzer     (502) staff       (20)     1700 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)      497 2024-01-06 15:51:04.692781 pystencils-1.3.3/pystencils/_version.py
--rw-r--r--   0 holzer     (502) staff       (20)     4895 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/alignedarray.py
--rw-r--r--   0 holzer     (502) staff       (20)     4429 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/assignment.py
--rw-r--r--   0 holzer     (502) staff       (20)    28965 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/astnodes.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.679229 pystencils-1.3.3/pystencils/backends/
--rw-r--r--   0 holzer     (502) staff       (20)      164 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     6279 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/arm_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)    42082 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/cbackend.py
--rw-r--r--   0 holzer     (502) staff       (20)     2824 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/cuda_backend.py
--rw-r--r--   0 holzer     (502) staff       (20)     3539 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/dot.py
--rw-r--r--   0 holzer     (502) staff       (20)     2479 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/json.py
--rw-r--r--   0 holzer     (502) staff       (20)     3931 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/ppc_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)     3670 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/riscv_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)     4896 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/simd_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)     7196 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/backends/x86_instruction_sets.py
--rw-r--r--   0 holzer     (502) staff       (20)     1707 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/bit_masks.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.681905 pystencils-1.3.3/pystencils/boundaries/
--rw-r--r--   0 holzer     (502) staff       (20)      284 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/boundaries/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     4344 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/boundaries/boundaryconditions.py
--rw-r--r--   0 holzer     (502) staff       (20)    21066 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/boundaries/boundaryhandling.py
--rw-r--r--   0 holzer     (502) staff       (20)     8226 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/boundaries/createindexlist.py
--rw-r--r--   0 holzer     (502) staff       (20)  2325927 2024-01-06 15:51:04.000000 pystencils-1.3.3/pystencils/boundaries/createindexlistcython.c
--rw-r--r--   0 holzer     (502) staff       (20)     8006 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/boundaries/createindexlistcython.pyx
--rw-r--r--   0 holzer     (502) staff       (20)     2031 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/boundaries/inkernel.py
--rw-r--r--   0 holzer     (502) staff       (20)     2406 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/cache.py
--rw-r--r--   0 holzer     (502) staff       (20)     9617 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/config.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.682768 pystencils-1.3.3/pystencils/cpu/
--rw-r--r--   0 holzer     (502) staff       (20)      266 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/cpu/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    27837 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/cpu/cpujit.py
--rw-r--r--   0 holzer     (502) staff       (20)    11361 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/cpu/kernelcreation.py
--rw-r--r--   0 holzer     (502) staff       (20)     3758 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/cpu/msvc_detection.py
--rw-r--r--   0 holzer     (502) staff       (20)    22384 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/cpu/vectorization.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.683865 pystencils-1.3.3/pystencils/datahandling/
--rw-r--r--   0 holzer     (502) staff       (20)     3490 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/datahandling/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     5636 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/datahandling/blockiteration.py
--rw-r--r--   0 holzer     (502) staff       (20)    20890 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/datahandling/datahandling_interface.py
--rw-r--r--   0 holzer     (502) staff       (20)    17403 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/datahandling/parallel_datahandling.py
--rw-r--r--   0 holzer     (502) staff       (20)    20768 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/datahandling/serial_datahandling.py
--rw-r--r--   0 holzer     (502) staff       (20)     2136 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/datahandling/vtk.py
--rw-r--r--   0 holzer     (502) staff       (20)     3482 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/display_utils.py
--rw-r--r--   0 holzer     (502) staff       (20)      713 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/enums.py
--rw-r--r--   0 holzer     (502) staff       (20)     2624 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/fast_approximation.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.684925 pystencils-1.3.3/pystencils/fd/
--rw-r--r--   0 holzer     (502) staff       (20)      880 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/fd/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    14981 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/fd/derivation.py
--rw-r--r--   0 holzer     (502) staff       (20)    21404 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/fd/derivative.py
--rw-r--r--   0 holzer     (502) staff       (20)    15080 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/fd/finitedifferences.py
--rw-r--r--   0 holzer     (502) staff       (20)    11806 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/fd/finitevolumes.py
--rw-r--r--   0 holzer     (502) staff       (20)     7060 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/fd/spatial.py
--rw-r--r--   0 holzer     (502) staff       (20)    46517 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/field.py
--rw-r--r--   0 holzer     (502) staff       (20)     1538 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/functions.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.685917 pystencils-1.3.3/pystencils/gpu/
--rw-r--r--   0 holzer     (502) staff       (20)      508 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/gpu/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     3640 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/gpu/gpu_array_handler.py
--rw-r--r--   0 holzer     (502) staff       (20)     8575 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/gpu/gpujit.py
--rw-r--r--   0 holzer     (502) staff       (20)    19013 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/gpu/indexing.py
--rw-r--r--   0 holzer     (502) staff       (20)     9960 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/gpu/kernelcreation.py
--rw-r--r--   0 holzer     (502) staff       (20)     2092 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/gpu/periodicity.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.689335 pystencils-1.3.3/pystencils/include/
--rw-r--r--   0 holzer     (502) staff       (20)      413 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/include/PyStencilsField.h
--rw-r--r--   0 holzer     (502) staff       (20)      114 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/include/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    28148 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/include/aesni_rand.h
--rw-r--r--   0 holzer     (502) staff       (20)     2208 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/include/arm_neon_helpers.h
--rw-r--r--   0 holzer     (502) staff       (20)      293 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/include/gpu_defines.h
--rw-r--r--   0 holzer     (502) staff       (20)      968 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/include/half_precision.h
--rw-r--r--   0 holzer     (502) staff       (20)     4012 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/include/myintrin.h
--rw-r--r--   0 holzer     (502) staff       (20)    58376 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/include/philox_rand.h
--rw-r--r--   0 holzer     (502) staff       (20)     1007 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/include/ppc_altivec_helpers.h
--rw-r--r--   0 holzer     (502) staff       (20)     6390 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/integer_functions.py
--rw-r--r--   0 holzer     (502) staff       (20)     2830 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/integer_set_analysis.py
--rw-r--r--   0 holzer     (502) staff       (20)     3989 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/jupyter.py
--rw-r--r--   0 holzer     (502) staff       (20)     5676 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/kernel_contrains_check.py
--rw-r--r--   0 holzer     (502) staff       (20)     5133 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/kernel_decorator.py
--rw-r--r--   0 holzer     (502) staff       (20)      545 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/kernel_wrapper.py
--rw-r--r--   0 holzer     (502) staff       (20)    19357 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/kernelcreation.py
--rw-r--r--   0 holzer     (502) staff       (20)     4176 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/node_collection.py
--rw-r--r--   0 holzer     (502) staff       (20)     2680 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/placeholder_function.py
--rw-r--r--   0 holzer     (502) staff       (20)    13234 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/plot.py
--rw-r--r--   0 holzer     (502) staff       (20)     4822 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/rng.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.689810 pystencils-1.3.3/pystencils/runhelper/
--rw-r--r--   0 holzer     (502) staff       (20)      150 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/runhelper/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     9989 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/runhelper/db.py
--rw-r--r--   0 holzer     (502) staff       (20)    17979 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/runhelper/parameterstudy.py
--rw-r--r--   0 holzer     (502) staff       (20)      286 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/session.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.690729 pystencils-1.3.3/pystencils/simp/
--rw-r--r--   0 holzer     (502) staff       (20)     1352 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/simp/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)    22033 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/simp/assignment_collection.py
--rw-r--r--   0 holzer     (502) staff       (20)    11459 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/simp/simplifications.py
--rw-r--r--   0 holzer     (502) staff       (20)     6854 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/simp/simplificationstrategy.py
--rw-r--r--   0 holzer     (502) staff       (20)     3334 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/simp/subexpression_insertion.py
--rw-r--r--   0 holzer     (502) staff       (20)      804 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/simplificationfactory.py
--rw-r--r--   0 holzer     (502) staff       (20)     9760 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/slicing.py
--rw-r--r--   0 holzer     (502) staff       (20)      546 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/spatial_coordinates.py
--rw-r--r--   0 holzer     (502) staff       (20)    18401 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/stencil.py
--rw-r--r--   0 holzer     (502) staff       (20)    27160 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/sympyextensions.py
--rw-r--r--   0 holzer     (502) staff       (20)     4300 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/timeloop.py
--rw-r--r--   0 holzer     (502) staff       (20)    48977 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/transformations.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.691933 pystencils-1.3.3/pystencils/typing/
--rw-r--r--   0 holzer     (502) staff       (20)     1292 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/typing/__init__.py
--rw-r--r--   0 holzer     (502) staff       (20)     4156 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/typing/cast_functions.py
--rw-r--r--   0 holzer     (502) staff       (20)    14111 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/typing/leaf_typing.py
--rw-r--r--   0 holzer     (502) staff       (20)      987 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/typing/transformations.py
--rw-r--r--   0 holzer     (502) staff       (20)     5816 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/typing/typed_sympy.py
--rw-r--r--   0 holzer     (502) staff       (20)     9562 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/typing/types.py
--rw-r--r--   0 holzer     (502) staff       (20)     9044 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/typing/utilities.py
--rw-r--r--   0 holzer     (502) staff       (20)     8153 2024-01-06 15:47:25.000000 pystencils-1.3.3/pystencils/utils.py
-drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-01-06 15:51:04.677318 pystencils-1.3.3/pystencils.egg-info/
--rw-r--r--   0 holzer     (502) staff       (20)     4822 2024-01-06 15:51:04.000000 pystencils-1.3.3/pystencils.egg-info/PKG-INFO
--rw-r--r--   0 holzer     (502) staff       (20)     3379 2024-01-06 15:51:04.000000 pystencils-1.3.3/pystencils.egg-info/SOURCES.txt
--rw-r--r--   0 holzer     (502) staff       (20)        1 2024-01-06 15:51:04.000000 pystencils-1.3.3/pystencils.egg-info/dependency_links.txt
--rw-r--r--   0 holzer     (502) staff       (20)      312 2024-01-06 15:51:04.000000 pystencils-1.3.3/pystencils.egg-info/requires.txt
--rw-r--r--   0 holzer     (502) staff       (20)       11 2024-01-06 15:51:04.000000 pystencils-1.3.3/pystencils.egg-info/top_level.txt
--rw-r--r--   0 holzer     (502) staff       (20)      217 2024-01-06 15:51:04.692455 pystencils-1.3.3/setup.cfg
--rw-r--r--   0 holzer     (502) staff       (20)     5198 2024-01-06 15:47:25.000000 pystencils-1.3.3/setup.py
--rw-r--r--   0 holzer     (502) staff       (20)    70144 2024-01-06 15:47:25.000000 pystencils-1.3.3/versioneer.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.901525 pystencils-1.3.4/
+-rw-r--r--   0 holzer     (502) staff       (20)      502 2024-05-15 07:41:39.000000 pystencils-1.3.4/AUTHORS.txt
+-rw-r--r--   0 holzer     (502) staff       (20)      209 2024-05-15 07:41:39.000000 pystencils-1.3.4/CHANGELOG.md
+-rw-r--r--   0 holzer     (502) staff       (20)     3797 2024-05-15 07:41:39.000000 pystencils-1.3.4/CONTRIBUTING.md
+-rw-r--r--   0 holzer     (502) staff       (20)    34523 2024-05-15 07:41:39.000000 pystencils-1.3.4/COPYING.txt
+-rw-r--r--   0 holzer     (502) staff       (20)       65 2024-05-15 07:41:39.000000 pystencils-1.3.4/MANIFEST.in
+-rw-r--r--   0 holzer     (502) staff       (20)    44610 2024-05-15 07:44:25.901324 pystencils-1.3.4/PKG-INFO
+-rw-r--r--   0 holzer     (502) staff       (20)     3676 2024-05-15 07:41:39.000000 pystencils-1.3.4/README.md
+-rw-r--r--   0 holzer     (502) staff       (20)     2425 2024-05-15 07:41:39.000000 pystencils-1.3.4/pyproject.toml
+-rw-r--r--   0 holzer     (502) staff       (20)       38 2024-05-15 07:44:25.901563 pystencils-1.3.4/setup.cfg
+-rw-r--r--   0 holzer     (502) staff       (20)      671 2024-05-15 07:41:39.000000 pystencils-1.3.4/setup.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.867425 pystencils-1.3.4/src/
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.878638 pystencils-1.3.4/src/pystencils/
+-rw-r--r--   0 holzer     (502) staff       (20)     1679 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)      497 2024-05-15 07:44:25.901708 pystencils-1.3.4/src/pystencils/_version.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4895 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/alignedarray.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4429 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/assignment.py
+-rw-r--r--   0 holzer     (502) staff       (20)    28965 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/astnodes.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.880997 pystencils-1.3.4/src/pystencils/backends/
+-rw-r--r--   0 holzer     (502) staff       (20)      164 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6279 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/arm_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)    42082 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/cbackend.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2824 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/cuda_backend.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3539 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/dot.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2479 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/json.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3931 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/ppc_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3801 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/riscv_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4896 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/simd_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7196 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/backends/x86_instruction_sets.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1707 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/bit_masks.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.881920 pystencils-1.3.4/src/pystencils/boundaries/
+-rw-r--r--   0 holzer     (502) staff       (20)      284 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/boundaries/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4344 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/boundaries/boundaryconditions.py
+-rw-r--r--   0 holzer     (502) staff       (20)    21066 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/boundaries/boundaryhandling.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7980 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/boundaries/createindexlist.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7830 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/boundaries/createindexlistcython.pyx
+-rw-r--r--   0 holzer     (502) staff       (20)     2031 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/boundaries/inkernel.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2406 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/cache.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9617 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/config.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.882717 pystencils-1.3.4/src/pystencils/cpu/
+-rw-r--r--   0 holzer     (502) staff       (20)      266 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/cpu/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    27837 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/cpu/cpujit.py
+-rw-r--r--   0 holzer     (502) staff       (20)    11361 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/cpu/kernelcreation.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3758 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/cpu/msvc_detection.py
+-rw-r--r--   0 holzer     (502) staff       (20)    22385 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/cpu/vectorization.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.883686 pystencils-1.3.4/src/pystencils/datahandling/
+-rw-r--r--   0 holzer     (502) staff       (20)     3490 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/datahandling/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5636 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/datahandling/blockiteration.py
+-rw-r--r--   0 holzer     (502) staff       (20)    20890 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/datahandling/datahandling_interface.py
+-rw-r--r--   0 holzer     (502) staff       (20)    17403 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/datahandling/parallel_datahandling.py
+-rw-r--r--   0 holzer     (502) staff       (20)    20768 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/datahandling/serial_datahandling.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2136 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/datahandling/vtk.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3482 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/display_utils.py
+-rw-r--r--   0 holzer     (502) staff       (20)      713 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/enums.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2624 2024-05-15 07:41:39.000000 pystencils-1.3.4/src/pystencils/fast_approximation.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.884607 pystencils-1.3.4/src/pystencils/fd/
+-rw-r--r--   0 holzer     (502) staff       (20)      880 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/fd/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    14981 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/fd/derivation.py
+-rw-r--r--   0 holzer     (502) staff       (20)    21404 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/fd/derivative.py
+-rw-r--r--   0 holzer     (502) staff       (20)    15080 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/fd/finitedifferences.py
+-rw-r--r--   0 holzer     (502) staff       (20)    11806 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/fd/finitevolumes.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7060 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/fd/spatial.py
+-rw-r--r--   0 holzer     (502) staff       (20)    46517 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/field.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1538 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/functions.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.885515 pystencils-1.3.4/src/pystencils/gpu/
+-rw-r--r--   0 holzer     (502) staff       (20)      508 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/gpu/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3640 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/gpu/gpu_array_handler.py
+-rw-r--r--   0 holzer     (502) staff       (20)     8575 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/gpu/gpujit.py
+-rw-r--r--   0 holzer     (502) staff       (20)    19013 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/gpu/indexing.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9960 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/gpu/kernelcreation.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2092 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/gpu/periodicity.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.887057 pystencils-1.3.4/src/pystencils/include/
+-rw-r--r--   0 holzer     (502) staff       (20)      413 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/PyStencilsField.h
+-rw-r--r--   0 holzer     (502) staff       (20)      114 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    28148 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/aesni_rand.h
+-rw-r--r--   0 holzer     (502) staff       (20)     2208 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/arm_neon_helpers.h
+-rw-r--r--   0 holzer     (502) staff       (20)      293 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/gpu_defines.h
+-rw-r--r--   0 holzer     (502) staff       (20)      968 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/half_precision.h
+-rw-r--r--   0 holzer     (502) staff       (20)     4012 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/myintrin.h
+-rw-r--r--   0 holzer     (502) staff       (20)    58376 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/philox_rand.h
+-rw-r--r--   0 holzer     (502) staff       (20)     1007 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/ppc_altivec_helpers.h
+-rw-r--r--   0 holzer     (502) staff       (20)     1004 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/include/riscv_v_helpers.h
+-rw-r--r--   0 holzer     (502) staff       (20)     6390 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/integer_functions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2830 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/integer_set_analysis.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3989 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/jupyter.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5676 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/kernel_contrains_check.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5133 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/kernel_decorator.py
+-rw-r--r--   0 holzer     (502) staff       (20)      545 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/kernel_wrapper.py
+-rw-r--r--   0 holzer     (502) staff       (20)    19357 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/kernelcreation.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4176 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/node_collection.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2680 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/placeholder_function.py
+-rw-r--r--   0 holzer     (502) staff       (20)    13234 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/plot.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4822 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/rng.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.887498 pystencils-1.3.4/src/pystencils/runhelper/
+-rw-r--r--   0 holzer     (502) staff       (20)      150 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/runhelper/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9989 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/runhelper/db.py
+-rw-r--r--   0 holzer     (502) staff       (20)    17979 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/runhelper/parameterstudy.py
+-rw-r--r--   0 holzer     (502) staff       (20)      286 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/session.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.888300 pystencils-1.3.4/src/pystencils/simp/
+-rw-r--r--   0 holzer     (502) staff       (20)     1352 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/simp/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)    22048 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/simp/assignment_collection.py
+-rw-r--r--   0 holzer     (502) staff       (20)    11459 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/simp/simplifications.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6854 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/simp/simplificationstrategy.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3334 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/simp/subexpression_insertion.py
+-rw-r--r--   0 holzer     (502) staff       (20)      804 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/simplificationfactory.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9760 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/slicing.py
+-rw-r--r--   0 holzer     (502) staff       (20)      546 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/spatial_coordinates.py
+-rw-r--r--   0 holzer     (502) staff       (20)    18401 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/stencil.py
+-rw-r--r--   0 holzer     (502) staff       (20)    27164 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/sympyextensions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4300 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/timeloop.py
+-rw-r--r--   0 holzer     (502) staff       (20)    48977 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/transformations.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.889412 pystencils-1.3.4/src/pystencils/typing/
+-rw-r--r--   0 holzer     (502) staff       (20)     1292 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/typing/__init__.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4156 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/typing/cast_functions.py
+-rw-r--r--   0 holzer     (502) staff       (20)    14111 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/typing/leaf_typing.py
+-rw-r--r--   0 holzer     (502) staff       (20)      987 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/typing/transformations.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5816 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/typing/typed_sympy.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9562 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/typing/types.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9044 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/typing/utilities.py
+-rw-r--r--   0 holzer     (502) staff       (20)     8153 2024-05-15 07:41:40.000000 pystencils-1.3.4/src/pystencils/utils.py
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.879423 pystencils-1.3.4/src/pystencils.egg-info/
+-rw-r--r--   0 holzer     (502) staff       (20)    44610 2024-05-15 07:44:25.000000 pystencils-1.3.4/src/pystencils.egg-info/PKG-INFO
+-rw-r--r--   0 holzer     (502) staff       (20)     6000 2024-05-15 07:44:25.000000 pystencils-1.3.4/src/pystencils.egg-info/SOURCES.txt
+-rw-r--r--   0 holzer     (502) staff       (20)        1 2024-05-15 07:44:25.000000 pystencils-1.3.4/src/pystencils.egg-info/dependency_links.txt
+-rw-r--r--   0 holzer     (502) staff       (20)      453 2024-05-15 07:44:25.000000 pystencils-1.3.4/src/pystencils.egg-info/requires.txt
+-rw-r--r--   0 holzer     (502) staff       (20)       11 2024-05-15 07:44:25.000000 pystencils-1.3.4/src/pystencils.egg-info/top_level.txt
+drwxr-xr-x   0 holzer     (502) staff       (20)        0 2024-05-15 07:44:25.901048 pystencils-1.3.4/tests/
+-rw-r--r--   0 holzer     (502) staff       (20)     3624 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_Min_Max.py
+-rw-r--r--   0 holzer     (502) staff       (20)      617 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_abs.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1552 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_address_of.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2823 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_aligned_array.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6832 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_assignment_collection.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1133 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_assignment_collection_dict_conversion.py
+-rw-r--r--   0 holzer     (502) staff       (20)      630 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_assignment_from_stencil.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2362 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_astnodes.py
+-rw-r--r--   0 holzer     (502) staff       (20)      941 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_augmented_assignment.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2578 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_base_pointer_specification.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1213 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_bit_masks.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3186 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_blocking.py
+-rw-r--r--   0 holzer     (502) staff       (20)      962 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_blocking_staggered.py
+-rw-r--r--   0 holzer     (502) staff       (20)     9946 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_boundary.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5333 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_boundary_indexlist_creation.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12127 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_buffer.py
+-rw-r--r--   0 holzer     (502) staff       (20)    15006 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_buffer_gpu.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2310 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_conditional_field_access.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4847 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_conditional_vec.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4433 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_config.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1285 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_create_kernel_config.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1637 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_custom_backends.py
+-rw-r--r--   0 holzer     (502) staff       (20)    13467 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_datahandling.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6680 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_datahandling_parallel.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1786 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_derivative.py
+-rw-r--r--   0 holzer     (502) staff       (20)      421 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_dot_printer.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1126 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_dtype_check.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1603 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_fast_approximation.py
+-rw-r--r--   0 holzer     (502) staff       (20)      735 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_fd_derivative.py
+-rw-r--r--   0 holzer     (502) staff       (20)     8348 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_field.py
+-rw-r--r--   0 holzer     (502) staff       (20)      790 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_field_access_poly.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3435 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_finite_differences.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1786 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_floor_ceil_int_optimization.py
+-rw-r--r--   0 holzer     (502) staff       (20)    26645 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_fvm.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4056 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_global_definitions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     8185 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_gpu.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1360 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_half_precision.py
+-rw-r--r--   0 holzer     (502) staff       (20)      954 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_helpful_errors.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3363 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_indexed_kernels.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2778 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_jacobi_cbackend.py
+-rw-r--r--   0 holzer     (502) staff       (20)      769 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_json_backend.py
+-rw-r--r--   0 holzer     (502) staff       (20)      898 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_json_serializer.py
+-rw-r--r--   0 holzer     (502) staff       (20)      585 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_logarithm.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5707 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_loop_cutting.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2454 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_match_subs_for_assignment_collection.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3833 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_math_functions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1643 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_modulo.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2131 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_move_constant_before_loop.py
+-rw-r--r--   0 holzer     (502) staff       (20)      487 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_nodecollection.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2680 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_parameterstudy.py
+-rw-r--r--   0 holzer     (502) staff       (20)      486 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_pickle_support.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1872 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_plot.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3869 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_printing.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2733 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_quicktests.py
+-rw-r--r--   0 holzer     (502) staff       (20)    10346 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_random.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1885 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_sharedmethodcache.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2940 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_simplification_strategy.py
+-rw-r--r--   0 holzer     (502) staff       (20)     6734 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_simplifications.py
+-rw-r--r--   0 holzer     (502) staff       (20)     4674 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_size_and_layout_checks.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1060 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_sliced_iteration.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2449 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_slicing.py
+-rw-r--r--   0 holzer     (502) staff       (20)      839 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_source_code_comment.py
+-rw-r--r--   0 holzer     (502) staff       (20)     3963 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_staggered_kernel.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1138 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_stencils.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1704 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_struct_types.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1540 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_subexpression_insertion.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2462 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_sum_prod.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7403 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_sympyextensions.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2561 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_timeloop.py
+-rw-r--r--   0 holzer     (502) staff       (20)     5431 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_transformations.py
+-rw-r--r--   0 holzer     (502) staff       (20)     1184 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_type_interference.py
+-rw-r--r--   0 holzer     (502) staff       (20)     7754 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_types.py
+-rw-r--r--   0 holzer     (502) staff       (20)     2389 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_utils.py
+-rw-r--r--   0 holzer     (502) staff       (20)    13297 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_vectorization.py
+-rw-r--r--   0 holzer     (502) staff       (20)    12917 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_vectorization_specific.py
+-rw-r--r--   0 holzer     (502) staff       (20)      278 2024-05-15 07:41:40.000000 pystencils-1.3.4/tests/test_version_string.py
```

### Comparing `pystencils-1.3.3/CONTRIBUTING.md` & `pystencils-1.3.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/COPYING.txt` & `pystencils-1.3.4/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/README.md` & `pystencils-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/__init__.py` & `pystencils-1.3.4/src/pystencils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,11 +32,9 @@
            'kernel', 'kernel_config',
            'x_', 'y_', 'z_',
            'x_staggered', 'y_staggered', 'z_staggered',
            'x_vector', 'x_staggered_vector',
            'fd',
            'stencil']
 
-from ._version import get_versions
-
-__version__ = get_versions()['version']
-del get_versions
+from . import _version
+__version__ = _version.get_versions()['version']
```

### Comparing `pystencils-1.3.3/pystencils/alignedarray.py` & `pystencils-1.3.4/src/pystencils/alignedarray.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/assignment.py` & `pystencils-1.3.4/src/pystencils/assignment.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/astnodes.py` & `pystencils-1.3.4/src/pystencils/astnodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,15 +669,15 @@
         printed_rhs = sp.latex(self.rhs)
         return f"${printed_lhs} \\leftarrow {printed_rhs}$"
 
     def __hash__(self):
         return hash((self.lhs, self.rhs))
 
     def __eq__(self, other):
-        return type(self) == type(other) and (self.lhs, self.rhs) == (other.lhs, other.rhs)
+        return type(self) is type(other) and (self.lhs, self.rhs) == (other.lhs, other.rhs)
 
 
 class ResolvedFieldAccess(sp.Indexed):
     def __new__(cls, base, linearized_index, field, offsets, idx_coordinate_values):
         if not isinstance(base, sp.IndexedBase):
             assert isinstance(base, TypedSymbol)
             base = sp.IndexedBase(base, shape=(1,))
```

### Comparing `pystencils-1.3.3/pystencils/backends/arm_instruction_sets.py` & `pystencils-1.3.4/src/pystencils/backends/arm_instruction_sets.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/backends/cbackend.py` & `pystencils-1.3.4/src/pystencils/backends/cbackend.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         return self._symbols_defined
 
     @property
     def undefined_symbols(self):
         return self._symbols_read - self._symbols_defined
 
     def __eq__(self, other):
-        return type(self) == type(other) and self._code == other._code
+        return type(self) is type(other) and self._code == other._code
 
     def __hash__(self):
         return hash(self._code)
 
 
 class PrintNode(CustomCodeNode):
     # noinspection SpellCheckingInspection
```

### Comparing `pystencils-1.3.3/pystencils/backends/cuda_backend.py` & `pystencils-1.3.4/src/pystencils/backends/cuda_backend.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/backends/dot.py` & `pystencils-1.3.4/src/pystencils/backends/dot.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/backends/json.py` & `pystencils-1.3.4/src/pystencils/backends/json.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/backends/ppc_instruction_sets.py` & `pystencils-1.3.4/src/pystencils/backends/ppc_instruction_sets.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/backends/riscv_instruction_sets.py` & `pystencils-1.3.4/src/pystencils/backends/riscv_instruction_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,13 +94,16 @@
     result['+int'] = f"vadd_vv_i{bits['int']}m1({{0}}, {{1}}, {int_vl})"
 
     result['float'] = f'vfloat{bits["float"]}m1_t'
     result['double'] = f'vfloat{bits["double"]}m1_t'
     result['int'] = f'vint{bits["int"]}m1_t'
     result['bool'] = f'vbool{bits[data_type]}_t'
 
-    result['headers'] = ['<riscv_vector.h>']
+    result['headers'] = ['<riscv_vector.h>', '"riscv_v_helpers.h"']
 
     result['any'] += ' > 0x0'
     result['all'] += f' == vsetvl_e{bits[data_type]}m1({vl})'
 
+    result['cachelineSize'] = 'cachelineSize()'
+    result['cachelineZero'] = 'cachelineZero((void*) {0})'
+
     return result
```

### Comparing `pystencils-1.3.3/pystencils/backends/simd_instruction_sets.py` & `pystencils-1.3.4/src/pystencils/backends/simd_instruction_sets.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/backends/x86_instruction_sets.py` & `pystencils-1.3.4/src/pystencils/backends/x86_instruction_sets.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/bit_masks.py` & `pystencils-1.3.4/src/pystencils/bit_masks.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/boundaries/boundaryconditions.py` & `pystencils-1.3.4/src/pystencils/boundaries/boundaryconditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             return [SympyAssignment(field(*idx), field[neighbor](*idx)) for idx in index_iter]
 
     def __hash__(self):
         # All boundaries of these class behave equal -> should also be equal
         return hash("Neumann")
 
     def __eq__(self, other):
-        return type(other) == Neumann
+        return type(other) is Neumann
 
 
 class Dirichlet(Boundary):
 
     inner_or_boundary = False
     single_link = True
```

### Comparing `pystencils-1.3.3/pystencils/boundaries/boundaryhandling.py` & `pystencils-1.3.4/src/pystencils/boundaries/boundaryhandling.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/boundaries/createindexlist.py` & `pystencils-1.3.4/src/pystencils/boundaries/createindexlist.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,88 @@
 import warnings
 
 import numpy as np
 
+
 try:
-    # Try to import right away - assume compiled code is available
-    # compile with: python setup.py build_ext --inplace --use-cython
-    from pystencils.boundaries.createindexlistcython import create_boundary_neighbor_index_list_2d, \
-        create_boundary_neighbor_index_list_3d, create_boundary_cell_index_list_2d, create_boundary_cell_index_list_3d
+    import pyximport
 
+    pyximport.install(language_level=3)
     cython_funcs_available = True
 except ImportError:
-    try:
-        # If not, try development mode and import via pyximport
-        import pyximport
-
-        pyximport.install(language_level=3)
-        cython_funcs_available = True
-    except ImportError:
-        cython_funcs_available = False
-    if cython_funcs_available:
-        from pystencils.boundaries.createindexlistcython import create_boundary_neighbor_index_list_2d, \
-            create_boundary_neighbor_index_list_3d, create_boundary_cell_index_list_2d, \
-            create_boundary_cell_index_list_3d
+    cython_funcs_available = False
+
+if cython_funcs_available:
+    from pystencils.boundaries.createindexlistcython import (
+        create_boundary_neighbor_index_list_2d,
+        create_boundary_neighbor_index_list_3d,
+        create_boundary_cell_index_list_2d,
+        create_boundary_cell_index_list_3d,
+    )
 
 boundary_index_array_coordinate_names = ["x", "y", "z"]
 direction_member_name = "dir"
 default_index_array_dtype = np.int32
 
 
 def numpy_data_type_for_boundary_object(boundary_object, dim):
     coordinate_names = boundary_index_array_coordinate_names[:dim]
-    return np.dtype([(name, default_index_array_dtype) for name in coordinate_names]
-                    + [(direction_member_name, default_index_array_dtype)]
-                    + [(i[0], i[1].numpy_dtype) for i in boundary_object.additional_data], align=True)
-
-
-def _create_index_list_python(flag_field_arr, boundary_mask,
-                              fluid_mask, stencil, single_link, inner_or_boundary=False, nr_of_ghost_layers=None):
-
+    return np.dtype(
+        [(name, default_index_array_dtype) for name in coordinate_names]
+        + [(direction_member_name, default_index_array_dtype)]
+        + [(i[0], i[1].numpy_dtype) for i in boundary_object.additional_data],
+        align=True,
+    )
+
+
+def _create_index_list_python(
+    flag_field_arr,
+    boundary_mask,
+    fluid_mask,
+    stencil,
+    single_link,
+    inner_or_boundary=False,
+    nr_of_ghost_layers=None,
+):
     if inner_or_boundary and nr_of_ghost_layers is None:
-        raise ValueError("If inner_or_boundary is set True the number of ghost layers "
-                         "around the inner domain has to be specified")
+        raise ValueError(
+            "If inner_or_boundary is set True the number of ghost layers "
+            "around the inner domain has to be specified"
+        )
 
     if nr_of_ghost_layers is None:
         nr_of_ghost_layers = 0
 
-    coordinate_names = boundary_index_array_coordinate_names[:len(flag_field_arr.shape)]
-    index_arr_dtype = np.dtype([(name, default_index_array_dtype) for name in coordinate_names]
-                               + [(direction_member_name, default_index_array_dtype)])
+    coordinate_names = boundary_index_array_coordinate_names[
+        : len(flag_field_arr.shape)
+    ]
+    index_arr_dtype = np.dtype(
+        [(name, default_index_array_dtype) for name in coordinate_names]
+        + [(direction_member_name, default_index_array_dtype)]
+    )
 
     # boundary cells are extracted via np.where. To ensure continous memory access in the compute kernel these cells
     # have to be sorted.
     boundary_cells = np.transpose(np.nonzero(flag_field_arr == boundary_mask))
     for i in range(len(flag_field_arr.shape)):
-        boundary_cells = boundary_cells[boundary_cells[:, i].argsort(kind='mergesort')]
+        boundary_cells = boundary_cells[boundary_cells[:, i].argsort(kind="mergesort")]
 
     # First a set is created to save all fluid cells which are near boundary
     fluid_cells = set()
     for cell in boundary_cells:
         cell = tuple(cell)
         for dir_idx, direction in enumerate(stencil):
-            neighbor_cell = tuple([cell_i + dir_i for cell_i, dir_i in zip(cell, direction)])
+            neighbor_cell = tuple(
+                [cell_i + dir_i for cell_i, dir_i in zip(cell, direction)]
+            )
             # prevent out ouf bounds access. If boundary cell is at the border, some stencil directions would be out.
-            if any(not 0 + nr_of_ghost_layers <= e < upper - nr_of_ghost_layers
-                   for e, upper in zip(neighbor_cell, flag_field_arr.shape)):
+            if any(
+                not 0 + nr_of_ghost_layers <= e < upper - nr_of_ghost_layers
+                for e, upper in zip(neighbor_cell, flag_field_arr.shape)
+            ):
                 continue
             if flag_field_arr[neighbor_cell] & fluid_mask:
                 fluid_cells.add(neighbor_cell)
 
     # then this is set is transformed to a list to make it sortable. This ensures continoous memory access later.
     fluid_cells = list(fluid_cells)
     if len(flag_field_arr.shape) == 3:
@@ -79,17 +94,22 @@
     checkmask = boundary_mask if inner_or_boundary else fluid_mask
 
     result = []
     for cell in cells_to_iterate:
         cell = tuple(cell)
         sum_cells = np.zeros(len(cell))
         for dir_idx, direction in enumerate(stencil):
-            neighbor_cell = tuple([cell_i + dir_i for cell_i, dir_i in zip(cell, direction)])
+            neighbor_cell = tuple(
+                [cell_i + dir_i for cell_i, dir_i in zip(cell, direction)]
+            )
             # prevent out ouf bounds access. If boundary cell is at the border, some stencil directions would be out.
-            if any(not 0 <= e < upper for e, upper in zip(neighbor_cell, flag_field_arr.shape)):
+            if any(
+                not 0 <= e < upper
+                for e, upper in zip(neighbor_cell, flag_field_arr.shape)
+            ):
                 continue
             if flag_field_arr[neighbor_cell] & checkmask:
                 if single_link:
                     sum_cells += np.array(direction)
                 else:
                     result.append(tuple(cell) + (dir_idx,))
 
@@ -97,16 +117,23 @@
         if single_link and any(sum_cells != 0):
             idx = np.argmax(np.inner(sum_cells, stencil))
             result.append(tuple(cell) + (idx,))
 
     return np.array(result, dtype=index_arr_dtype)
 
 
-def create_boundary_index_list(flag_field, stencil, boundary_mask, fluid_mask,
-                               nr_of_ghost_layers=1, inner_or_boundary=True, single_link=False):
+def create_boundary_index_list(
+    flag_field,
+    stencil,
+    boundary_mask,
+    fluid_mask,
+    nr_of_ghost_layers=1,
+    inner_or_boundary=True,
+    single_link=False,
+):
     """Creates a numpy array storing links (connections) between domain cells and boundary cells.
 
     Args:
         flag_field: flag integer array where boundary and domain cells are marked (interpreted as bit vector)
         stencil: list of directions, for possible links. When single_link is set to true the order matters, because
                  then only the first link is added to the list
         boundary_mask: cells where (cell & mask) is true are considered boundary cells
@@ -115,19 +142,28 @@
         inner_or_boundary: if true, the result contains the cell coordinates of the domain cells -
                     if false the boundary cells are listed
         single_link: if true only the link in normal direction to this cell is reported
 
     """
     dim = len(flag_field.shape)
     coordinate_names = boundary_index_array_coordinate_names[:dim]
-    index_arr_dtype = np.dtype([(name, default_index_array_dtype) for name in coordinate_names]
-                               + [(direction_member_name, default_index_array_dtype)])
+    index_arr_dtype = np.dtype(
+        [(name, default_index_array_dtype) for name in coordinate_names]
+        + [(direction_member_name, default_index_array_dtype)]
+    )
 
     stencil = np.array(stencil, dtype=default_index_array_dtype)
-    args = (flag_field, nr_of_ghost_layers, boundary_mask, fluid_mask, stencil, single_link)
+    args = (
+        flag_field,
+        nr_of_ghost_layers,
+        boundary_mask,
+        fluid_mask,
+        stencil,
+        single_link,
+    )
     args_no_gl = (flag_field, boundary_mask, fluid_mask, stencil, single_link)
 
     if cython_funcs_available:
         if dim == 2:
             if inner_or_boundary:
                 idx_list = create_boundary_neighbor_index_list_2d(*args)
             else:
@@ -138,28 +174,48 @@
             else:
                 idx_list = create_boundary_cell_index_list_3d(*args_no_gl)
         else:
             raise ValueError("Flag field has to be a 2 or 3 dimensional numpy array")
         return np.array(idx_list, dtype=index_arr_dtype)
     else:
         if flag_field.size > 1e6:
-            warnings.warn("Boundary setup may take very long! Consider installing cython to speed it up")
-        return _create_index_list_python(*args_no_gl, inner_or_boundary=inner_or_boundary,
-                                         nr_of_ghost_layers=nr_of_ghost_layers)
-
-
-def create_boundary_index_array(flag_field, stencil, boundary_mask, fluid_mask, boundary_object,
-                                nr_of_ghost_layers=1, inner_or_boundary=True, single_link=False):
-    idx_array = create_boundary_index_list(flag_field, stencil, boundary_mask, fluid_mask,
-                                           nr_of_ghost_layers, inner_or_boundary, single_link)
+            warnings.warn(
+                "Boundary setup may take very long! Consider installing cython to speed it up"
+            )
+        return _create_index_list_python(
+            *args_no_gl,
+            inner_or_boundary=inner_or_boundary,
+            nr_of_ghost_layers=nr_of_ghost_layers,
+        )
+
+
+def create_boundary_index_array(
+    flag_field,
+    stencil,
+    boundary_mask,
+    fluid_mask,
+    boundary_object,
+    nr_of_ghost_layers=1,
+    inner_or_boundary=True,
+    single_link=False,
+):
+    idx_array = create_boundary_index_list(
+        flag_field,
+        stencil,
+        boundary_mask,
+        fluid_mask,
+        nr_of_ghost_layers,
+        inner_or_boundary,
+        single_link,
+    )
     dim = len(flag_field.shape)
 
     if boundary_object.additional_data:
         coordinate_names = boundary_index_array_coordinate_names[:dim]
         index_arr_dtype = numpy_data_type_for_boundary_object(boundary_object, dim)
         extended_idx_field = np.empty(len(idx_array), dtype=index_arr_dtype)
-        for prop in coordinate_names + ['dir']:
+        for prop in coordinate_names + ["dir"]:
             extended_idx_field[prop] = idx_array[prop]
 
         idx_array = extended_idx_field
 
     return idx_array
```

### Comparing `pystencils-1.3.3/pystencils/boundaries/createindexlistcython.pyx` & `pystencils-1.3.4/src/pystencils/boundaries/createindexlistcython.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# distutils: language=c
-# Workaround for cython bug
-# see https://stackoverflow.com/questions/8024805/cython-compiled-c-extension-importerror-dynamic-module-does-not-define-init-fu
-WORKAROUND = "Something"
+# cython: language_level=3str
 
 import cython
 
 ctypedef fused IntegerType:
     short
     int
     long
```

### Comparing `pystencils-1.3.3/pystencils/boundaries/inkernel.py` & `pystencils-1.3.4/src/pystencils/boundaries/inkernel.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/cache.py` & `pystencils-1.3.4/src/pystencils/cache.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/config.py` & `pystencils-1.3.4/src/pystencils/config.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/cpu/cpujit.py` & `pystencils-1.3.4/src/pystencils/cpu/cpujit.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/cpu/kernelcreation.py` & `pystencils-1.3.4/src/pystencils/cpu/kernelcreation.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/cpu/msvc_detection.py` & `pystencils-1.3.4/src/pystencils/cpu/msvc_detection.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/cpu/vectorization.py` & `pystencils-1.3.4/src/pystencils/cpu/vectorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
     def visit_expr(expr, default_type='double', force_vectorize=False):
         if isinstance(expr, VectorMemoryAccess):
             return VectorMemoryAccess(*expr.args[0:4], visit_expr(expr.args[4], default_type, force_vectorize),
                                       *expr.args[5:])
         elif isinstance(expr, CastFunc):
             cast_type = expr.args[1]
             arg = visit_expr(expr.args[0], default_type, force_vectorize)
-            assert cast_type in [BasicType('float32'), BasicType('float64')],\
+            assert cast_type in [BasicType('float32'), BasicType('float64')], \
                 f'Vectorization cannot vectorize type {cast_type}'
             return expr.func(arg, VectorType(cast_type, instruction_set['width']))
         elif expr.func is sp.Abs and 'abs' not in instruction_set:
             new_arg = visit_expr(expr.args[0], default_type, force_vectorize)
             base_type = get_type_of_expression(expr.args[0]).base_type if type(expr.args[0]) is VectorMemoryAccess \
                 else get_type_of_expression(expr.args[0])
             pw = sp.Piecewise((-new_arg, new_arg < CastFunc(0, base_type.numpy_dtype)),
```

### Comparing `pystencils-1.3.3/pystencils/datahandling/__init__.py` & `pystencils-1.3.4/src/pystencils/datahandling/__init__.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/datahandling/blockiteration.py` & `pystencils-1.3.4/src/pystencils/datahandling/blockiteration.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/datahandling/datahandling_interface.py` & `pystencils-1.3.4/src/pystencils/datahandling/datahandling_interface.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/datahandling/parallel_datahandling.py` & `pystencils-1.3.4/src/pystencils/datahandling/parallel_datahandling.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/datahandling/serial_datahandling.py` & `pystencils-1.3.4/src/pystencils/datahandling/serial_datahandling.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/datahandling/vtk.py` & `pystencils-1.3.4/src/pystencils/datahandling/vtk.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/display_utils.py` & `pystencils-1.3.4/src/pystencils/display_utils.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/enums.py` & `pystencils-1.3.4/src/pystencils/enums.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/fast_approximation.py` & `pystencils-1.3.4/src/pystencils/fast_approximation.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/fd/__init__.py` & `pystencils-1.3.4/src/pystencils/fd/__init__.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/fd/derivation.py` & `pystencils-1.3.4/src/pystencils/fd/derivation.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/fd/derivative.py` & `pystencils-1.3.4/src/pystencils/fd/derivative.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/fd/finitedifferences.py` & `pystencils-1.3.4/src/pystencils/fd/finitedifferences.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/fd/finitevolumes.py` & `pystencils-1.3.4/src/pystencils/fd/finitevolumes.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/fd/spatial.py` & `pystencils-1.3.4/src/pystencils/fd/spatial.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/field.py` & `pystencils-1.3.4/src/pystencils/field.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/functions.py` & `pystencils-1.3.4/src/pystencils/functions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/gpu/gpu_array_handler.py` & `pystencils-1.3.4/src/pystencils/gpu/gpu_array_handler.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/gpu/gpujit.py` & `pystencils-1.3.4/src/pystencils/gpu/gpujit.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/gpu/indexing.py` & `pystencils-1.3.4/src/pystencils/gpu/indexing.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/gpu/kernelcreation.py` & `pystencils-1.3.4/src/pystencils/gpu/kernelcreation.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/gpu/periodicity.py` & `pystencils-1.3.4/src/pystencils/gpu/periodicity.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/include/aesni_rand.h` & `pystencils-1.3.4/src/pystencils/include/aesni_rand.h`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/include/arm_neon_helpers.h` & `pystencils-1.3.4/src/pystencils/include/arm_neon_helpers.h`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/include/half_precision.h` & `pystencils-1.3.4/src/pystencils/include/half_precision.h`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/include/myintrin.h` & `pystencils-1.3.4/src/pystencils/include/myintrin.h`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/include/philox_rand.h` & `pystencils-1.3.4/src/pystencils/include/philox_rand.h`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/include/ppc_altivec_helpers.h` & `pystencils-1.3.4/src/pystencils/include/ppc_altivec_helpers.h`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/integer_functions.py` & `pystencils-1.3.4/src/pystencils/integer_functions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/integer_set_analysis.py` & `pystencils-1.3.4/src/pystencils/integer_set_analysis.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/jupyter.py` & `pystencils-1.3.4/src/pystencils/jupyter.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/kernel_contrains_check.py` & `pystencils-1.3.4/src/pystencils/kernel_contrains_check.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/kernel_decorator.py` & `pystencils-1.3.4/src/pystencils/kernel_decorator.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/kernel_wrapper.py` & `pystencils-1.3.4/src/pystencils/kernel_wrapper.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/kernelcreation.py` & `pystencils-1.3.4/src/pystencils/kernelcreation.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/node_collection.py` & `pystencils-1.3.4/src/pystencils/node_collection.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/placeholder_function.py` & `pystencils-1.3.4/src/pystencils/placeholder_function.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/plot.py` & `pystencils-1.3.4/src/pystencils/plot.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/rng.py` & `pystencils-1.3.4/src/pystencils/rng.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         return ", ".join([str(s) for s in self.result_symbols]) + " \\leftarrow " + \
             self._name.capitalize() + "_RNG(" + ", ".join([str(a) for a in self.args]) + ")"
 
     def _hashable_content(self):
         return (self._name, *self.result_symbols, *self.args)
 
     def __eq__(self, other):
-        return type(self) == type(other) and self._hashable_content() == other._hashable_content()
+        return type(self) is type(other) and self._hashable_content() == other._hashable_content()
 
     def __hash__(self):
         return hash(self._hashable_content())
 
 
 class PhiloxTwoDoubles(RNGBase):
     _name = "philox_double2"
```

### Comparing `pystencils-1.3.3/pystencils/runhelper/db.py` & `pystencils-1.3.4/src/pystencils/runhelper/db.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/runhelper/parameterstudy.py` & `pystencils-1.3.4/src/pystencils/runhelper/parameterstudy.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/simp/__init__.py` & `pystencils-1.3.4/src/pystencils/simp/__init__.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/simp/assignment_collection.py` & `pystencils-1.3.4/src/pystencils/simp/assignment_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,20 +282,21 @@
 
         own_subexpression_symbols = {e.lhs: e.rhs for e in self.subexpressions}
         substitution_dict = {}
 
         processed_other_subexpression_equations = []
         for other_subexpression_eq in other.subexpressions:
             if other_subexpression_eq.lhs in own_subexpression_symbols:
-                if other_subexpression_eq.rhs == own_subexpression_symbols[other_subexpression_eq.lhs]:
+                new_rhs = fast_subs(other_subexpression_eq.rhs, substitution_dict)
+                if new_rhs == own_subexpression_symbols[other_subexpression_eq.lhs]:
                     continue  # exact the same subexpression equation exists already
                 else:
                     # different definition - a new name has to be introduced
                     new_lhs = next(self.subexpression_symbol_generator)
-                    new_eq = Assignment(new_lhs, fast_subs(other_subexpression_eq.rhs, substitution_dict))
+                    new_eq = Assignment(new_lhs, new_rhs)
                     processed_other_subexpression_equations.append(new_eq)
                     substitution_dict[other_subexpression_eq.lhs] = new_lhs
             else:
                 processed_other_subexpression_equations.append(fast_subs(other_subexpression_eq, substitution_dict))
 
         processed_other_main_assignments = [fast_subs(eq, substitution_dict) for eq in other.main_assignments]
         return self.copy(self.main_assignments + processed_other_main_assignments,
```

### Comparing `pystencils-1.3.3/pystencils/simp/simplifications.py` & `pystencils-1.3.4/src/pystencils/simp/simplifications.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/simp/simplificationstrategy.py` & `pystencils-1.3.4/src/pystencils/simp/simplificationstrategy.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/simp/subexpression_insertion.py` & `pystencils-1.3.4/src/pystencils/simp/subexpression_insertion.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/simplificationfactory.py` & `pystencils-1.3.4/src/pystencils/simplificationfactory.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/slicing.py` & `pystencils-1.3.4/src/pystencils/slicing.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/spatial_coordinates.py` & `pystencils-1.3.4/src/pystencils/spatial_coordinates.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/stencil.py` & `pystencils-1.3.4/src/pystencils/stencil.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/sympyextensions.py` & `pystencils-1.3.4/src/pystencils/sympyextensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,31 +352,31 @@
     result = 0
     expr = expr.expand()
 
     def velocity_factors_in_product(product):
         factor_count = 0
         if type(product) is Mul:
             for factor in product.args:
-                if type(factor) == Pow:
+                if type(factor) is Pow:
                     if factor.args[0] in symbols:
                         factor_count += factor.args[1]
                 if factor in symbols:
                     factor_count += 1
         elif type(product) is Pow:
             if product.args[0] in symbols:
                 factor_count += product.args[1]
         return factor_count
 
-    if type(expr) == Mul or type(expr) == Pow:
+    if type(expr) is Mul or type(expr) is Pow:
         if velocity_factors_in_product(expr) <= order:
             return expr
         else:
             return Zero()
 
-    if type(expr) != Add:
+    if type(expr) is not Add:
         return expr
 
     for sum_term in expr.args:
         if velocity_factors_in_product(sum_term) <= order:
             result += sum_term
     return result
```

### Comparing `pystencils-1.3.3/pystencils/timeloop.py` & `pystencils-1.3.4/src/pystencils/timeloop.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/transformations.py` & `pystencils-1.3.4/src/pystencils/transformations.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/typing/__init__.py` & `pystencils-1.3.4/src/pystencils/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/typing/cast_functions.py` & `pystencils-1.3.4/src/pystencils/typing/cast_functions.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/typing/leaf_typing.py` & `pystencils-1.3.4/src/pystencils/typing/leaf_typing.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/typing/transformations.py` & `pystencils-1.3.4/src/pystencils/typing/transformations.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/typing/typed_sympy.py` & `pystencils-1.3.4/src/pystencils/typing/typed_sympy.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/typing/types.py` & `pystencils-1.3.4/src/pystencils/typing/types.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/typing/utilities.py` & `pystencils-1.3.4/src/pystencils/typing/utilities.py`

 * *Files identical despite different names*

### Comparing `pystencils-1.3.3/pystencils/utils.py` & `pystencils-1.3.4/src/pystencils/utils.py`

 * *Files identical despite different names*

