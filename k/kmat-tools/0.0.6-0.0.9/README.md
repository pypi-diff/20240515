# Comparing `tmp/kmat_tools-0.0.6.tar.gz` & `tmp/kmat_tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmat_tools-0.0.6.tar", last modified: Mon May 13 11:57:56 2024, max compression
+gzip compressed data, was "kmat_tools-0.0.9.tar", last modified: Mon May 13 16:41:25 2024, max compression
```

## Comparing `kmat_tools-0.0.6.tar` & `kmat_tools-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,66 @@
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.225576 kmat_tools-0.0.6/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1075 2024-05-10 13:32:59.000000 kmat_tools-0.0.6/LICENSE
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       36 2024-04-25 14:25:41.000000 kmat_tools-0.0.6/MANIFEST.in
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1478 2024-05-13 11:57:56.225108 kmat_tools-0.0.6/PKG-INFO
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      984 2024-05-10 13:44:58.000000 kmat_tools-0.0.6/README.md
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.228228 kmat_tools-0.0.6/kmat_tools.egg-info/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1478 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/PKG-INFO
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1771 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)        1 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      338 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/entry_points.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       44 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/top_level.txt
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.161024 kmat_tools-0.0.6/kmtools_cython/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)   301593 2024-05-13 11:57:55.000000 kmat_tools-0.0.6/kmtools_cython/km_basic_filter.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      131 2024-05-02 16:15:26.000000 kmat_tools-0.0.6/kmtools_cython/km_basic_filter.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1117 2024-05-07 12:15:08.000000 kmat_tools-0.0.6/kmtools_cython/km_basic_filter.pyx
--rw-r--r--   0 cduitama (36963) seqbio   (97979)   290013 2024-05-13 11:57:55.000000 kmat_tools-0.0.6/kmtools_cython/km_fasta.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      149 2024-05-07 10:18:19.000000 kmat_tools-0.0.6/kmtools_cython/km_fasta.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1036 2024-05-07 11:08:30.000000 kmat_tools-0.0.6/kmtools_cython/km_fasta.pyx
--rw-r--r--   0 cduitama (36963) seqbio   (97979)   221907 2024-05-06 16:37:02.000000 kmat_tools-0.0.6/kmtools_cython/km_reset.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      104 2024-05-06 16:36:55.000000 kmat_tools-0.0.6/kmtools_cython/km_reset.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       68 2024-05-06 16:33:39.000000 kmat_tools-0.0.6/kmtools_cython/km_reset.pyx
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       92 2024-05-02 13:30:32.000000 kmat_tools-0.0.6/kmtools_cython/km_select.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2631 2024-04-25 14:16:14.000000 kmat_tools-0.0.6/kmtools_cython/km_select.pyx
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.178300 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2024-05-07 14:14:50.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__init__.py
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.182877 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      210 2024-05-07 14:21:11.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2521 2024-05-09 13:49:00.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1690 2024-05-09 13:49:00.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2177 2024-05-09 14:29:01.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1617 2024-05-09 13:44:33.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_basic_filter_wrapper.py
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      917 2024-05-09 13:44:24.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_fasta_wrapper.py
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1303 2024-05-09 13:48:28.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_unitig_wrapper.py
--rw-r--r--   0 cduitama (36963) seqbio   (97979)   290130 2024-05-13 11:57:55.000000 kmat_tools-0.0.6/kmtools_cython/km_unitig.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      119 2024-05-03 12:56:30.000000 kmat_tools-0.0.6/kmtools_cython/km_unitig.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1048 2024-05-09 14:35:01.000000 kmat_tools-0.0.6/kmtools_cython/km_unitig.pyx
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.080724 kmat_tools-0.0.6/kmtools_cython/lib/
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.199470 kmat_tools-0.0.6/kmtools_cython/lib/include/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     7236 2024-05-02 14:08:34.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/common.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)    21542 2024-04-15 17:11:50.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/khash.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     7269 2024-04-25 15:01:55.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/km_basic_filter.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     7255 2024-05-02 15:16:58.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/km_fasta.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       85 2024-05-06 16:23:50.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/km_reset.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     7257 2024-05-03 12:56:22.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/km_unitig.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     8633 2024-04-15 17:11:50.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/kseq.h
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.223915 kmat_tools-0.0.6/kmtools_cython/lib/src/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     4563 2024-05-07 11:48:34.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_basic_filter.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     3576 2024-04-08 14:46:29.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_diff.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2285 2024-05-09 14:31:18.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_fasta.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     4242 2024-04-08 14:46:29.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_merge.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      141 2024-05-07 11:23:29.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_reset.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2957 2024-04-08 14:46:29.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_reverse.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     3591 2024-04-25 13:02:14.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_select.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2334 2024-04-24 12:11:44.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_tools.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     6253 2024-05-07 11:49:02.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_unitig.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      117 2024-04-25 13:57:27.000000 kmat_tools-0.0.6/kmtools_cython/pyproject.toml
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      117 2024-05-13 11:00:32.000000 kmat_tools-0.0.6/pyproject.toml
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       38 2024-05-13 11:57:56.227263 kmat_tools-0.0.6/setup.cfg
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2682 2024-05-13 11:57:05.000000 kmat_tools-0.0.6/setup.py
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:25.030597 kmat_tools-0.0.9/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1075 2024-05-10 13:32:59.000000 kmat_tools-0.0.9/LICENSE
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       28 2024-05-13 15:28:25.000000 kmat_tools-0.0.9/MANIFEST.in
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1478 2024-05-13 16:41:25.030423 kmat_tools-0.0.9/PKG-INFO
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      984 2024-05-10 13:44:58.000000 kmat_tools-0.0.9/README.md
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:24.950548 kmat_tools-0.0.9/cython/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 15:13:24.000000 kmat_tools-0.0.9/cython/__init__.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)   301462 2024-05-13 16:41:24.000000 kmat_tools-0.0.9/cython/km_basic_filter.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      131 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_basic_filter.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1183 2024-05-13 15:36:59.000000 kmat_tools-0.0.9/cython/km_basic_filter.pyx
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)   289985 2024-05-13 16:41:24.000000 kmat_tools-0.0.9/cython/km_fasta.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      149 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_fasta.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1133 2024-05-13 15:37:33.000000 kmat_tools-0.0.9/cython/km_fasta.pyx
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)   221771 2024-05-13 15:13:05.000000 kmat_tools-0.0.9/cython/km_reset.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      104 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_reset.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       68 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_reset.pyx
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       92 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_select.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2631 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_select.pyx
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:24.960779 kmat_tools-0.0.9/cython/km_tools_wrappers/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_tools_wrappers/__init__.py
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:24.972177 kmat_tools-0.0.9/cython/km_tools_wrappers/__pycache__/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      210 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_tools_wrappers/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2521 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1690 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2177 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1617 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_tools_wrappers/km_basic_filter_wrapper.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      917 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_tools_wrappers/km_fasta_wrapper.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1303 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_tools_wrappers/km_unitig_wrapper.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)   290007 2024-05-13 16:41:24.000000 kmat_tools-0.0.9/cython/km_unitig.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      119 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/km_unitig.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1114 2024-05-13 15:37:46.000000 kmat_tools-0.0.9/cython/km_unitig.pyx
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:24.902608 kmat_tools-0.0.9/cython/lib/
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:24.983348 kmat_tools-0.0.9/cython/lib/include/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     7236 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/include/common.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)    21542 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/include/khash.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     7269 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/include/km_basic_filter.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     7255 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/include/km_fasta.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       85 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/include/km_reset.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     7257 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/include/km_unitig.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     8633 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/include/kseq.h
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:25.009085 kmat_tools-0.0.9/cython/lib/src/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     4563 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/src/km_basic_filter.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     3576 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/src/km_diff.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2285 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/src/km_fasta.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     4242 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/src/km_merge.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      141 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/src/km_reset.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2957 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/src/km_reverse.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     3591 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/src/km_select.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2334 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/src/km_tools.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     6253 2024-05-13 14:59:24.000000 kmat_tools-0.0.9/cython/lib/src/km_unitig.c
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:25.011888 kmat_tools-0.0.9/kmat_tools/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2024-04-25 15:08:35.000000 kmat_tools-0.0.9/kmat_tools/__init__.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)    11180 2024-05-10 13:24:37.000000 kmat_tools-0.0.9/kmat_tools/__main__.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       21 2024-05-10 13:18:13.000000 kmat_tools-0.0.9/kmat_tools/__version__.py
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:25.032511 kmat_tools-0.0.9/kmat_tools/utils/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2024-04-15 14:41:31.000000 kmat_tools-0.0.9/kmat_tools/utils/__init__.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      819 2024-04-15 16:39:50.000000 kmat_tools-0.0.9/kmat_tools/utils/utils.py
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 16:41:25.035000 kmat_tools-0.0.9/kmat_tools.egg-info/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1478 2024-05-13 16:41:24.000000 kmat_tools-0.0.9/kmat_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1583 2024-05-13 16:41:24.000000 kmat_tools-0.0.9/kmat_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        1 2024-05-13 16:41:24.000000 kmat_tools-0.0.9/kmat_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      314 2024-05-13 16:41:24.000000 kmat_tools-0.0.9/kmat_tools.egg-info/entry_points.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       62 2024-05-13 16:41:24.000000 kmat_tools-0.0.9/kmat_tools.egg-info/top_level.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      129 2024-05-13 16:00:20.000000 kmat_tools-0.0.9/pyproject.toml
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       38 2024-05-13 16:41:25.033914 kmat_tools-0.0.9/setup.cfg
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2763 2024-05-13 16:28:23.000000 kmat_tools-0.0.9/setup.py
```

### Comparing `kmat_tools-0.0.6/LICENSE` & `kmat_tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/PKG-INFO` & `kmat_tools-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmat_tools
-Version: 0.0.6
+Version: 0.0.9
 Home-page: https://github.com/CamilaDuitama/kmat_tools
 Author: Riccardo Vicedomini, Francesco Andreace, Camila Duitama
 Author-email: cduitama@pasteur.fr
 Project-URL: Bug Tracker, https://github.com/CamilaDuitama/kmat_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kmat_tools-0.0.6/README.md` & `kmat_tools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmat_tools.egg-info/PKG-INFO` & `kmat_tools-0.0.9/kmat_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmat_tools
-Version: 0.0.6
+Version: 0.0.9
 Home-page: https://github.com/CamilaDuitama/kmat_tools
 Author: Riccardo Vicedomini, Francesco Andreace, Camila Duitama
 Author-email: cduitama@pasteur.fr
 Project-URL: Bug Tracker, https://github.com/CamilaDuitama/kmat_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kmat_tools-0.0.6/kmat_tools.egg-info/SOURCES.txt` & `kmat_tools-0.0.9/kmat_tools.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+cython/__init__.py
+cython/km_basic_filter.c
+cython/km_basic_filter.pxd
+cython/km_basic_filter.pyx
+cython/km_fasta.c
+cython/km_fasta.pxd
+cython/km_fasta.pyx
+cython/km_reset.c
+cython/km_reset.pxd
+cython/km_reset.pyx
+cython/km_select.pxd
+cython/km_select.pyx
+cython/km_unitig.c
+cython/km_unitig.pxd
+cython/km_unitig.pyx
+cython/km_tools_wrappers/__init__.py
+cython/km_tools_wrappers/km_basic_filter_wrapper.py
+cython/km_tools_wrappers/km_fasta_wrapper.py
+cython/km_tools_wrappers/km_unitig_wrapper.py
+cython/km_tools_wrappers/__pycache__/__init__.cpython-312.pyc
+cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc
+cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc
+cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc
+cython/lib/include/common.h
+cython/lib/include/khash.h
+cython/lib/include/km_basic_filter.h
+cython/lib/include/km_fasta.h
+cython/lib/include/km_reset.h
+cython/lib/include/km_unitig.h
+cython/lib/include/kseq.h
+cython/lib/src/km_basic_filter.c
+cython/lib/src/km_diff.c
+cython/lib/src/km_fasta.c
+cython/lib/src/km_merge.c
+cython/lib/src/km_reset.c
+cython/lib/src/km_reverse.c
+cython/lib/src/km_select.c
+cython/lib/src/km_tools.c
+cython/lib/src/km_unitig.c
+kmat_tools/__init__.py
+kmat_tools/__main__.py
+kmat_tools/__version__.py
 kmat_tools.egg-info/PKG-INFO
 kmat_tools.egg-info/SOURCES.txt
 kmat_tools.egg-info/dependency_links.txt
 kmat_tools.egg-info/entry_points.txt
 kmat_tools.egg-info/top_level.txt
