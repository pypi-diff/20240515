# Comparing `tmp/fsspec-2024.3.0.tar.gz` & `tmp/fsspec-2024.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsspec-2024.3.0.tar", last modified: Fri Mar 15 20:15:57 2024, max compression
+gzip compressed data, was "fsspec-2024.3.1.tar", last modified: Mon Mar 18 19:35:00 2024, max compression
```

## Comparing `fsspec-2024.3.0.tar` & `fsspec-2024.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-15 20:15:57.388300 fsspec-2024.3.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1513 2022-09-16 19:17:16.000000 fsspec-2024.3.0/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)       85 2024-02-04 01:54:21.000000 fsspec-2024.3.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     6738 2024-03-15 20:15:57.388192 fsspec-2024.3.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     3591 2023-11-16 01:55:40.000000 fsspec-2024.3.0/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-15 20:15:57.375146 fsspec-2024.3.0/fsspec/
--rw-r--r--   0 mdurant    (502) staff       (20)     2010 2024-03-09 20:10:50.000000 fsspec-2024.3.0/fsspec/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2024-03-15 20:15:57.388843 fsspec-2024.3.0/fsspec/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2386 2023-12-11 19:44:13.000000 fsspec-2024.3.0/fsspec/archive.py
--rw-r--r--   0 mdurant    (502) staff       (20)    36404 2024-03-15 19:38:41.000000 fsspec-2024.3.0/fsspec/asyn.py
--rw-r--r--   0 mdurant    (502) staff       (20)    28819 2024-03-09 20:10:50.000000 fsspec-2024.3.0/fsspec/caching.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9210 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/callbacks.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4859 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/compression.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4279 2023-11-16 01:55:40.000000 fsspec-2024.3.0/fsspec/config.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1245 2022-09-21 20:03:17.000000 fsspec-2024.3.0/fsspec/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)    22448 2024-03-09 20:10:50.000000 fsspec-2024.3.0/fsspec/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2717 2024-03-08 18:56:35.000000 fsspec-2024.3.0/fsspec/dircache.py
--rw-r--r--   0 mdurant    (502) staff       (20)      330 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/exceptions.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10145 2023-11-16 01:55:40.000000 fsspec-2024.3.0/fsspec/fuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13575 2024-03-14 22:06:19.000000 fsspec-2024.3.0/fsspec/generic.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13932 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/gui.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-15 20:15:57.383505 fsspec-2024.3.0/fsspec/implementations/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2024.3.0/fsspec/implementations/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8649 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/implementations/arrow.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2429 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/implementations/cache_mapper.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8576 2023-11-16 01:55:40.000000 fsspec-2024.3.0/fsspec/implementations/cache_metadata.py
--rw-r--r--   0 mdurant    (502) staff       (20)    33029 2024-03-14 22:06:19.000000 fsspec-2024.3.0/fsspec/implementations/cached.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4466 2023-11-16 01:55:40.000000 fsspec-2024.3.0/fsspec/implementations/dask.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1658 2024-02-22 14:59:52.000000 fsspec-2024.3.0/fsspec/implementations/data.py
--rw-r--r--   0 mdurant    (502) staff       (20)    15014 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/implementations/dbfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    11384 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/implementations/dirfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    11655 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/implementations/ftp.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4034 2023-11-16 01:55:40.000000 fsspec-2024.3.0/fsspec/implementations/git.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7565 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/implementations/github.py
--rw-r--r--   0 mdurant    (502) staff       (20)    29601 2024-03-15 19:38:41.000000 fsspec-2024.3.0/fsspec/implementations/http.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3811 2023-11-16 01:55:40.000000 fsspec-2024.3.0/fsspec/implementations/jupyter.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7102 2023-12-05 15:09:52.000000 fsspec-2024.3.0/fsspec/implementations/libarchive.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13454 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/implementations/local.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9778 2024-03-14 22:06:19.000000 fsspec-2024.3.0/fsspec/implementations/memory.py
--rw-r--r--   0 mdurant    (502) staff       (20)    43871 2024-03-09 20:10:50.000000 fsspec-2024.3.0/fsspec/implementations/reference.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5631 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/implementations/sftp.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10804 2024-03-04 19:56:14.000000 fsspec-2024.3.0/fsspec/implementations/smb.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4111 2023-12-05 15:09:52.000000 fsspec-2024.3.0/fsspec/implementations/tar.py
--rw-r--r--   0 mdurant    (502) staff       (20)    16745 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/implementations/webhdfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4417 2024-03-04 19:56:14.000000 fsspec-2024.3.0/fsspec/implementations/zip.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8261 2024-03-15 13:19:25.000000 fsspec-2024.3.0/fsspec/mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)    19463 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/parquet.py
--rw-r--r--   0 mdurant    (502) staff       (20)    11173 2024-03-09 20:10:50.000000 fsspec-2024.3.0/fsspec/registry.py
--rw-r--r--   0 mdurant    (502) staff       (20)    66277 2024-02-04 01:54:21.000000 fsspec-2024.3.0/fsspec/spec.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-15 20:15:57.365843 fsspec-2024.3.0/fsspec/tests/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-15 20:15:57.385004 fsspec-2024.3.0/fsspec/tests/abstract/
--rw-r--r--   0 mdurant    (502) staff       (20)    10028 2023-11-16 01:55:40.000000 fsspec-2024.3.0/fsspec/tests/abstract/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4973 2023-11-16 01:55:40.000000 fsspec-2024.3.0/fsspec/tests/abstract/common.py
--rw-r--r--   0 mdurant    (502) staff       (20)    19967 2024-02-05 01:21:52.000000 fsspec-2024.3.0/fsspec/tests/abstract/copy.py
--rw-r--r--   0 mdurant    (502) staff       (20)    20755 2023-11-16 01:55:40.000000 fsspec-2024.3.0/fsspec/tests/abstract/get.py
--rw-r--r--   0 mdurant    (502) staff       (20)    21201 2024-02-05 01:21:52.000000 fsspec-2024.3.0/fsspec/tests/abstract/put.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2398 2024-03-14 22:06:19.000000 fsspec-2024.3.0/fsspec/transaction.py
--rw-r--r--   0 mdurant    (502) staff       (20)    23052 2024-02-22 14:59:52.000000 fsspec-2024.3.0/fsspec/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-15 20:15:57.385536 fsspec-2024.3.0/fsspec.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     6738 2024-03-15 20:15:57.000000 fsspec-2024.3.0/fsspec.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     1542 2024-03-15 20:15:57.000000 fsspec-2024.3.0/fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-03-15 20:15:57.000000 fsspec-2024.3.0/fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-11-16 01:26:52.000000 fsspec-2024.3.0/fsspec.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      590 2024-03-15 20:15:57.000000 fsspec-2024.3.0/fsspec.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        7 2024-03-15 20:15:57.000000 fsspec-2024.3.0/fsspec.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)     1364 2024-03-09 20:10:50.000000 fsspec-2024.3.0/pyproject.toml
--rw-r--r--   0 mdurant    (502) staff       (20)     1141 2024-03-15 20:15:57.388701 fsspec-2024.3.0/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     2367 2024-02-04 01:54:21.000000 fsspec-2024.3.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    86836 2023-11-16 01:55:40.000000 fsspec-2024.3.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:35:00.695715 fsspec-2024.3.1/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1513 2022-09-16 19:17:16.000000 fsspec-2024.3.1/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)       85 2024-02-04 01:54:21.000000 fsspec-2024.3.1/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     6738 2024-03-18 19:35:00.695601 fsspec-2024.3.1/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     3591 2023-11-16 01:55:40.000000 fsspec-2024.3.1/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:35:00.680684 fsspec-2024.3.1/fsspec/
+-rw-r--r--   0 mdurant    (502) staff       (20)     2010 2024-03-09 20:10:50.000000 fsspec-2024.3.1/fsspec/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2024-03-18 19:35:00.696218 fsspec-2024.3.1/fsspec/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2386 2023-12-11 19:44:13.000000 fsspec-2024.3.1/fsspec/archive.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    36404 2024-03-15 19:38:41.000000 fsspec-2024.3.1/fsspec/asyn.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    28819 2024-03-09 20:10:50.000000 fsspec-2024.3.1/fsspec/caching.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9210 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/callbacks.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4859 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/compression.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4279 2023-11-16 01:55:40.000000 fsspec-2024.3.1/fsspec/config.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1245 2022-09-21 20:03:17.000000 fsspec-2024.3.1/fsspec/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    22471 2024-03-18 18:57:32.000000 fsspec-2024.3.1/fsspec/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2717 2024-03-08 18:56:35.000000 fsspec-2024.3.1/fsspec/dircache.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      330 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/exceptions.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10145 2023-11-16 01:55:40.000000 fsspec-2024.3.1/fsspec/fuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13575 2024-03-14 22:06:19.000000 fsspec-2024.3.1/fsspec/generic.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13932 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/gui.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:35:00.691038 fsspec-2024.3.1/fsspec/implementations/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2024.3.1/fsspec/implementations/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8649 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/implementations/arrow.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2429 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/implementations/cache_mapper.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8576 2023-11-16 01:55:40.000000 fsspec-2024.3.1/fsspec/implementations/cache_metadata.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    33029 2024-03-14 22:06:19.000000 fsspec-2024.3.1/fsspec/implementations/cached.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4466 2023-11-16 01:55:40.000000 fsspec-2024.3.1/fsspec/implementations/dask.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1658 2024-02-22 14:59:52.000000 fsspec-2024.3.1/fsspec/implementations/data.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    15014 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/implementations/dbfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    11384 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/implementations/dirfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    11655 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/implementations/ftp.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4034 2023-11-16 01:55:40.000000 fsspec-2024.3.1/fsspec/implementations/git.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7565 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/implementations/github.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    29601 2024-03-15 19:38:41.000000 fsspec-2024.3.1/fsspec/implementations/http.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3811 2023-11-16 01:55:40.000000 fsspec-2024.3.1/fsspec/implementations/jupyter.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7102 2023-12-05 15:09:52.000000 fsspec-2024.3.1/fsspec/implementations/libarchive.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    14327 2024-03-18 18:57:32.000000 fsspec-2024.3.1/fsspec/implementations/local.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9778 2024-03-14 22:06:19.000000 fsspec-2024.3.1/fsspec/implementations/memory.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    43871 2024-03-09 20:10:50.000000 fsspec-2024.3.1/fsspec/implementations/reference.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5631 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/implementations/sftp.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10804 2024-03-18 18:57:13.000000 fsspec-2024.3.1/fsspec/implementations/smb.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4111 2023-12-05 15:09:52.000000 fsspec-2024.3.1/fsspec/implementations/tar.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    16745 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/implementations/webhdfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4417 2024-03-04 19:56:14.000000 fsspec-2024.3.1/fsspec/implementations/zip.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8261 2024-03-18 18:57:32.000000 fsspec-2024.3.1/fsspec/mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    19463 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/parquet.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    11173 2024-03-09 20:10:50.000000 fsspec-2024.3.1/fsspec/registry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    66277 2024-02-04 01:54:21.000000 fsspec-2024.3.1/fsspec/spec.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:35:00.669504 fsspec-2024.3.1/fsspec/tests/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:35:00.692584 fsspec-2024.3.1/fsspec/tests/abstract/
+-rw-r--r--   0 mdurant    (502) staff       (20)    10028 2023-11-16 01:55:40.000000 fsspec-2024.3.1/fsspec/tests/abstract/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4973 2023-11-16 01:55:40.000000 fsspec-2024.3.1/fsspec/tests/abstract/common.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    19967 2024-02-05 01:21:52.000000 fsspec-2024.3.1/fsspec/tests/abstract/copy.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    20755 2023-11-16 01:55:40.000000 fsspec-2024.3.1/fsspec/tests/abstract/get.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    21201 2024-02-05 01:21:52.000000 fsspec-2024.3.1/fsspec/tests/abstract/put.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2398 2024-03-14 22:06:19.000000 fsspec-2024.3.1/fsspec/transaction.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    23052 2024-02-22 14:59:52.000000 fsspec-2024.3.1/fsspec/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 19:35:00.692975 fsspec-2024.3.1/fsspec.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     6738 2024-03-18 19:35:00.000000 fsspec-2024.3.1/fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1542 2024-03-18 19:35:00.000000 fsspec-2024.3.1/fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-03-18 19:35:00.000000 fsspec-2024.3.1/fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-11-16 01:26:52.000000 fsspec-2024.3.1/fsspec.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      590 2024-03-18 19:35:00.000000 fsspec-2024.3.1/fsspec.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        7 2024-03-18 19:35:00.000000 fsspec-2024.3.1/fsspec.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)     1364 2024-03-09 20:10:50.000000 fsspec-2024.3.1/pyproject.toml
+-rw-r--r--   0 mdurant    (502) staff       (20)     1141 2024-03-18 19:35:00.696095 fsspec-2024.3.1/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     2367 2024-02-04 01:54:21.000000 fsspec-2024.3.1/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    86836 2023-11-16 01:55:40.000000 fsspec-2024.3.1/versioneer.py
```

### Comparing `fsspec-2024.3.0/LICENSE` & `fsspec-2024.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/PKG-INFO` & `fsspec-2024.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec
-Version: 2024.3.0
+Version: 2024.3.1
 Summary: File-system specification
 Home-page: https://github.com/fsspec/filesystem_spec
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Project-URL: Changelog, https://filesystem-spec.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://filesystem-spec.readthedocs.io/en/latest/
```

### Comparing `fsspec-2024.3.0/README.md` & `fsspec-2024.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/__init__.py` & `fsspec-2024.3.1/fsspec/__init__.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/archive.py` & `fsspec-2024.3.1/fsspec/archive.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/asyn.py` & `fsspec-2024.3.1/fsspec/asyn.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/caching.py` & `fsspec-2024.3.1/fsspec/caching.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/callbacks.py` & `fsspec-2024.3.1/fsspec/callbacks.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/compression.py` & `fsspec-2024.3.1/fsspec/compression.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/config.py` & `fsspec-2024.3.1/fsspec/config.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/conftest.py` & `fsspec-2024.3.1/fsspec/conftest.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/core.py` & `fsspec-2024.3.1/fsspec/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,24 +452,25 @@
     they map across to see the latest online documentation:
 
     - For implementations built into ``fsspec`` see
       https://filesystem-spec.readthedocs.io/en/latest/api.html#built-in-implementations
     - For implementations in separate packages see
       https://filesystem-spec.readthedocs.io/en/latest/api.html#other-known-implementations
     """
+    kw = {"expand": False}
+    kw.update(kwargs)
     out = open_files(
         urlpath=[urlpath],
         mode=mode,
         compression=compression,
         encoding=encoding,
         errors=errors,
         protocol=protocol,
         newline=newline,
-        expand=False,
-        **kwargs,
+        **kw,
     )
     if not out:
         raise FileNotFoundError(urlpath)
     return out[0]
 
 
 def open_local(
```

### Comparing `fsspec-2024.3.0/fsspec/dircache.py` & `fsspec-2024.3.1/fsspec/dircache.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/fuse.py` & `fsspec-2024.3.1/fsspec/fuse.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/generic.py` & `fsspec-2024.3.1/fsspec/generic.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/gui.py` & `fsspec-2024.3.1/fsspec/gui.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/arrow.py` & `fsspec-2024.3.1/fsspec/implementations/arrow.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/cache_mapper.py` & `fsspec-2024.3.1/fsspec/implementations/cache_mapper.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/cache_metadata.py` & `fsspec-2024.3.1/fsspec/implementations/cache_metadata.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/cached.py` & `fsspec-2024.3.1/fsspec/implementations/cached.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/dask.py` & `fsspec-2024.3.1/fsspec/implementations/dask.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/data.py` & `fsspec-2024.3.1/fsspec/implementations/data.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/dbfs.py` & `fsspec-2024.3.1/fsspec/implementations/dbfs.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/dirfs.py` & `fsspec-2024.3.1/fsspec/implementations/dirfs.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/ftp.py` & `fsspec-2024.3.1/fsspec/implementations/ftp.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/git.py` & `fsspec-2024.3.1/fsspec/implementations/git.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/github.py` & `fsspec-2024.3.1/fsspec/implementations/github.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/http.py` & `fsspec-2024.3.1/fsspec/implementations/http.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/jupyter.py` & `fsspec-2024.3.1/fsspec/implementations/jupyter.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/libarchive.py` & `fsspec-2024.3.1/fsspec/implementations/libarchive.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/local.py` & `fsspec-2024.3.1/fsspec/implementations/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import datetime
 import io
 import logging
 import os
 import os.path as osp
-import re
 import shutil
 import stat
 import tempfile
 
 from fsspec import AbstractFileSystem
 from fsspec.compression import compr
 from fsspec.core import get_compression
 from fsspec.utils import isfilelike, stringify_path
 
 logger = logging.getLogger("fsspec.local")
 
 
+def _remove_prefix(text: str, prefix: str):
+    if text.startswith(prefix):
+        return text[len(prefix) :]
+    return text
+
+
 class LocalFileSystem(AbstractFileSystem):
     """Interface to files on local storage
 
     Parameters
     ----------
     auto_mkdir: bool
         Whether, when opening a file, the directory containing it should
