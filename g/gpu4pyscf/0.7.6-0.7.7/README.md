# Comparing `tmp/gpu4pyscf-0.7.6.tar.gz` & `tmp/gpu4pyscf-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpu4pyscf-0.7.6.tar", last modified: Sun Apr  7 17:40:23 2024, max compression
+gzip compressed data, was "gpu4pyscf-0.7.7.tar", last modified: Wed May 15 06:45:05 2024, max compression
```

## Comparing `gpu4pyscf-0.7.6.tar` & `gpu4pyscf-0.7.7.tar`

### file list

```diff
@@ -1,113 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.621297 gpu4pyscf-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 17:40:23.621297 gpu4pyscf-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.605296 gpu4pyscf-0.7.6/gpu4pyscf/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/__config__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.609296 gpu4pyscf-0.7.6/gpu4pyscf/cc/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24054 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/cc/ccsd_incore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.609296 gpu4pyscf-0.7.6/gpu4pyscf/df/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/cderi.py
--rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/df.py
--rw-r--r--   0 runner    (1001) docker     (127)    15227 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/df_jk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.609296 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/grad/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.609296 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    30912 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/uks.py
--rw-r--r--   0 runner    (1001) docker     (127)    66842 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/df/int3c2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/dft/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21779 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/gen_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/gks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/libxc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/libxc_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    75728 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/numint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/radi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/roks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/uks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/xc_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/dft/xc_deriv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/fci/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/fci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/fci/direct_spin1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25756 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19167 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/grad/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/gto/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/gto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/gto/mole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25241 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/rhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    30559 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/rks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20051 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/uhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    42163 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/hessian/uks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.613296 gpu4pyscf-0.7.6/gpu4pyscf/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/cublas.py
--rw-r--r--   0 runner    (1001) docker     (127)    23683 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/cupy_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/cusolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/cutensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/dftd3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/dftd4.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/diis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/mp/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/mp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/mp/dfmp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/mp/mp2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/qmmm/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/qmmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/qmmm/chelpg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/scf/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/_response_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/cphf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/diis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/ghf.py
--rw-r--r--   0 runner    (1001) docker     (127)    38435 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/int4c2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/rohf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/ucphf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/scf/uhf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/solvent/
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/_attach_solvent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12921 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/smd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.617296 gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13153 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/smd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/pcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    27453 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf/solvent/smd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:40:23.605296 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/gpu4pyscf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 17:40:23.621297 gpu4pyscf-0.7.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4469 2024-04-07 17:40:23.000000 gpu4pyscf-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24054 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/cc/ccsd_incore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf/df/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/cderi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15569 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/df_jk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/grad/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24763 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30903 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/uks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67266 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/df/int3c2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21779 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/gen_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/gks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/libxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/libxc_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75748 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/numint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/radi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/roks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/uks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/xc_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/dft/xc_deriv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/fci/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/fci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/fci/direct_spin1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/grad/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.235337 gpu4pyscf-0.7.7/gpu4pyscf/gto/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/gto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/gto/mole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25241 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/rhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30559 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/rks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20252 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/uhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42163 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/hessian/uks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/cublas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/cupy_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/cusolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/cutensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/dftd3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/dftd4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/diis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/mp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/mp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/mp/dfmp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/mp/mp2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/properties/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/properties/polarizability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/properties/shielding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.239337 gpu4pyscf-0.7.7/gpu4pyscf/qmmm/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/qmmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/qmmm/chelpg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/gpu4pyscf/scf/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/_response_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/cphf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/diis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/ghf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38454 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/int4c2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/rohf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/ucphf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/scf/uhf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/gpu4pyscf/solvent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/_attach_solvent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/smd_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/smd_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15225 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/smd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/gpu4pyscf/solvent/smd_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:45:05.231337 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 06:45:05.000000 gpu4pyscf-0.7.7/gpu4pyscf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:45:05.243337 gpu4pyscf-0.7.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4469 2024-05-15 06:45:04.000000 gpu4pyscf-0.7.7/setup.py
```

### Comparing `gpu4pyscf-0.7.6/LICENSE` & `gpu4pyscf-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/MANIFEST.in` & `gpu4pyscf-0.7.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/README.md` & `gpu4pyscf-0.7.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 GPU plugin for PySCF
 ====================
