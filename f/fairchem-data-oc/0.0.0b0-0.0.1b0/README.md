# Comparing `tmp/fairchem_data_oc-0.0.0b0.tar.gz` & `tmp/fairchem_data_oc-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairchem_data_oc-0.0.0b0.tar", last modified: Mon May 13 23:57:55 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fairchem_data_oc-0.0.0b0.tar` & `fairchem_data_oc-0.0.1b0.tar`

### file list

```diff
@@ -1,11 +1,28 @@
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-13 23:57:55.134973 fairchem_data_oc-0.0.0b0/
--rw-r--r--   0 lbluque    (501) staff       (20)      204 2024-05-13 23:57:55.134313 fairchem_data_oc-0.0.0b0/PKG-INFO
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-13 23:57:55.128678 fairchem_data_oc-0.0.0b0/fairchem/
--rw-r--r--   0 lbluque    (501) staff       (20)        0 2024-05-09 23:33:00.000000 fairchem_data_oc-0.0.0b0/fairchem/__init__.py
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-13 23:57:55.133689 fairchem_data_oc-0.0.0b0/fairchem_data_oc.egg-info/
--rw-r--r--   0 lbluque    (501) staff       (20)      204 2024-05-13 23:57:55.000000 fairchem_data_oc-0.0.0b0/fairchem_data_oc.egg-info/PKG-INFO
--rw-r--r--   0 lbluque    (501) staff       (20)      195 2024-05-13 23:57:55.000000 fairchem_data_oc-0.0.0b0/fairchem_data_oc.egg-info/SOURCES.txt
--rw-r--r--   0 lbluque    (501) staff       (20)        1 2024-05-13 23:57:55.000000 fairchem_data_oc-0.0.0b0/fairchem_data_oc.egg-info/dependency_links.txt
--rw-r--r--   0 lbluque    (501) staff       (20)        9 2024-05-13 23:57:55.000000 fairchem_data_oc-0.0.0b0/fairchem_data_oc.egg-info/top_level.txt
--rw-r--r--   0 lbluque    (501) staff       (20)      274 2024-05-13 23:57:49.000000 fairchem_data_oc-0.0.0b0/pyproject.toml
--rw-r--r--   0 lbluque    (501) staff       (20)       38 2024-05-13 23:57:55.135047 fairchem_data_oc-0.0.0b0/setup.cfg
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/.flake8
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/LICENSE.md
+-rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/README.md
+-rw-r--r--   0        0        0     8795 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/README_legacy_OC20.md
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/codecov.yml
+-rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/ocdata_workflow.png
+-rw-r--r--   0        0        0    14359 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/structure_generator.py
+-rw-r--r--   0        0        0    58230 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/workflow_image.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/__init__.py
+-rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/adsorbate.py
+-rw-r--r--   0        0        0    21903 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/adsorbate_slab_config.py
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/bulk.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/multi_adsorbate_slab_config.py
+-rw-r--r--   0        0        0    21698 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/slab.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/__init__.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/update.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/pkls/__init__.py
+-rw-r--r--   0        0        0    52517 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/pkls/adsorbates.pkl
+-rw-r--r--   0        0        0 36088635 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/pkls/bulks.pkl
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/scripts/precompute_sample_structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/tests/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/utils/__init__.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/utils/flag_anomaly.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/utils/vasp.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/PKG-INFO
```