@@ -112,38 +117,46 @@
                 result["size"] = 0
         return result
 
     def lexists(self, path, **kwargs):
         return osp.lexists(path)
 
     def cp_file(self, path1, path2, **kwargs):
-        path1 = self._strip_protocol(path1).rstrip("/")
-        path2 = self._strip_protocol(path2).rstrip("/")
+        path1 = self._strip_protocol(path1, remove_trailing_slash=True)
+        path2 = self._strip_protocol(path2, remove_trailing_slash=True)
         if self.auto_mkdir:
             self.makedirs(self._parent(path2), exist_ok=True)
         if self.isfile(path1):
             shutil.copyfile(path1, path2)
         elif self.isdir(path1):
             self.mkdirs(path2, exist_ok=True)
         else:
             raise FileNotFoundError(path1)
 
+    def isfile(self, path):
+        path = self._strip_protocol(path)
+        return os.path.isfile(path)
+
+    def isdir(self, path):
+        path = self._strip_protocol(path)
+        return os.path.isdir(path)
+
     def get_file(self, path1, path2, callback=None, **kwargs):
         if isfilelike(path2):
             with open(path1, "rb") as f:
                 shutil.copyfileobj(f, path2)
         else:
             return self.cp_file(path1, path2, **kwargs)
 
     def put_file(self, path1, path2, callback=None, **kwargs):
         return self.cp_file(path1, path2, **kwargs)
 
     def mv_file(self, path1, path2, **kwargs):