+[![arXiv](https://img.shields.io/badge/arXiv-2404.09452-b31b1b.svg)](https://arxiv.org/abs/2404.09452)
+![nightly](https://github.com/pyscf/gpu4pyscf/actions/workflows/nightly_build.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/gpu4pyscf-cuda11x.svg)](https://badge.fury.io/py/gpu4pyscf-cuda11x)
+
 Installation
 --------
 
 > [!NOTE]
 > The compiled binary packages support compute capability 6.0 and later (Pascal and later, such as Tesla P100, RTX 10 series and later).
 
 Run ```nvidia-smi``` in your terminal to check the installed CUDA version.
@@ -52,16 +56,16 @@
 - Unrestricted Hartree-Fock and Unrestricted DFT, gradient, and Hessian
 - MP2/DF-MP2 and CCSD (experimental)
 
 Limitations
 --------
 - Rys roots up to 9 for density fitting scheme and direct scf scheme;
 - Atomic basis up to g orbitals;
-- Auxiliary basis up to h orbitals;
-- Density fitting scheme up to ~168 atoms with def2-tzvpd basis, bounded CPU memory;
+- Auxiliary basis up to i orbitals;
+- Density fitting scheme up to ~168 atoms with def2-tzvpd basis, bounded by CPU memory;
 - Hessian is unavailable for Direct SCF yet;
 - meta-GGA without density laplacian;
 
 Examples
 --------
 ```python
 import pyscf
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/__config__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/__config__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     min_grid_blksize = 128*128
     ao_aligned = 32
     grid_aligned = 128
     mem_fraction = 0.9
     number_of_threads = 1024 * 80
 # other gaming cards
 else:
-    min_ao_blksize = 32
-    min_grid_blksize = 32*32
-    ao_aligned = 8
+    min_ao_blksize = 64
+    min_grid_blksize = 64*64
+    ao_aligned = 32
     grid_aligned = 128
     mem_fraction = 0.9
     number_of_threads = 1024 * 80
 
 cupy.get_default_memory_pool().set_limit(fraction=mem_fraction)
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/cc/ccsd_incore.py` & `gpu4pyscf-0.7.7/gpu4pyscf/cc/ccsd_incore.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/cderi.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/cderi.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/df.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/df.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 
 import copy
 import cupy
 import ctypes
 import numpy as np
 from cupyx.scipy.linalg import solve_triangular
 from pyscf import lib
-from pyscf.df import df, addons
+from pyscf.df import df, addons, incore
 from gpu4pyscf.lib.cupy_helper import (
     cholesky, tag_array, get_avail_mem, cart2sph, take_last2d, transpose_sum)
 from gpu4pyscf.df import int3c2e, df_jk
 from gpu4pyscf.lib import logger
 from gpu4pyscf import __config__
 from cupyx import scipy
 
 MIN_BLK_SIZE = getattr(__config__, 'min_ao_blksize', 128)
 ALIGNED = getattr(__config__, 'ao_aligned', 32)
-LINEAR_DEP_TOL = 1e-7
+LINEAR_DEP_TOL = incore.LINEAR_DEP_THR
 
 class DF(lib.StreamObject):
     from gpu4pyscf.lib.utils import to_gpu, device
 
     _keys = {'intopt', 'mol', 'auxmol'}
 
     def __init__(self, mol, auxbasis=None):
@@ -132,31 +132,27 @@
         blksize = min(blksize, MIN_BLK_SIZE)
         log = logger.new_logger(self.mol, self.mol.verbose)
         log.debug(f"GPU Memory {mem_avail/1e9:.3f} GB available, block size = {blksize}")
         if blksize < ALIGNED:
             raise RuntimeError("Not enough GPU memory")
         return blksize
 
-
     def loop(self, blksize=None, unpack=True):
-        '''
-        loop over all cderi and unpack
-        '''
+        ''' loop over all cderi and unpack the CDERI in (Lij) format '''
         cderi_sparse = self._cderi
         if blksize is None:
             blksize = self.get_blksize()
         nao = self.nao
         naux = self.naux
         rows = self.intopt.cderi_row
         cols = self.intopt.cderi_col
         buf_prefetch = None
         buf_cderi = cupy.zeros([blksize,nao,nao])
         data_stream = cupy.cuda.stream.Stream(non_blocking=True)
         compute_stream = cupy.cuda.get_current_stream()
-        #compute_stream = cupy.cuda.stream.Stream()
         for p0, p1 in lib.prange(0, naux, blksize):
             p2 = min(naux, p1+blksize)
             if isinstance(cderi_sparse, cupy.ndarray):
                 buf = cderi_sparse[p0:p1,:]
             if isinstance(cderi_sparse, np.ndarray):
                 # first block
                 if buf_prefetch is None:
@@ -225,14 +221,15 @@
             cderi = np.ndarray([naux, npair], dtype=np.float64, order='C', buffer=mem)
         except Exception:
             raise RuntimeError('Out of CPU memory')
     if(not use_gpu_memory):
         data_stream = cupy.cuda.stream.Stream(non_blocking=False)
     count = 0
     nq = len(intopt.log_qs)
+    cd_low_f = cupy.array(cd_low, order='F', copy=False)
     for cp_ij_id, _ in enumerate(intopt.log_qs):
         if len(intopt.ao_pairs_row[cp_ij_id]) == 0: continue
         t1 = log.init_timer()
         cpi = intopt.cp_idx[cp_ij_id]
         cpj = intopt.cp_jdx[cp_ij_id]
         li = intopt.angular[cpi]
         lj = intopt.angular[cpj]
@@ -272,17 +269,15 @@
         col = intopt.ao_pairs_col[cp_ij_id] - j0
 
         ints_slices = ints_slices[:,col,row]
         if cd_low.tag == 'eig':
             cderi_block = cupy.dot(cd_low.T, ints_slices)
             ints_slices = None
         elif cd_low.tag == 'cd':
-            #cderi_block = solve_triangular(cd_low, ints_slices)
-            # TODO: create array in f-contiguous to avoid memory copy
-            cderi_block = solve_triangular(cd_low, ints_slices, lower=True, overwrite_b=False)
+            cderi_block = solve_triangular(cd_low_f, ints_slices, lower=True, overwrite_b=True)
         ij0, ij1 = count, count+cderi_block.shape[1]
         count = ij1
         if isinstance(cderi, cupy.ndarray):
             cderi[:,ij0:ij1] = cderi_block
         else:
             with data_stream:
                 for i in range(naux):
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/df_jk.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/df_jk.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             The default basis 'weigend+etb' means weigend-coulomb-fit basis
             for light elements and even-tempered basis for heavy elements.
         with_df : DF object
             Set mf.with_df = None to switch off density fitting mode.
     '''
     to_gpu = utils.to_gpu
     device = utils.device
-
+    __name_mixin__ = 'DF'
     _keys = {'rhoj', 'rhok', 'disp', 'screen_tol'}
 
     def __init__(self, mf, dfobj, only_dfj):
         self.__dict__.update(mf.__dict__)
         self._eri = None
         self.rhoj = None
         self.rhok = None
@@ -238,15 +238,14 @@
         else:
             raise NotImplementedError("Please check the dimension of the density matrix, it should not reach here.")
 
     def to_cpu(self):
         obj = self.undo_df().to_cpu().density_fit()
         return utils.to_cpu(self, obj)
 
-
 def get_jk(dfobj, dms_tag, hermi=1, with_j=True, with_k=True, direct_scf_tol=1e-14, omega=None):
     '''
     get jk with density fitting
     outputs and input are on the same device
     TODO: separate into three cases: j only, k only, j and k
     '''
 
@@ -281,86 +280,96 @@
         vj = cupy.zeros_like(dms)
 
     if with_k:
         vk = cupy.zeros_like(dms)
 
     # SCF K matrix with occ
     if getattr(dms_tag, 'mo_coeff', None) is not None:
-        #occ_coeff = cupy.asarray(dms_tag.occ_coeff[ao_idx, :], order='C')
         mo_occ = dms_tag.mo_occ
         mo_coeff = dms_tag.mo_coeff
         nmo = mo_occ.shape[-1]
         mo_coeff = mo_coeff.reshape(-1,nao,nmo)
         mo_occ   = mo_occ.reshape(-1,nmo)
         nocc = 0
         occ_coeff = [0]*nset
         for i in range(nset):
-            occ_coeff[i] = mo_coeff[i][:,mo_occ[i]>0][ao_idx] * mo_occ[i][mo_occ[i]>0]**0.5
+            occ_idx = mo_occ[i] > 0
+            occ_coeff[i] = mo_coeff[i][:,occ_idx][ao_idx] * mo_occ[i][occ_idx]**0.5
             nocc += mo_occ[i].sum()
         blksize = dfobj.get_blksize(extra=nao*nocc)
         if with_j:
             vj_packed = cupy.zeros_like(dm_sparse)
         for cderi, cderi_sparse in dfobj.loop(blksize=blksize, unpack=with_k):
             # leading dimension is 1
             if with_j:
                 rhoj = 2.0*dm_sparse.dot(cderi_sparse)
                 vj_packed += cupy.dot(rhoj, cderi_sparse.T)
             for i in range(nset):
                 if with_k:
-                    rhok = contract('Lij,jk->Lki', cderi, occ_coeff[i])
-                    #vk[0] += 2.0 * contract('Lki,Lkj->ij', rhok, rhok)
-                    cublas.syrk('T', rhok.reshape([-1,nao]), out=vk[i], alpha=1.0, beta=1.0, lower=True)
+                    rhok = contract('Lji,jk->Lki', cderi, occ_coeff[i])
+                    # In most cases, syrk does not outperform cupy.dot
+                    #cublas.syrk('T', rhok.reshape([-1,nao]), out=vk[i], alpha=1.0, beta=1.0, lower=True)
+                    rhok = rhok.reshape([-1,nao])
+                    vk[i] += cupy.dot(rhok.T, rhok)
         if with_j:
             vj[:,rows,cols] = vj_packed
             vj[:,cols,rows] = vj_packed
-        if with_k:
-            diag_idx = numpy.diag_indices(nao)
-            for i in range(nset):
-                vk[i][diag_idx] *= 0.5
-            transpose_sum(vk)
+
     # CP-HF K matrix
     elif hasattr(dms_tag, 'mo1'):
+        occ_coeffs = dms_tag.occ_coeff
+        mo1s = dms_tag.mo1
+        mo_occ = dms_tag.mo_occ
+        if not isinstance(occ_coeffs, list):
+            occ_coeffs = [occ_coeffs * 2.0] # For restricted
+        if not isinstance(mo1s, list):
+            mo1s = [mo1s]
+
+        occ_coeffs = [occ_coeff[ao_idx] for occ_coeff in occ_coeffs]
+        mo1s = [mo1[:,ao_idx] for mo1 in mo1s]
+
         if with_j:
             vj_sparse = cupy.zeros_like(dm_sparse)
-        mo1 = dms_tag.mo1[:,ao_idx,:]
-        nocc = mo1.shape[2]
-        # 2.0 due to rhok and rhok1, put it here for symmetry
-        occ_coeff = dms_tag.occ_coeff[ao_idx,:] * 2.0
+
+        nocc = max([mo1.shape[2] for mo1 in mo1s])
+
         blksize = dfobj.get_blksize(extra=2*nao*nocc)
         for cderi, cderi_sparse in dfobj.loop(blksize=blksize, unpack=with_k):
             if with_j:
-                #vj += get_j(cderi_sparse)
                 rhoj = 2.0*dm_sparse.dot(cderi_sparse)
                 vj_sparse += cupy.dot(rhoj, cderi_sparse.T)
             if with_k:
-                rhok = contract('Lij,jk->Lki', cderi, occ_coeff)
-                for i in range(mo1.shape[0]):
-                    rhok1 = contract('Lij,jk->Lki', cderi, mo1[i])
-                    #vk[i] += contract('Lki,Lkj->ij', rhok, rhok1)
-                    contract('Lki,Lkj->ij', rhok, rhok1, alpha=1.0, beta=1.0, out=vk[i])
+                iset = 0
+                for occ_coeff, mo1 in zip(occ_coeffs, mo1s):
+                    rhok = contract('Lij,jk->Lki', cderi, occ_coeff).reshape([-1,nao])
+                    for i in range(mo1.shape[0]):
+                        rhok1 = contract('Lij,jk->Lki', cderi, mo1[i]).reshape([-1,nao])
+                        #contract('Lki,Lkj->ij', rhok, rhok1, alpha=1.0, beta=1.0, out=vk[iset])
+                        vk[iset] += cupy.dot(rhok.T, rhok1)
+                        iset += 1
         occ_coeff = rhok1 = rhok = mo1 = None
         if with_j:
             vj[:,rows,cols] = vj_sparse
             vj[:,cols,rows] = vj_sparse
         if with_k:
-            #vk = vk + vk.transpose(0,2,1)
             transpose_sum(vk)
     # general K matrix with density matrix
     else:
         if with_j:
             vj_sparse = cupy.zeros_like(dm_sparse)
         blksize = dfobj.get_blksize()
         for cderi, cderi_sparse in dfobj.loop(blksize=blksize, unpack=with_k):
             if with_j:
                 rhoj = 2.0*dm_sparse.dot(cderi_sparse)
                 vj_sparse += cupy.dot(rhoj, cderi_sparse.T)
             if with_k:
                 for k in range(nset):
-                    rhok = contract('Lij,jk->Lki', cderi, dms[k])
-                    vk[k] += contract('Lki,Lkj->ij', cderi, rhok)
+                    rhok = contract('Lij,jk->Lki', cderi, dms[k]).reshape([-1,nao])
+                    #vk[k] += contract('Lki,Lkj->ij', cderi, rhok)
+                    vk[k] += cupy.dot(cderi.reshape([-1,nao]).T, rhok)
         if with_j:
             vj[:,rows,cols] = vj_sparse
             vj[:,cols,rows] = vj_sparse
         rhok = None
 
     rev_ao_idx = dfobj.intopt.rev_ao_idx
     if with_j:
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/rhf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/rhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,17 +239,17 @@
 class Gradients(rhf_grad.Gradients):
     from gpu4pyscf.lib.utils import to_gpu, device
 
     _keys = {'with_df', 'auxbasis_response'}
     def __init__(self, mf):
         # Whether to include the response of DF auxiliary basis when computing
         # nuclear gradients of J/K matrices
-        self.auxbasis_response = True
         rhf_grad.Gradients.__init__(self, mf)
 
+    auxbasis_response = True
     get_jk = get_jk
     grad_elec = rhf_grad.grad_elec
     check_sanity = NotImplemented
 
     def get_j(self, mol=None, dm=None, hermi=0):
         vj, _, vjaux, _ = self.get_jk(mol, dm, with_k=False)
         return vj, vjaux
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/rks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/rks.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,16 +115,22 @@
         e1_aux = None
     vxc = tag_array(vxc, aux=e1_aux)
     return vxc
 
 class Gradients(rks_grad.Gradients):
     from gpu4pyscf.lib.utils import to_gpu, device
 
-    _keys = df_rks_grad.Gradients._keys
-    __init__ = df_rks_grad.Gradients.__init__
+    _keys = {'with_df', 'auxbasis_response'}
+
+    def __init__(self, mf):
+        rks_grad.Gradients.__init__(self, mf)
+
+    # Whether to include the response of DF auxiliary basis when computing
+    # nuclear gradients of J/K matrices
+    auxbasis_response = True
 
     get_jk = df_rhf_grad.Gradients.get_jk
     grad_elec = df_rhf_grad.Gradients.grad_elec
     get_veff = get_veff
 
     def get_j(self, mol=None, dm=None, hermi=0, omega=None):
         vj, _, vjaux, _ = self.get_jk(mol, dm, with_k=False, omega=omega)
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/uhf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/uhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,20 +262,20 @@
 
 class Gradients(uhf_grad.Gradients):
     '''Unrestricted density-fitting Hartree-Fock gradients'''
 
     _keys = {'with_df', 'auxbasis_response'}
 
     def __init__(self, mf):
-        # Whether to include the response of DF auxiliary basis when computing
-        # nuclear gradients of J/K matrices
-        self.auxbasis_response = True
         self._keys = self._keys.union(['auxbasis_response'])
         uhf_grad.Gradients.__init__(self, mf)
 
+    # Whether to include the response of DF auxiliary basis when computing
+    # nuclear gradients of J/K matrices
+    auxbasis_response = True
     get_jk = get_jk
 
     # TODO: finish these two functions
     def get_j(self, mol=None, dm=None, hermi=0, mo_coeff=None, mo_occ=None, dm2 = None):
         vj, _, vjaux, _ =  self.get_jk(mol, dm, with_k=False, mo_coeff=mo_coeff, mo_occ=mo_occ, dm2=dm2)
         return vj, vjaux
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/grad/uks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/grad/uks.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,19 +136,19 @@
 
 
 class Gradients(uks_grad.Gradients):
 
     _keys = {'with_df', 'auxbasis_response'}
 
     def __init__(self, mf):
-        # Whether to include the response of DF auxiliary basis when computing
-        # nuclear gradients of J/K matrices
-        self.auxbasis_response = True
         uks_grad.Gradients.__init__(self, mf)
 
+    # Whether to include the response of DF auxiliary basis when computing
+    # nuclear gradients of J/K matrices
+    auxbasis_response = True
     get_jk = get_jk
 
     def get_j(self, mol=None, dm=None, hermi=0, mo_coeff=None, mo_occ=None, dm2 = None, omega=None):
         vj, _, vjaux, _ = self.get_jk(mol, dm, with_k=False, mo_coeff=mo_coeff, mo_occ=mo_occ, dm2=dm2, omega=omega)
         return vj, vjaux
 
     def get_k(self, mol=None, dm=None, hermi=0, mo_coeff=None, mo_occ=None, dm2 = None, omega=None):
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/rhf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/rhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,14 +576,14 @@
         yield ia, h1, vj1, vk1
 
 class Hessian(rhf_hess.Hessian):
     '''Non-relativistic restricted Hartree-Fock hessian'''
 
     from gpu4pyscf.lib.utils import to_gpu, device
     def __init__(self, mf):
-        self.auxbasis_response = 1
         rhf_hess.Hessian.__init__(self, mf)
 
+    auxbasis_response = 1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
     kernel = rhf_hess.kernel
     hess = kernel
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/rks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/rks.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,14 @@
     return h1ao
 
 class Hessian(rks_hess.Hessian):
     '''Non-relativistic RKS hessian'''
     from gpu4pyscf.lib.utils import to_gpu, device
 
     def __init__(self, mf):
-        self.auxbasis_response = 1
         rks_hess.Hessian.__init__(self, mf)
 
+    auxbasis_response = 1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
     kernel = rhf_hess.kernel
     hess = kernel
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/uhf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/uhf.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,14 +683,14 @@
 
 class Hessian(uhf_hess.Hessian):
     '''Non-relativistic restricted Hartree-Fock hessian'''
 
     from gpu4pyscf.lib.utils import to_gpu, device
 
     def __init__(self, mf):
-        self.auxbasis_response = 1
         uhf_hess.Hessian.__init__(self, mf)
 
+    auxbasis_response = 1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
     kernel = rhf_hess.kernel
     hess = kernel
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/hessian/uks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/hessian/uks.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,20 +119,20 @@
     return h1aoa, h1aob
 
 class Hessian(uks_hess.Hessian):
     '''Non-relativistic RKS hessian'''
     from gpu4pyscf.lib.utils import to_gpu, device
 
     def __init__(self, mf):
-        self.auxbasis_response = 1
         uks_hess.Hessian.__init__(self, mf)
 
     def solve_mo1(self, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                   fx=None, atmlst=None, max_memory=4000, verbose=None):
         return uhf_hess.solve_mo1(self.base, mo_energy, mo_coeff, mo_occ, h1ao_or_chkfile,
                          fx, atmlst, max_memory, verbose)
 
+    auxbasis_response = 1
     partial_hess_elec = partial_hess_elec
     make_h1 = make_h1
     hess_elec = uhf_hess.hess_elec
     kernel = rhf_hess.kernel
     hess = kernel
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/df/int3c2e.py` & `gpu4pyscf-0.7.7/gpu4pyscf/df/int3c2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,15 +351,23 @@
             self.ao_idx = self.sph_ao_idx
         if self._auxmol.cart:
             self.aux_ao_loc = self.cart_aux_loc
             self.aux_ao_idx = self.cart_aux_idx
         else:
             self.aux_ao_loc = self.sph_aux_loc
             self.aux_ao_idx = self.sph_aux_idx
+
         self.rev_ao_idx = np.argsort(self.ao_idx, kind='stable').astype(np.int32)
+        self.ao_idx = cupy.array(self.ao_idx)
+        self.cart_ao_idx = cupy.array(self.cart_ao_idx)
+        self.sph_ao_idx = cupy.array(self.sph_ao_idx)
+        self.aux_ao_idx = cupy.array(self.aux_ao_idx)
+        self.cart_aux_idx = cupy.array(self.cart_aux_idx)
+        self.sph_aux_idx = cupy.array(self.sph_aux_idx)
+        self.rev_ao_idx = cupy.array(self.rev_ao_idx)
 
 def get_int3c2e_wjk(mol, auxmol, dm0_tag, thred=1e-12, omega=None, with_k=True):
     intopt = VHFOpt(mol, auxmol, 'int2e')
     intopt.build(thred, diag_block_with_triu=True, aosym=True, group_size=BLKSIZE, group_size_aux=BLKSIZE)
     orbo = dm0_tag.occ_coeff
     nao = mol.nao
     naux = auxmol.nao
@@ -1660,14 +1668,15 @@
     _l_ctrs = []
     _l_ctr_counts = []
     for l_ctr, counts in zip(uniq_l_ctr, l_ctr_counts):
         l = l_ctr[0]
         nf = (l + 1) * (l + 2) // 2
         aligned_size = (group_size // nf // 1) * 1
         max_shells = max(aligned_size, 2)
+        assert max_shells * nf <= group_size
         if l > LMAX_ON_GPU or counts <= max_shells:
             _l_ctrs.append(l_ctr)
             _l_ctr_counts.append(counts)
             continue
 
         nsubs, rests = counts.__divmod__(max_shells)
         _l_ctrs.extend([l_ctr] * nsubs)
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/gen_grid.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/gen_grid.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/gks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/gks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/libxc.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/libxc.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/libxc_structs.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/libxc_structs.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/numint.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/numint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1089,18 +1089,20 @@
     coeff = cupy.asarray(opt.coeff)
     nao, nao0 = coeff.shape
     dma, dmb = dms
     dm_shape = dma.shape
     # AO basis -> gdftopt AO basis
     with_mocc = hasattr(dms, 'mo1')
     if with_mocc:
-        mo1a = contract('nio,pi->npo', dma.mo1, coeff) * 2.0**0.5
-        mo1b = contract('nio,pi->npo', dmb.mo1, coeff) * 2.0**0.5
-        occ_coeff_a = contract('io,pi->po', dma.occ_coeff, coeff) * 2.0**0.5
-        occ_coeff_b = contract('io,pi->po', dmb.occ_coeff, coeff) * 2.0**0.5
+        mo1a, mo1b = dms.mo1
+        occ_coeffa, occ_coeffb = dms.occ_coeff
+        mo1a = contract('nio,pi->npo', mo1a, coeff)
+        mo1b = contract('nio,pi->npo', mo1b, coeff)
+        occ_coeff_a = contract('io,pi->po', occ_coeffa, coeff)
+        occ_coeff_b = contract('io,pi->po', occ_coeffb, coeff)
 
     dma = cupy.asarray(dma).reshape(-1,nao0,nao0)
     dmb = cupy.asarray(dmb).reshape(-1,nao0,nao0)
     dma = contract('nij,qj->niq', dma, coeff)
     dma = contract('pi,niq->npq', coeff, dma)
     dmb = contract('nij,qj->niq', dmb, coeff)
     dmb = contract('pi,niq->npq', coeff, dmb)
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/radi.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/radi.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/rks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/rks.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,16 @@
     e2 = ecoul + exc
     ks.scf_summary['e1'] = e1
     ks.scf_summary['coul'] = ecoul
     ks.scf_summary['exc'] = exc
     logger.debug(ks, 'E1 = %s  Ecoul = %s  Exc = %s', e1, ecoul, exc)
     return e1+e2, e2
 
-class KohnShamDFT:
+# Inherit pyscf KohnShamDFT class since this is tested in the pyscf dispersion code
+class KohnShamDFT(rks.KohnShamDFT):
 
     _keys = rks.KohnShamDFT._keys
 
     def __init__(self, xc='LDA,VWN'):
         self.xc = xc
         self.disp = None
         self.disp_with_3body = None
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/roks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/roks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/uks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/uks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/xc_alias.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/xc_alias.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/dft/xc_deriv.py` & `gpu4pyscf-0.7.7/gpu4pyscf/dft/xc_deriv.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/fci/direct_spin1.py` & `gpu4pyscf-0.7.7/gpu4pyscf/fci/direct_spin1.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/grad/dispersion.py` & `gpu4pyscf-0.7.7/gpu4pyscf/grad/dispersion.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,14 @@
         res = dftd3_model.get_dispersion(grad=True)
         return res['gradient']
 
     elif disp_version[:2].upper() == 'D4':
         from gpu4pyscf.lib import dftd4
         dftd4_model = dftd4.DFTD4Dispersion(mol, xc=method)
         res = dftd4_model.get_dispersion(grad=True)
-        print(method, disp_version)
-        print(res.get("gradient"))
         return res.get("gradient")
     else:
         raise RuntimeError(f'dispersion correction: {disp_version} is not supported.')
 
 # Inject to Gradient
 from gpu4pyscf.grad import rhf, uhf, rks, uks
 rhf.Gradients.get_dispersion = get_dispersion
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/grad/rhf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/grad/rhf.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,16 +543,16 @@
         g_disp = mf_grad.get_dispersion()
         mf_grad.grad_disp = g_disp
         mf_grad.grad_mf = de
 
     if log.verbose >= logger.DEBUG:
         log.timer_debug1('gradients of electronic part', *t0)
 
-    # net force should be zero
-    de -= cupy.sum(de, axis=0)/len(atmlst)
+    ## net force should be zero
+    #de -= cupy.sum(de, axis=0)/len(atmlst)
     return de.get()
 
 def get_grad_hcore(mf_grad, mo_coeff=None, mo_occ=None):
     '''
     derivative of hcore in MO
     '''
     mf = mf_grad.base
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/grad/rks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/grad/rks.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,14 @@
     _keys = rks_grad.Gradients._keys
 
     # method
     def __init__ (self, mf):
         rhf_grad.Gradients.__init__(self, mf)
         self.grids = None
         self.nlcgrids = None
-        self.grid_response = False
 
     get_veff = _get_veff
     # TODO: add grid response into this function
     def extra_force(self, atom_id, envs):
         return 0
 
 Grad = Gradients
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/grad/uhf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/grad/uhf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/grad/uks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/grad/uks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/gto/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/gto/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/gto/mole.py` & `gpu4pyscf-0.7.7/gpu4pyscf/gto/mole.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/hessian/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/hessian/dispersion.py` & `gpu4pyscf-0.7.7/gpu4pyscf/hessian/dispersion.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/hessian/rhf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/hessian/rhf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/hessian/rks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/hessian/rks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/hessian/uhf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/hessian/uhf.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,29 +413,34 @@
 
     def fx(mo1):
         mo1 = cupy.asarray(mo1)
         mo1 = mo1.reshape(-1,nmoa*nocca+nmob*noccb)
         nset = len(mo1)
 
         x = mo1[:,:nmoa*nocca].reshape(nset,nmoa,nocca)
-        mo1_mo = contract('npo,ip->nio', x, mo_coeff[0])
-        dma = contract('nio,jo->nij', mo1_mo, mocca)
+        mo1_moa = contract('npo,ip->nio', x, mo_coeff[0])
+        dma = contract('nio,jo->nij', mo1_moa, mocca)
 
         x = mo1[:,nmoa*nocca:].reshape(nset,nmob,noccb)
-        mo1_mo = contract('npo,ip->nio', x, mo_coeff[1])
-        dmb = contract('nio,jo->nij', mo1_mo, moccb)
+        mo1_mob = contract('npo,ip->nio', x, mo_coeff[1])
+        dmb = contract('nio,jo->nij', mo1_mob, moccb)
 
         dm1 = cupy.empty([2,nset,nao,nao])
         dm1[0] = dma + dma.transpose(0,2,1)
         dm1[1] = dmb + dmb.transpose(0,2,1)
 
+        #v1_old = vresp(dm1)
         # TODO: improve the efficiency with occ_coeff
-        #dm1 = tag_array(dm1, mo1=mo1_mo, occ_coeff=mocc, mo_occ=mo_occ)
+        dm1 = tag_array(dm1, mo1=[mo1_moa,mo1_mob], occ_coeff=[mocca,moccb], mo_occ=mo_occ)
+        #print(dm1.shape)
         v1 = vresp(dm1)
-
+        #print(cupy.linalg.norm(v1 - v1_old))
+        #print(cupy.linalg.norm(v1))
+        #print(v1.shape)
+        #exit()
         v1vo = cupy.empty_like(mo1)
         tmp = contract('nij,jo->nio', v1[0], mocca)
         v1vo[:,:nmoa*nocca] = contract('nio,ip->npo', tmp, mo_coeff[0]).reshape(nset,-1)
 
         tmp = contract('nij,jo->nio', v1[1], moccb)
         v1vo[:,nmoa*nocca:] = contract('nio,ip->npo', tmp, mo_coeff[1]).reshape(nset,-1)
         return v1vo
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/hessian/uks.py` & `gpu4pyscf-0.7.7/gpu4pyscf/hessian/uks.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/cublas.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/cublas.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/cupy_helper.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/cupy_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,17 +389,17 @@
         ctypes.cast(mat.data.ptr, ctypes.c_void_p),
         ctypes.c_int(n), ctypes.c_int(counts))
     if err != 0:
         raise RuntimeError('failed in symm_triu kernel')
 
     return mat
 
-def cart2sph(t, axis=0, ang=1, out=None):
+def cart2sph_cutensor(t, axis=0, ang=1, out=None):
     '''
-    transform 'axis' of a tensor from cartesian basis into spherical basis
+    transform 'axis' of a tensor from cartesian basis into spherical basis with cutensor
     '''
     if(ang <= 1):
         if(out is not None): out[:] = t
         return t
     size = list(t.shape)
     c2s = c2s_l[ang]
     if(not t.flags['C_CONTIGUOUS']): t = cupy.asarray(t, order='C')
@@ -411,14 +411,50 @@
 
     t_cart = t.reshape([i0*nli, li_size[0], i3])
     if(out is not None):
         out = out.reshape([i0*nli, li_size[1], i3])
     t_sph = contract('min,ip->mpn', t_cart, c2s, out=out)
     return t_sph.reshape(out_shape)
 
+def cart2sph(t, axis=0, ang=1, out=None, stream=None):
+    '''
+    transform 'axis' of a tensor from cartesian basis into spherical basis
+    '''
+    if(ang <= 1):
+        if(out is not None): out[:] = t
+        return t
+    size = list(t.shape)
+    c2s = c2s_l[ang]
+    if(not t.flags['C_CONTIGUOUS']): t = cupy.asarray(t, order='C')
+    li_size = c2s.shape
+    nli = size[axis] // li_size[0]
+    i0 = max(1, np.prod(size[:axis]))
+    i3 = max(1, np.prod(size[axis+1:]))
+    out_shape = size[:axis] + [nli*li_size[1]] + size[axis+1:]
+
+    t_cart = t.reshape([i0*nli, li_size[0], i3])
+    if(out is not None):
+        out = out.reshape([i0*nli, li_size[1], i3])
+    else:
+        out = cupy.empty(out_shape)
+    count = i0*nli*i3
+    if stream is None:
+        stream = cupy.cuda.get_current_stream()
+    err = libcupy_helper.cart2sph(
+        ctypes.cast(stream.ptr, ctypes.c_void_p),
+        ctypes.cast(t_cart.data.ptr, ctypes.c_void_p),
+        ctypes.cast(out.data.ptr, ctypes.c_void_p),
+        ctypes.c_int(i3),
+        ctypes.c_int(count),
+        ctypes.c_int(ang)
+    )
+    if err != 0:
+        raise RuntimeError('failed in cart2sph kernel')
+    return out.reshape(out_shape)
+
 # a copy with modification from
 # https://github.com/pyscf/pyscf/blob/9219058ac0a1bcdd8058166cad0fb9127b82e9bf/pyscf/lib/linalg_helper.py#L1536
 def krylov(aop, b, x0=None, tol=1e-10, max_cycle=30, dot=cupy.dot,
            lindep=DSOLVE_LINDEP, callback=None, hermi=False,
            verbose=logger.WARN):
     r'''Krylov subspace method to solve  (1+a) x = b.  Ref:
     J. A. Pople et al, Int. J.  Quantum. Chem.  Symp. 13, 225 (1979).
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/cusolver.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/cusolver.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/cutensor.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/cutensor.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/dftd3.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/dftd3.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/dftd4.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/dftd4.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/diis.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/diis.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/logger.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/logger.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/lib/utils.py` & `gpu4pyscf-0.7.7/gpu4pyscf/lib/utils.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/mp/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/mp/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/mp/dfmp2.py` & `gpu4pyscf-0.7.7/gpu4pyscf/mp/dfmp2.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/mp/mp2.py` & `gpu4pyscf-0.7.7/gpu4pyscf/mp/mp2.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/qmmm/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/qmmm/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/qmmm/chelpg.py` & `gpu4pyscf-0.7.7/gpu4pyscf/qmmm/chelpg.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/_response_functions.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/_response_functions.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/cphf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/cphf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/diis.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/diis.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/dispersion.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/dispersion.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/ghf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/ghf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/hf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/hf.py`

 * *Files 0% similar despite different names*

```diff
@@ -665,15 +665,15 @@
 
 from gpu4pyscf.lib import utils
 class RHF(SCF):
 
     to_gpu = utils.to_gpu
     device = utils.device
 
-    _keys = {'e_disp', 'h1e', 's1e', 'e_mf', 'screen_tol', 'conv_tol_cpscf'}
+    _keys = {'e_disp', 'h1e', 's1e', 'e_mf', 'screen_tol', 'conv_tol_cpscf', 'disp_with_3body'}
 
     screen_tol = 1e-14
     conv_tol_cpscf = 1e-3
     DIIS = diis.SCF_DIIS
     get_jk = _get_jk
     _eigh = staticmethod(eigh)
     make_rdm1 = make_rdm1
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/int4c2e.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/int4c2e.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/rohf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/rohf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/ucphf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/ucphf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/scf/uhf.py` & `gpu4pyscf-0.7.7/gpu4pyscf/scf/uhf.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/solvent/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/solvent/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/solvent/_attach_solvent.py` & `gpu4pyscf-0.7.7/gpu4pyscf/solvent/_attach_solvent.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,141 +12,149 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import cupy
 from pyscf import lib
 from pyscf.lib import logger
-from pyscf.solvent._attach_solvent import _Solvation
 from gpu4pyscf.lib.cupy_helper import tag_array
 from gpu4pyscf import scf
 
-# NOTE: copied from pyscf, different from the latest version
-
 def _for_scf(mf, solvent_obj, dm=None):
     '''Add solvent model to SCF (HF and DFT) method.
 
     Kwargs:
         dm : if given, solvent does not respond to the change of density
             matrix. A frozen ddCOSMO potential is added to the results.
     '''
     if isinstance(mf, _Solvation):
         mf.with_solvent = solvent_obj
         return mf
 
-    oldMF = mf.__class__
-
     if dm is not None:
         solvent_obj.e, solvent_obj.v = solvent_obj.kernel(dm)
         solvent_obj.frozen = True
 
-    class SCFWithSolvent(_Solvation, oldMF):
-        def __init__(self, mf, solvent):
-            self.__dict__.update(mf.__dict__)
-            self.with_solvent = solvent
-            self._keys.update(['with_solvent'])
-
-        def dump_flags(self, verbose=None):
-            oldMF.dump_flags(self, verbose)
-            self.with_solvent.check_sanity()
-            self.with_solvent.dump_flags(verbose)
-            return self
-
-        def reset(self, mol=None):
-            self.with_solvent.reset(mol)
-            return oldMF.reset(self, mol)
-
-        # Note v_solvent should not be added to get_hcore for scf methods.
-        # get_hcore is overloaded by many post-HF methods. Modifying
-        # SCF.get_hcore may lead error.
-
-        def get_veff(self, mol=None, dm=None, *args, **kwargs):
-            vhf = oldMF.get_veff(self, mol, dm, *args, **kwargs)
-            with_solvent = self.with_solvent
-            if not with_solvent.frozen:
-                with_solvent.e, with_solvent.v = with_solvent.kernel(dm)
-            e_solvent, v_solvent = with_solvent.e, with_solvent.v
-
-            # NOTE: v_solvent should not be added to vhf in this place. This is
-            # because vhf is used as the reference for direct_scf in the next
-            # iteration. If v_solvent is added here, it may break direct SCF.
-            return tag_array(vhf, e_solvent=e_solvent, v_solvent=v_solvent)
-
-        def get_fock(self, h1e=None, s1e=None, vhf=None, dm=None, cycle=-1,
-                     diis=None, diis_start_cycle=None,
-                     level_shift_factor=None, damp_factor=None):
-            # DIIS was called inside oldMF.get_fock. v_solvent, as a function of
-            # dm, should be extrapolated as well. To enable it, v_solvent has to be
-            # added to the fock matrix before DIIS was called.
-            if getattr(vhf, 'v_solvent', None) is None:
-                vhf = self.get_veff(self.mol, dm)
-            return oldMF.get_fock(self, h1e, s1e, vhf+vhf.v_solvent, dm, cycle, diis,
-                                  diis_start_cycle, level_shift_factor, damp_factor)
-
-        def energy_elec(self, dm=None, h1e=None, vhf=None):
-            if dm is None:
-                dm = self.make_rdm1()
-            if getattr(vhf, 'e_solvent', None) is None:
-                vhf = self.get_veff(self.mol, dm)
-
-            e_tot, e_coul = oldMF.energy_elec(self, dm, h1e, vhf)
-            e_solvent = vhf.e_solvent
-            if isinstance(e_solvent, cupy.ndarray):
-                e_solvent = e_solvent.get()[()]
-            e_tot += e_solvent
-            self.scf_summary['e_solvent'] = vhf.e_solvent.real
-
-            if self.with_solvent.method.upper() == 'SMD':
-                if self.with_solvent.e_cds is None:
-                    e_cds = self.with_solvent.get_cds()
-                    self.with_solvent.e_cds = e_cds
-                else:
-                    e_cds = self.with_solvent.e_cds
-                if isinstance(e_cds, cupy.ndarray):
-                    e_cds = e_cds.get()[()]
-                e_tot += e_cds
-                self.scf_summary['e_cds'] = e_cds
-                logger.info(self, f'CDS correction = {e_cds:.15f}')
-            logger.info(self, 'Solvent Energy = %.15g', vhf.e_solvent)
-
-            return e_tot, e_coul
-
-        def nuc_grad_method(self):
-            grad_method = oldMF.nuc_grad_method(self)
-            return self.with_solvent.nuc_grad_method(grad_method)
-
-        Gradients = nuc_grad_method
-
-        def Hessian(self):
-            hess_method = oldMF.Hessian(self)
-            return self.with_solvent.Hessian(hess_method)
-
-        def gen_response(self, *args, **kwargs):
-            vind = oldMF.gen_response(self, *args, **kwargs)
-            is_uhf = isinstance(self, scf.uhf.UHF)
-            # singlet=None is orbital hessian or CPHF type response function
-            singlet = kwargs.get('singlet', True)
-            singlet = singlet or singlet is None
-            def vind_with_solvent(dm1):
-                v = vind(dm1)
-                if self.with_solvent.equilibrium_solvation:
-                    if is_uhf:
-                        v_solvent = self.with_solvent._B_dot_x(dm1)
-                        v += v_solvent[0] + v_solvent[1]
-                    elif singlet:
-                        v += self.with_solvent._B_dot_x(dm1)
-                return v
-            return vind_with_solvent
-
-        def stability(self, *args, **kwargs):
-            # When computing orbital hessian, the second order derivatives of
-            # solvent energy needs to be computed. It is enabled by
-            # the attribute equilibrium_solvation in gen_response method.
-            # If solvent was frozen, its contribution is treated as the
-            # external potential. The response of solvent does not need to
-            # be considered in stability analysis.
-            with lib.temporary_env(self.with_solvent,
-                                   equilibrium_solvation=not self.with_solvent.frozen):
-                return oldMF.stability(self, *args, **kwargs)
-
-    mf1 = SCFWithSolvent(mf, solvent_obj)
-    return mf1
+    sol_mf = SCFWithSolvent(mf, solvent_obj)
+    name = solvent_obj.__class__.__name__ + mf.__class__.__name__
+    return lib.set_class(sol_mf, (SCFWithSolvent, mf.__class__), name)
+
+# 1. A tag to label the derived method class
+class _Solvation:
+    pass
+
+class SCFWithSolvent(_Solvation):
+    from gpu4pyscf.lib.utils import to_gpu, device
+
+    _keys = {'with_solvent'}
+
+    def __init__(self, mf, solvent):
+        self.__dict__.update(mf.__dict__)
+        self.with_solvent = solvent
+
+    def undo_solvent(self):
+        cls = self.__class__
+        name_mixin = self.with_solvent.__class__.__name__
+        obj = lib.view(self, lib.drop_class(cls, SCFWithSolvent, name_mixin))
+        del obj.with_solvent
+        return obj
+
+    def to_cpu(self):
+        from pyscf.solvent import _attach_solvent
+        solvent_obj = self.with_solvent.to_cpu()
+        obj = _attach_solvent._for_scf(self.undo_solvent().to_cpu(), solvent_obj)
+        return obj
+
+    def dump_flags(self, verbose=None):
+        super().dump_flags(verbose)
+        self.with_solvent.check_sanity()
+        self.with_solvent.dump_flags(verbose)
+        return self
+
+    def reset(self, mol=None):
+        self.with_solvent.reset(mol)
+        return super().reset(mol)
+
+    def get_veff(self, mol=None, dm=None, *args, **kwargs):
+        vhf = super().get_veff(mol, dm, *args, **kwargs)
+        with_solvent = self.with_solvent
+        if not with_solvent.frozen:
+            with_solvent.e, with_solvent.v = with_solvent.kernel(dm)
+        e_solvent, v_solvent = with_solvent.e, with_solvent.v
+        return tag_array(vhf, e_solvent=e_solvent, v_solvent=v_solvent)
+
+    def get_fock(self, h1e=None, s1e=None, vhf=None, dm=None, cycle=-1,
+                 diis=None, diis_start_cycle=None,
+                 level_shift_factor=None, damp_factor=None, fock_last=None):
+        # DIIS was called inside oldMF.get_fock. v_solvent, as a function of
+        # dm, should be extrapolated as well. To enable it, v_solvent has to be
+        # added to the fock matrix before DIIS was called.
+        if getattr(vhf, 'v_solvent', None) is None:
+            vhf = self.get_veff(self.mol, dm)
+        return super().get_fock(h1e, s1e, vhf+vhf.v_solvent, dm, cycle, diis,
+                                diis_start_cycle, level_shift_factor, damp_factor)
+
+    def energy_elec(self, dm=None, h1e=None, vhf=None):
+        if dm is None:
+            dm = self.make_rdm1()
+        if getattr(vhf, 'e_solvent', None) is None:
+            vhf = self.get_veff(self.mol, dm)
+
+        e_tot, e_coul = super().energy_elec(dm, h1e, vhf)
+        e_solvent = vhf.e_solvent
+        if isinstance(e_solvent, cupy.ndarray):
+            e_solvent = e_solvent.get()[()]
+        e_tot += e_solvent
+        self.scf_summary['e_solvent'] = vhf.e_solvent.real
+
+        if (hasattr(self.with_solvent, 'method') and self.with_solvent.method.upper() == 'SMD'):
+            if self.with_solvent.e_cds is None:
+                e_cds = self.with_solvent.get_cds()
+                self.with_solvent.e_cds = e_cds
+            else:
+                e_cds = self.with_solvent.e_cds
+            if isinstance(e_cds, cupy.ndarray):
+                e_cds = e_cds.get()[()]
+            e_tot += e_cds
+            self.scf_summary['e_cds'] = e_cds
+            logger.info(self, f'CDS correction = {e_cds:.15f}')
+        logger.info(self, 'Solvent Energy = %.15g', vhf.e_solvent)
+
+        return e_tot, e_coul
+
+    def nuc_grad_method(self):
+        grad_method = super().nuc_grad_method()
+        return self.with_solvent.nuc_grad_method(grad_method)
+
+    Gradients = nuc_grad_method
+
+    def Hessian(self):
+        hess_method = super().Hessian()
+        return self.with_solvent.Hessian(hess_method)
+
+    def gen_response(self, *args, **kwargs):
+        vind = super().gen_response(*args, **kwargs)
+        is_uhf = isinstance(self, scf.uhf.UHF)
+        # singlet=None is orbital hessian or CPHF type response function
+        singlet = kwargs.get('singlet', True)
+        singlet = singlet or singlet is None
+        def vind_with_solvent(dm1):
+            v = vind(dm1)
+            if self.with_solvent.equilibrium_solvation:
+                if is_uhf:
+                    v_solvent = self.with_solvent._B_dot_x(dm1)
+                    v += v_solvent[0] + v_solvent[1]
+                elif singlet:
+                    v += self.with_solvent._B_dot_x(dm1)
+            return v
+        return vind_with_solvent
+
+    def stability(self, *args, **kwargs):
+        # When computing orbital hessian, the second order derivatives of
+        # solvent energy needs to be computed. It is enabled by
+        # the attribute equilibrium_solvation in gen_response method.
+        # If solvent was frozen, its contribution is treated as the
+        # external potential. The response of solvent does not need to
+        # be considered in stability analysis.
+        with lib.temporary_env(self.with_solvent,
+                                equilibrium_solvation=not self.with_solvent.frozen):
+            return super().stability(*args, **kwargs)
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/__init__.py` & `gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/__init__.py`

 * *Files identical despite different names*

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/pcm.py` & `gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/pcm.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,26 +16,28 @@
 '''
 Gradient of PCM family solvent model
 '''
 # pylint: disable=C0103
 
 import numpy
 import cupy
+import ctypes
 from cupyx import scipy
 from pyscf import lib
-from pyscf import gto, df
+from pyscf import gto
 from pyscf.grad import rhf as rhf_grad
-from pyscf.solvent import ddcosmo_grad
 
 from gpu4pyscf.solvent.pcm import PI, switch_h
 from gpu4pyscf.df import int3c2e
-from gpu4pyscf.lib.cupy_helper import contract
+from gpu4pyscf.lib.cupy_helper import contract, load_library
 from gpu4pyscf.lib import logger
+from pyscf import lib as pyscf_lib
 
 libdft = lib.load_library('libdft')
+libsolvent = load_library('libsolvent')
 
 def grad_switch_h(x):
     ''' first derivative of h(x)'''
     dy = 30.0*x**2 - 60.0*x**3 + 30.0*x**4
     dy[x<0] = 0.0
     dy[x>1] = 0.0
     return dy
@@ -95,15 +97,15 @@
         Fi = cupy.expand_dims(Fi, axis=-2)
         Ai = cupy.expand_dims(Ai, axis=-2)
         dF[p0:p1,:,:] -= Fi * dfiJ
         dA[p0:p1,:,:] -= Ai * dfiJ
 
     return dF, dA
 
-def get_dD_dS(surface, dF, with_S=True, with_D=False):
+def get_dD_dS_slow(surface, dF, with_S=True, with_D=False):
     '''
     derivative of D and S w.r.t grids, partial_i D_ij = -partial_j D_ij
     S is symmetric, D is not
     '''
     grid_coords = surface['grid_coords']
     exponents   = surface['charge_exp']
     norm_vec    = surface['norm_vec']
@@ -138,19 +140,57 @@
         dD = dD_dri * drij + dS_dr * (-nj/rij + 3.0*nj_rij/rij**2 * drij)
         dD_dri = None
     dSii_dF = -exponents * (2.0/PI)**0.5 / switch_fun**2
     dSii = cupy.expand_dims(dSii_dF, axis=(1,2)) * dF
 
     return dD, dS, dSii
 
+def get_dD_dS(surface, dF, with_S=True, with_D=False, stream=None):
+    charge_exp  = surface['charge_exp']
+    grid_coords = surface['grid_coords']
+    switch_fun  = surface['switch_fun']
+    norm_vec    = surface['norm_vec']
+    R_vdw       = surface['R_vdw']
+    n = charge_exp.shape[0]
+    dS = cupy.empty([n,n,3])
+    dD = None
+    dS_ptr = ctypes.cast(dS.data.ptr, ctypes.c_void_p)
+    dD_ptr = pyscf_lib.c_null_ptr()
+    if with_D:
+        dD = cupy.empty([n,n,3])
+        dD_ptr = ctypes.cast(dD.data.ptr, ctypes.c_void_p)
+    if stream is None:
+        stream = cupy.cuda.get_current_stream()
+    err = libsolvent.pcm_dd_ds(
+        ctypes.cast(stream.ptr, ctypes.c_void_p),
+        dD_ptr, dS_ptr,
+        ctypes.cast(grid_coords.data.ptr, ctypes.c_void_p),
+        ctypes.cast(norm_vec.data.ptr, ctypes.c_void_p),
+        ctypes.cast(R_vdw.data.ptr, ctypes.c_void_p),
+        ctypes.cast(charge_exp.data.ptr, ctypes.c_void_p),
+        ctypes.cast(switch_fun.data.ptr, ctypes.c_void_p),
+        ctypes.c_int(n)
+    )
+    if err != 0:
+        raise RuntimeError('Failed in generating PCM dD and dS matrices.')
+
+    dSii_dF = -charge_exp * (2.0/PI)**0.5 / switch_fun**2
+    dSii = cupy.expand_dims(dSii_dF, axis=(1,2)) * dF
+    return dD, dS, dSii
+
 def grad_nuc(pcmobj, dm):
     mol = pcmobj.mol
     log = logger.new_logger(mol, mol.verbose)
     t1 = log.init_timer()
-    if not pcmobj._intermediates or 'q_sym' not in pcmobj._intermediates:
+    if not pcmobj._intermediates:
+        pcmobj.build()
+    dm_cache = pcmobj._intermediates.get('dm', None)
+    if dm_cache is not None and cupy.linalg.norm(dm_cache - dm) < 1e-10:
+        pass
+    else:
         pcmobj._get_vind(dm)
 
     mol = pcmobj.mol
     q_sym        = pcmobj._intermediates['q_sym'].get()
     gridslice    = pcmobj.surface['gslice_by_atom']
     grid_coords  = pcmobj.surface['grid_coords'].get()
     exponents    = pcmobj.surface['charge_exp'].get()
@@ -176,25 +216,31 @@
     t1 = log.timer_debug1('grad nuc', *t1)
     return de
 
 def grad_qv(pcmobj, dm):
     '''
     contributions due to integrals
     '''
-    if not pcmobj._intermediates or 'q_sym' not in pcmobj._intermediates:
+    if not pcmobj._intermediates:
+        pcmobj.build()
+    dm_cache = pcmobj._intermediates.get('dm', None)
+    if dm_cache is not None and cupy.linalg.norm(dm_cache - dm) < 1e-10:
+        pass
+    else:
         pcmobj._get_vind(dm)
     mol = pcmobj.mol
     log = logger.new_logger(mol, mol.verbose)
     t1 = log.init_timer()
-    gridslice    = pcmobj.surface['gslice_by_atom']
-    q_sym        = pcmobj._intermediates['q_sym']
+    gridslice   = pcmobj.surface['gslice_by_atom']
+    charge_exp  = pcmobj.surface['charge_exp']
+    grid_coords = pcmobj.surface['grid_coords']
+    q_sym       = pcmobj._intermediates['q_sym']
 
-    intopt = pcmobj.intopt
-    intopt.clear()
-    # rebuild with aosym
+    auxmol = gto.fakemol_for_charges(grid_coords.get(), expnt=charge_exp.get()**2)
+    intopt = int3c2e.VHFOpt(mol, auxmol, 'int2e')
     intopt.build(1e-14, diag_block_with_triu=True, aosym=False)
     coeff = intopt.coeff
     dm_cart = coeff @ dm @ coeff.T
 
     dvj, _ = int3c2e.get_int3c2e_ip_jk(intopt, 0, 'ip1', q_sym, None, dm_cart)
     dq, _ = int3c2e.get_int3c2e_ip_jk(intopt, 0, 'ip2', q_sym, None, dm_cart)
 
@@ -213,15 +259,20 @@
     '''
     dE = 0.5*v* d(K^-1 R) *v + q*dv
     v^T* d(K^-1 R)v = v^T*K^-1(dR - dK K^-1R)v = v^T K^-1(dR - dK q)
     '''
     mol = pcmobj.mol
     log = logger.new_logger(mol, mol.verbose)
     t1 = log.init_timer()
-    if not pcmobj._intermediates or 'q_sym' not in pcmobj._intermediates:
+    if not pcmobj._intermediates:
+        pcmobj.build()
+    dm_cache = pcmobj._intermediates.get('dm', None)
+    if dm_cache is not None and cupy.linalg.norm(dm_cache - dm) < 1e-10:
+        pass
+    else:
         pcmobj._get_vind(dm)
 
     gridslice    = pcmobj.surface['gslice_by_atom']
     v_grids      = pcmobj._intermediates['v_grids']
     A            = pcmobj._intermediates['A']
     D            = pcmobj._intermediates['D']
     S            = pcmobj._intermediates['S']
@@ -321,14 +372,16 @@
 
     name = (grad_method.base.with_solvent.__class__.__name__
             + grad_method.__class__.__name__)
     return lib.set_class(WithSolventGrad(grad_method),
                          (WithSolventGrad, grad_method.__class__), name)
 
 class WithSolventGrad:
+    from gpu4pyscf.lib.utils import to_gpu, device
+
     _keys = {'de_solvent', 'de_solute'}
 
     def __init__(self, grad_method):
         self.__dict__.update(grad_method.__dict__)
         self.de_solvent = None
         self.de_solute = None
 
@@ -336,14 +389,19 @@
         cls = self.__class__
         name_mixin = self.base.with_solvent.__class__.__name__
         obj = lib.view(self, lib.drop_class(cls, WithSolventGrad, name_mixin))
         del obj.de_solvent
         del obj.de_solute
         return obj
 
+    def to_cpu(self):
+        from pyscf.solvent.grad import pcm  # type: ignore
+        grad_method = self.undo_solvent().to_cpu()
+        return pcm.make_grad_object(grad_method)
+
     def kernel(self, *args, dm=None, atmlst=None, **kwargs):
         dm = kwargs.pop('dm', None)
         if dm is None:
             dm = self.base.make_rdm1(ao_repr=True)
         if dm.ndim == 3:
             dm = dm[0] + dm[1]
         self.de_solute = super().kernel(*args, **kwargs)
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/solvent/grad/smd.py` & `gpu4pyscf-0.7.7/gpu4pyscf/solvent/grad/smd_experiment.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,42 +10,34 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 '''
-Gradient of PCM family solvent model
+Gradient of SMD solvent model (for experiment and education)
 '''
-# pylint: disable=C0103
 
 import numpy as np
 import cupy
-#from cupyx import scipy, jit
-from pyscf import lib
-from pyscf import gto, df
-from pyscf.grad import rhf as rhf_grad
 from pyscf.data import radii
-from pyscf.solvent import ddcosmo_grad
-
-from gpu4pyscf.solvent import pcm, smd
+from gpu4pyscf.solvent import pcm
+from gpu4pyscf.solvent import smd_experiment as smd
 from gpu4pyscf.solvent.grad import pcm as pcm_grad
-from gpu4pyscf.solvent.smd import (
-    sigma_water, sigma_n, sigma_alpha, sigma_beta, r_zz, swtich_function,
-    hartree2kcal)
-from gpu4pyscf.df import int3c2e
-from gpu4pyscf.lib.cupy_helper import contract
-from gpu4pyscf.lib import logger
 
-def grad_swtich_function(R, r, dr):
+def grad_switch_function(R, r, dr):
     if R < r + dr:
         return -np.exp(dr/(R-dr-r)) * dr / (R-dr-r)**2
     else:
         return 0.0
 
+from gpu4pyscf.solvent.smd import (
+    sigma_water, sigma_n, sigma_alpha, sigma_beta, r_zz, switch_function,
+    hartree2kcal)
+
 def atomic_surface_tension(symbols, coords, n, alpha, beta, water=True):
     '''
     - list of atomic symbols
     - atomic coordinates in Anstrong
     - solvent descriptors: n, alpha, beta
     '''
 
@@ -84,20 +76,20 @@
 
         if sym_i == 'H':
             dt_HC = np.zeros([natm,3])
             dt_HO = np.zeros([natm,3])
             for j, sym_j in enumerate(symbols):
                 if sym_j == 'C':
                     r, dr = r_zz.get(('H','C'), (0.0, 0.0))
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j]
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j]
                     dt_HC[i] += dt_drij
                     dt_HC[j] -= dt_drij
                 if sym_j == 'O':
                     r, dr = r_zz.get(('H','O'), (0.0, 0.0))
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j]
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j]
                     dt_HO[i] += dt_drij
                     dt_HO[j] -= dt_drij
             sig_HC = get_bond_tension(('H','C'))
             sig_HO = get_bond_tension(('H','O'))
             tension += sig_HC * dt_HC + sig_HO * dt_HO
             tensions.append(tension)
             continue