-kmtools_cython/km_basic_filter.c
-kmtools_cython/km_basic_filter.pxd
-kmtools_cython/km_basic_filter.pyx
-kmtools_cython/km_fasta.c
-kmtools_cython/km_fasta.pxd
-kmtools_cython/km_fasta.pyx
-kmtools_cython/km_reset.c
-kmtools_cython/km_reset.pxd
-kmtools_cython/km_reset.pyx
-kmtools_cython/km_select.pxd
-kmtools_cython/km_select.pyx
-kmtools_cython/km_unitig.c
-kmtools_cython/km_unitig.pxd
-kmtools_cython/km_unitig.pyx
-kmtools_cython/pyproject.toml
-kmtools_cython/km_tools_wrappers/__init__.py
-kmtools_cython/km_tools_wrappers/km_basic_filter_wrapper.py
-kmtools_cython/km_tools_wrappers/km_fasta_wrapper.py
-kmtools_cython/km_tools_wrappers/km_unitig_wrapper.py
-kmtools_cython/km_tools_wrappers/__pycache__/__init__.cpython-312.pyc
-kmtools_cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc
-kmtools_cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc
-kmtools_cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc
-kmtools_cython/lib/include/common.h
-kmtools_cython/lib/include/khash.h
-kmtools_cython/lib/include/km_basic_filter.h
-kmtools_cython/lib/include/km_fasta.h
-kmtools_cython/lib/include/km_reset.h
-kmtools_cython/lib/include/km_unitig.h
-kmtools_cython/lib/include/kseq.h
-kmtools_cython/lib/src/km_basic_filter.c
-kmtools_cython/lib/src/km_diff.c
-kmtools_cython/lib/src/km_fasta.c
-kmtools_cython/lib/src/km_merge.c
-kmtools_cython/lib/src/km_reset.c
-kmtools_cython/lib/src/km_reverse.c
-kmtools_cython/lib/src/km_select.c
-kmtools_cython/lib/src/km_tools.c
-kmtools_cython/lib/src/km_unitig.c
+kmat_tools/utils/__init__.py
+kmat_tools/utils/utils.py
```

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_basic_filter.c` & `kmat_tools-0.0.9/cython/km_basic_filter.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "kmtools_cython/lib/include/km_basic_filter.h"
+            "cython/lib/include/km_basic_filter.h"
         ],
         "extra_compile_args": [
             "-Wall",
             "-Wno-unused-function",
             "-O3",
             "-pedantic"
         ],
         "include_dirs": [
-            "kmtools_cython",
-            "kmtools_cython/lib/include"
+            "cython",
+            "cython/lib/include"
         ],
         "libraries": [
             "z",
             "m"
         ],
         "name": "km_basic_filter",
         "sources": [
-            "kmtools_cython/km_basic_filter.pyx",
-            "kmtools_cython/lib/src/km_basic_filter.c"
+            "cython/km_basic_filter.pyx",
+            "cython/lib/src/km_basic_filter.c"
         ]
     },
     "module_name": "km_basic_filter"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -1245,17 +1245,17 @@
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
 #define __PYX_HAVE__km_basic_filter
 #define __PYX_HAVE_API__km_basic_filter
 /* Early includes */
-#include "lib/include/km_basic_filter.h"
 #include <string.h>
 #include <stdlib.h>
+#include "lib/include/km_basic_filter.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -1496,15 +1496,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "kmtools_cython/km_basic_filter.pyx",
+  "cython/km_basic_filter.pyx",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -2167,16 +2167,16 @@
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_km_basic_filter[] = "km_basic_filter";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_py_main_basic_filter[] = "py_main_basic_filter";
 static const char __pyx_k_Failed_to_allocate_memory[] = "Failed to allocate memory";
 static const char __pyx_k_Invalid_argument_at_index[] = "Invalid argument at index {}";
+static const char __pyx_k_cython_km_basic_filter_pyx[] = "cython/km_basic_filter.pyx";
 static const char __pyx_k_Failed_to_allocate_memory_for_ar[] = "Failed to allocate memory for argument {}";
-static const char __pyx_k_kmtools_cython_km_basic_filter_p[] = "kmtools_cython/km_basic_filter.pyx";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_15km_basic_filter_py_main_basic_filter(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_argv); /* proto */
 static PyObject *__pyx_pf_15km_basic_filter_2cython_main(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_argv); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
@@ -2205,38 +2205,38 @@
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
-  PyObject *__pyx_kp_u_Failed_to_allocate_memory;
-  PyObject *__pyx_kp_u_Failed_to_allocate_memory_for_ar;
-  PyObject *__pyx_kp_u_Invalid_argument_at_index;
+  PyObject *__pyx_kp_s_Failed_to_allocate_memory;
+  PyObject *__pyx_kp_s_Failed_to_allocate_memory_for_ar;
+  PyObject *__pyx_kp_s_Invalid_argument_at_index;
   PyObject *__pyx_n_s_MemoryError;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s__6;
   PyObject *__pyx_n_s_argc;
   PyObject *__pyx_n_s_argv;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_c_argv;
   PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_kp_s_cython_km_basic_filter_pyx;
   PyObject *__pyx_n_s_cython_main;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_format;
   PyObject *__pyx_n_s_i;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_n_s_km_basic_filter;
-  PyObject *__pyx_kp_s_kmtools_cython_km_basic_filter_p;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_py_main_basic_filter;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_test;
-  PyObject *__pyx_kp_u_utf_8;
+  PyObject *__pyx_kp_s_utf_8;
   PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_codeobj__3;
   PyObject *__pyx_codeobj__5;
 } __pyx_mstate;
 
@@ -2276,38 +2276,38 @@
   Py_CLEAR(clear_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Failed_to_allocate_memory);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Failed_to_allocate_memory_for_ar);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_argument_at_index);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Failed_to_allocate_memory);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Failed_to_allocate_memory_for_ar);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Invalid_argument_at_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s__6);
   Py_CLEAR(clear_module_state->__pyx_n_s_argc);
   Py_CLEAR(clear_module_state->__pyx_n_s_argv);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_c_argv);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_cython_km_basic_filter_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_cython_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_format);
   Py_CLEAR(clear_module_state->__pyx_n_s_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_n_s_km_basic_filter);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_kmtools_cython_km_basic_filter_p);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_py_main_basic_filter);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_utf_8);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_codeobj__3);
   Py_CLEAR(clear_module_state->__pyx_codeobj__5);
   return 0;
 }
@@ -2325,38 +2325,38 @@
   Py_VISIT(traverse_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Failed_to_allocate_memory);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Failed_to_allocate_memory_for_ar);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_argument_at_index);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Failed_to_allocate_memory);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Failed_to_allocate_memory_for_ar);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Invalid_argument_at_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s__6);
   Py_VISIT(traverse_module_state->__pyx_n_s_argc);
   Py_VISIT(traverse_module_state->__pyx_n_s_argv);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_c_argv);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_cython_km_basic_filter_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_cython_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_format);
   Py_VISIT(traverse_module_state->__pyx_n_s_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_n_s_km_basic_filter);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_kmtools_cython_km_basic_filter_p);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_py_main_basic_filter);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_utf_8);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_codeobj__3);
   Py_VISIT(traverse_module_state->__pyx_codeobj__5);
   return 0;
 }
@@ -2388,47 +2388,47 @@
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
-#define __pyx_kp_u_Failed_to_allocate_memory __pyx_mstate_global->__pyx_kp_u_Failed_to_allocate_memory
-#define __pyx_kp_u_Failed_to_allocate_memory_for_ar __pyx_mstate_global->__pyx_kp_u_Failed_to_allocate_memory_for_ar
-#define __pyx_kp_u_Invalid_argument_at_index __pyx_mstate_global->__pyx_kp_u_Invalid_argument_at_index
+#define __pyx_kp_s_Failed_to_allocate_memory __pyx_mstate_global->__pyx_kp_s_Failed_to_allocate_memory
+#define __pyx_kp_s_Failed_to_allocate_memory_for_ar __pyx_mstate_global->__pyx_kp_s_Failed_to_allocate_memory_for_ar
+#define __pyx_kp_s_Invalid_argument_at_index __pyx_mstate_global->__pyx_kp_s_Invalid_argument_at_index
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
 #define __pyx_n_s_argc __pyx_mstate_global->__pyx_n_s_argc
 #define __pyx_n_s_argv __pyx_mstate_global->__pyx_n_s_argv
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_c_argv __pyx_mstate_global->__pyx_n_s_c_argv
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_kp_s_cython_km_basic_filter_pyx __pyx_mstate_global->__pyx_kp_s_cython_km_basic_filter_pyx
 #define __pyx_n_s_cython_main __pyx_mstate_global->__pyx_n_s_cython_main
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
 #define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_n_s_km_basic_filter __pyx_mstate_global->__pyx_n_s_km_basic_filter
-#define __pyx_kp_s_kmtools_cython_km_basic_filter_p __pyx_mstate_global->__pyx_kp_s_kmtools_cython_km_basic_filter_p
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_py_main_basic_filter __pyx_mstate_global->__pyx_n_s_py_main_basic_filter
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
-#define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
+#define __pyx_kp_s_utf_8 __pyx_mstate_global->__pyx_kp_s_utf_8
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_codeobj__3 __pyx_mstate_global->__pyx_codeobj__3
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
 /* #### Code section: module_code ### */
 
-/* "km_basic_filter.pyx":5
- * from libc.string cimport strdup
+/* "km_basic_filter.pyx":7
+ *     int main_basic_filter(int argc, char **argv) nogil
  * 
  * def py_main_basic_filter(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
 
 /* Python wrapper */
@@ -2480,45 +2480,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_argv)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 5, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 7, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "py_main_basic_filter") < 0)) __PYX_ERR(0, 5, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "py_main_basic_filter") < 0)) __PYX_ERR(0, 7, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_argv = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("py_main_basic_filter", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 5, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("py_main_basic_filter", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 7, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("km_basic_filter.py_main_basic_filter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_argv), (&PyList_Type), 1, "argv", 1))) __PYX_ERR(0, 5, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_argv), (&PyList_Type), 1, "argv", 1))) __PYX_ERR(0, 7, __pyx_L1_error)
   __pyx_r = __pyx_pf_15km_basic_filter_py_main_basic_filter(__pyx_self, __pyx_v_argv);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2558,147 +2558,147 @@
   PyObject *__pyx_t_18 = NULL;
   int __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("py_main_basic_filter", 1);
 
-  /* "km_basic_filter.pyx":6
+  /* "km_basic_filter.pyx":8
  * 
  * def py_main_basic_filter(list argv):
  *     cdef int argc = len(argv)             # <<<<<<<<<<<<<<
  * 
  *     if argc == 0:
  */
   if (unlikely(__pyx_v_argv == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 6, __pyx_L1_error)
+    __PYX_ERR(0, 8, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_argv); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_argv); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 8, __pyx_L1_error)
   __pyx_v_argc = __pyx_t_1;
 
-  /* "km_basic_filter.pyx":8
+  /* "km_basic_filter.pyx":10
  *     cdef int argc = len(argv)
  * 
  *     if argc == 0:             # <<<<<<<<<<<<<<
  *         # Handle empty argv gracefully
  *         return
  */
   __pyx_t_2 = (__pyx_v_argc == 0);
   if (__pyx_t_2) {
 
-    /* "km_basic_filter.pyx":10
+    /* "km_basic_filter.pyx":12
  *     if argc == 0:
  *         # Handle empty argv gracefully
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "km_basic_filter.pyx":8
+    /* "km_basic_filter.pyx":10
  *     cdef int argc = len(argv)
  * 
  *     if argc == 0:             # <<<<<<<<<<<<<<
  *         # Handle empty argv gracefully
  *         return
  */
   }
 
-  /* "km_basic_filter.pyx":12
+  /* "km_basic_filter.pyx":14
  *         return
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))             # <<<<<<<<<<<<<<
  *     if c_argv is NULL:
  *         # Handle allocation failure
  */
   __pyx_v_c_argv = ((char **)malloc(((__pyx_v_argc + 1) * (sizeof(char *)))));
 
-  /* "km_basic_filter.pyx":13
+  /* "km_basic_filter.pyx":15
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))
  *     if c_argv is NULL:             # <<<<<<<<<<<<<<
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")
  */
   __pyx_t_2 = (__pyx_v_c_argv == NULL);
   if (unlikely(__pyx_t_2)) {
 
-    /* "km_basic_filter.pyx":15
+    /* "km_basic_filter.pyx":17
  *     if c_argv is NULL:
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 15, __pyx_L1_error)
+    __PYX_ERR(0, 17, __pyx_L1_error)
 
-    /* "km_basic_filter.pyx":13
+    /* "km_basic_filter.pyx":15
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))
  *     if c_argv is NULL:             # <<<<<<<<<<<<<<
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")
  */
   }
 
-  /* "km_basic_filter.pyx":17
+  /* "km_basic_filter.pyx":19
  *         raise MemoryError("Failed to allocate memory")
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         for i in range(argc):
  *             if argv[i] is None:
  */
   /*try:*/ {
 
-    /* "km_basic_filter.pyx":18
+    /* "km_basic_filter.pyx":20
  * 
  *     try:
  *         for i in range(argc):             # <<<<<<<<<<<<<<
  *             if argv[i] is None:
  *                 # Handle invalid argument
  */
     __pyx_t_4 = __pyx_v_argc;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "km_basic_filter.pyx":19
+      /* "km_basic_filter.pyx":21
  *     try:
  *         for i in range(argc):
  *             if argv[i] is None:             # <<<<<<<<<<<<<<
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))
  */
       if (unlikely(__pyx_v_argv == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 19, __pyx_L6_error)
+        __PYX_ERR(0, 21, __pyx_L6_error)
       }
-      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L6_error)
+      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_2 = (__pyx_t_3 == Py_None);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (unlikely(__pyx_t_2)) {
 
-        /* "km_basic_filter.pyx":21
+        /* "km_basic_filter.pyx":23
  *             if argv[i] is None:
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))             # <<<<<<<<<<<<<<
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))
  *             if c_argv[i] is NULL:
  */
-        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Invalid_argument_at_index, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 21, __pyx_L6_error)
+        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Invalid_argument_at_index, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 23, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 21, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 23, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_9 = NULL;
         __pyx_t_10 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_7))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
           if (likely(__pyx_t_9)) {
@@ -2711,48 +2711,48 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_8};
           __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L6_error)
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
-        __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 21, __pyx_L6_error)
+        __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 23, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_7, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __PYX_ERR(0, 21, __pyx_L6_error)
+        __PYX_ERR(0, 23, __pyx_L6_error)
 
-        /* "km_basic_filter.pyx":19
+        /* "km_basic_filter.pyx":21
  *     try:
  *         for i in range(argc):
  *             if argv[i] is None:             # <<<<<<<<<<<<<<
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))
  */
       }
 
-      /* "km_basic_filter.pyx":22
+      /* "km_basic_filter.pyx":24
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))             # <<<<<<<<<<<<<<
  *             if c_argv[i] is NULL:
  *                 # Handle strdup failure
  */
       if (unlikely(__pyx_v_argv == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 22, __pyx_L6_error)
+        __PYX_ERR(0, 24, __pyx_L6_error)
       }
-      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L6_error)
+      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 22, __pyx_L6_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 24, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
@@ -2762,45 +2762,45 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
           __pyx_t_10 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_utf_8};
+        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_s_utf_8};
         __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 22, __pyx_L6_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 24, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
-      __pyx_t_11 = __Pyx_PyObject_AsString(__pyx_t_7); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 22, __pyx_L6_error)
+      __pyx_t_11 = __Pyx_PyObject_AsString(__pyx_t_7); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L6_error)
       (__pyx_v_c_argv[__pyx_v_i]) = strdup(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "km_basic_filter.pyx":23
+      /* "km_basic_filter.pyx":25
  *                 raise ValueError("Invalid argument at index {}".format(i))
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))
  *             if c_argv[i] is NULL:             # <<<<<<<<<<<<<<
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  */
       __pyx_t_2 = ((__pyx_v_c_argv[__pyx_v_i]) == NULL);
       if (unlikely(__pyx_t_2)) {
 
-        /* "km_basic_filter.pyx":25
+        /* "km_basic_filter.pyx":27
  *             if c_argv[i] is NULL:
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))             # <<<<<<<<<<<<<<
  *         c_argv[argc] = NULL
- *         return km_basic_filter.main_basic_filter(argc, c_argv)
+ *         return main_basic_filter(argc, c_argv)
  */
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Failed_to_allocate_memory_for_ar, __pyx_n_s_format); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 25, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Failed_to_allocate_memory_for_ar, __pyx_n_s_format); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 27, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L6_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_9 = NULL;
         __pyx_t_10 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
           if (likely(__pyx_t_9)) {
@@ -2813,61 +2813,61 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_3};
           __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 25, __pyx_L6_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 27, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
-        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_MemoryError, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 25, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_MemoryError, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 27, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_8, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __PYX_ERR(0, 25, __pyx_L6_error)
+        __PYX_ERR(0, 27, __pyx_L6_error)
 
-        /* "km_basic_filter.pyx":23
+        /* "km_basic_filter.pyx":25
  *                 raise ValueError("Invalid argument at index {}".format(i))
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))
  *             if c_argv[i] is NULL:             # <<<<<<<<<<<<<<
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  */
       }
     }
 
-    /* "km_basic_filter.pyx":26
+    /* "km_basic_filter.pyx":28
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  *         c_argv[argc] = NULL             # <<<<<<<<<<<<<<
- *         return km_basic_filter.main_basic_filter(argc, c_argv)
+ *         return main_basic_filter(argc, c_argv)
  *     finally:
  */
     (__pyx_v_c_argv[__pyx_v_argc]) = NULL;
 
-    /* "km_basic_filter.pyx":27
+    /* "km_basic_filter.pyx":29
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  *         c_argv[argc] = NULL
- *         return km_basic_filter.main_basic_filter(argc, c_argv)             # <<<<<<<<<<<<<<
+ *         return main_basic_filter(argc, c_argv)             # <<<<<<<<<<<<<<
  *     finally:
  *         for i in range(argc):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_8 = __Pyx_PyInt_From_int(main_basic_filter(__pyx_v_argc, __pyx_v_c_argv)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 27, __pyx_L6_error)
+    __pyx_t_8 = __Pyx_PyInt_From_int(main_basic_filter(__pyx_v_argc, __pyx_v_c_argv)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 29, __pyx_L6_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L5_return;
   }
 
-  /* "km_basic_filter.pyx":29
- *         return km_basic_filter.main_basic_filter(argc, c_argv)
+  /* "km_basic_filter.pyx":31
+ *         return main_basic_filter(argc, c_argv)
  *     finally:
  *         for i in range(argc):             # <<<<<<<<<<<<<<
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  */
   /*finally:*/ {
     __pyx_L6_error:;
@@ -2890,44 +2890,44 @@
       __pyx_t_4 = __pyx_lineno; __pyx_t_5 = __pyx_clineno; __pyx_t_12 = __pyx_filename;
       {
         __pyx_t_6 = __pyx_v_argc;
         __pyx_t_10 = __pyx_t_6;
         for (__pyx_t_19 = 0; __pyx_t_19 < __pyx_t_10; __pyx_t_19+=1) {
           __pyx_v_i = __pyx_t_19;
 
-          /* "km_basic_filter.pyx":30
+          /* "km_basic_filter.pyx":32
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
           __pyx_t_2 = ((__pyx_v_c_argv[__pyx_v_i]) != NULL);
           if (__pyx_t_2) {
 
-            /* "km_basic_filter.pyx":31
+            /* "km_basic_filter.pyx":33
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])             # <<<<<<<<<<<<<<
  *         free(c_argv)
  * 
  */
             free((__pyx_v_c_argv[__pyx_v_i]));
 
-            /* "km_basic_filter.pyx":30
+            /* "km_basic_filter.pyx":32
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
           }
         }
 
-        /* "km_basic_filter.pyx":32
+        /* "km_basic_filter.pyx":34
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  *         free(c_argv)             # <<<<<<<<<<<<<<
  * 
  * def cython_main(argv):
  */
         free(__pyx_v_c_argv);
@@ -2946,71 +2946,71 @@
       __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_5; __pyx_filename = __pyx_t_12;
       goto __pyx_L1_error;
     }
     __pyx_L5_return: {
       __pyx_t_18 = __pyx_r;
       __pyx_r = 0;
 
-      /* "km_basic_filter.pyx":29
- *         return km_basic_filter.main_basic_filter(argc, c_argv)
+      /* "km_basic_filter.pyx":31
+ *         return main_basic_filter(argc, c_argv)
  *     finally:
  *         for i in range(argc):             # <<<<<<<<<<<<<<
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  */
       __pyx_t_5 = __pyx_v_argc;
       __pyx_t_4 = __pyx_t_5;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_4; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "km_basic_filter.pyx":30
+        /* "km_basic_filter.pyx":32
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
         __pyx_t_2 = ((__pyx_v_c_argv[__pyx_v_i]) != NULL);
         if (__pyx_t_2) {
 
-          /* "km_basic_filter.pyx":31
+          /* "km_basic_filter.pyx":33
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])             # <<<<<<<<<<<<<<
  *         free(c_argv)
  * 
  */
           free((__pyx_v_c_argv[__pyx_v_i]));
 
-          /* "km_basic_filter.pyx":30
+          /* "km_basic_filter.pyx":32
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
         }
       }
 
-      /* "km_basic_filter.pyx":32
+      /* "km_basic_filter.pyx":34
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  *         free(c_argv)             # <<<<<<<<<<<<<<
  * 
  * def cython_main(argv):
  */
       free(__pyx_v_c_argv);
       __pyx_r = __pyx_t_18;
       __pyx_t_18 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "km_basic_filter.pyx":5
- * from libc.string cimport strdup
+  /* "km_basic_filter.pyx":7
+ *     int main_basic_filter(int argc, char **argv) nogil
  * 
  * def py_main_basic_filter(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
 
   /* function exit code */
@@ -3023,15 +3023,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "km_basic_filter.pyx":34
+/* "km_basic_filter.pyx":36
  *         free(c_argv)
  * 
  * def cython_main(argv):             # <<<<<<<<<<<<<<
  *     py_main_basic_filter(argv)
  */
 
 /* Python wrapper */
@@ -3083,31 +3083,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_argv)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "cython_main") < 0)) __PYX_ERR(0, 34, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "cython_main") < 0)) __PYX_ERR(0, 36, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_argv = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("cython_main", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 34, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("cython_main", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 36, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -3138,20 +3138,20 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cython_main", 1);
 
-  /* "km_basic_filter.pyx":35
+  /* "km_basic_filter.pyx":37
  * 
  * def cython_main(argv):
  *     py_main_basic_filter(argv)             # <<<<<<<<<<<<<<
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_py_main_basic_filter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_py_main_basic_filter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -3163,21 +3163,21 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_argv};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "km_basic_filter.pyx":34
+  /* "km_basic_filter.pyx":36
  *         free(c_argv)
  * 
  * def cython_main(argv):             # <<<<<<<<<<<<<<
  *     py_main_basic_filter(argv)
  */
 
   /* function exit code */
@@ -3207,90 +3207,90 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
-    {&__pyx_kp_u_Failed_to_allocate_memory, __pyx_k_Failed_to_allocate_memory, sizeof(__pyx_k_Failed_to_allocate_memory), 0, 1, 0, 0},
-    {&__pyx_kp_u_Failed_to_allocate_memory_for_ar, __pyx_k_Failed_to_allocate_memory_for_ar, sizeof(__pyx_k_Failed_to_allocate_memory_for_ar), 0, 1, 0, 0},
-    {&__pyx_kp_u_Invalid_argument_at_index, __pyx_k_Invalid_argument_at_index, sizeof(__pyx_k_Invalid_argument_at_index), 0, 1, 0, 0},
+    {&__pyx_kp_s_Failed_to_allocate_memory, __pyx_k_Failed_to_allocate_memory, sizeof(__pyx_k_Failed_to_allocate_memory), 0, 0, 1, 0},
+    {&__pyx_kp_s_Failed_to_allocate_memory_for_ar, __pyx_k_Failed_to_allocate_memory_for_ar, sizeof(__pyx_k_Failed_to_allocate_memory_for_ar), 0, 0, 1, 0},
+    {&__pyx_kp_s_Invalid_argument_at_index, __pyx_k_Invalid_argument_at_index, sizeof(__pyx_k_Invalid_argument_at_index), 0, 0, 1, 0},
     {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
     {&__pyx_n_s_argc, __pyx_k_argc, sizeof(__pyx_k_argc), 0, 0, 1, 1},
     {&__pyx_n_s_argv, __pyx_k_argv, sizeof(__pyx_k_argv), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_c_argv, __pyx_k_c_argv, sizeof(__pyx_k_c_argv), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_kp_s_cython_km_basic_filter_pyx, __pyx_k_cython_km_basic_filter_pyx, sizeof(__pyx_k_cython_km_basic_filter_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_cython_main, __pyx_k_cython_main, sizeof(__pyx_k_cython_main), 0, 0, 1, 1},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
     {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_n_s_km_basic_filter, __pyx_k_km_basic_filter, sizeof(__pyx_k_km_basic_filter), 0, 0, 1, 1},
-    {&__pyx_kp_s_kmtools_cython_km_basic_filter_p, __pyx_k_kmtools_cython_km_basic_filter_p, sizeof(__pyx_k_kmtools_cython_km_basic_filter_p), 0, 0, 1, 0},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_py_main_basic_filter, __pyx_k_py_main_basic_filter, sizeof(__pyx_k_py_main_basic_filter), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-    {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
+    {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 15, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 18, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 23, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "km_basic_filter.pyx":15
+  /* "km_basic_filter.pyx":17
  *     if c_argv is NULL:
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Failed_to_allocate_memory); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Failed_to_allocate_memory); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "km_basic_filter.pyx":5
- * from libc.string cimport strdup
+  /* "km_basic_filter.pyx":7
+ *     int main_basic_filter(int argc, char **argv) nogil
  * 
  * def py_main_basic_filter(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(4, __pyx_n_s_argv, __pyx_n_s_argc, __pyx_n_s_c_argv, __pyx_n_s_i); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(4, __pyx_n_s_argv, __pyx_n_s_argc, __pyx_n_s_c_argv, __pyx_n_s_i); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmtools_cython_km_basic_filter_p, __pyx_n_s_py_main_basic_filter, 5, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cython_km_basic_filter_pyx, __pyx_n_s_py_main_basic_filter, 7, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 7, __pyx_L1_error)
 
-  /* "km_basic_filter.pyx":34
+  /* "km_basic_filter.pyx":36
  *         free(c_argv)
  * 
  * def cython_main(argv):             # <<<<<<<<<<<<<<
  *     py_main_basic_filter(argv)
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_argv); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_argv); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmtools_cython_km_basic_filter_p, __pyx_n_s_cython_main, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cython_km_basic_filter_pyx, __pyx_n_s_cython_main, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -3646,41 +3646,41 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "km_basic_filter.pyx":5
- * from libc.string cimport strdup
+  /* "km_basic_filter.pyx":7
+ *     int main_basic_filter(int argc, char **argv) nogil
  * 
  * def py_main_basic_filter(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_15km_basic_filter_1py_main_basic_filter, 0, __pyx_n_s_py_main_basic_filter, NULL, __pyx_n_s_km_basic_filter, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_15km_basic_filter_1py_main_basic_filter, 0, __pyx_n_s_py_main_basic_filter, NULL, __pyx_n_s_km_basic_filter, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_main_basic_filter, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_main_basic_filter, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "km_basic_filter.pyx":34
+  /* "km_basic_filter.pyx":36
  *         free(c_argv)
  * 
  * def cython_main(argv):             # <<<<<<<<<<<<<<
  *     py_main_basic_filter(argv)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_15km_basic_filter_3cython_main, 0, __pyx_n_s_cython_main, NULL, __pyx_n_s_km_basic_filter, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_15km_basic_filter_3cython_main, 0, __pyx_n_s_cython_main, NULL, __pyx_n_s_km_basic_filter, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cython_main, __pyx_t_2) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cython_main, __pyx_t_2) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "km_basic_filter.pyx":1
- * cimport km_basic_filter             # <<<<<<<<<<<<<<
- * from libc.stdlib cimport malloc, free
+ * from libc.stdlib cimport malloc, free             # <<<<<<<<<<<<<<
  * from libc.string cimport strdup
+ * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
```

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_basic_filter.pyx` & `kmat_tools-0.0.9/cython/km_basic_filter.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-cimport km_basic_filter
 from libc.stdlib cimport malloc, free
 from libc.string cimport strdup
 