-        path1 = self._strip_protocol(path1).rstrip("/")
-        path2 = self._strip_protocol(path2).rstrip("/")
+        path1 = self._strip_protocol(path1, remove_trailing_slash=True)
+        path2 = self._strip_protocol(path2, remove_trailing_slash=True)
         shutil.move(path1, path2)
 
     def link(self, src, dst, **kwargs):
         src = self._strip_protocol(src)
         dst = self._strip_protocol(dst)
         os.link(src, dst, **kwargs)
 
@@ -159,15 +172,15 @@
         os.remove(self._strip_protocol(path))
 
     def rm(self, path, recursive=False, maxdepth=None):
         if not isinstance(path, list):
             path = [path]
 
         for p in path:
-            p = self._strip_protocol(p).rstrip("/")
+            p = self._strip_protocol(p, remove_trailing_slash=True)
             if self.isdir(p):
                 if not recursive:
                     raise ValueError("Cannot delete directory, set recursive=True")
                 if osp.abspath(p) == os.getcwd():
                     raise ValueError("Cannot delete current working directory")
                 shutil.rmtree(p)
             else:
@@ -202,85 +215,88 @@
 
     def modified(self, path):
         info = self.info(path=path)
         return datetime.datetime.fromtimestamp(info["mtime"], tz=datetime.timezone.utc)
 
     @classmethod
     def _parent(cls, path):