@@ -105,21 +97,21 @@
         if sym_i == 'C':
             dt_CC = np.zeros([natm,3])
             dt_CN = np.zeros([natm,3])
             t_CN = 0.0
             for j, sym_j in enumerate(symbols):
                 if sym_j == 'C' and i != j:
                     r, dr = r_zz.get(('C', 'C'), (0.0, 0.0))
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j]
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j]
                     dt_CC[i] += dt_drij
                     dt_CC[j] -= dt_drij
                 if sym_j == 'N':
                     r, dr = r_zz.get(('C', 'N'), (0.0, 0.0))
-                    t_CN += swtich_function(rij[i,j], r, dr)
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j]
+                    t_CN += switch_function(rij[i,j], r, dr)
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j]
                     dt_CN[i] += dt_drij
                     dt_CN[j] -= dt_drij
             sig_CC = get_bond_tension(('C','C'))
             sig_CN = get_bond_tension(('C','N'))
             tension += sig_CC * dt_CC + sig_CN * (2 * t_CN * dt_CN)
             tensions.append(tension)
             continue
@@ -132,29 +124,29 @@
                 if sym_j == 'C':
                     r, dr = r_zz.get(('N','C'), (0.0, 0.0))
                     tk = 0.0
                     dtk = np.zeros([natm,3])
                     for k, sym_k in enumerate(symbols):
                         if k != i and k != j:
                             rjk, drjk = r_zz.get(('C', sym_k), (0.0, 0.0))
