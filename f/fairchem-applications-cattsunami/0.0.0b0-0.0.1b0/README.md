# Comparing `tmp/fairchem_applications_cattsunami-0.0.0b0.tar.gz` & `tmp/fairchem_applications_cattsunami-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairchem_applications_cattsunami-0.0.0b0.tar", last modified: Mon May 13 23:55:35 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fairchem_applications_cattsunami-0.0.0b0.tar` & `fairchem_applications_cattsunami-0.0.1b0.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-13 23:55:35.215869 fairchem_applications_cattsunami-0.0.0b0/
--rw-r--r--   0 lbluque    (501) staff       (20)      220 2024-05-13 23:55:35.214244 fairchem_applications_cattsunami-0.0.0b0/PKG-INFO
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-13 23:55:35.202590 fairchem_applications_cattsunami-0.0.0b0/fairchem/
--rw-r--r--   0 lbluque    (501) staff       (20)        0 2024-05-09 23:33:00.000000 fairchem_applications_cattsunami-0.0.0b0/fairchem/__init__.py
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-13 23:55:35.213275 fairchem_applications_cattsunami-0.0.0b0/fairchem_applications_cattsunami.egg-info/
--rw-r--r--   0 lbluque    (501) staff       (20)      220 2024-05-13 23:55:35.000000 fairchem_applications_cattsunami-0.0.0b0/fairchem_applications_cattsunami.egg-info/PKG-INFO
--rw-r--r--   0 lbluque    (501) staff       (20)      259 2024-05-13 23:55:35.000000 fairchem_applications_cattsunami-0.0.0b0/fairchem_applications_cattsunami.egg-info/SOURCES.txt
--rw-r--r--   0 lbluque    (501) staff       (20)        1 2024-05-13 23:55:35.000000 fairchem_applications_cattsunami-0.0.0b0/fairchem_applications_cattsunami.egg-info/dependency_links.txt
--rw-r--r--   0 lbluque    (501) staff       (20)        9 2024-05-13 23:55:35.000000 fairchem_applications_cattsunami-0.0.0b0/fairchem_applications_cattsunami.egg-info/top_level.txt
--rw-r--r--   0 lbluque    (501) staff       (20)      290 2024-05-13 23:55:13.000000 fairchem_applications_cattsunami-0.0.0b0/pyproject.toml
--rw-r--r--   0 lbluque    (501) staff       (20)       38 2024-05-13 23:55:35.216020 fairchem_applications_cattsunami-0.0.0b0/setup.cfg
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/DATASET.md
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/README.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/__init__.py
+-rw-r--r--   0        0        0   771334 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/summary_fig.png
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/__init__.py
+-rw-r--r--   0        0        0    69388 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/autoframe.py
+-rw-r--r--   0        0        0    11428 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/ocpneb.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/reaction.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/__init__.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/desorptions_9Aug23.pkl
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/dissociation_reactions_20Oct23.pkl
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/transfers_5Sept23.pkl
+-rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/run_validation.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/run_validation.sh
+-rw-r--r--   0        0        0    35873 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/mapping_files/desorption_mapping.pkl
+-rw-r--r--   0        0        0    41063 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/mapping_files/dissociation_mapping.pkl
+-rw-r--r--   0        0        0    50571 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/mapping_files/transfer_mapping.pkl
+-rw-r--r--   0        0        0    82245 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/tutorial/dissociation_scheme.png
+-rw-r--r--   0        0        0    10757 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/tutorial/workbook.ipynb
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/PKG-INFO
```