-        path = cls._strip_protocol(path).rstrip("/")
-        if "/" in path:
-            return path.rsplit("/", 1)[0]
+        path = cls._strip_protocol(path, remove_trailing_slash=True)
+        if os.sep == "/":
+            # posix native
+            return path.rsplit("/", 1)[0] or "/"
         else:
-            return cls.root_marker
+            # NT
+            path_ = path.rsplit("/", 1)[0]
+            if len(path_) <= 3:
+                if path_[1:2] == ":":
+                    # nt root (something like c:/)
+                    return path_[0] + ":/"
+            # More cases may be required here
+            return path_
 
     @classmethod
-    def _strip_protocol(cls, path):
+    def _strip_protocol(cls, path, remove_trailing_slash=False):
         path = stringify_path(path)
-        if path.startswith("file://"):
-            path = path[7:]
-        elif path.startswith("file:"):
-            path = path[5:]
-        elif path.startswith("local://"):
-            path = path[8:]
+        if path.startswith("file:"):
+            path = _remove_prefix(_remove_prefix(path, "file://"), "file:")
+            if os.sep == "\\":
+                path = path.lstrip("/")
         elif path.startswith("local:"):
-            path = path[6:]
-        return make_path_posix(path).rstrip("/") or cls.root_marker
+            path = _remove_prefix(_remove_prefix(path, "local://"), "local:")
+            if os.sep == "\\":
+                path = path.lstrip("/")
+        return make_path_posix(path, remove_trailing_slash)
 
     def _isfilestore(self):
         # Inheriting from DaskFileSystem makes this False (S3, etc. were)
         # the original motivation. But we are a posix-like file system.
         # See https://github.com/dask/dask/issues/5526
         return True
 
     def chmod(self, path, mode):
         path = stringify_path(path)
         return os.chmod(path, mode)
 
 