-                            tk += swtich_function(rij[j,k], rjk, drjk)
-                            dtk_rjk = grad_swtich_function(rij[j,k], rjk, drjk) * drij[j,k]
+                            tk += switch_function(rij[j,k], rjk, drjk)
+                            dtk_rjk = grad_switch_function(rij[j,k], rjk, drjk) * drij[j,k]
                             dtk[j] += dtk_rjk
                             dtk[k] -= dtk_rjk
 
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j] * tk**2
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j] * tk**2
                     dt_NC[i] += dt_drij
                     dt_NC[j] -= dt_drij
 
-                    t = swtich_function(rij[i,j], r, dr)
+                    t = switch_function(rij[i,j], r, dr)
                     dt_NC += t * (2 * tk * dtk)
                     t_NC += t * tk**2
 
                     r, dr = r_zz.get(('N','C3'), (0.0, 0.0))
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j]
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j]
                     dt_NC3[i] += dt_drij
                     dt_NC3[j] -= dt_drij
             sig_NC = get_bond_tension(('N','C'))
             sig_NC3= get_bond_tension(('N','C3'))
             tension += sig_NC * (1.3 * t_NC**0.3 * dt_NC) + sig_NC3 * dt_NC3
             tensions.append(tension)
             continue
@@ -163,30 +155,30 @@
             dt_OC = np.zeros([natm,3])
             dt_ON = np.zeros([natm,3])
             dt_OO = np.zeros([natm,3])
             dt_OP = np.zeros([natm,3])
             for j, sym_j in enumerate(symbols):
                 if sym_j == 'C':
                     r, dr = r_zz.get(('O','C'), (0.0, 0.0))
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j]
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j]
                     dt_OC[i] += dt_drij
                     dt_OC[j] -= dt_drij
                 if sym_j == 'N':
                     r, dr = r_zz.get(('O','N'), (0.0, 0.0))
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j]
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j]
                     dt_ON[i] += dt_drij
                     dt_ON[j] -= dt_drij
                 if sym_j == 'O' and j != i:
                     r, dr = r_zz.get(('O','O'), (0.0, 0.0))
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j]
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j]
                     dt_OO[i] += dt_drij
                     dt_OO[j] -= dt_drij
                 if sym_j == 'P':
                     r, dr = r_zz.get(('O','P'), (0.0, 0.0))
