# Comparing `tmp/ebi_eva_common_pyutils-0.6.6.tar.gz` & `tmp/ebi_eva_common_pyutils-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.6.6.tar", last modified: Mon Apr 15 15:13:43 2024, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.6.7.tar", last modified: Wed May 15 08:28:35 2024, max compression
```

## Comparing `ebi_eva_common_pyutils-0.6.6.tar` & `ebi_eva_common_pyutils-0.6.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.038334 ebi_eva_common_pyutils-0.6.6/
--rw-r--r--   0 tcezard    (502) staff       (20)     2993 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/CHANGELOG.md
--rw-r--r--   0 tcezard    (502) staff       (20)    11357 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/LICENSE
--rw-r--r--   0 tcezard    (502) staff       (20)       28 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/MANIFEST.in
--rw-r--r--   0 tcezard    (502) staff       (20)      541 2024-04-15 15:13:43.038497 ebi_eva_common_pyutils-0.6.6/PKG-INFO
--rw-r--r--   0 tcezard    (502) staff       (20)     1434 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/README.md
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.026939 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/__init__.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.029814 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly/
--rw-r--r--   0 tcezard    (502) staff       (20)       67 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3142 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly/assembly.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4187 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2340 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/command_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     1192 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/common_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4828 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/config.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.030782 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/contig_alias/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3056 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-r--r--   0 tcezard    (502) staff       (20)     1465 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/ena_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     1375 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/file_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     5093 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/logger.py
--rw-r--r--   0 tcezard    (502) staff       (20)     5005 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/ncbi_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2648 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/network_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.032161 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/
--rw-r--r--   0 tcezard    (502) staff       (20)      134 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)    12162 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/assembly.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3911 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/sequence.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.032864 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/taxonomy/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2259 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.033541 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/variation/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/variation/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     5230 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.029012 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 tcezard    (502) staff       (20)      541 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 tcezard    (502) staff       (20)     1653 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 tcezard    (502) staff       (20)        1 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 tcezard    (502) staff       (20)       97 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-r--r--   0 tcezard    (502) staff       (20)       48 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/top_level.txt
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.036237 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4989 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/archive_directory.py
--rw-r--r--   0 tcezard    (502) staff       (20)     7909 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/config_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)    15221 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/metadata_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3575 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongo_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.037125 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongodb/
--rw-r--r--   0 tcezard    (502) staff       (20)       76 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongodb/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     9596 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongodb/mongo_database.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-04-15 15:13:43.037942 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/nextflow/
--rw-r--r--   0 tcezard    (502) staff       (20)      122 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/nextflow/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)    10114 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4398 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/pg_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)    15265 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/spring_properties.py
--rw-r--r--   0 tcezard    (502) staff       (20)      225 2024-04-15 15:13:43.039066 ebi_eva_common_pyutils-0.6.6/setup.cfg
--rw-r--r--   0 tcezard    (502) staff       (20)      926 2024-04-15 15:13:42.000000 ebi_eva_common_pyutils-0.6.6/setup.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.382071 ebi_eva_common_pyutils-0.6.7/
+-rw-r--r--   0 tcezard    (502) staff       (20)     3132 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/CHANGELOG.md
+-rw-r--r--   0 tcezard    (502) staff       (20)    11357 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/LICENSE
+-rw-r--r--   0 tcezard    (502) staff       (20)       28 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/MANIFEST.in
+-rw-r--r--   0 tcezard    (502) staff       (20)      541 2024-05-15 08:28:35.382227 ebi_eva_common_pyutils-0.6.7/PKG-INFO
+-rw-r--r--   0 tcezard    (502) staff       (20)     1434 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/README.md
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.370707 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/__init__.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.373596 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/assembly/
+-rw-r--r--   0 tcezard    (502) staff       (20)       67 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     3142 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     4187 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/assembly_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     2340 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/command_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     1192 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/common_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     4828 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/config.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.374458 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/contig_alias/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     3056 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     1465 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/ena_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     1375 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/file_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     5093 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/logger.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     5005 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     2648 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/network_utils.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.375822 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/reference/
+-rw-r--r--   0 tcezard    (502) staff       (20)      134 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/reference/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)    12162 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/reference/assembly.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     3911 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/reference/sequence.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.376512 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/taxonomy/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     2259 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.377177 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/variation/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/variation/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     5230 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.372806 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 tcezard    (502) staff       (20)      541 2024-05-15 08:28:35.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 tcezard    (502) staff       (20)     1653 2024-05-15 08:28:35.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 tcezard    (502) staff       (20)        1 2024-05-15 08:28:35.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 tcezard    (502) staff       (20)       97 2024-05-15 08:28:35.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-r--r--   0 tcezard    (502) staff       (20)       48 2024-05-15 08:28:35.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils.egg-info/top_level.txt
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.379799 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/
+-rw-r--r--   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     4989 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/archive_directory.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     7909 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/config_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)    15221 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/metadata_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     3575 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/mongo_utils.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.380633 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/mongodb/
+-rw-r--r--   0 tcezard    (502) staff       (20)       76 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/mongodb/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     9596 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/mongodb/mongo_database.py
+drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2024-05-15 08:28:35.381529 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/nextflow/
+-rw-r--r--   0 tcezard    (502) staff       (20)      122 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/nextflow/__init__.py
+-rw-r--r--   0 tcezard    (502) staff       (20)    10114 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py
+-rw-r--r--   0 tcezard    (502) staff       (20)     4398 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/pg_utils.py
+-rw-r--r--   0 tcezard    (502) staff       (20)    15161 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/spring_properties.py
+-rw-r--r--   0 tcezard    (502) staff       (20)      225 2024-05-15 08:28:35.382839 ebi_eva_common_pyutils-0.6.7/setup.cfg
+-rw-r--r--   0 tcezard    (502) staff       (20)      926 2024-05-15 08:28:34.000000 ebi_eva_common_pyutils-0.6.7/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.6.6/CHANGELOG.md` & `ebi_eva_common_pyutils-0.6.7/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 Changelog for ebi_eva_common_pyutils
 ===========================
 