+cdef extern from "lib/include/km_basic_filter.h":
+    int main_basic_filter(int argc, char **argv) nogil
+
 def py_main_basic_filter(list argv):
     cdef int argc = len(argv)
     
     if argc == 0:
         # Handle empty argv gracefully
         return
     
@@ -20,15 +22,15 @@
                 # Handle invalid argument
                 raise ValueError("Invalid argument at index {}".format(i))
             c_argv[i] = strdup(argv[i].encode('utf-8'))
             if c_argv[i] is NULL:
                 # Handle strdup failure
                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
         c_argv[argc] = NULL
-        return km_basic_filter.main_basic_filter(argc, c_argv)
+        return main_basic_filter(argc, c_argv)
     finally:
         for i in range(argc):
             if c_argv[i] is not NULL:
                 free(c_argv[i])
         free(c_argv)
 
 def cython_main(argv):
```

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_fasta.c` & `kmat_tools-0.0.9/cython/km_fasta.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "kmtools_cython/lib/include/km_fasta.h"
+            "cython/lib/include/km_fasta.h"
         ],
         "extra_compile_args": [
             "-Wall",
             "-Wno-unused-function",
             "-O3",
             "-pedantic"
         ],
         "include_dirs": [
-            "kmtools_cython",
-            "kmtools_cython/lib/include"
+            "cython",
+            "cython/lib/include"
         ],
         "libraries": [
             "z",
             "m"
         ],
         "name": "km_fasta",
         "sources": [
-            "kmtools_cython/km_fasta.pyx",
-            "kmtools_cython/lib/src/km_fasta.c"
+            "cython/km_fasta.pyx",
+            "cython/lib/src/km_fasta.c"
         ]
     },
     "module_name": "km_fasta"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -1245,17 +1245,17 @@
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
 #define __PYX_HAVE__km_fasta
 #define __PYX_HAVE_API__km_fasta
 /* Early includes */
-#include "lib/include/km_fasta.h"
 #include <string.h>
 #include <stdlib.h>
+#include "lib/include/km_fasta.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -1496,15 +1496,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "kmtools_cython/km_fasta.pyx",
+  "cython/km_fasta.pyx",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -2143,17 +2143,17 @@
 static const char __pyx_k_km_fasta[] = "km_fasta";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_py_main_fasta[] = "py_main_fasta";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_cython_km_fasta_pyx[] = "cython/km_fasta.pyx";
 static const char __pyx_k_Failed_to_allocate_memory[] = "Failed to allocate memory";
 static const char __pyx_k_Invalid_argument_at_index[] = "Invalid argument at index {}";
-static const char __pyx_k_kmtools_cython_km_fasta_pyx[] = "kmtools_cython/km_fasta.pyx";
 static const char __pyx_k_Failed_to_allocate_memory_for_ar[] = "Failed to allocate memory for argument {}";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8km_fasta_py_main_fasta(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_argv); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
@@ -2182,37 +2182,37 @@
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
-  PyObject *__pyx_kp_u_Failed_to_allocate_memory;
-  PyObject *__pyx_kp_u_Failed_to_allocate_memory_for_ar;
-  PyObject *__pyx_kp_u_Invalid_argument_at_index;
+  PyObject *__pyx_kp_s_Failed_to_allocate_memory;
+  PyObject *__pyx_kp_s_Failed_to_allocate_memory_for_ar;
+  PyObject *__pyx_kp_s_Invalid_argument_at_index;
   PyObject *__pyx_n_s_MemoryError;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s__4;
   PyObject *__pyx_n_s_argc;
   PyObject *__pyx_n_s_argv;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_c_argv;
   PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_kp_s_cython_km_fasta_pyx;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_format;
   PyObject *__pyx_n_s_i;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_n_s_km_fasta;
-  PyObject *__pyx_kp_s_kmtools_cython_km_fasta_pyx;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_py_main_fasta;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_test;
-  PyObject *__pyx_kp_u_utf_8;
+  PyObject *__pyx_kp_s_utf_8;
   PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_codeobj__3;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
@@ -2250,37 +2250,37 @@
   Py_CLEAR(clear_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Failed_to_allocate_memory);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Failed_to_allocate_memory_for_ar);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_argument_at_index);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Failed_to_allocate_memory);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Failed_to_allocate_memory_for_ar);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Invalid_argument_at_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s__4);
   Py_CLEAR(clear_module_state->__pyx_n_s_argc);
   Py_CLEAR(clear_module_state->__pyx_n_s_argv);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_c_argv);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_cython_km_fasta_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_format);
   Py_CLEAR(clear_module_state->__pyx_n_s_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_n_s_km_fasta);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_kmtools_cython_km_fasta_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_py_main_fasta);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_utf_8);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_codeobj__3);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
@@ -2296,37 +2296,37 @@
   Py_VISIT(traverse_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Failed_to_allocate_memory);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Failed_to_allocate_memory_for_ar);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_argument_at_index);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Failed_to_allocate_memory);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Failed_to_allocate_memory_for_ar);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Invalid_argument_at_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s__4);
   Py_VISIT(traverse_module_state->__pyx_n_s_argc);
   Py_VISIT(traverse_module_state->__pyx_n_s_argv);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_c_argv);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_cython_km_fasta_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_format);
   Py_VISIT(traverse_module_state->__pyx_n_s_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_n_s_km_fasta);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_kmtools_cython_km_fasta_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_py_main_fasta);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_utf_8);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_codeobj__3);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
@@ -2356,44 +2356,44 @@
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
-#define __pyx_kp_u_Failed_to_allocate_memory __pyx_mstate_global->__pyx_kp_u_Failed_to_allocate_memory
-#define __pyx_kp_u_Failed_to_allocate_memory_for_ar __pyx_mstate_global->__pyx_kp_u_Failed_to_allocate_memory_for_ar
-#define __pyx_kp_u_Invalid_argument_at_index __pyx_mstate_global->__pyx_kp_u_Invalid_argument_at_index
+#define __pyx_kp_s_Failed_to_allocate_memory __pyx_mstate_global->__pyx_kp_s_Failed_to_allocate_memory
+#define __pyx_kp_s_Failed_to_allocate_memory_for_ar __pyx_mstate_global->__pyx_kp_s_Failed_to_allocate_memory_for_ar
+#define __pyx_kp_s_Invalid_argument_at_index __pyx_mstate_global->__pyx_kp_s_Invalid_argument_at_index
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s__4 __pyx_mstate_global->__pyx_n_s__4
 #define __pyx_n_s_argc __pyx_mstate_global->__pyx_n_s_argc
 #define __pyx_n_s_argv __pyx_mstate_global->__pyx_n_s_argv
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_c_argv __pyx_mstate_global->__pyx_n_s_c_argv
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_kp_s_cython_km_fasta_pyx __pyx_mstate_global->__pyx_kp_s_cython_km_fasta_pyx
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
 #define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_n_s_km_fasta __pyx_mstate_global->__pyx_n_s_km_fasta
-#define __pyx_kp_s_kmtools_cython_km_fasta_pyx __pyx_mstate_global->__pyx_kp_s_kmtools_cython_km_fasta_pyx
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_py_main_fasta __pyx_mstate_global->__pyx_n_s_py_main_fasta
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
-#define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
+#define __pyx_kp_s_utf_8 __pyx_mstate_global->__pyx_kp_s_utf_8
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_codeobj__3 __pyx_mstate_global->__pyx_codeobj__3
 /* #### Code section: module_code ### */
 
-/* "km_fasta.pyx":6
- * 
+/* "km_fasta.pyx":9
+ *     int main_fasta(int argc, char **argv)
  * 
  * def py_main_fasta(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
 
 /* Python wrapper */
@@ -2445,45 +2445,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_argv)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 6, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 9, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "py_main_fasta") < 0)) __PYX_ERR(0, 6, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "py_main_fasta") < 0)) __PYX_ERR(0, 9, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_argv = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("py_main_fasta", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 6, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("py_main_fasta", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 9, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("km_fasta.py_main_fasta", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_argv), (&PyList_Type), 1, "argv", 1))) __PYX_ERR(0, 6, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_argv), (&PyList_Type), 1, "argv", 1))) __PYX_ERR(0, 9, __pyx_L1_error)
   __pyx_r = __pyx_pf_8km_fasta_py_main_fasta(__pyx_self, __pyx_v_argv);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2523,147 +2523,147 @@
   PyObject *__pyx_t_18 = NULL;
   int __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("py_main_fasta", 1);
 
-  /* "km_fasta.pyx":7
+  /* "km_fasta.pyx":10
  * 
  * def py_main_fasta(list argv):
  *     cdef int argc = len(argv)             # <<<<<<<<<<<<<<
  * 
  *     if argc == 0:
  */
   if (unlikely(__pyx_v_argv == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 7, __pyx_L1_error)
+    __PYX_ERR(0, 10, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_argv); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_argv); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 10, __pyx_L1_error)
   __pyx_v_argc = __pyx_t_1;
 
-  /* "km_fasta.pyx":9
+  /* "km_fasta.pyx":12
  *     cdef int argc = len(argv)
  * 
  *     if argc == 0:             # <<<<<<<<<<<<<<
  *         # Handle empty argv gracefully
  *         return
  */
   __pyx_t_2 = (__pyx_v_argc == 0);
   if (__pyx_t_2) {
 
-    /* "km_fasta.pyx":11
+    /* "km_fasta.pyx":14
  *     if argc == 0:
  *         # Handle empty argv gracefully
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "km_fasta.pyx":9
+    /* "km_fasta.pyx":12
  *     cdef int argc = len(argv)
  * 
  *     if argc == 0:             # <<<<<<<<<<<<<<
  *         # Handle empty argv gracefully
  *         return
  */
   }
 
-  /* "km_fasta.pyx":13
+  /* "km_fasta.pyx":16
  *         return
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))             # <<<<<<<<<<<<<<
  *     if c_argv is NULL:
  *         # Handle allocation failure
  */
   __pyx_v_c_argv = ((char **)malloc(((__pyx_v_argc + 1) * (sizeof(char *)))));
 
-  /* "km_fasta.pyx":14
+  /* "km_fasta.pyx":17
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))
  *     if c_argv is NULL:             # <<<<<<<<<<<<<<
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")
  */
   __pyx_t_2 = (__pyx_v_c_argv == NULL);
   if (unlikely(__pyx_t_2)) {
 
-    /* "km_fasta.pyx":16
+    /* "km_fasta.pyx":19
  *     if c_argv is NULL:
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 16, __pyx_L1_error)
+    __PYX_ERR(0, 19, __pyx_L1_error)
 
-    /* "km_fasta.pyx":14
+    /* "km_fasta.pyx":17
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))
  *     if c_argv is NULL:             # <<<<<<<<<<<<<<
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")
  */
   }
 
-  /* "km_fasta.pyx":18
+  /* "km_fasta.pyx":21
  *         raise MemoryError("Failed to allocate memory")
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         for i in range(argc):
  *             if argv[i] is None:
  */
   /*try:*/ {
 
-    /* "km_fasta.pyx":19
+    /* "km_fasta.pyx":22
  * 
  *     try:
  *         for i in range(argc):             # <<<<<<<<<<<<<<
  *             if argv[i] is None:
  *                 # Handle invalid argument
  */
     __pyx_t_4 = __pyx_v_argc;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "km_fasta.pyx":20
+      /* "km_fasta.pyx":23
  *     try:
  *         for i in range(argc):
  *             if argv[i] is None:             # <<<<<<<<<<<<<<
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))
  */
       if (unlikely(__pyx_v_argv == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 20, __pyx_L6_error)
+        __PYX_ERR(0, 23, __pyx_L6_error)
       }
-      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L6_error)
+      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_2 = (__pyx_t_3 == Py_None);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (unlikely(__pyx_t_2)) {
 
-        /* "km_fasta.pyx":22
+        /* "km_fasta.pyx":25
  *             if argv[i] is None:
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))             # <<<<<<<<<<<<<<
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))
  *             if c_argv[i] is NULL:
  */
-        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Invalid_argument_at_index, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 22, __pyx_L6_error)
+        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Invalid_argument_at_index, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 25, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 22, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 25, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_9 = NULL;
         __pyx_t_10 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_7))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
           if (likely(__pyx_t_9)) {
@@ -2676,48 +2676,48 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_8};
           __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L6_error)
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
-        __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 22, __pyx_L6_error)
+        __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 25, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_7, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __PYX_ERR(0, 22, __pyx_L6_error)
+        __PYX_ERR(0, 25, __pyx_L6_error)
 
-        /* "km_fasta.pyx":20
+        /* "km_fasta.pyx":23
  *     try:
  *         for i in range(argc):
  *             if argv[i] is None:             # <<<<<<<<<<<<<<
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))
  */
       }
 
-      /* "km_fasta.pyx":23
+      /* "km_fasta.pyx":26
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))             # <<<<<<<<<<<<<<
  *             if c_argv[i] is NULL:
  *                 # Handle strdup failure
  */
       if (unlikely(__pyx_v_argv == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 23, __pyx_L6_error)
+        __PYX_ERR(0, 26, __pyx_L6_error)
       }
-      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L6_error)
+      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 23, __pyx_L6_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 26, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
@@ -2727,45 +2727,45 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
           __pyx_t_10 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_utf_8};
+        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_s_utf_8};
         __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 23, __pyx_L6_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 26, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
-      __pyx_t_11 = __Pyx_PyObject_AsString(__pyx_t_7); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L6_error)
+      __pyx_t_11 = __Pyx_PyObject_AsString(__pyx_t_7); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L6_error)
       (__pyx_v_c_argv[__pyx_v_i]) = strdup(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "km_fasta.pyx":24
+      /* "km_fasta.pyx":27
  *                 raise ValueError("Invalid argument at index {}".format(i))
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))
  *             if c_argv[i] is NULL:             # <<<<<<<<<<<<<<
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  */
       __pyx_t_2 = ((__pyx_v_c_argv[__pyx_v_i]) == NULL);
       if (unlikely(__pyx_t_2)) {
 
-        /* "km_fasta.pyx":26
+        /* "km_fasta.pyx":29
  *             if c_argv[i] is NULL:
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))             # <<<<<<<<<<<<<<
  *         c_argv[argc] = NULL
- *         return km_fasta.main_fasta(argc, c_argv)
+ *         return main_fasta(argc, c_argv)
  */
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Failed_to_allocate_memory_for_ar, __pyx_n_s_format); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 26, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Failed_to_allocate_memory_for_ar, __pyx_n_s_format); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 29, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L6_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 29, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_9 = NULL;
         __pyx_t_10 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
           if (likely(__pyx_t_9)) {
@@ -2778,61 +2778,61 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_3};
           __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 26, __pyx_L6_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 29, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
-        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_MemoryError, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 26, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_MemoryError, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 29, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_8, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __PYX_ERR(0, 26, __pyx_L6_error)
+        __PYX_ERR(0, 29, __pyx_L6_error)
 
-        /* "km_fasta.pyx":24
+        /* "km_fasta.pyx":27
  *                 raise ValueError("Invalid argument at index {}".format(i))
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))
  *             if c_argv[i] is NULL:             # <<<<<<<<<<<<<<
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  */
       }
     }
 
-    /* "km_fasta.pyx":27
+    /* "km_fasta.pyx":30
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  *         c_argv[argc] = NULL             # <<<<<<<<<<<<<<
- *         return km_fasta.main_fasta(argc, c_argv)
+ *         return main_fasta(argc, c_argv)
  *     finally:
  */
     (__pyx_v_c_argv[__pyx_v_argc]) = NULL;
 
-    /* "km_fasta.pyx":28
+    /* "km_fasta.pyx":31
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  *         c_argv[argc] = NULL
- *         return km_fasta.main_fasta(argc, c_argv)             # <<<<<<<<<<<<<<
+ *         return main_fasta(argc, c_argv)             # <<<<<<<<<<<<<<
  *     finally:
  *         for i in range(argc):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_8 = __Pyx_PyInt_From_int(main_fasta(__pyx_v_argc, __pyx_v_c_argv)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 28, __pyx_L6_error)
+    __pyx_t_8 = __Pyx_PyInt_From_int(main_fasta(__pyx_v_argc, __pyx_v_c_argv)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 31, __pyx_L6_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L5_return;
   }
 
-  /* "km_fasta.pyx":30
- *         return km_fasta.main_fasta(argc, c_argv)
+  /* "km_fasta.pyx":33
+ *         return main_fasta(argc, c_argv)
  *     finally:
  *         for i in range(argc):             # <<<<<<<<<<<<<<
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  */
   /*finally:*/ {
     __pyx_L6_error:;
@@ -2855,43 +2855,43 @@
       __pyx_t_4 = __pyx_lineno; __pyx_t_5 = __pyx_clineno; __pyx_t_12 = __pyx_filename;
       {
         __pyx_t_6 = __pyx_v_argc;
         __pyx_t_10 = __pyx_t_6;
         for (__pyx_t_19 = 0; __pyx_t_19 < __pyx_t_10; __pyx_t_19+=1) {
           __pyx_v_i = __pyx_t_19;
 
-          /* "km_fasta.pyx":31
+          /* "km_fasta.pyx":34
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
           __pyx_t_2 = ((__pyx_v_c_argv[__pyx_v_i]) != NULL);
           if (__pyx_t_2) {
 
-            /* "km_fasta.pyx":32
+            /* "km_fasta.pyx":35
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])             # <<<<<<<<<<<<<<
  *         free(c_argv)
  */
             free((__pyx_v_c_argv[__pyx_v_i]));
 
-            /* "km_fasta.pyx":31
+            /* "km_fasta.pyx":34
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
           }
         }
 
-        /* "km_fasta.pyx":33
+        /* "km_fasta.pyx":36
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  *         free(c_argv)             # <<<<<<<<<<<<<<
  */
         free(__pyx_v_c_argv);
       }
       if (PY_MAJOR_VERSION >= 3) {
@@ -2908,68 +2908,68 @@
       __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_5; __pyx_filename = __pyx_t_12;
       goto __pyx_L1_error;
     }
     __pyx_L5_return: {
       __pyx_t_18 = __pyx_r;
       __pyx_r = 0;
 
-      /* "km_fasta.pyx":30
- *         return km_fasta.main_fasta(argc, c_argv)
+      /* "km_fasta.pyx":33
+ *         return main_fasta(argc, c_argv)
  *     finally:
  *         for i in range(argc):             # <<<<<<<<<<<<<<
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  */
       __pyx_t_5 = __pyx_v_argc;
       __pyx_t_4 = __pyx_t_5;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_4; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "km_fasta.pyx":31
+        /* "km_fasta.pyx":34
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
         __pyx_t_2 = ((__pyx_v_c_argv[__pyx_v_i]) != NULL);
         if (__pyx_t_2) {
 
-          /* "km_fasta.pyx":32
+          /* "km_fasta.pyx":35
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])             # <<<<<<<<<<<<<<
  *         free(c_argv)
  */
           free((__pyx_v_c_argv[__pyx_v_i]));
 
-          /* "km_fasta.pyx":31
+          /* "km_fasta.pyx":34
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
         }
       }
 
-      /* "km_fasta.pyx":33
+      /* "km_fasta.pyx":36
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  *         free(c_argv)             # <<<<<<<<<<<<<<
  */
       free(__pyx_v_c_argv);
       __pyx_r = __pyx_t_18;
       __pyx_t_18 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "km_fasta.pyx":6
- * 
+  /* "km_fasta.pyx":9
+ *     int main_fasta(int argc, char **argv)
  * 
  * def py_main_fasta(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
 
   /* function exit code */
@@ -2998,78 +2998,78 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
-    {&__pyx_kp_u_Failed_to_allocate_memory, __pyx_k_Failed_to_allocate_memory, sizeof(__pyx_k_Failed_to_allocate_memory), 0, 1, 0, 0},
-    {&__pyx_kp_u_Failed_to_allocate_memory_for_ar, __pyx_k_Failed_to_allocate_memory_for_ar, sizeof(__pyx_k_Failed_to_allocate_memory_for_ar), 0, 1, 0, 0},
-    {&__pyx_kp_u_Invalid_argument_at_index, __pyx_k_Invalid_argument_at_index, sizeof(__pyx_k_Invalid_argument_at_index), 0, 1, 0, 0},
+    {&__pyx_kp_s_Failed_to_allocate_memory, __pyx_k_Failed_to_allocate_memory, sizeof(__pyx_k_Failed_to_allocate_memory), 0, 0, 1, 0},
+    {&__pyx_kp_s_Failed_to_allocate_memory_for_ar, __pyx_k_Failed_to_allocate_memory_for_ar, sizeof(__pyx_k_Failed_to_allocate_memory_for_ar), 0, 0, 1, 0},
+    {&__pyx_kp_s_Invalid_argument_at_index, __pyx_k_Invalid_argument_at_index, sizeof(__pyx_k_Invalid_argument_at_index), 0, 0, 1, 0},
     {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 0, 1, 1},
     {&__pyx_n_s_argc, __pyx_k_argc, sizeof(__pyx_k_argc), 0, 0, 1, 1},
     {&__pyx_n_s_argv, __pyx_k_argv, sizeof(__pyx_k_argv), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_c_argv, __pyx_k_c_argv, sizeof(__pyx_k_c_argv), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_kp_s_cython_km_fasta_pyx, __pyx_k_cython_km_fasta_pyx, sizeof(__pyx_k_cython_km_fasta_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
     {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_n_s_km_fasta, __pyx_k_km_fasta, sizeof(__pyx_k_km_fasta), 0, 0, 1, 1},
-    {&__pyx_kp_s_kmtools_cython_km_fasta_pyx, __pyx_k_kmtools_cython_km_fasta_pyx, sizeof(__pyx_k_kmtools_cython_km_fasta_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_py_main_fasta, __pyx_k_py_main_fasta, sizeof(__pyx_k_py_main_fasta), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-    {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
+    {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 16, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 19, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 25, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "km_fasta.pyx":16
+  /* "km_fasta.pyx":19
  *     if c_argv is NULL:
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Failed_to_allocate_memory); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Failed_to_allocate_memory); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "km_fasta.pyx":6
- * 
+  /* "km_fasta.pyx":9
+ *     int main_fasta(int argc, char **argv)
  * 
  * def py_main_fasta(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(4, __pyx_n_s_argv, __pyx_n_s_argc, __pyx_n_s_c_argv, __pyx_n_s_i); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(4, __pyx_n_s_argv, __pyx_n_s_argc, __pyx_n_s_c_argv, __pyx_n_s_i); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmtools_cython_km_fasta_pyx, __pyx_n_s_py_main_fasta, 6, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cython_km_fasta_pyx, __pyx_n_s_py_main_fasta, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -3425,30 +3425,30 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "km_fasta.pyx":6
- * 
+  /* "km_fasta.pyx":9
+ *     int main_fasta(int argc, char **argv)
  * 
  * def py_main_fasta(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8km_fasta_1py_main_fasta, 0, __pyx_n_s_py_main_fasta, NULL, __pyx_n_s_km_fasta, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8km_fasta_1py_main_fasta, 0, __pyx_n_s_py_main_fasta, NULL, __pyx_n_s_km_fasta, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_main_fasta, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_main_fasta, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "km_fasta.pyx":1
- * cimport km_fasta             # <<<<<<<<<<<<<<
- * from libc.stdlib cimport malloc, free
+ * from libc.stdlib cimport malloc, free             # <<<<<<<<<<<<<<
  * from libc.string cimport strdup
+ * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
```

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_fasta.pyx` & `kmat_tools-0.0.9/cython/km_fasta.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-cimport km_fasta
 from libc.stdlib cimport malloc, free
 from libc.string cimport strdup
 
 