-                    dt_drij = grad_swtich_function(rij[i,j], r, dr) * drij[i,j]
+                    dt_drij = grad_switch_function(rij[i,j], r, dr) * drij[i,j]
                     dt_OP[i] += dt_drij
                     dt_OP[j] -= dt_drij
             sig_OC = get_bond_tension(('O','C'))
             sig_ON = get_bond_tension(('O','N'))
             sig_OO = get_bond_tension(('O','O'))
             sig_OP = get_bond_tension(('O','P'))
             tension += sig_OC * dt_OC + sig_ON * dt_ON + sig_OO * dt_OO + sig_OP * dt_OP
@@ -219,62 +211,8 @@
     grad_SASA = cupy.asarray([cupy.sum(grad_area[p0:p1], axis=0) for p0,p1, in gridslice]).get()
     SASA *= radii.BOHR**2
     grad_SASA *= radii.BOHR**2
     mol_cds = mol_tension * np.sum(grad_SASA, axis=0) / 1000
     grad_tension *= radii.BOHR
     atm_cds = np.einsum('i,ijx->jx', SASA, grad_tension.get()) / 1000
     atm_cds+= np.einsum('i,ijx->jx', atm_tension.get(), grad_SASA) / 1000
-    return (mol_cds + atm_cds)/hartree2kcal # hartree
-
-def make_grad_object(grad_method):
-    '''For grad_method in vacuum, add nuclear gradients of solvent pcmobj'''
-    if grad_method.base.with_solvent.frozen:
-        raise RuntimeError('Frozen solvent model is not avialbe for energy gradients')
-
-    name = (grad_method.base.with_solvent.__class__.__name__
-            + grad_method.__class__.__name__)
-    return lib.set_class(WithSolventGrad(grad_method),
-                         (WithSolventGrad, grad_method.__class__), name)
-
-class WithSolventGrad:
-    _keys = {'de_solvent', 'de_solute'}
-
-    def __init__(self, grad_method):
-        self.__dict__.update(grad_method.__dict__)
-        self.de_solvent = None
-        self.de_solute = None
-
-    def undo_solvent(self):
-        cls = self.__class__
-        name_mixin = self.base.with_solvent.__class__.__name__
-        obj = lib.view(self, lib.drop_class(cls, WithSolventGrad, name_mixin))
-        del obj.de_solvent
-        del obj.de_solute
-        return obj
-
-    def kernel(self, *args, dm=None, atmlst=None, **kwargs):
-        dm = kwargs.pop('dm', None)
-        if dm is None:
-            dm = self.base.make_rdm1(ao_repr=True)
-        if dm.ndim == 3:
-            dm = dm[0] + dm[1]
-        self.de_solute  = super().kernel(*args, **kwargs)
-        self.de_solvent = pcm_grad.grad_qv(self.base.with_solvent, dm)
-        self.de_solvent+= pcm_grad.grad_solver(self.base.with_solvent, dm)
-        self.de_solvent+= pcm_grad.grad_nuc(self.base.with_solvent, dm)
-        self.de_cds     = get_cds(self.base.with_solvent)
-        self.de = self.de_solute + self.de_solvent + self.de_cds
-
-        if self.verbose >= logger.NOTE:
-            logger.note(self, '--------------- %s (+%s) gradients ---------------',
-                        self.base.__class__.__name__,
-                        self.base.with_solvent.__class__.__name__)
-            rhf_grad._write(self, self.mol, self.de, self.atmlst)
-            logger.note(self, '----------------------------------------------')
-        return self.de
-
-    def _finalize(self):
-        # disable _finalize. It is called in grad_method.kernel method
-        # where self.de was not yet initialized.
-        pass
-
-
+    return (mol_cds + atm_cds)/hartree2kcal # hartree
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/solvent/hessian/pcm.py` & `gpu4pyscf-0.7.7/gpu4pyscf/solvent/hessian/pcm.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,32 +10,28 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 '''
-Gradient of PCM family solvent model
+Hessian of PCM family solvent model
 '''
 # pylint: disable=C0103
 
 import numpy
 import cupy