+## 0.6.7 (2024-05-15)
+---------------------
+
+- Remove the instance id and add required dummy cutoff day for accessioning and clustering 
+
+
 ## 0.6.6 (2024-04-15)
 ---------------------
 
 - Allow NCBI function ot use API key
 
 
 ## 0.6.5 (2024-04-02)
```

### Comparing `ebi_eva_common_pyutils-0.6.6/LICENSE` & `ebi_eva_common_pyutils-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/PKG-INFO` & `ebi_eva_common_pyutils-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi_eva_common_pyutils
-Version: 0.6.6
+Version: 0.6.7
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ebi_eva_common_pyutils-0.6.6/README.md` & `ebi_eva_common_pyutils-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/assembly_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/PKG-INFO` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi-eva-common-pyutils
-Version: 0.6.6
+Version: 0.6.7
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.6.6/ebi_eva_internal_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.6.7/ebi_eva_internal_pyutils/spring_properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,36 +113,37 @@
             'spring.data.mongodb.database': accession_db,
             'parameters.assemblyAccession': assembly_accession,
         }
 
         merge = {**self._common_properties(read_preference=read_preference, chunk_size=chunk_size), **props}
         return merge
 
-    def _common_accessioning_clustering_properties(self, *, instance='', assembly_accession, read_preference, chunk_size):
+    def _common_accessioning_clustering_properties(self, *, assembly_accession, read_preference, chunk_size):
         """Properties common to accessioning and clustering pipelines."""
         props = {
-            'accessioning.instanceId': self._format_str('instance-{0}', instance),
             'accessioning.submitted.categoryId': 'ss',
             'accessioning.clustered.categoryId': 'rs',
             'accessioning.monotonic.ss.blockSize': 100000,
             'accessioning.monotonic.ss.blockStartValue': 5000000000,
             'accessioning.monotonic.ss.nextBlockInterval': 1000000000,
             'accessioning.monotonic.rs.blockSize': 100000,
             'accessioning.monotonic.rs.blockStartValue': 3000000000,
             'accessioning.monotonic.rs.nextBlockInterval': 1000000000,
+            # This value is not used but is required to create beans in Java
+            'recovery.cutoff.days': 9999999
         }
         merge = {**self._common_accessioning_properties(assembly_accession, read_preference, chunk_size), **props}
         return merge
 
-    def get_accessioning_properties(self, *, instance=None, target_assembly=None, fasta=None, assembly_report=None,
+    def get_accessioning_properties(self, *, target_assembly=None, fasta=None, assembly_report=None,
                                     project_accession=None, aggregation='BASIC', taxonomy_accession=None,
                                     vcf_file='', output_vcf='', chunk_size=100):
         """Properties for accessioning pipeline."""
         return self._format(
-            self._common_accessioning_clustering_properties(instance=instance, assembly_accession=target_assembly,
+            self._common_accessioning_clustering_properties(assembly_accession=target_assembly,
                                                             read_preference='secondaryPreferred', chunk_size=chunk_size),
             {
                 'spring.batch.job.names': 'CREATE_SUBSNP_ACCESSION_JOB',
                 'parameters.assemblyReportUrl': self._format_str('file:{0}', assembly_report),
                 'parameters.contigNaming': 'NO_REPLACEMENT',
                 'parameters.fasta': fasta,
                 'parameters.forceRestart': 'false',
@@ -150,29 +151,28 @@
                 'parameters.taxonomyAccession': taxonomy_accession,
                 'parameters.vcfAggregation': aggregation,
                 'parameters.vcf': vcf_file,
                 'parameters.outputVcf': output_vcf
             },
         )
 
-    def get_clustering_properties(self, *, instance=None, read_preference='primary',
-                                  job_name=None, source_assembly='', target_assembly='', rs_report_path='', projects='',
+    def get_clustering_properties(self, *, read_preference='primary', job_name=None, source_assembly='',
+                                  target_assembly='', rs_report_path='', projects='',
                                   project_accession='', vcf=''):
         """Properties common to all clustering pipelines, though not all are always used."""
         return self._format(
-            self._common_accessioning_clustering_properties(instance=instance, assembly_accession=target_assembly,
-                                                            read_preference=read_preference, chunk_size=100,
-                                                            ),
+            self._common_accessioning_clustering_properties(assembly_accession=target_assembly,
+                                                            read_preference=read_preference, chunk_size=100),
             {
                 'spring.batch.job.names': job_name,
                 'parameters.remappedFrom': source_assembly,
                 'parameters.projects': projects,
                 'parameters.projectAccession': project_accession,
                 'parameters.vcf': vcf,
-                'parameters.rsReportPath': rs_report_path
+                'parameters.rsReportPath': rs_report_path,
             }
         )
 
     def get_remapping_extraction_properties(self, *, taxonomy=None, source_assembly=None, fasta=None,
                                             assembly_report=None,
                                             projects='', output_folder=None):
         """Properties for remapping extraction pipeline."""
```

### Comparing `ebi_eva_common_pyutils-0.6.6/setup.py` & `ebi_eva_common_pyutils-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_internal_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.6.6',
+    version='0.6.7',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['requests', 'lxml', 'pyyaml', 'cached-property', 'retry'],
     extras_require={'eva-internal': ['psycopg2-binary', 'pymongo', 'networkx<=2.5']},
     classifiers=[
```