-def make_path_posix(path, sep=os.sep):
-    """Make path generic"""
-    if isinstance(path, (list, set, tuple)):
-        return type(path)(make_path_posix(p) for p in path)
-    if "~" in path:
-        path = osp.expanduser(path)
-    if sep == "/":
-        # most common fast case for posix
+def make_path_posix(path, remove_trailing_slash=False):
+    """Make path generic for current OS"""
+    if not isinstance(path, str):
+        if isinstance(path, (list, set, tuple)):
+            return type(path)(make_path_posix(p, remove_trailing_slash) for p in path)
+        else:
+            path = str(stringify_path(path))
+    if os.sep == "/":
+        # Native posix
         if path.startswith("/"):
-            return path
-        if path.startswith("./"):
+            # most common fast case for posix
+            return path.rstrip("/") or "/" if remove_trailing_slash else path
+        elif path.startswith("~"):
+            return make_path_posix(osp.expanduser(path), remove_trailing_slash)
+        elif path.startswith("./"):
             path = path[2:]
+            path = f"{os.getcwd()}/{path}"
+            return path.rstrip("/") or "/" if remove_trailing_slash else path
         return f"{os.getcwd()}/{path}"
-    if (
-        (sep not in path and "/" not in path)
-        or (sep == "/" and not path.startswith("/"))
-        or (sep == "\\" and ":" not in path and not path.startswith("\\\\"))
-    ):
-        # relative path like "path" or "rel\\path" (win) or rel/path"
-        if os.sep == "\\":
-            # abspath made some more '\\' separators
-            return make_path_posix(osp.abspath(path))
-        else:
-            return f"{os.getcwd()}/{path}"
-    if path.startswith("file://"):
-        path = path[7:]
-    if re.match("/[A-Za-z]:", path):
-        # for windows file URI like "file:///C:/folder/file"
-        # or "file:///C:\\dir\\file"
-        path = path[1:].replace("\\", "/").replace("//", "/")
-    if path.startswith("\\\\"):
-        # special case for windows UNC/DFS-style paths, do nothing,
-        # just flip the slashes around (case below does not work!)
-        return path.replace("\\", "/")
-    if re.match("[A-Za-z]:", path):
-        # windows full path like "C:\\local\\path"
-        return path.lstrip("\\").replace("\\", "/").replace("//", "/")
-    if path.startswith("\\"):
-        # windows network path like "\\server\\path"
-        return "/" + path.lstrip("\\").replace("\\", "/").replace("//", "/")
-    return path
+    else:
+        # NT handling
+        if len(path) > 1:
+            if path[1] == ":":
+                # windows full path like "C:\\local\\path"
+                if len(path) <= 3:
+                    # nt root (something like c:/)
+                    return path[0] + ":/"
+                path = path.replace("\\", "/").replace("//", "/")
+                return path.rstrip("/") if remove_trailing_slash else path
+            elif path[0] == "~":
+                return make_path_posix(osp.expanduser(path), remove_trailing_slash)
+            elif path.startswith(("\\\\", "//")):
+                # windows UNC/DFS-style paths
+                path = "//" + path[2:].replace("\\", "/").replace("//", "/")
+                return path.rstrip("/") if remove_trailing_slash else path
+        return make_path_posix(osp.abspath(path), remove_trailing_slash)
 
 
 def trailing_sep(path):
     """Return True if the path ends with a path separator.
 
     A forward slash is always considered a path separator, even on Operating
     Systems that normally use a backslash.
```

### Comparing `fsspec-2024.3.0/fsspec/implementations/memory.py` & `fsspec-2024.3.1/fsspec/implementations/memory.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/reference.py` & `fsspec-2024.3.1/fsspec/implementations/reference.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/sftp.py` & `fsspec-2024.3.1/fsspec/implementations/sftp.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/smb.py` & `fsspec-2024.3.1/fsspec/implementations/smb.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/tar.py` & `fsspec-2024.3.1/fsspec/implementations/tar.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/webhdfs.py` & `fsspec-2024.3.1/fsspec/implementations/webhdfs.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/implementations/zip.py` & `fsspec-2024.3.1/fsspec/implementations/zip.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/mapping.py` & `fsspec-2024.3.1/fsspec/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ['loc1']
     >>> d['loc1']  # doctest: +SKIP
     b'Hello World'
     """
 
     def __init__(self, root, fs, check=False, create=False, missing_exceptions=None):
         self.fs = fs