-from cupyx import scipy
-from pyscf import lib, gto, df
-from pyscf.grad import rhf as rhf_grad
+from pyscf import lib, gto
 from gpu4pyscf import scf
-from gpu4pyscf.solvent.pcm import PI, switch_h
-from gpu4pyscf.solvent.grad.pcm import grad_switch_h, get_dF_dA, get_dD_dS, grad_qv, grad_solver, grad_nuc
+from gpu4pyscf.solvent.pcm import PI
+from gpu4pyscf.solvent.grad.pcm import grad_qv, grad_solver, grad_nuc
 from gpu4pyscf.df import int3c2e
 from gpu4pyscf.lib.cupy_helper import contract
 from gpu4pyscf.lib import logger
 
-libdft = lib.load_library('libdft')
-
 def hess_nuc(pcmobj):
     if not pcmobj._intermediates:
         pcmobj.build()
     mol = pcmobj.mol
     q_sym        = pcmobj._intermediates['q_sym'].get()
     gridslice    = pcmobj.surface['gslice_by_atom']
     grid_coords  = pcmobj.surface['grid_coords'].get()
@@ -140,19 +136,17 @@
     de = numpy.zeros([mol.natm, mol.natm, 3, 3])
     eps = 1e-3
     for ia in range(mol.natm):
         for ix in range(3):
             dv = numpy.zeros_like(coords)
             dv[ia,ix] = eps
             mol.set_geom_(coords + dv, unit='Bohr')
-            mol.build()
             g0 = pcm_grad_scanner(mol)
 
             mol.set_geom_(coords - dv, unit='Bohr')
-            mol.build()
             g1 = pcm_grad_scanner(mol)
             de[ia,:,ix] = (g0 - g1)/2.0/eps
     t1 = log.timer_debug1('solvent energy', *t1)
     pcmobj.reset(pmol)
     return de
 
 def fd_grad_vmat(pcmobj, dm, mo_coeff, mo_occ, atmlst=None, verbose=None):
@@ -179,19 +173,17 @@
     vmat = cupy.empty([len(atmlst), 3, nao, nocc])
     eps = 1e-3
     for i0, ia in enumerate(atmlst):
         for ix in range(3):
             dv = numpy.zeros_like(coords)
             dv[ia,ix] = eps
             mol.set_geom_(coords + dv, unit='Bohr')
-            mol.build()
             vmat0 = pcm_vmat_scanner(mol)
 
             mol.set_geom_(coords - dv, unit='Bohr')
-            mol.build()
             vmat1 = pcm_vmat_scanner(mol)
 
             grad_vmat = (vmat0 - vmat1)/2.0/eps
             grad_vmat = contract("ij,jq->iq", grad_vmat, mocc)
             grad_vmat = contract("iq,ip->pq", grad_vmat, mo_coeff)
             vmat[i0,ix] = grad_vmat
     t1 = log.timer_debug1('computing solvent grad veff', *t1)
@@ -234,21 +226,36 @@
 
     name = (hess_method.base.with_solvent.__class__.__name__
             + hess_method.__class__.__name__)
     return lib.set_class(WithSolventHess(hess_method),
                          (WithSolventHess, hess_method.__class__), name)
 
 class WithSolventHess:
+    from gpu4pyscf.lib.utils import to_gpu, device
+
     _keys = {'de_solvent', 'de_solute'}
 
     def __init__(self, hess_method):
         self.__dict__.update(hess_method.__dict__)
         self.de_solvent = None
         self.de_solute = None
 
+    def undo_solvent(self):
+        cls = self.__class__
+        name_mixin = self.base.with_solvent.__class__.__name__
+        obj = lib.view(self, lib.drop_class(cls, WithSolventHess, name_mixin))
+        del obj.de_solvent
+        del obj.de_solute
+        return obj
+
+    def to_cpu(self):
+        from pyscf.solvent.hessian import pcm           # type: ignore
+        hess_method = self.undo_solvent().to_cpu()
+        return pcm.make_hess_object(hess_method)
+
     def kernel(self, *args, dm=None, atmlst=None, **kwargs):
         dm = kwargs.pop('dm', None)
         if dm is None:
             dm = self.base.make_rdm1(ao_repr=True)
         if dm.ndim == 3:
             dm = dm[0] + dm[1]
         is_equilibrium = self.base.with_solvent.equilibrium_solvation
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/solvent/pcm.py` & `gpu4pyscf-0.7.7/gpu4pyscf/solvent/pcm.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,24 +18,25 @@
 '''
 # pylint: disable=C0103
 import ctypes
 import numpy
 import cupy
 import cupyx.scipy as scipy
 from pyscf import lib
-from pyscf import gto, df
+from pyscf import gto
 from pyscf.dft import gen_grid
 from pyscf.data import radii
-from pyscf.solvent import ddcosmo#, _attach_solvent
+from pyscf.solvent import ddcosmo
 from gpu4pyscf.solvent import _attach_solvent
 from gpu4pyscf.df import int3c2e
 from gpu4pyscf.lib import logger
-from gpu4pyscf.lib.cupy_helper import dist_matrix
+from gpu4pyscf.lib.cupy_helper import dist_matrix, load_library
 
 libdft = lib.load_library('libdft')
+libsolvent = load_library('libsolvent')
 
 @lib.with_doc(_attach_solvent._for_scf.__doc__)
 def pcm_for_scf(mf, solvent_obj=None, dm=None):
     if solvent_obj is None:
         solvent_obj = PCM(mf.mol)
     return _attach_solvent._for_scf(mf, solvent_obj, dm)
 
@@ -175,84 +176,125 @@
     '''
     R_vdw = surface['R_vdw']
     switch_fun = surface['switch_fun']
     weights = surface['weights']
     A = weights*R_vdw**2*switch_fun
     return switch_fun, A
 
-def get_D_S(surface, with_S=True, with_D=False):
+def get_D_S_slow(surface, with_S=True, with_D=False):
     '''
     generate D and S matrix in  J. Chem. Phys. 133, 244111 (2010)
     The diagonal entries of S is not filled
     '''
     charge_exp  = surface['charge_exp']
     grid_coords = surface['grid_coords']
     switch_fun  = surface['switch_fun']
     norm_vec    = surface['norm_vec']
     R_vdw       = surface['R_vdw']
 
     xi_i, xi_j = cupy.meshgrid(charge_exp, charge_exp, indexing='ij')
     xi_ij = xi_i * xi_j / (xi_i**2 + xi_j**2)**0.5
-    #rij = scipy.spatial.distance.cdist(grid_coords, grid_coords)
-    #rij = cupy.sum((grid_coords[:,None,:] - grid_coords[None,:,:])**2, axis=2)**0.5
     rij = dist_matrix(grid_coords, grid_coords)
     xi_r_ij = xi_ij * rij
     cupy.fill_diagonal(rij, 1)
     S = scipy.special.erf(xi_r_ij) / rij
     cupy.fill_diagonal(S, charge_exp * (2.0 / PI)**0.5 / switch_fun)
 
     D = None
     if with_D:
-        #drij = cupy.expand_dims(grid_coords, axis=1) - grid_coords
-        #nri = cupy.sum(grid_coords * norm_vec, axis=-1)
-        #nrij = cupy.expand_dims(nri, axis=1) - nri
-        #cupy.expand_dims(grid_coords, axis=1) * norm_vec
         nrij = grid_coords.dot(norm_vec.T) - cupy.sum(grid_coords * norm_vec, axis=-1)
-
-        #nrij = cupy.sum(drij * norm_vec, axis=-1)
-
         D = S*nrij/rij**2 -2.0*xi_r_ij/PI**0.5*cupy.exp(-xi_r_ij**2)*nrij/rij**3
         cupy.fill_diagonal(D, -charge_exp * (2.0 / PI)**0.5 / (2.0 * R_vdw))
+    return D, S
 
+def get_D_S(surface, with_S=True, with_D=False, stream=None):
+    ''' Efficiently generating D matrix and S matrix in PCM models '''
+    charge_exp  = surface['charge_exp']
+    grid_coords = surface['grid_coords']
+    switch_fun  = surface['switch_fun']
+    norm_vec    = surface['norm_vec']
+    R_vdw       = surface['R_vdw']
+    n = charge_exp.shape[0]
+    S = cupy.empty([n,n])
+    D = None
+    S_ptr = ctypes.cast(S.data.ptr, ctypes.c_void_p)
+    D_ptr = lib.c_null_ptr()
+    if with_D:
+        D = cupy.empty([n,n])
+        D_ptr = ctypes.cast(D.data.ptr, ctypes.c_void_p)
+    if stream is None:
+        stream = cupy.cuda.get_current_stream()
+    err = libsolvent.pcm_d_s(
+        ctypes.cast(stream.ptr, ctypes.c_void_p),
+        D_ptr, S_ptr,
+        ctypes.cast(grid_coords.data.ptr, ctypes.c_void_p),
+        ctypes.cast(norm_vec.data.ptr, ctypes.c_void_p),
+        ctypes.cast(R_vdw.data.ptr, ctypes.c_void_p),
+        ctypes.cast(charge_exp.data.ptr, ctypes.c_void_p),
+        ctypes.cast(switch_fun.data.ptr, ctypes.c_void_p),
+        ctypes.c_int(n)
+    )
+    if err != 0:
+        raise RuntimeError('Failed in generating PCM D and S matrices.')
     return D, S
 
 class PCM(lib.StreamObject):
     _keys = {
         'method', 'vdw_scale', 'surface', 'r_probe', 'intopt',
         'mol', 'radii_table', 'atom_radii', 'lebedev_order', 'lmax', 'eta',
         'eps', 'grids', 'max_cycle', 'conv_tol', 'state_id', 'frozen',
         'equilibrium_solvation', 'e', 'v',
     }
