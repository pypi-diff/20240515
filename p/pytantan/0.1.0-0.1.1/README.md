# Comparing `tmp/pytantan-0.1.0.tar.gz` & `tmp/pytantan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytantan-0.1.0.tar", last modified: Wed May  8 10:45:18 2024, max compression
+gzip compressed data, was "pytantan-0.1.1.tar", last modified: Wed May 15 09:42:28 2024, max compression
```

## Comparing `pytantan-0.1.0.tar` & `pytantan-0.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:18.045122 pytantan-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 10:45:12.000000 pytantan-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-08 10:45:12.000000 pytantan-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-08 10:45:12.000000 pytantan-0.1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-08 10:45:12.000000 pytantan-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-05-08 10:45:18.045122 pytantan-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-05-08 10:45:12.000000 pytantan-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 10:45:17.000000 pytantan-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:18.037121 pytantan-0.1.0/pytantan/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/_mask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/lib.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:18.041121 pytantan-0.1.0/pytantan/platform/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/platform/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/platform/pxd.in
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/platform/pyx.in
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:18.041121 pytantan-0.1.0/pytantan/tantan/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tantan/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tantan/alphabet.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tantan/lc.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tantan/options.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tantan/score_matrix.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tantan/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tantan/version.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:18.041121 pytantan-0.1.0/pytantan/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tests/test_alphabet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-08 10:45:12.000000 pytantan-0.1.0/pytantan/tests/test_repeat_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:18.041121 pytantan-0.1.0/pytantan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-05-08 10:45:18.000000 pytantan-0.1.0/pytantan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-08 10:45:18.000000 pytantan-0.1.0/pytantan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:45:18.000000 pytantan-0.1.0/pytantan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:45:18.000000 pytantan-0.1.0/pytantan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 10:45:18.000000 pytantan-0.1.0/pytantan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 10:45:18.000000 pytantan-0.1.0/pytantan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-08 10:45:18.049121 pytantan-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    23131 2024-05-08 10:45:12.000000 pytantan-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:18.037121 pytantan-0.1.0/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:18.041121 pytantan-0.1.0/vendor/tantan/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:45:18.045122 pytantan-0.1.0/vendor/tantan/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/LambdaCalculator.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/LambdaCalculator.hh
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/cbrc_linalg.cc
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/cbrc_linalg.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_alphabet.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_fasta_sequence.cc
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_fasta_sequence.hh
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_score_matrix.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_score_matrix.hh
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_simd.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_tantan_options.cc
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_tantan_options.hh
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_util.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_util.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/mcf_zstream.hh
--rw-r--r--   0 runner    (1001) docker     (127)    16946 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/tantan.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/tantan.hh
--rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/tantan_app.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/tantan_repeat_finder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-08 10:45:13.000000 pytantan-0.1.0/vendor/tantan/src/tantan_repeat_finder.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:28.747731 pytantan-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-15 09:42:23.000000 pytantan-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-15 09:42:23.000000 pytantan-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-15 09:42:23.000000 pytantan-0.1.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-15 09:42:23.000000 pytantan-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-05-15 09:42:28.747731 pytantan-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-15 09:42:23.000000 pytantan-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 09:42:28.000000 pytantan-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:28.743731 pytantan-0.1.1/pytantan/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/_mask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/lib.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:28.743731 pytantan-0.1.1/pytantan/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/platform/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/platform/pxd.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/platform/pyx.in
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:28.743731 pytantan-0.1.1/pytantan/tantan/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tantan/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tantan/alphabet.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tantan/lc.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tantan/options.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tantan/score_matrix.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tantan/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tantan/version.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:28.743731 pytantan-0.1.1/pytantan/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tests/test_alphabet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-15 09:42:23.000000 pytantan-0.1.1/pytantan/tests/test_repeat_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:28.743731 pytantan-0.1.1/pytantan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-05-15 09:42:28.000000 pytantan-0.1.1/pytantan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-15 09:42:28.000000 pytantan-0.1.1/pytantan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:42:28.000000 pytantan-0.1.1/pytantan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:42:28.000000 pytantan-0.1.1/pytantan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 09:42:28.000000 pytantan-0.1.1/pytantan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 09:42:28.000000 pytantan-0.1.1/pytantan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-15 09:42:28.751731 pytantan-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    23124 2024-05-15 09:42:23.000000 pytantan-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:28.739730 pytantan-0.1.1/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:28.747731 pytantan-0.1.1/vendor/tantan/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:42:28.747731 pytantan-0.1.1/vendor/tantan/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/LambdaCalculator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/LambdaCalculator.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/cbrc_linalg.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/cbrc_linalg.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_alphabet.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_fasta_sequence.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_fasta_sequence.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_score_matrix.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_score_matrix.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_simd.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_tantan_options.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_tantan_options.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_util.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_util.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/mcf_zstream.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    16946 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/tantan.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/tantan.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/tantan_app.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/tantan_repeat_finder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-15 09:42:24.000000 pytantan-0.1.1/vendor/tantan/src/tantan_repeat_finder.hh
```

### Comparing `pytantan-0.1.0/CONTRIBUTING.md` & `pytantan-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/COPYING` & `pytantan-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/MANIFEST.in` & `pytantan-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/PKG-INFO` & `pytantan-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytantan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cython bindings and Python interface to Tantan, a fast method for identifying repeats in DNA and protein sequences.
 Home-page: https://github.com/althonos/pytantan
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
-License: GPLv3+
+License: GPL-3.0-or-later
 Project-URL: Documentation, https://pytantan.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pytantan/issues
 Project-URL: Changelog, https://github.com/althonos/pytantan/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/althonos/pytantan/
 Project-URL: Builds, https://github.com/althonos/pytantan/actions
 Project-URL: PyPI, https://pypi.org/project/pytantan
 Keywords: bioinformatics,sequence,repeats,masking