-        self.root = fs._strip_protocol(root).rstrip("/")
+        self.root = fs._strip_protocol(root)
         self._root_key_to_str = fs._strip_protocol(posixpath.join(root, "x"))[:-1]
         if missing_exceptions is None:
             missing_exceptions = (
                 FileNotFoundError,
                 IsADirectoryError,
                 NotADirectoryError,
             )
@@ -138,15 +138,15 @@
             warnings.warn(
                 "from fsspec 2023.5 onward FSMap non-str keys will raise TypeError",
                 DeprecationWarning,
             )
             if isinstance(key, list):
                 key = tuple(key)
             key = str(key)
-        return f"{self._root_key_to_str}{key}"
+        return f"{self._root_key_to_str}{key}".rstrip("/")
 
     def _str_to_key(self, s):
         """Strip path of to leave key name"""
         return s[len(self.root) :].lstrip("/")
 
     def __getitem__(self, key, default=None):
         """Retrieve data"""
```

### Comparing `fsspec-2024.3.0/fsspec/parquet.py` & `fsspec-2024.3.1/fsspec/parquet.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/registry.py` & `fsspec-2024.3.1/fsspec/registry.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/spec.py` & `fsspec-2024.3.1/fsspec/spec.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/tests/abstract/__init__.py` & `fsspec-2024.3.1/fsspec/tests/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/tests/abstract/common.py` & `fsspec-2024.3.1/fsspec/tests/abstract/common.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/tests/abstract/copy.py` & `fsspec-2024.3.1/fsspec/tests/abstract/copy.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/tests/abstract/get.py` & `fsspec-2024.3.1/fsspec/tests/abstract/get.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/tests/abstract/put.py` & `fsspec-2024.3.1/fsspec/tests/abstract/put.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/transaction.py` & `fsspec-2024.3.1/fsspec/transaction.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec/utils.py` & `fsspec-2024.3.1/fsspec/utils.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec.egg-info/PKG-INFO` & `fsspec-2024.3.1/fsspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec
-Version: 2024.3.0
+Version: 2024.3.1
 Summary: File-system specification
 Home-page: https://github.com/fsspec/filesystem_spec
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Project-URL: Changelog, https://filesystem-spec.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://filesystem-spec.readthedocs.io/en/latest/
```

### Comparing `fsspec-2024.3.0/fsspec.egg-info/SOURCES.txt` & `fsspec-2024.3.1/fsspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/fsspec.egg-info/requires.txt` & `fsspec-2024.3.1/fsspec.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/pyproject.toml` & `fsspec-2024.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/setup.cfg` & `fsspec-2024.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/setup.py` & `fsspec-2024.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `fsspec-2024.3.0/versioneer.py` & `fsspec-2024.3.1/versioneer.py`

 * *Files identical despite different names*