-
+    from gpu4pyscf.lib.utils import to_gpu, device
     kernel = ddcosmo.DDCOSMO.kernel
 
     def __init__(self, mol):
-        ddcosmo.DDCOSMO.__init__(self, mol)
+        self.mol = mol
+        self.stdout = mol.stdout
+        self.verbose = mol.verbose
+        self.max_memory = mol.max_memory
         self.method = 'C-PCM'
+
         self.vdw_scale = 1.2 # default value in qchem
+        self.surface = {}
         self.r_probe = 0.0
         self.radii_table = None
-        self.surface = {}
+        self.atom_radii = None
+        self.lebedev_order = 29
         self._intermediates = {}
+        self.eps = 78.3553
+
+        self.max_cycle = 20
+        self.conv_tol = 1e-7
+        self.state_id = 0
+
+        self.frozen = False
+        self.equilibrium_solvation = False
+
+        self.e = None
+        self.v = None
+        self._dm = None
 
     def dump_flags(self, verbose=None):
         logger.info(self, '******** %s ********', self.__class__)
         logger.info(self, 'lebedev_order = %s (%d grids per sphere)',
                     self.lebedev_order, gen_grid.LEBEDEV_ORDER[self.lebedev_order])
-        logger.info(self, 'lmax = %s'         , self.lmax)
-        logger.info(self, 'eta = %s'          , self.eta)
         logger.info(self, 'eps = %s'          , self.eps)
         logger.info(self, 'frozen = %s'       , self.frozen)
         logger.info(self, 'equilibrium_solvation = %s', self.equilibrium_solvation)
         logger.debug2(self, 'radii_table %s', self.radii_table)
         if self.atom_radii:
             logger.info(self, 'User specified atomic radii %s', str(self.atom_radii))
-        self.grids.dump_flags(verbose)
         return self
 
+    def to_cpu(self):
+        from gpu4pyscf.lib.utils import to_cpu
+        obj = to_cpu(self)
+        return obj.reset()
+
     def build(self, ng=None):
         if self.radii_table is None:
             vdw_scale = self.vdw_scale
             self.radii_table = vdw_scale * modified_Bondi + self.r_probe
         mol = self.mol
         if ng is None:
             ng = gen_grid.LEBEDEV_ORDER[self.lebedev_order]
@@ -267,15 +309,15 @@
             f_epsilon = (epsilon-1.)/epsilon
             K = S
             R = -f_epsilon * cupy.eye(K.shape[0])
         elif self.method.upper() == 'COSMO':
             f_epsilon = (epsilon - 1.0)/(epsilon + 1.0/2.0)
             K = S
             R = -f_epsilon * cupy.eye(K.shape[0])
-        elif self.method.upper() in ['IEF-PCM', 'IEFPCM', 'SMD']:
+        elif self.method.upper() in ['IEF-PCM', 'IEFPCM']:
             f_epsilon = (epsilon - 1.0)/(epsilon + 1.0)
             DA = D*A
             DAS = cupy.dot(DA, S)
             K = S - f_epsilon/(2.0*PI) * DAS
             R = -f_epsilon * (cupy.eye(K.shape[0]) - 1.0/(2.0*PI)*DA)
         elif self.method.upper() == 'SS(V)PE':
             f_epsilon = (epsilon - 1.0)/(epsilon + 1.0)
@@ -297,15 +339,14 @@
         self._intermediates.update(intermediates)
 
         charge_exp  = self.surface['charge_exp']
         grid_coords = self.surface['grid_coords']
         atom_coords = mol.atom_coords(unit='B')
         atom_charges = mol.atom_charges()
 
-        # Move this to GPU
         auxmol = gto.fakemol_for_charges(grid_coords.get(), expnt=charge_exp.get()**2)
         intopt = int3c2e.VHFOpt(mol, auxmol, 'int2e')
         intopt.build(1e-14, diag_block_with_triu=False, aosym=True, group_size=256)
         self.intopt = intopt
 
         int2c2e = mol._add_suffix('int2c2e')
         fakemol_nuc = gto.fakemol_for_charges(atom_coords)
@@ -381,15 +422,14 @@
             return pcm_hess.make_hess_object(hess_method)
         else:
             raise RuntimeError('Only SCF gradient is supported')
 
     def reset(self, mol=None):
         if mol is not None:
             self.mol = mol
-            self.grids.reset(mol)
         self._intermediates = None
         self.surface = None
         self.intopt = None
         return self
 
     def _B_dot_x(self, dms):
         if not self._intermediates:
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf/solvent/smd.py` & `gpu4pyscf-0.7.7/gpu4pyscf/solvent/smd.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,109 +14,33 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 '''
 SMD solvent model
 '''
 
 import numpy as np
-import scipy
 import cupy
-from pyscf import lib
+from pyscf import lib, gto
 from pyscf.data import radii
 from pyscf.dft import gen_grid
 from gpu4pyscf.solvent import pcm, _attach_solvent
 from gpu4pyscf.lib import logger
-from gpu4pyscf.lib.cupy_helper import dist_matrix
+from gpu4pyscf.df import int3c2e
 
 @lib.with_doc(_attach_solvent._for_scf.__doc__)
 def smd_for_scf(mf, solvent_obj=None, dm=None):
     if solvent_obj is None:
         solvent_obj = SMD(mf.mol)
     return _attach_solvent._for_scf(mf, solvent_obj, dm)
 
 # Inject PCM to SCF, TODO: add it to other methods later
 from gpu4pyscf import scf
 scf.hf.RHF.SMD = smd_for_scf
 scf.uhf.UHF.SMD = smd_for_scf