@@ -86,30 +86,29 @@
 ## 🔧 Installing
 
 PyTantan is available for all modern versions (3.6+), depending only on the
 [`scoring-matrices`](https://pypi.org/project/scoring-matrices) package, and
 optionally on the lightweight [`archspec`](https://pypi.org/project/archspec)
 package for runtime CPU feature detection.
 
-<!-- It can be installed directly from [PyPI](https://pypi.org/project/pytantan/),
-which hosts some pre-built x86-64 wheels for Linux, MacOS, and Windows,
-Aarch64 wheels for Linux and MacOS, as well as the code required to 
-compile from source with Cython:
+It can be installed directly from [PyPI](https://pypi.org/project/pytantan/),
+which hosts some pre-built wheels for Linux and MacOS, as well as the code 
+required to compile from source with Cython:
 ```console
 $ pip install pytantan
-``` -->
+```
 
 <!-- Otherwise, PyTantan is also available as a [Bioconda](https://bioconda.github.io/)
 package:
 ```console
 $ conda install -c bioconda pytantan
 ``` -->
 
-<!-- Check the [*install* page](https://pytantan.readthedocs.io/en/stable/install.html)
-of the documentation for other ways to install PyTantan on your machine. -->
+Check the [*install* page](https://pytantan.readthedocs.io/en/stable/install.html)
+of the documentation for other ways to install PyTantan on your machine.
 
 ## 💡 Example
 
 The top-level function `pytantan.mask_repeats` can be used to mask a sequence
 without having to manage intermediate objects:
 
 ```python
```

### Comparing `pytantan-0.1.0/README.md` & `pytantan-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,30 +47,29 @@
 ## 🔧 Installing
 
 PyTantan is available for all modern versions (3.6+), depending only on the
 [`scoring-matrices`](https://pypi.org/project/scoring-matrices) package, and
 optionally on the lightweight [`archspec`](https://pypi.org/project/archspec)
 package for runtime CPU feature detection.
 
-<!-- It can be installed directly from [PyPI](https://pypi.org/project/pytantan/),
-which hosts some pre-built x86-64 wheels for Linux, MacOS, and Windows,
-Aarch64 wheels for Linux and MacOS, as well as the code required to 
-compile from source with Cython:
+It can be installed directly from [PyPI](https://pypi.org/project/pytantan/),
+which hosts some pre-built wheels for Linux and MacOS, as well as the code 
+required to compile from source with Cython:
 ```console
 $ pip install pytantan
-``` -->
+```
 
 <!-- Otherwise, PyTantan is also available as a [Bioconda](https://bioconda.github.io/)
 package:
 ```console
 $ conda install -c bioconda pytantan
 ``` -->
 
-<!-- Check the [*install* page](https://pytantan.readthedocs.io/en/stable/install.html)
-of the documentation for other ways to install PyTantan on your machine. -->
+Check the [*install* page](https://pytantan.readthedocs.io/en/stable/install.html)
+of the documentation for other ways to install PyTantan on your machine.
 
 ## 💡 Example
 
 The top-level function `pytantan.mask_repeats` can be used to mask a sequence
 without having to manage intermediate objects:
 
 ```python
```

### Comparing `pytantan-0.1.0/pytantan/__init__.py` & `pytantan-0.1.1/pytantan/__init__.py`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/_mask.py` & `pytantan-0.1.1/pytantan/_mask.py`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/lib.pyi` & `pytantan-0.1.1/pytantan/lib.pyi`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/lib.pyx` & `pytantan-0.1.1/pytantan/lib.pyx`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/platform/__init__.pxd` & `pytantan-0.1.1/pytantan/platform/__init__.pxd`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/platform/pxd.in` & `pytantan-0.1.1/pytantan/platform/pxd.in`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/platform/pyx.in` & `pytantan-0.1.1/pytantan/platform/pyx.in`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/tantan/__init__.pxd` & `pytantan-0.1.1/pytantan/tantan/__init__.pxd`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/tantan/alphabet.pxd` & `pytantan-0.1.1/pytantan/tantan/alphabet.pxd`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/tantan/options.pxd` & `pytantan-0.1.1/pytantan/tantan/options.pxd`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/tantan/score_matrix.pxd` & `pytantan-0.1.1/pytantan/tantan/score_matrix.pxd`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/tests/test_alphabet.py` & `pytantan-0.1.1/pytantan/tests/test_alphabet.py`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/tests/test_doctest.py` & `pytantan-0.1.1/pytantan/tests/test_doctest.py`

 * *Files 23% similar despite different names*

```diff
@@ -66,42 +66,19 @@
     if sys.argv[0].endswith("green"):
         return tests
 
     # recursively traverse all library submodules and load tests from them
     packages = [None, pytantan.lib]
 
     for pkg in iter(packages.pop, None):
-        globs = dict(pyopal=pytantan, ScoringMatrix=ScoringMatrix, Bio=Bio, **pkg.__dict__)
+        globs = dict(pytantan=pytantan, ScoringMatrix=ScoringMatrix, Bio=Bio, **pkg.__dict__)
         tests.addTests(
             doctest.DocTestSuite(
                 pkg,
                 globs=globs,
                 setUp=setUp,
                 tearDown=tearDown,
                 optionflags=+doctest.ELLIPSIS,
             )
         )
-        # for (_, subpkgname, subispkg) in pkgutil.walk_packages(pkg.__path__):
-        #     # do not import __main__ module to avoid side effects!
-        #     if subpkgname == "__main__" or subpkgname.startswith("tests"):
-        #         continue
-        #     # import the submodule and add it to the tests
-        #     module = importlib.import_module(".".join([pkg.__name__, subpkgname]))
-        #     if hasattr(module, "__test__"):
-        #         del module.__test__
-        #     globs = dict(pyopal=pytantan, Bio=Bio, **module.__dict__)
-        #     tests.addTests(
-        #         doctest.DocTestSuite(
-        #             module,
-        #             globs=globs,
-        #             setUp=setUp,
-        #             tearDown=tearDown,
-        #             optionflags=+doctest.ELLIPSIS,
-        #         )
-        #     )
-        #     # if the submodule is a package, we need to process its submodules
-        #     # as well, so we add it to the package queue, unless it is the
-        #     # `pyopal.tests` package (we don't need to check for doctests there)
-        #     if subispkg and subpkgname != "tests":
-        #         packages.append(module)
 
     return tests
```

### Comparing `pytantan-0.1.0/pytantan/tests/test_mask.py` & `pytantan-0.1.1/pytantan/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan/tests/test_repeat_finder.py` & `pytantan-0.1.1/pytantan/tests/test_repeat_finder.py`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/pytantan.egg-info/PKG-INFO` & `pytantan-0.1.1/pytantan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytantan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cython bindings and Python interface to Tantan, a fast method for identifying repeats in DNA and protein sequences.
 Home-page: https://github.com/althonos/pytantan
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
-License: GPLv3+
+License: GPL-3.0-or-later
 Project-URL: Documentation, https://pytantan.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pytantan/issues
 Project-URL: Changelog, https://github.com/althonos/pytantan/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/althonos/pytantan/
 Project-URL: Builds, https://github.com/althonos/pytantan/actions
 Project-URL: PyPI, https://pypi.org/project/pytantan
 Keywords: bioinformatics,sequence,repeats,masking
@@ -86,30 +86,29 @@
 ## 🔧 Installing
 
 PyTantan is available for all modern versions (3.6+), depending only on the
 [`scoring-matrices`](https://pypi.org/project/scoring-matrices) package, and
 optionally on the lightweight [`archspec`](https://pypi.org/project/archspec)
 package for runtime CPU feature detection.
 
-<!-- It can be installed directly from [PyPI](https://pypi.org/project/pytantan/),
-which hosts some pre-built x86-64 wheels for Linux, MacOS, and Windows,
-Aarch64 wheels for Linux and MacOS, as well as the code required to 
-compile from source with Cython:
+It can be installed directly from [PyPI](https://pypi.org/project/pytantan/),
+which hosts some pre-built wheels for Linux and MacOS, as well as the code 
+required to compile from source with Cython:
 ```console
 $ pip install pytantan
-``` -->
+```
 
 <!-- Otherwise, PyTantan is also available as a [Bioconda](https://bioconda.github.io/)
 package:
 ```console
 $ conda install -c bioconda pytantan
 ``` -->
 
-<!-- Check the [*install* page](https://pytantan.readthedocs.io/en/stable/install.html)
-of the documentation for other ways to install PyTantan on your machine. -->
+Check the [*install* page](https://pytantan.readthedocs.io/en/stable/install.html)
+of the documentation for other ways to install PyTantan on your machine.
 
 ## 💡 Example
 
 The top-level function `pytantan.mask_repeats` can be used to mask a sequence
 without having to manage intermediate objects:
 
 ```python
```

### Comparing `pytantan-0.1.0/pytantan.egg-info/SOURCES.txt` & `pytantan-0.1.1/pytantan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/setup.cfg` & `pytantan-0.1.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version = attr: pytantan._version.__version__
 author = Martin Larralde
 author_email = martin.larralde@embl.de
 url = https://github.com/althonos/pytantan
 description = Cython bindings and Python interface to Tantan, a fast method for identifying repeats in DNA and protein sequences.
 long_description = file: README.md
 long_description_content_type = text/markdown
-license = GPLv3+
+license = GPL-3.0-or-later
 platform = any
 keywords = bioinformatics, sequence, repeats, masking
 classifier = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -42,18 +42,18 @@
 zip_safe = false
 packages = pytantan, pytantan.tests, pytantan.platform
 include_package_data = true
 python_requires = >=3.5
 setup_requires = 
 	setuptools >=46.4
 	cython ~=3.0
-	scoring-matrices ~=0.2
+	scoring-matrices ~=0.2.0
 install_requires = 
 	archspec ~=0.2      ; os_name != 'nt'
-	scoring-matrices ~=0.2
+	scoring-matrices ~=0.2.0
 tests_require = 
 	importlib-resources ; python_version < '3.7'
 
 [options.package_data]
 pytantan = py.typed, *.pyi, *.pxd, *.h
 pytantan.tests = requirements.txt
```

### Comparing `pytantan-0.1.0/setup.py` & `pytantan-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,25 +51,25 @@
 
 def _split_multiline(value):
     value = value.strip()
     sep = max('\n,;', key=value.count)
     return list(filter(None, map(lambda x: x.strip(), value.split(sep))))
 
 
-def _patch_osx_compiler(compiler):
+def _patch_osx_compiler(compiler, machine):
     # On newer OSX, Python has been compiled as a universal binary, so
     # it will attempt to pass universal binary flags when building the
     # extension. This will not work because the code makes use of SSE2.
     for tool in ("compiler", "compiler_so", "linker_so"):
         flags = getattr(compiler, tool)
         i = next(
             (
                 i
                 for i in range(1, len(flags))
-                if flags[i - 1] == "-arch" and flags[i] != platform.machine()
+                if flags[i - 1] == "-arch" and flags[i] != machine
             ),
             None,
         )
         if i is not None:
             flags.pop(i)
             flags.pop(i - 1)
 
@@ -287,18 +287,18 @@
         return ["-mfpu=neon"] if self.target_cpu == "arm" else []
 
     def _check_neon(self):
         return self._check_simd_generic(
             "NEON",
             self._neon_flags(),
             header="arm_neon.h",
-            vector="int16x8_t",
-            set="vdupq_n_s16",
-            op="vabsq_s16",
-            extract="vgetq_lane_s16",
+            vector="float64x2_t",
+            set="vdupq_n_f64",
+            op="vabsq_f64",
+            extract="vgetq_lane_f64",
         )
 
     def _check_getid(self):
         _eprint('checking whether `PyInterpreterState_GetID` is available')
 
         base = "have_getid"
         testfile = os.path.join(self.build_temp, "{}.c".format(base))
@@ -400,15 +400,15 @@
         if isinstance(cythonize, ImportError):
             raise RuntimeError(
                 "Cython is required to run `build_ext` command"
             ) from cythonize
 
         # remove universal compilation flags for OSX
         if platform.system() == "Darwin":
-            _patch_osx_compiler(self.compiler)
+            _patch_osx_compiler(self.compiler, self.target_machine)
 
         # generate files from templates:
         for i, ext in enumerate(self.extensions):
             if isinstance(ext, ExtensionTemplate):
                 self.generate_extension(ext)
 
         # use debug directives with Cython if building in debug mode
@@ -465,15 +465,15 @@
                 self._simd_flags["SSE4"].extend(self._sse4_flags())
                 self._simd_defines["SSE4"].append(("__SSE4_1__", 1))
             if not self._simd_disabled["SSE2"] and self._check_sse2():
                 cython_args["compile_time_env"]["SSE2_BUILD_SUPPORT"] = True
                 self._simd_supported["SSE2"] = True
                 self._simd_flags["SSE2"].extend(self._sse2_flags())
                 self._simd_defines["SSE2"].append(("__SSE2__", 1))
-        elif self.target_cpu == "arm" or self.target_cpu == "aarch64":
+        elif self.target_cpu == "aarch64":
             if not self._simd_disabled["NEON"] and self._check_neon():
                 cython_args["compile_time_env"]["NEON_BUILD_SUPPORT"] = True
                 self._simd_supported["NEON"] = True
                 self._simd_flags["NEON"].extend(self._neon_flags())
                 self._simd_defines["NEON"].append(("__ARM_NEON__", 1))
 
         # filter out extensions missing required CPU features
```

### Comparing `pytantan-0.1.0/vendor/tantan/COPYING.txt` & `pytantan-0.1.1/vendor/tantan/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/README.rst` & `pytantan-0.1.1/vendor/tantan/README.rst`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/LambdaCalculator.cc` & `pytantan-0.1.1/vendor/tantan/src/LambdaCalculator.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/LambdaCalculator.hh` & `pytantan-0.1.1/vendor/tantan/src/LambdaCalculator.hh`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/cbrc_linalg.cc` & `pytantan-0.1.1/vendor/tantan/src/cbrc_linalg.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/cbrc_linalg.hh` & `pytantan-0.1.1/vendor/tantan/src/cbrc_linalg.hh`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_alphabet.cc` & `pytantan-0.1.1/vendor/tantan/src/mcf_alphabet.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_alphabet.hh` & `pytantan-0.1.1/vendor/tantan/src/mcf_alphabet.hh`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_fasta_sequence.cc` & `pytantan-0.1.1/vendor/tantan/src/mcf_fasta_sequence.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_score_matrix.cc` & `pytantan-0.1.1/vendor/tantan/src/mcf_score_matrix.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_score_matrix.hh` & `pytantan-0.1.1/vendor/tantan/src/mcf_score_matrix.hh`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_simd.hh` & `pytantan-0.1.1/vendor/tantan/src/mcf_simd.hh`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_tantan_options.cc` & `pytantan-0.1.1/vendor/tantan/src/mcf_tantan_options.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_tantan_options.hh` & `pytantan-0.1.1/vendor/tantan/src/mcf_tantan_options.hh`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_util.cc` & `pytantan-0.1.1/vendor/tantan/src/mcf_util.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_util.hh` & `pytantan-0.1.1/vendor/tantan/src/mcf_util.hh`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/mcf_zstream.hh` & `pytantan-0.1.1/vendor/tantan/src/mcf_zstream.hh`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/tantan.cc` & `pytantan-0.1.1/vendor/tantan/src/tantan.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/tantan.hh` & `pytantan-0.1.1/vendor/tantan/src/tantan.hh`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/tantan_app.cc` & `pytantan-0.1.1/vendor/tantan/src/tantan_app.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/tantan_repeat_finder.cc` & `pytantan-0.1.1/vendor/tantan/src/tantan_repeat_finder.cc`

 * *Files identical despite different names*

### Comparing `pytantan-0.1.0/vendor/tantan/src/tantan_repeat_finder.hh` & `pytantan-0.1.1/vendor/tantan/src/tantan_repeat_finder.hh`

 * *Files identical despite different names*