+# Declare main_fasta function from C
+cdef extern from "lib/include/km_fasta.h":
+    int main_fasta(int argc, char **argv)
+
 def py_main_fasta(list argv):
     cdef int argc = len(argv)
     
     if argc == 0:
         # Handle empty argv gracefully
         return
     
@@ -21,13 +24,13 @@
                 # Handle invalid argument
                 raise ValueError("Invalid argument at index {}".format(i))
             c_argv[i] = strdup(argv[i].encode('utf-8'))
             if c_argv[i] is NULL:
                 # Handle strdup failure
                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
         c_argv[argc] = NULL
-        return km_fasta.main_fasta(argc, c_argv)
+        return main_fasta(argc, c_argv)
     finally:
         for i in range(argc):
             if c_argv[i] is not NULL:
                 free(c_argv[i])
         free(c_argv)
```

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_reset.c` & `kmat_tools-0.0.9/cython/km_reset.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "kmtools_cython/lib/include/km_reset.h"
+            "cython/lib/include/km_reset.h"
         ],
         "extra_compile_args": [
             "-Wall",
             "-Wno-unused-function",
             "-O3",
             "-pedantic"
         ],
         "include_dirs": [
-            "kmtools_cython",
-            "kmtools_cython/lib/include"
+            "cython",
+            "cython/lib/include"
         ],
         "libraries": [
             "z",
             "m"
         ],
         "name": "km_reset",
         "sources": [
-            "kmtools_cython/km_reset.pyx",
-            "kmtools_cython/lib/src/km_reset.c"
+            "cython/km_reset.pyx",
+            "cython/lib/src/km_reset.c"
         ]
     },
     "module_name": "km_reset"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -1494,15 +1494,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "kmtools_cython/km_reset.pyx",
+  "cython/km_reset.pyx",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -1988,15 +1988,15 @@
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_km_reset[] = "km_reset";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_reset_getopt[] = "reset_getopt";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_kmtools_cython_km_reset_pyx[] = "kmtools_cython/km_reset.pyx";
+static const char __pyx_k_cython_km_reset_pyx[] = "cython/km_reset.pyx";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8km_reset_reset_getopt(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
@@ -2023,17 +2023,17 @@
   PyTypeObject *__pyx_CoroutineType;
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   PyObject *__pyx_n_s__2;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_kp_s_cython_km_reset_pyx;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_n_s_km_reset;
-  PyObject *__pyx_kp_s_kmtools_cython_km_reset_pyx;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_reset_getopt;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_codeobj_;
 } __pyx_mstate;
 
@@ -2076,17 +2076,17 @@
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_n_s__2);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_cython_km_reset_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_n_s_km_reset);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_kmtools_cython_km_reset_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_reset_getopt);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_codeobj_);
   return 0;
 }
@@ -2107,17 +2107,17 @@
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_n_s__2);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_cython_km_reset_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_n_s_km_reset);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_kmtools_cython_km_reset_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_reset_getopt);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_codeobj_);
   return 0;
 }
@@ -2148,17 +2148,17 @@
 #define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #define __pyx_n_s__2 __pyx_mstate_global->__pyx_n_s__2
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_kp_s_cython_km_reset_pyx __pyx_mstate_global->__pyx_kp_s_cython_km_reset_pyx
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_n_s_km_reset __pyx_mstate_global->__pyx_n_s_km_reset
-#define __pyx_kp_s_kmtools_cython_km_reset_pyx __pyx_mstate_global->__pyx_kp_s_kmtools_cython_km_reset_pyx
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_reset_getopt __pyx_mstate_global->__pyx_n_s_reset_getopt
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_codeobj_ __pyx_mstate_global->__pyx_codeobj_
 /* #### Code section: module_code ### */
 
@@ -2226,17 +2226,17 @@
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_n_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_kp_s_cython_km_reset_pyx, __pyx_k_cython_km_reset_pyx, sizeof(__pyx_k_cython_km_reset_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_n_s_km_reset, __pyx_k_km_reset, sizeof(__pyx_k_km_reset), 0, 0, 1, 1},
-    {&__pyx_kp_s_kmtools_cython_km_reset_pyx, __pyx_k_kmtools_cython_km_reset_pyx, sizeof(__pyx_k_kmtools_cython_km_reset_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_reset_getopt, __pyx_k_reset_getopt, sizeof(__pyx_k_reset_getopt), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
@@ -2253,15 +2253,15 @@
 
   /* "km_reset.pyx":5
  * cimport km_reset
  * 
  * def reset_getopt():             # <<<<<<<<<<<<<<
  *     km_reset()
  */
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmtools_cython_km_reset_pyx, __pyx_n_s_reset_getopt, 5, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cython_km_reset_pyx, __pyx_n_s_reset_getopt, 5, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
```

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_select.pyx` & `kmat_tools-0.0.9/cython/km_select.pyx`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc` & `kmat_tools-0.0.9/cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc` & `kmat_tools-0.0.9/cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc` & `kmat_tools-0.0.9/cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_basic_filter_wrapper.py` & `kmat_tools-0.0.9/cython/km_tools_wrappers/km_basic_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_fasta_wrapper.py` & `kmat_tools-0.0.9/cython/km_tools_wrappers/km_fasta_wrapper.py`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_unitig_wrapper.py` & `kmat_tools-0.0.9/cython/km_tools_wrappers/km_unitig_wrapper.py`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_unitig.c` & `kmat_tools-0.0.9/cython/km_unitig.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "kmtools_cython/lib/include/km_unitig.h"
+            "cython/lib/include/km_unitig.h"
         ],
         "extra_compile_args": [
             "-Wall",
             "-Wno-unused-function",
             "-O3",
             "-pedantic"
         ],
         "include_dirs": [
-            "kmtools_cython",
-            "kmtools_cython/lib/include"
+            "cython",
+            "cython/lib/include"
         ],
         "libraries": [
             "z",
             "m"
         ],
         "name": "km_unitig",
         "sources": [
-            "kmtools_cython/km_unitig.pyx",
-            "kmtools_cython/lib/src/km_unitig.c"
+            "cython/km_unitig.pyx",
+            "cython/lib/src/km_unitig.c"
         ]
     },
     "module_name": "km_unitig"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -1245,17 +1245,17 @@
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
 #define __PYX_HAVE__km_unitig
 #define __PYX_HAVE_API__km_unitig
 /* Early includes */
-#include "lib/include/km_unitig.h"
 #include <string.h>
 #include <stdlib.h>
+#include "lib/include/km_unitig.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -1496,15 +1496,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "kmtools_cython/km_unitig.pyx",
+  "cython/km_unitig.pyx",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -2143,17 +2143,17 @@
 static const char __pyx_k_km_unitig[] = "km_unitig";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_py_main_unitig[] = "py_main_unitig";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_cython_km_unitig_pyx[] = "cython/km_unitig.pyx";
 static const char __pyx_k_Failed_to_allocate_memory[] = "Failed to allocate memory";
 static const char __pyx_k_Invalid_argument_at_index[] = "Invalid argument at index {}";
-static const char __pyx_k_kmtools_cython_km_unitig_pyx[] = "kmtools_cython/km_unitig.pyx";
 static const char __pyx_k_Failed_to_allocate_memory_for_ar[] = "Failed to allocate memory for argument {}";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_9km_unitig_py_main_unitig(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_argv); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
@@ -2182,37 +2182,37 @@
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
-  PyObject *__pyx_kp_u_Failed_to_allocate_memory;
-  PyObject *__pyx_kp_u_Failed_to_allocate_memory_for_ar;
-  PyObject *__pyx_kp_u_Invalid_argument_at_index;
+  PyObject *__pyx_kp_s_Failed_to_allocate_memory;
+  PyObject *__pyx_kp_s_Failed_to_allocate_memory_for_ar;
+  PyObject *__pyx_kp_s_Invalid_argument_at_index;
   PyObject *__pyx_n_s_MemoryError;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s__4;
   PyObject *__pyx_n_s_argc;
   PyObject *__pyx_n_s_argv;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_c_argv;
   PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_kp_s_cython_km_unitig_pyx;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_format;
   PyObject *__pyx_n_s_i;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_n_s_km_unitig;
-  PyObject *__pyx_kp_s_kmtools_cython_km_unitig_pyx;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_py_main_unitig;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_test;
-  PyObject *__pyx_kp_u_utf_8;
+  PyObject *__pyx_kp_s_utf_8;
   PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_codeobj__3;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
@@ -2250,37 +2250,37 @@
   Py_CLEAR(clear_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Failed_to_allocate_memory);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Failed_to_allocate_memory_for_ar);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_argument_at_index);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Failed_to_allocate_memory);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Failed_to_allocate_memory_for_ar);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Invalid_argument_at_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s__4);
   Py_CLEAR(clear_module_state->__pyx_n_s_argc);
   Py_CLEAR(clear_module_state->__pyx_n_s_argv);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_c_argv);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_cython_km_unitig_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_format);
   Py_CLEAR(clear_module_state->__pyx_n_s_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_n_s_km_unitig);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_kmtools_cython_km_unitig_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_py_main_unitig);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_utf_8);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_codeobj__3);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
@@ -2296,37 +2296,37 @@
   Py_VISIT(traverse_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Failed_to_allocate_memory);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Failed_to_allocate_memory_for_ar);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_argument_at_index);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Failed_to_allocate_memory);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Failed_to_allocate_memory_for_ar);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Invalid_argument_at_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s__4);
   Py_VISIT(traverse_module_state->__pyx_n_s_argc);
   Py_VISIT(traverse_module_state->__pyx_n_s_argv);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_c_argv);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_cython_km_unitig_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_format);
   Py_VISIT(traverse_module_state->__pyx_n_s_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_n_s_km_unitig);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_kmtools_cython_km_unitig_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_py_main_unitig);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_utf_8);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_codeobj__3);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
@@ -2356,44 +2356,44 @@
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
-#define __pyx_kp_u_Failed_to_allocate_memory __pyx_mstate_global->__pyx_kp_u_Failed_to_allocate_memory
-#define __pyx_kp_u_Failed_to_allocate_memory_for_ar __pyx_mstate_global->__pyx_kp_u_Failed_to_allocate_memory_for_ar
-#define __pyx_kp_u_Invalid_argument_at_index __pyx_mstate_global->__pyx_kp_u_Invalid_argument_at_index
+#define __pyx_kp_s_Failed_to_allocate_memory __pyx_mstate_global->__pyx_kp_s_Failed_to_allocate_memory
+#define __pyx_kp_s_Failed_to_allocate_memory_for_ar __pyx_mstate_global->__pyx_kp_s_Failed_to_allocate_memory_for_ar
+#define __pyx_kp_s_Invalid_argument_at_index __pyx_mstate_global->__pyx_kp_s_Invalid_argument_at_index
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s__4 __pyx_mstate_global->__pyx_n_s__4
 #define __pyx_n_s_argc __pyx_mstate_global->__pyx_n_s_argc
 #define __pyx_n_s_argv __pyx_mstate_global->__pyx_n_s_argv
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_c_argv __pyx_mstate_global->__pyx_n_s_c_argv
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_kp_s_cython_km_unitig_pyx __pyx_mstate_global->__pyx_kp_s_cython_km_unitig_pyx
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
 #define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_n_s_km_unitig __pyx_mstate_global->__pyx_n_s_km_unitig
-#define __pyx_kp_s_kmtools_cython_km_unitig_pyx __pyx_mstate_global->__pyx_kp_s_kmtools_cython_km_unitig_pyx
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_py_main_unitig __pyx_mstate_global->__pyx_n_s_py_main_unitig
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
-#define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
+#define __pyx_kp_s_utf_8 __pyx_mstate_global->__pyx_kp_s_utf_8
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_codeobj__3 __pyx_mstate_global->__pyx_codeobj__3
 /* #### Code section: module_code ### */
 
-/* "km_unitig.pyx":5
- * from libc.string cimport strdup
+/* "km_unitig.pyx":7
+ *     int main_unitig(int argc, char **argv) nogil
  * 
  * def py_main_unitig(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
 
 /* Python wrapper */
@@ -2445,45 +2445,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_argv)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 5, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 7, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "py_main_unitig") < 0)) __PYX_ERR(0, 5, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "py_main_unitig") < 0)) __PYX_ERR(0, 7, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_argv = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("py_main_unitig", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 5, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("py_main_unitig", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 7, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("km_unitig.py_main_unitig", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_argv), (&PyList_Type), 1, "argv", 1))) __PYX_ERR(0, 5, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_argv), (&PyList_Type), 1, "argv", 1))) __PYX_ERR(0, 7, __pyx_L1_error)
   __pyx_r = __pyx_pf_9km_unitig_py_main_unitig(__pyx_self, __pyx_v_argv);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2523,147 +2523,147 @@
   PyObject *__pyx_t_18 = NULL;
   int __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("py_main_unitig", 1);
 
-  /* "km_unitig.pyx":6
+  /* "km_unitig.pyx":8
  * 
  * def py_main_unitig(list argv):
  *     cdef int argc = len(argv)             # <<<<<<<<<<<<<<
  * 
  *     if argc == 0:
  */
   if (unlikely(__pyx_v_argv == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 6, __pyx_L1_error)
+    __PYX_ERR(0, 8, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_argv); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_argv); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 8, __pyx_L1_error)
   __pyx_v_argc = __pyx_t_1;
 
-  /* "km_unitig.pyx":8
+  /* "km_unitig.pyx":10
  *     cdef int argc = len(argv)
  * 
  *     if argc == 0:             # <<<<<<<<<<<<<<
  *         # Handle empty argv gracefully
  *         return
  */
   __pyx_t_2 = (__pyx_v_argc == 0);
   if (__pyx_t_2) {
 
-    /* "km_unitig.pyx":10
+    /* "km_unitig.pyx":12
  *     if argc == 0:
  *         # Handle empty argv gracefully
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "km_unitig.pyx":8
+    /* "km_unitig.pyx":10
  *     cdef int argc = len(argv)
  * 
  *     if argc == 0:             # <<<<<<<<<<<<<<
  *         # Handle empty argv gracefully
  *         return
  */
   }
 
-  /* "km_unitig.pyx":12
+  /* "km_unitig.pyx":14
  *         return
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))             # <<<<<<<<<<<<<<
  *     if c_argv is NULL:
  *         # Handle allocation failure
  */
   __pyx_v_c_argv = ((char **)malloc(((__pyx_v_argc + 1) * (sizeof(char *)))));
 
-  /* "km_unitig.pyx":13
+  /* "km_unitig.pyx":15
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))
  *     if c_argv is NULL:             # <<<<<<<<<<<<<<
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")
  */
   __pyx_t_2 = (__pyx_v_c_argv == NULL);
   if (unlikely(__pyx_t_2)) {
 
-    /* "km_unitig.pyx":15
+    /* "km_unitig.pyx":17
  *     if c_argv is NULL:
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 15, __pyx_L1_error)
+    __PYX_ERR(0, 17, __pyx_L1_error)
 
-    /* "km_unitig.pyx":13
+    /* "km_unitig.pyx":15
  * 
  *     cdef char **c_argv = <char **>malloc((argc+1) * sizeof(char *))
  *     if c_argv is NULL:             # <<<<<<<<<<<<<<
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")
  */
   }
 
-  /* "km_unitig.pyx":17
+  /* "km_unitig.pyx":19
  *         raise MemoryError("Failed to allocate memory")
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         for i in range(argc):
  *             if argv[i] is None:
  */
   /*try:*/ {
 
-    /* "km_unitig.pyx":18
+    /* "km_unitig.pyx":20
  * 
  *     try:
  *         for i in range(argc):             # <<<<<<<<<<<<<<
  *             if argv[i] is None:
  *                 # Handle invalid argument
  */
     __pyx_t_4 = __pyx_v_argc;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "km_unitig.pyx":19
+      /* "km_unitig.pyx":21
  *     try:
  *         for i in range(argc):
  *             if argv[i] is None:             # <<<<<<<<<<<<<<
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))
  */
       if (unlikely(__pyx_v_argv == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 19, __pyx_L6_error)
+        __PYX_ERR(0, 21, __pyx_L6_error)
       }
-      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L6_error)
+      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_2 = (__pyx_t_3 == Py_None);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (unlikely(__pyx_t_2)) {
 
-        /* "km_unitig.pyx":21
+        /* "km_unitig.pyx":23
  *             if argv[i] is None:
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))             # <<<<<<<<<<<<<<
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))
  *             if c_argv[i] is NULL:
  */
-        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Invalid_argument_at_index, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 21, __pyx_L6_error)
+        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Invalid_argument_at_index, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 23, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 21, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 23, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_9 = NULL;
         __pyx_t_10 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_7))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
           if (likely(__pyx_t_9)) {
@@ -2676,48 +2676,48 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_8};
           __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L6_error)
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
-        __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 21, __pyx_L6_error)
+        __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 23, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_7, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __PYX_ERR(0, 21, __pyx_L6_error)
+        __PYX_ERR(0, 23, __pyx_L6_error)
 
-        /* "km_unitig.pyx":19
+        /* "km_unitig.pyx":21
  *     try:
  *         for i in range(argc):
  *             if argv[i] is None:             # <<<<<<<<<<<<<<
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))
  */
       }
 
-      /* "km_unitig.pyx":22
+      /* "km_unitig.pyx":24
  *                 # Handle invalid argument
  *                 raise ValueError("Invalid argument at index {}".format(i))
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))             # <<<<<<<<<<<<<<
  *             if c_argv[i] is NULL:
  *                 # Handle strdup failure
  */
       if (unlikely(__pyx_v_argv == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 22, __pyx_L6_error)
+        __PYX_ERR(0, 24, __pyx_L6_error)
       }
-      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L6_error)
+      __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_argv, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 22, __pyx_L6_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 24, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
@@ -2727,45 +2727,45 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
           __pyx_t_10 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_utf_8};
+        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_s_utf_8};
         __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 22, __pyx_L6_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 24, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
-      __pyx_t_11 = __Pyx_PyObject_AsString(__pyx_t_7); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 22, __pyx_L6_error)
+      __pyx_t_11 = __Pyx_PyObject_AsString(__pyx_t_7); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L6_error)
       (__pyx_v_c_argv[__pyx_v_i]) = strdup(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "km_unitig.pyx":23
+      /* "km_unitig.pyx":25
  *                 raise ValueError("Invalid argument at index {}".format(i))
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))
  *             if c_argv[i] is NULL:             # <<<<<<<<<<<<<<
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  */
       __pyx_t_2 = ((__pyx_v_c_argv[__pyx_v_i]) == NULL);
       if (unlikely(__pyx_t_2)) {
 
-        /* "km_unitig.pyx":25
+        /* "km_unitig.pyx":27
  *             if c_argv[i] is NULL:
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))             # <<<<<<<<<<<<<<
  *         c_argv[argc] = NULL
  * 
  */
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Failed_to_allocate_memory_for_ar, __pyx_n_s_format); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 25, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Failed_to_allocate_memory_for_ar, __pyx_n_s_format); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 27, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L6_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_9 = NULL;
         __pyx_t_10 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
           if (likely(__pyx_t_9)) {
@@ -2778,61 +2778,61 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_3};
           __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 25, __pyx_L6_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 27, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
-        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_MemoryError, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 25, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_MemoryError, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 27, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_8, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __PYX_ERR(0, 25, __pyx_L6_error)
+        __PYX_ERR(0, 27, __pyx_L6_error)
 
-        /* "km_unitig.pyx":23
+        /* "km_unitig.pyx":25
  *                 raise ValueError("Invalid argument at index {}".format(i))
  *             c_argv[i] = strdup(argv[i].encode('utf-8'))
  *             if c_argv[i] is NULL:             # <<<<<<<<<<<<<<
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  */
       }
     }
 
-    /* "km_unitig.pyx":26
+    /* "km_unitig.pyx":28
  *                 # Handle strdup failure
  *                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
  *         c_argv[argc] = NULL             # <<<<<<<<<<<<<<
  * 
- *         return km_unitig.main_unitig(argc, c_argv)
+ *         return main_unitig(argc, c_argv)
  */
     (__pyx_v_c_argv[__pyx_v_argc]) = NULL;
 
-    /* "km_unitig.pyx":28
+    /* "km_unitig.pyx":30
  *         c_argv[argc] = NULL
  * 
- *         return km_unitig.main_unitig(argc, c_argv)             # <<<<<<<<<<<<<<
+ *         return main_unitig(argc, c_argv)             # <<<<<<<<<<<<<<
  *     finally:
  *         for i in range(argc):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_8 = __Pyx_PyInt_From_int(main_unitig(__pyx_v_argc, __pyx_v_c_argv)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 28, __pyx_L6_error)
+    __pyx_t_8 = __Pyx_PyInt_From_int(main_unitig(__pyx_v_argc, __pyx_v_c_argv)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 30, __pyx_L6_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L5_return;
   }
 
-  /* "km_unitig.pyx":30
- *         return km_unitig.main_unitig(argc, c_argv)
+  /* "km_unitig.pyx":32
+ *         return main_unitig(argc, c_argv)
  *     finally:
  *         for i in range(argc):             # <<<<<<<<<<<<<<
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  */
   /*finally:*/ {
     __pyx_L6_error:;
@@ -2855,43 +2855,43 @@
       __pyx_t_4 = __pyx_lineno; __pyx_t_5 = __pyx_clineno; __pyx_t_12 = __pyx_filename;
       {
         __pyx_t_6 = __pyx_v_argc;
         __pyx_t_10 = __pyx_t_6;
         for (__pyx_t_19 = 0; __pyx_t_19 < __pyx_t_10; __pyx_t_19+=1) {
           __pyx_v_i = __pyx_t_19;
 
-          /* "km_unitig.pyx":31
+          /* "km_unitig.pyx":33
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
           __pyx_t_2 = ((__pyx_v_c_argv[__pyx_v_i]) != NULL);
           if (__pyx_t_2) {
 
-            /* "km_unitig.pyx":32
+            /* "km_unitig.pyx":34
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])             # <<<<<<<<<<<<<<
  *         free(c_argv)
  */
             free((__pyx_v_c_argv[__pyx_v_i]));
 
-            /* "km_unitig.pyx":31
+            /* "km_unitig.pyx":33
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
           }
         }
 
-        /* "km_unitig.pyx":33
+        /* "km_unitig.pyx":35
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  *         free(c_argv)             # <<<<<<<<<<<<<<
  */
         free(__pyx_v_c_argv);
       }
       if (PY_MAJOR_VERSION >= 3) {
@@ -2908,68 +2908,68 @@
       __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_5; __pyx_filename = __pyx_t_12;
       goto __pyx_L1_error;
     }
     __pyx_L5_return: {
       __pyx_t_18 = __pyx_r;
       __pyx_r = 0;
 
-      /* "km_unitig.pyx":30
- *         return km_unitig.main_unitig(argc, c_argv)
+      /* "km_unitig.pyx":32
+ *         return main_unitig(argc, c_argv)
  *     finally:
  *         for i in range(argc):             # <<<<<<<<<<<<<<
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  */
       __pyx_t_5 = __pyx_v_argc;
       __pyx_t_4 = __pyx_t_5;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_4; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "km_unitig.pyx":31
+        /* "km_unitig.pyx":33
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
         __pyx_t_2 = ((__pyx_v_c_argv[__pyx_v_i]) != NULL);
         if (__pyx_t_2) {
 
-          /* "km_unitig.pyx":32
+          /* "km_unitig.pyx":34
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])             # <<<<<<<<<<<<<<
  *         free(c_argv)
  */
           free((__pyx_v_c_argv[__pyx_v_i]));
 
-          /* "km_unitig.pyx":31
+          /* "km_unitig.pyx":33
  *     finally:
  *         for i in range(argc):
  *             if c_argv[i] is not NULL:             # <<<<<<<<<<<<<<
  *                 free(c_argv[i])
  *         free(c_argv)
  */
         }
       }
 
-      /* "km_unitig.pyx":33
+      /* "km_unitig.pyx":35
  *             if c_argv[i] is not NULL:
  *                 free(c_argv[i])
  *         free(c_argv)             # <<<<<<<<<<<<<<
  */
       free(__pyx_v_c_argv);
       __pyx_r = __pyx_t_18;
       __pyx_t_18 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "km_unitig.pyx":5
- * from libc.string cimport strdup
+  /* "km_unitig.pyx":7
+ *     int main_unitig(int argc, char **argv) nogil
  * 
  * def py_main_unitig(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
 
   /* function exit code */
@@ -2998,78 +2998,78 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
-    {&__pyx_kp_u_Failed_to_allocate_memory, __pyx_k_Failed_to_allocate_memory, sizeof(__pyx_k_Failed_to_allocate_memory), 0, 1, 0, 0},
-    {&__pyx_kp_u_Failed_to_allocate_memory_for_ar, __pyx_k_Failed_to_allocate_memory_for_ar, sizeof(__pyx_k_Failed_to_allocate_memory_for_ar), 0, 1, 0, 0},
-    {&__pyx_kp_u_Invalid_argument_at_index, __pyx_k_Invalid_argument_at_index, sizeof(__pyx_k_Invalid_argument_at_index), 0, 1, 0, 0},
+    {&__pyx_kp_s_Failed_to_allocate_memory, __pyx_k_Failed_to_allocate_memory, sizeof(__pyx_k_Failed_to_allocate_memory), 0, 0, 1, 0},
+    {&__pyx_kp_s_Failed_to_allocate_memory_for_ar, __pyx_k_Failed_to_allocate_memory_for_ar, sizeof(__pyx_k_Failed_to_allocate_memory_for_ar), 0, 0, 1, 0},
+    {&__pyx_kp_s_Invalid_argument_at_index, __pyx_k_Invalid_argument_at_index, sizeof(__pyx_k_Invalid_argument_at_index), 0, 0, 1, 0},
     {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 0, 1, 1},
     {&__pyx_n_s_argc, __pyx_k_argc, sizeof(__pyx_k_argc), 0, 0, 1, 1},
     {&__pyx_n_s_argv, __pyx_k_argv, sizeof(__pyx_k_argv), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_c_argv, __pyx_k_c_argv, sizeof(__pyx_k_c_argv), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_kp_s_cython_km_unitig_pyx, __pyx_k_cython_km_unitig_pyx, sizeof(__pyx_k_cython_km_unitig_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
     {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_n_s_km_unitig, __pyx_k_km_unitig, sizeof(__pyx_k_km_unitig), 0, 0, 1, 1},
-    {&__pyx_kp_s_kmtools_cython_km_unitig_pyx, __pyx_k_kmtools_cython_km_unitig_pyx, sizeof(__pyx_k_kmtools_cython_km_unitig_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_py_main_unitig, __pyx_k_py_main_unitig, sizeof(__pyx_k_py_main_unitig), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-    {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
+    {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 15, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 18, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 23, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "km_unitig.pyx":15
+  /* "km_unitig.pyx":17
  *     if c_argv is NULL:
  *         # Handle allocation failure
  *         raise MemoryError("Failed to allocate memory")             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Failed_to_allocate_memory); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Failed_to_allocate_memory); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "km_unitig.pyx":5
- * from libc.string cimport strdup
+  /* "km_unitig.pyx":7
+ *     int main_unitig(int argc, char **argv) nogil
  * 
  * def py_main_unitig(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(4, __pyx_n_s_argv, __pyx_n_s_argc, __pyx_n_s_c_argv, __pyx_n_s_i); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(4, __pyx_n_s_argv, __pyx_n_s_argc, __pyx_n_s_c_argv, __pyx_n_s_i); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kmtools_cython_km_unitig_pyx, __pyx_n_s_py_main_unitig, 5, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cython_km_unitig_pyx, __pyx_n_s_py_main_unitig, 7, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -3425,30 +3425,30 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "km_unitig.pyx":5
- * from libc.string cimport strdup
+  /* "km_unitig.pyx":7
+ *     int main_unitig(int argc, char **argv) nogil
  * 
  * def py_main_unitig(list argv):             # <<<<<<<<<<<<<<
  *     cdef int argc = len(argv)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9km_unitig_1py_main_unitig, 0, __pyx_n_s_py_main_unitig, NULL, __pyx_n_s_km_unitig, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9km_unitig_1py_main_unitig, 0, __pyx_n_s_py_main_unitig, NULL, __pyx_n_s_km_unitig, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_main_unitig, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_main_unitig, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "km_unitig.pyx":1
- * cimport km_unitig             # <<<<<<<<<<<<<<
- * from libc.stdlib cimport malloc, free
+ * from libc.stdlib cimport malloc, free             # <<<<<<<<<<<<<<
  * from libc.string cimport strdup
+ * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
```