-hartree2kcal = 627.5
-# see https://pubs.acs.org/doi/epdf/10.1021/jp810292n
-
-sigma_water = {
-    ('H'): 48.69,
-    ('C'): 129.74,
-    ('H','C'): -60.77,
-    ('C','C'): -72.95,
-    ('O','C'): 68.69,
-    ('N','C'): -48.22,
-    ('N','C3'): 84.10,
-    ('O','N'): 121.98,
-    ('F'): 38.18,
-    ('Cl'): 9.82,
-    ('Br'): -8.72,
-    ('S'): -9.10,
-    ('O','P'): 68.85}
-
-sigma_n = {
-    ('C'): 58.10,
-    ('H','C'): -36.37,
-    ('C','C'): -62.05,
-    ('O'): -17.56,
-    ('H','O'): -19.39,
-    ('O','C'): -15.70,
-    ('N'): 32.62,
-    ('C','N'): -99.76,
-    ('Cl'): -24.31,
-    ('Br'): -35.42,
-    ('S'): -33.17,
-    ('Si'): -18.04
-}
-
-sigma_alpha = {
-    ('C'): 48.10,
-    ('O'): 193.06,
-    ('O','C'): 95.99,
-    ('C','N'): 152.20,
-    ('N','C'): -41.00
-}
-
-sigma_beta = {
-    ('C'): 32.87,
-    ('O'): -43.79,
-    ('O','O'):-128.16,
-    ('O','N'):79.13
-}
-
-# Molecular surface tension (cal/mol*AA^-2)
-sigma_gamma = 0.35
-sigma_phi2 = -4.19
-sigma_psi2 = -6.68
-sigma_beta2 = 0.0
-gamma0 = 1.0
-
-# rzz and delta r_zz in AA
-r_zz = {
-    ('H','C'): [1.55, 0.3],
-    ('H','O'): [1.55, 0.3],
-    ('C','H'): [1.55, 0.3],
-    ('C','C'): [1.84, 0.3],
-    ('C','N'): [1.84, 0.3],
-    ('C','O'): [1.84, 0.3],
-    ('C','F'): [1.84, 0.3],
-    ('C','P'): [2.2, 0.3],
-    ('C','S'): [2.2, 0.3],
-    ('C','Cl'): [2.1, 0.3],
-    ('C','Br'): [2.3, 0.3],
-    ('C','I'): [2.6, 0.3],
-    ('N','C'): [1.84, 0.3],
-    ('N','C3'): [1.225, 0.065],
-    ('O','C'): [1.33, 0.1],
-    ('O','N'): [1.5, 0.3],
-    ('O','O'): [1.8, 0.3],
-    ('O','P'): [2.1, 0.3]
-}
+hartree2kcal = 627.509451
 
 # database from https://comp.chem.umn.edu/solvation/mnsddb.pdf
 # solvent name: [n, n25, alpha, beta, gamma, epsilon, phi, psi)
 solvent_db = {
     '1,1,1-trichloroethane':[1.4379, 1.4313, 0.0, 0.09, 36.24, 7.0826, 0.0, 0.60],
     '1,1,2-trichloroethane':[1.4717, 1.4689, 0.13, 0.13, 48.97, 7.1937, 0.0, 0.60],
     '1,2,4-trimethylbenzene':[1.5048, 1.5024, 0.0, 0.19, 42.03, 2.3653, 0.667, 0.0],
@@ -323,183 +247,56 @@
     #radii_table[35] = 3.06 # original SMD
     # following value from SMD18
     # https://chemistry-europe.onlinelibrary.wiley.com/doi/10.1002/chem.201803652
     radii_table[35] = 2.60
     radii_table[53] = 2.74
     return radii_table/radii.BOHR
 
-def swtich_function(R, r, dr):
-    return np.exp(dr/(R-dr-r)) if R<r+dr else 0
-
-def atomic_surface_tension(symbols, coords, n, alpha, beta, water=True):
-    '''
-    - list of atomic symbols
-    - atomic coordinates in Anstrong
-    - solvent descriptors: n, alpha, beta
-    '''
-
-    def get_bond_tension(bond):
-        if water:
-            return sigma_water.get(bond, 0.0)
-        t = 0.0
-        t += sigma_n.get(bond, 0.0) * n
-        t += sigma_alpha.get(bond, 0.0) * alpha
-        t += sigma_beta.get(bond, 0.0) * beta
-        return t
-
-    def get_atom_tension(sym_i):
-        if water:
-            return sigma_water.get(sym_i, 0.0)
-        t = 0.0
-        t += sigma_n.get(sym_i, 0.0) * n
-        t += sigma_alpha.get(sym_i, 0.0) * alpha
-        t += sigma_beta.get(sym_i, 0.0) * beta
-        return t
-
-    rij = scipy.spatial.distance.cdist(coords, coords)
-    tensions = []
-    for i, sym_i in enumerate(symbols):
-        if sym_i not in ['H', 'C', 'N', 'O', 'F', 'Si', 'S', 'Cl', 'Br']:
-            tensions.append(0)
-            continue
-
-        tension = get_atom_tension(sym_i)
-        if sym_i in ['F', 'Si', 'S', 'Cl', 'Br']:
-            tensions.append(tension)
-            continue
-
-        if sym_i == 'H':
-            t_HC = 0.0
-            t_HO = 0.0
-            for j, sym_j in enumerate(symbols):
-                if sym_j == 'C':
-                    r, dr = r_zz.get(('H','C'), (0.0, 0.0))
-                    t_HC += swtich_function(rij[i,j], r, dr)
-                if sym_j == 'O':
-                    r, dr = r_zz.get(('H','O'), (0.0, 0.0))
-                    t_HO += swtich_function(rij[i,j], r, dr)
-            sig_HC = get_bond_tension(('H','C'))
-            sig_HO = get_bond_tension(('H','O'))
-            tension += sig_HC * t_HC + sig_HO * t_HO
-            tensions.append(tension)
-            continue
-
-        if sym_i == 'C':
-            t_CC = 0.0
-            t_CN = 0.0
-            for j, sym_j in enumerate(symbols):
-                if sym_j == 'C' and i != j:
-                    r, dr = r_zz.get(('C', 'C'), (0.0, 0.0))
-                    t_CC += swtich_function(rij[i,j], r, dr)
-                if sym_j == 'N':
-                    r, dr = r_zz.get(('C', 'N'), (0.0, 0.0))
-                    t_CN += swtich_function(rij[i,j], r, dr)
-            sig_CC = get_bond_tension(('C','C'))
-            sig_CN = get_bond_tension(('C','N'))
-            tension += sig_CC * t_CC + sig_CN * t_CN**2
-            tensions.append(tension)
-            continue
-
-        if sym_i == 'N':
-            t_NC = 0.0
-            t_NC3 = 0.0
-            for j, sym_j in enumerate(symbols):
-                if sym_j == 'C':
-                    r, dr = r_zz.get(('N','C'), (0.0,0.0))
-                    tk = 0.0
-                    for k, sym_k in enumerate(symbols):
-                        if k != i and k != j:
-                            rjk, drjk = r_zz.get(('C', sym_k), (0.0,0.0))
-                            tk += swtich_function(rij[j,k], rjk, drjk)
-                    t_NC += swtich_function(rij[i,j], r, dr) * tk**2
-
-                    r, dr = r_zz.get(('N','C3'), (0.0, 0.0))
-                    t_NC3 += swtich_function(rij[i,j], r, dr)
-            sig_NC = get_bond_tension(('N','C'))
-            sig_NC3= get_bond_tension(('N','C3'))
-            tension += sig_NC * t_NC**1.3 + sig_NC3 * t_NC3
-            tensions.append(tension)
-            continue
-
-        if sym_i == 'O':
-            t_OC = 0.0
-            t_ON = 0.0
-            t_OO = 0.0
-            t_OP = 0.0
-            for j, sym_j in enumerate(symbols):
-                if sym_j == 'C':
-                    r, dr = r_zz.get(('O','C'), (0.0, 0.0))
-                    t_OC += swtich_function(rij[i,j], r, dr)
-                if sym_j == 'N':
-                    r, dr = r_zz.get(('O','N'), (0.0, 0.0))
-                    t_ON += swtich_function(rij[i,j], r, dr)
-                if sym_j == 'O' and j != i:
-                    r, dr = r_zz.get(('O','O'), (0.0, 0.0))
-                    t_OO += swtich_function(rij[i,j], r, dr)
-                if sym_j == 'P':
-                    r, dr = r_zz.get(('O','P'), (0.0, 0.0))
-                    t_OP += swtich_function(rij[i,j], r, dr)
-            sig_OC = get_bond_tension(('O','C'))
-            sig_ON = get_bond_tension(('O','N'))
-            sig_OO = get_bond_tension(('O','O'))
-            sig_OP = get_bond_tension(('O','P'))
-            tension += sig_OC * t_OC + sig_ON * t_ON + sig_OO * t_OO + sig_OP * t_OP
-            tensions.append(tension)
-            continue
-    return cupy.asarray(tensions)
-
-def molecular_surface_tension(beta, gamma, phi, psi):
-    sig_gamma = sigma_gamma * gamma / gamma0
-    sig_phi = sigma_phi2 * phi**2
-    sig_psi = sigma_psi2 * psi**2
-    sig_beta= sigma_beta2 * beta**2
-    return sig_gamma + sig_phi + sig_psi + sig_beta
-
-def naive_sasa(mol, rad):
-    coords = mol.atom_coords(unit='A')
-    charges = mol.atom_charges()
-    radius = [rad[ch] for ch in charges]
-    sasa = []
-    for i in range(mol.natm):
-        area = 4 * np.pi * radius[i]
-        for j in range(mol.natm):
-            if i != j:
-                dr = coords[i] - coords[j]
-                r = (dr[0]**2 + dr[1]**2 + dr[2]**2)**0.5
-                r1 = radius[i]
-                r2 = radius[j]
-                if r < r1 + r2:
-                    overlap = (r1 + r2 - r) / (r1 + r2)
-                    area -= overlap * area
-        sasa.append(area)
-    return cupy.asarray(sasa)
-
-def get_cds(smdobj):
+import ctypes
+from gpu4pyscf.lib.cupy_helper import load_library
+libsolvent = load_library('libsolvent')
+def get_cds_legacy(smdobj):
     mol = smdobj.mol
-    n, _, alpha, beta, gamma, _, phi, psi = smdobj.solvent_descriptors
-    symbols = [mol.atom_symbol(ia) for ia in range(mol.natm)]
-    coords = mol.atom_coords(unit='A')
-    if smdobj._solvent.lower() != 'water':
-        atm_tension = atomic_surface_tension(symbols, coords, n, alpha, beta, water=False)
-        mol_tension = molecular_surface_tension(beta, gamma, phi, psi)
-    else:
-        logger.info(mol, 'no solvent descriptor is needed for water')
-        atm_tension = atomic_surface_tension(symbols, coords, n, alpha, beta, water=True)
-        mol_tension = 0.0
-
-    # generate surface for calculating SASA
-    rad = radii.VDW + 0.4/radii.BOHR
-    surface = pcm.gen_surface(mol, ng=smdobj.sasa_ng, rad=rad)
-    area = surface['area']
-    gridslice = surface['gslice_by_atom']
-    SASA = cupy.asarray([cupy.sum(area[p0:p1], axis=0) for p0,p1, in gridslice])
-    SASA *= radii.BOHR**2
-    mol_cds = mol_tension * cupy.sum(SASA) / 1000 # in kcal/mol
-    atm_cds = cupy.sum(SASA * atm_tension) / 1000 # in kcal/mol
-    return (mol_cds + atm_cds)/hartree2kcal # hartree
+    natm = mol.natm
+    soln, _, sola, solb, solg, _, solc, solh = smdobj.solvent_descriptors
+    #symbols = [mol.atom_s(ia) for ia in range(mol.natm)]
+    charges = np.asarray(mol.atom_charges(), dtype=np.int32, order='F')
+    coords = np.asarray(mol.atom_coords(unit='B'), dtype=np.float64, order='C')
+    icds = 1 if smdobj.solvent.upper() == 'WATER' else 2
+    dcds = np.empty([natm,3])
+    mnsol_interface =  libsolvent.mnsol_interface_
+
+    double_ndptr = np.ctypeslib.ndpointer(dtype=np.float64)
+    int_ndptr = np.ctypeslib.ndpointer(dtype=np.int32)
+    double_ptr = ctypes.POINTER(ctypes.c_double)
+    int_ptr = ctypes.POINTER(ctypes.c_int)
+
+    mnsol_interface.argtypes = [
+        double_ndptr, int_ndptr,
+        int_ptr,
+        double_ptr, double_ptr, double_ptr, double_ptr, double_ptr, double_ptr,
+        int_ptr,
+        double_ptr, double_ptr, double_ndptr]
+    natm = ctypes.byref(ctypes.c_int(natm))
+    icds = ctypes.byref(ctypes.c_int(icds))
+    soln = ctypes.byref(ctypes.c_double(soln))
+    sola = ctypes.byref(ctypes.c_double(sola))
+    solb = ctypes.byref(ctypes.c_double(solb))
+    solg = ctypes.byref(ctypes.c_double(solg))
+    solc = ctypes.byref(ctypes.c_double(solc))
+    solh = ctypes.byref(ctypes.c_double(solh))
+    gcds = ctypes.c_double()
+    areacds = ctypes.c_double()
+
+    mnsol_interface(coords, charges,
+                    natm,
+                    sola, solb, solc, solg, solh, soln,
+                    icds,
+                    ctypes.byref(gcds), ctypes.byref(areacds), dcds)
+    return gcds.value / hartree2kcal, dcds
 
 class SMD(pcm.PCM):
     _keys = {
         'intopt', 'method', 'e_cds', 'solvent_descriptors', 'r_probe', 'sasa_ng'
     }
     def __init__(self, mol, solvent=''):
         super().__init__(mol)
@@ -541,35 +338,79 @@
         self.eps = values[5]
 
     def dump_flags(self, verbose=None):
         n, _, alpha, beta, gamma, _, phi, psi = self.solvent_descriptors
         logger.info(self, '******** %s ********', self.__class__)
         logger.info(self, 'lebedev_order = %s (%d grids per sphere)',
                     self.lebedev_order, gen_grid.LEBEDEV_ORDER[self.lebedev_order])
-        logger.info(self, 'lmax = %s'         , self.lmax)
-        logger.info(self, 'eta = %s'          , self.eta)
         logger.info(self, 'eps = %s'          , self.eps)
         logger.info(self, 'frozen = %s'       , self.frozen)
         logger.info(self, '---------- SMD solvent descriptors -------')
         logger.info(self, f'n     = {n}')
         logger.info(self, f'alpha = {alpha}')
         logger.info(self, f'beta  = {beta}')
         logger.info(self, f'gamma = {gamma}')
         logger.info(self, f'phi   = {phi}')
         logger.info(self, f'psi   = {psi}')
         logger.info(self, '--------------------- end ----------------')
         logger.info(self, 'equilibrium_solvation = %s', self.equilibrium_solvation)
         logger.info(self, 'radii_table %s', self.radii_table*radii.BOHR)
         if self.atom_radii:
             logger.info(self, 'User specified atomic radii %s', str(self.atom_radii))
-        self.grids.dump_flags(verbose)
         return self
 
+    def build(self, ng=None):
+        if self.radii_table is None:
+            vdw_scale = self.vdw_scale
+            self.radii_table = vdw_scale * pcm.modified_Bondi + self.r_probe
+        mol = self.mol
+        if ng is None:
+            ng = gen_grid.LEBEDEV_ORDER[self.lebedev_order]
+
+        self.surface = pcm.gen_surface(mol, rad=self.radii_table, ng=ng)
+        self._intermediates = {}
+        F, A = pcm.get_F_A(self.surface)
+        D, S = pcm.get_D_S(self.surface, with_S=True, with_D=True)
+
+        epsilon = self.eps
+        f_epsilon = (epsilon - 1.0)/(epsilon + 1.0)
+        DA = D*A
+        DAS = cupy.dot(DA, S)
+        K = S - f_epsilon/(2.0*np.pi) * DAS
+        R = -f_epsilon * (cupy.eye(K.shape[0]) - 1.0/(2.0*np.pi)*DA)
+
+        intermediates = {
+            'S': cupy.asarray(S),
+            'D': cupy.asarray(D),
+            'A': cupy.asarray(A),
+            'K': cupy.asarray(K),
+            'R': cupy.asarray(R),
+            'f_epsilon': f_epsilon
+        }
+        self._intermediates.update(intermediates)
+
+        charge_exp  = self.surface['charge_exp']
+        grid_coords = self.surface['grid_coords']
+        atom_coords = mol.atom_coords(unit='B')
+        atom_charges = mol.atom_charges()
+
+        # Move this to GPU
+        auxmol = gto.fakemol_for_charges(grid_coords.get(), expnt=charge_exp.get()**2)
+        intopt = int3c2e.VHFOpt(mol, auxmol, 'int2e')
+        intopt.build(1e-14, diag_block_with_triu=False, aosym=True, group_size=256)
+        self.intopt = intopt
+
+        int2c2e = mol._add_suffix('int2c2e')
+        fakemol_nuc = gto.fakemol_for_charges(atom_coords)
+        v_ng = gto.mole.intor_cross(int2c2e, fakemol_nuc, auxmol)
+        v_grids_n = np.dot(atom_charges, v_ng)
+        self.v_grids_n = cupy.asarray(v_grids_n)
+
     def get_cds(self):
-        return get_cds(self)
+        return get_cds_legacy(self)[0]
 
     def nuc_grad_method(self, grad_method):
         from gpu4pyscf.solvent.grad import smd as smd_grad
         if self.frozen:
             raise RuntimeError('Frozen solvent model is not supported')
         from gpu4pyscf import scf
         if isinstance(grad_method.base, (scf.hf.RHF, scf.uhf.UHF)):
```

### Comparing `gpu4pyscf-0.7.6/gpu4pyscf.egg-info/SOURCES.txt` & `gpu4pyscf-0.7.7/gpu4pyscf.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -63,14 +63,18 @@
 gpu4pyscf/lib/dftd4.py
 gpu4pyscf/lib/diis.py
 gpu4pyscf/lib/logger.py
 gpu4pyscf/lib/utils.py
 gpu4pyscf/mp/__init__.py
 gpu4pyscf/mp/dfmp2.py
 gpu4pyscf/mp/mp2.py
+gpu4pyscf/properties/__init__.py
+gpu4pyscf/properties/ir.py
+gpu4pyscf/properties/polarizability.py
+gpu4pyscf/properties/shielding.py
 gpu4pyscf/qmmm/__init__.py
 gpu4pyscf/qmmm/chelpg.py
 gpu4pyscf/scf/__init__.py
 gpu4pyscf/scf/_response_functions.py
 gpu4pyscf/scf/cphf.py
 gpu4pyscf/scf/diis.py
 gpu4pyscf/scf/dispersion.py
@@ -80,13 +84,16 @@
 gpu4pyscf/scf/rohf.py
 gpu4pyscf/scf/ucphf.py
 gpu4pyscf/scf/uhf.py
 gpu4pyscf/solvent/__init__.py
 gpu4pyscf/solvent/_attach_solvent.py
 gpu4pyscf/solvent/pcm.py
 gpu4pyscf/solvent/smd.py
+gpu4pyscf/solvent/smd_experiment.py
 gpu4pyscf/solvent/grad/__init__.py
 gpu4pyscf/solvent/grad/pcm.py
 gpu4pyscf/solvent/grad/smd.py
+gpu4pyscf/solvent/grad/smd_experiment.py
 gpu4pyscf/solvent/hessian/__init__.py
 gpu4pyscf/solvent/hessian/pcm.py
-gpu4pyscf/solvent/hessian/smd.py
+gpu4pyscf/solvent/hessian/smd.py
+gpu4pyscf/solvent/hessian/smd_experiment.py
```

### Comparing `gpu4pyscf-0.7.6/setup.py` & `gpu4pyscf-0.7.7/setup.py`

 * *Files identical despite different names*