### Comparing `kmat_tools-0.0.6/kmtools_cython/km_unitig.pyx` & `kmat_tools-0.0.9/cython/km_unitig.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-cimport km_unitig
 from libc.stdlib cimport malloc, free
 from libc.string cimport strdup
 
+cdef extern from "lib/include/km_unitig.h":
+    int main_unitig(int argc, char **argv) nogil
+
 def py_main_unitig(list argv):
     cdef int argc = len(argv)
     
     if argc == 0:
         # Handle empty argv gracefully
         return
     
@@ -21,13 +23,13 @@
                 raise ValueError("Invalid argument at index {}".format(i))
             c_argv[i] = strdup(argv[i].encode('utf-8'))
             if c_argv[i] is NULL:
                 # Handle strdup failure
                 raise MemoryError("Failed to allocate memory for argument {}".format(i))
         c_argv[argc] = NULL
         
-        return km_unitig.main_unitig(argc, c_argv)
+        return main_unitig(argc, c_argv)
     finally:
         for i in range(argc):
             if c_argv[i] is not NULL:
                 free(c_argv[i])
         free(c_argv)
```

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/include/common.h` & `kmat_tools-0.0.9/cython/lib/include/common.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/include/khash.h` & `kmat_tools-0.0.9/cython/lib/include/khash.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/include/km_basic_filter.h` & `kmat_tools-0.0.9/cython/lib/include/km_basic_filter.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/include/km_fasta.h` & `kmat_tools-0.0.9/cython/lib/include/km_fasta.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/include/km_unitig.h` & `kmat_tools-0.0.9/cython/lib/include/km_unitig.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/include/kseq.h` & `kmat_tools-0.0.9/cython/lib/include/kseq.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/src/km_basic_filter.c` & `kmat_tools-0.0.9/cython/lib/src/km_basic_filter.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/src/km_diff.c` & `kmat_tools-0.0.9/cython/lib/src/km_diff.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/src/km_fasta.c` & `kmat_tools-0.0.9/cython/lib/src/km_fasta.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/src/km_merge.c` & `kmat_tools-0.0.9/cython/lib/src/km_merge.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/src/km_reverse.c` & `kmat_tools-0.0.9/cython/lib/src/km_reverse.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/src/km_select.c` & `kmat_tools-0.0.9/cython/lib/src/km_select.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/src/km_tools.c` & `kmat_tools-0.0.9/cython/lib/src/km_tools.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/kmtools_cython/lib/src/km_unitig.c` & `kmat_tools-0.0.9/cython/lib/src/km_unitig.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.6/setup.py` & `kmat_tools-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from setuptools import setup,Extension
+from setuptools import setup,Extension,find_packages
 from Cython.Build import cythonize
 
-EXTENSION_PATH = "kmtools_cython"
+EXTENSION_PATH = "cython"
 
 ext1 = Extension("km_basic_filter",
                  sources=[f"{EXTENSION_PATH}/km_basic_filter.pyx", f"{EXTENSION_PATH}/lib/src/km_basic_filter.c"],
                  include_dirs=[f"{EXTENSION_PATH}/lib/include"],
                  extra_compile_args=['-Wall', '-Wno-unused-function', '-O3', '-pedantic'],
                  libraries=['z', 'm'])
 
@@ -28,26 +28,27 @@
                  libraries=['z', 'm'])
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="kmat_tools",
-    version="0.0.6",
+    version="0.0.9",
     author="Riccardo Vicedomini, Francesco Andreace, Camila Duitama",
     author_email="cduitama@pasteur.fr",
     include_package_data=True,
-    package_data={"": ["MANIFEST", "LICENSE"]},
+    packages=find_packages(),
+    package_data={"": ["kmat_tools/*","cython/*.pxd","cython/*.pyx","cython/lib/include/*.h","cython/lib/src/*.c"]},
     ext_modules = cythonize([ext1,ext2,ext3,ext4]),
     entry_points={
         "console_scripts": [
             "kmat_tools = kmat_tools.__main__:main",
-            'km_basic_filter = kmat_tools.kmtools_cython.km_tools_wrappers.km_basic_filter_wrapper:km_basic_filter_main',
-            'km_fasta = kmat_tools.kmtools_cython.km_tools_wrappers.km_fasta_wrapper:km_fasta_main',
-            'km_unitig = kmat_tools.kmtools_cython.km_tools_wrappers.km_unitig_wrapper:km_unitig_main'
+            'km_basic_filter = kmat_tools.cython.km_tools_wrappers.km_basic_filter_wrapper:km_basic_filter_main',
+            'km_fasta = kmat_tools.cython.km_tools_wrappers.km_fasta_wrapper:km_fasta_main',
+            'km_unitig = kmat_tools.cython.km_tools_wrappers.km_unitig_wrapper:km_unitig_main'
        ]
     },
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CamilaDuitama/kmat_tools",
     project_urls={
         "Bug Tracker": "https://github.com/CamilaDuitama/kmat_tools/issues",
```

