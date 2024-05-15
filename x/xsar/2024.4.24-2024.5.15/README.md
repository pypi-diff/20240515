# Comparing `tmp/xsar-2024.4.24.tar.gz` & `tmp/xsar-2024.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsar-2024.4.24.tar", last modified: Wed Apr 24 18:35:35 2024, max compression
+gzip compressed data, was "xsar-2024.5.15.tar", last modified: Wed May 15 08:50:43 2024, max compression
```

## Comparing `xsar-2024.4.24.tar` & `xsar-2024.5.15.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.562019 xsar-2024.4.24/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 18:35:25.000000 xsar-2024.4.24/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-24 18:35:25.000000 xsar-2024.4.24/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 18:35:25.000000 xsar-2024.4.24/.gitconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/.github/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/actions/dynamic_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/workflows/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/workflows/conda-feedstock-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/workflows/install-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-24 18:35:25.000000 xsar-2024.4.24/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-24 18:35:25.000000 xsar-2024.4.24/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 18:35:25.000000 xsar-2024.4.24/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-24 18:35:25.000000 xsar-2024.4.24/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 18:35:25.000000 xsar-2024.4.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 18:35:25.000000 xsar-2024.4.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 18:35:35.562019 xsar-2024.4.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-24 18:35:25.000000 xsar-2024.4.24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-24 18:35:25.000000 xsar-2024.4.24/README_dev.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 18:35:25.000000 xsar-2024.4.24/condarc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.546019 xsar-2024.4.24/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/_static/css/xsar.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.554019 xsar-2024.4.24/docs/_static/uml/
--rw-r--r--   0 runner    (1001) docker     (127)   856119 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/_static/uml/classes_all_attributes.png
--rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/_static/uml/packages_all_attributes.png
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.554019 xsar-2024.4.24/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/mask.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/projections.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/radarsat2.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19403 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/rcm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar_advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   664426 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar_batch_datarmor.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar_multiple.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar_tops_slc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/uml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-24 18:35:25.000000 xsar-2024.4.24/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.554019 xsar-2024.4.24/highlevel-checks/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-24 18:35:25.000000 xsar-2024.4.24/highlevel-checks/check_s1_xsar_opendataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 18:35:25.000000 xsar-2024.4.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 18:35:25.000000 xsar-2024.4.24/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:35:35.562019 xsar-2024.4.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-24 18:35:25.000000 xsar-2024.4.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.546019 xsar-2024.4.24/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.554019 xsar-2024.4.24/src/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4082 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/scripts/compress_safe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.558019 xsar-2024.4.24/src/xsar/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37154 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/base_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/ipython_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)    32278 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/radarsat2_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/radarsat2_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/raster_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    34783 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/rcm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/rcm_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    68497 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/sentinel1_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/sentinel1_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/xarray_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/xsar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.558019 xsar-2024.4.24/src/xsar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.558019 xsar-2024.4.24/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-24 18:35:25.000000 xsar-2024.4.24/test/test_raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.616173 xsar-2024.5.15/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 08:50:32.000000 xsar-2024.5.15/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 08:50:32.000000 xsar-2024.5.15/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-15 08:50:32.000000 xsar-2024.5.15/.gitconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/.github/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/actions/dynamic_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/workflows/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/workflows/conda-feedstock-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/workflows/install-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-15 08:50:32.000000 xsar-2024.5.15/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-15 08:50:32.000000 xsar-2024.5.15/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-15 08:50:32.000000 xsar-2024.5.15/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 08:50:32.000000 xsar-2024.5.15/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 08:50:32.000000 xsar-2024.5.15/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 08:50:32.000000 xsar-2024.5.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 08:50:32.000000 xsar-2024.5.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 08:50:43.616173 xsar-2024.5.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-15 08:50:32.000000 xsar-2024.5.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-15 08:50:32.000000 xsar-2024.5.15/README_dev.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 08:50:32.000000 xsar-2024.5.15/condarc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.604173 xsar-2024.5.15/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/_static/css/xsar.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.608173 xsar-2024.5.15/docs/_static/uml/
+-rw-r--r--   0 runner    (1001) docker     (127)   856119 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/_static/uml/classes_all_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/_static/uml/packages_all_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.612173 xsar-2024.5.15/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/mask.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/projections.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/radarsat2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19403 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/rcm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar_advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   664426 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar_batch_datarmor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar_multiple.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/examples/xsar_tops_slc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 08:50:32.000000 xsar-2024.5.15/docs/uml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 08:50:32.000000 xsar-2024.5.15/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.612173 xsar-2024.5.15/highlevel-checks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 08:50:32.000000 xsar-2024.5.15/highlevel-checks/check_s1_xsar_opendataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 08:50:32.000000 xsar-2024.5.15/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-15 08:50:32.000000 xsar-2024.5.15/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:50:43.616173 xsar-2024.5.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-15 08:50:32.000000 xsar-2024.5.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.604173 xsar-2024.5.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.612173 xsar-2024.5.15/src/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4082 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/scripts/compress_safe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.616173 xsar-2024.5.15/src/xsar/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37154 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/base_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/ipython_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32278 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/radarsat2_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/radarsat2_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/raster_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34783 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/rcm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/rcm_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72519 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/sentinel1_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/sentinel1_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/xarray_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-15 08:50:32.000000 xsar-2024.5.15/src/xsar/xsar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.616173 xsar-2024.5.15/src/xsar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 08:50:43.000000 xsar-2024.5.15/src/xsar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:50:43.616173 xsar-2024.5.15/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-15 08:50:32.000000 xsar-2024.5.15/test/test_raster_readers.py
```

### Comparing `xsar-2024.4.24/.github/actions/dynamic_matrix.py` & `xsar-2024.5.15/.github/actions/dynamic_matrix.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/.github/workflows/README.md` & `xsar-2024.5.15/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/.github/workflows/conda-feedstock-check.yml` & `xsar-2024.5.15/.github/workflows/conda-feedstock-check.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/.github/workflows/install-test.yml` & `xsar-2024.5.15/.github/workflows/install-test.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/.github/workflows/publish.yml` & `xsar-2024.5.15/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/.gitignore` & `xsar-2024.5.15/.gitignore`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/.gitlab-ci.yml` & `xsar-2024.5.15/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/Dockerfile` & `xsar-2024.5.15/Dockerfile`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/LICENSE` & `xsar-2024.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/PKG-INFO` & `xsar-2024.5.15/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsar
-Version: 2024.4.24
+Version: 2024.5.15
 Summary: xarray L1 SAR mapper
 Home-page: https://github.com/umr-lops/xsar
 Author: Olivier Archer, Alexandre Levieux, Antoine Grouazel
 Author-email: Olivier.Archer@ifremer.fr, Alexandre.Levieux@gmail.com, Antoine.Grouazel@ifremer.fr
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `xsar-2024.4.24/README.md` & `xsar-2024.5.15/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,61 @@
 ![Install test](https://github.com/umr-lops/xsar/actions/workflows/install-test.yml/badge.svg)
 # xsar
 
 Synthetic Aperture Radar (SAR) Level-1 GRD python mapper for efficient xarray/dask based processing
 
- 
+This python library allow to apply different operation on SAR images such as:
+ - calibration
+ - de-noising
+ - re-sampling
+
+The library is working regardless it is a **Sentinel-1**, a **RadarSAT-2** or a **RCM** product.
+
+The library is providing variables such as `longitude` , `latitude`, `incidence_angle` or `sigma0` at native product resolution or coarser resolution.
+
+The library perform resampling that are suitable for GRD (i.e. ground projected) SAR images. The same method is used for WV SLC, and one can consider the approximation still valid because the WV image is only 20 km X 20 km.
+
+But for TOPS (IW or EW) SLC products we recommend to use [xsarslc](https://github.com/umr-lops/xsar_slc.git)
 
 # Install
 
 ## Conda
 
 1) Install `xsar` (without the readers)
 
 For a faster installation and less conflicts between packages, it is better
-to make the installation with `mamba`
+to make the installation with `micromamba`
 
 ```bash
 conda install -c conda-forge mamba
 ```
 
 2) install `xsar` (without the readers)
 
 ```bash
-mamba install -c conda-forge xsar
+micromamba install -c conda-forge xsar
 ```
 3) Add optional dependencies
 
 - Add use of Radarsat-2 :
 
 ```bash
-mamba install -c conda-forge xradarsat2
+micromamba install -c conda-forge xradarsat2
 ```
 
 - Add use of RCM (RadarSat Constellation Mission)
 
 ```bash
 pip install xarray-safe-rcm
 ```
 
 - Add use of Sentinel-1
 
 ```bash
-mamba install -c conda-forge xarray-safe-s1
+micromamba install -c conda-forge xarray-safe-s1
 ```
 
 ## Pypi
 
 1) install `xsar` (this will only allow to use Sentinel-1)
 
 ```bash
@@ -121,8 +132,7 @@
 ```
 
 
 
 # More information
 
 For more install options and to use xsar, see [documentation](https://cyclobs.ifremer.fr/static/sarwing_datarmor/xsar/)
-
```

### Comparing `xsar-2024.4.24/README_dev.md` & `xsar-2024.5.15/README_dev.md`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/Makefile` & `xsar-2024.5.15/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/_static/uml/classes_all_attributes.png` & `xsar-2024.5.15/docs/_static/uml/classes_all_attributes.png`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/_static/uml/packages_all_attributes.png` & `xsar-2024.5.15/docs/_static/uml/packages_all_attributes.png`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/basic_api.rst` & `xsar-2024.5.15/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/conf.py` & `xsar-2024.5.15/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/examples/mask.ipynb` & `xsar-2024.5.15/docs/examples/mask.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/examples/projections.ipynb` & `xsar-2024.5.15/docs/examples/projections.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989375858516484%*

 * *Differences: {"'cells'": '{11: {\'source\': {insert: [(2, "(gv.tile_sources.EsriImagery * sigma0_image * '*

 * *            'gv.feature.coastline.options(scale=\'10m\')).opts(width=600,height=600)")], delete: '*

 * *            '[2]}}, 13: {\'source\': ["s0vvproj = sigma0_proj.sel(pol=\'VV\')\\n", '*

 * *            '"s0vvproj.attrs[\'name\'] = \'sigma0 VV projected using rioxarray\'\\n", '*

 * *            '"s0vvproj.rio.to_raster(\'/tmp/sigma0_nocolor.tiff\')"]}, 15: {\'source\': {insert: '*

 * *            '[(5, "gv.tile_sources.EsriImagery  […]*

```diff
@@ -142,15 +142,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "sigma0_image = gv.Image(sigma0_proj.sel(pol='VV')).opts(alpha=0.3, cmap='gray', clim=(0,0.05))\n",
                 "#(gv.tile_sources.Wikipedia * gv.feature.land.options(scale='50m') * sigma0_image).opts(width=600,height=600)\n",
-                "(gv.tile_sources.Wikipedia * sigma0_image * gv.feature.coastline.options(scale='10m')).opts(width=600,height=600)"
+                "(gv.tile_sources.EsriImagery * sigma0_image * gv.feature.coastline.options(scale='10m')).opts(width=600,height=600)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "604b45d7-fe32-40d0-bd34-686a41f1097d",
             "metadata": {},
             "source": [
@@ -166,15 +166,17 @@
             "execution_count": null,
             "id": "b9d8658b-a5e3-456f-b046-db180b01d48e",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "sigma0_proj.sel(pol='VV').rio.to_raster('/tmp/sigma0_nocolor.tiff')"
+                "s0vvproj = sigma0_proj.sel(pol='VV')\n",
+                "s0vvproj.attrs['name'] = 'sigma0 VV projected using rioxarray'\n",
+                "s0vvproj.rio.to_raster('/tmp/sigma0_nocolor.tiff')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2f872bee-95b4-4109-9f54-63da680bd3c9",
             "metadata": {},
             "source": [
@@ -191,15 +193,15 @@
             "outputs": [],
             "source": [
                 "#gv.tile_sources.Wikipedia * gv.load_tiff('/tmp/sigma0_nocolor.tiff').opts(alpha=0.7, cmap='gray', clim=(0,0.05))\n",
                 "import rioxarray\n",
                 "tmp = rioxarray.open_rasterio('/tmp/sigma0_nocolor.tiff')\n",
                 "tmp = tmp.rename('sigma0_nocolor')\n",
                 "tmp2 = gv.util.from_xarray(tmp)\n",
-                "gv.tile_sources.Wikipedia * gv.Image(tmp2,vdims='sigma0_nocolor',kdims=['x','y']).opts(alpha=0.7, cmap='gray', clim=(0,0.05),colorbar=True,width=500,height=200)"
+                "gv.tile_sources.EsriImagery * gv.Image(tmp2,kdims=['x','y']).opts(alpha=0.7, cmap='gray', clim=(0,0.05),colorbar=True,width=500,height=200) # vdims='sigma0_nocolor'"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b4e8fb2c-d7e9-4247-be51-c51686d423ad",
             "metadata": {},
             "source": [
@@ -246,34 +248,37 @@
             },
             "outputs": [],
             "source": [
                 "#xsar_obj.dataset['sigma0_rgba'] = rgb_sigma0 \n",
                 "rgb_sigma0.name = 'sigma0_rgba'\n",
                 "xsar_obj.datatree['measurement'] = xsar_obj.datatree['measurement'].assign(xr.merge([xsar_obj.dataset,rgb_sigma0]))\n",
                 "xsar_obj.recompute_attrs()\n",
-                "xsar_obj.dataset['sigma0_rgba'].rio.reproject('epsg:4326',shape=(1000,1000),nodata=0).rio.to_raster('/tmp/sigma0_color.tiff')"
+                "s0rgba = xsar_obj.dataset['sigma0_rgba'].rio.reproject('epsg:4326',shape=(1000,1000),nodata=0)\n",
+                "s0rgba.attrs['name'] = 'sigma0 RGBA projected using rioxarray'\n",
+                "s0rgba.rio.to_raster('/tmp/sigma0_color.tiff')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "13bf1e5b-4641-4536-b487-28d4062cf1dc",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# there is a transparency bug in geoviews (https://github.com/holoviz/geoviews/issues/571)\n",
                 "# but if loading this tiff in google earth, it should render properly\n",
                 "tmp = rioxarray.open_rasterio('/tmp/sigma0_color.tiff')\n",
-                "tmp = tmp.rename('sigma0_color').isel(band=0)\n",
-                "tmp2 = gv.util.from_xarray(tmp)\n",
-                "print(tmp2)\n",
+                "tmp = tmp.rename('sigma0_color').isel(band=1)\n",
+                "print(tmp)\n",
+                "# tmp2 = gv.util.from_xarray(tmp,vdims='sigma0_color')\n",
+                "# print('empt2\\n====================',tmp2)\n",
                 "# (gv.tile_sources.Wikipedia * gv.load_tiff('/tmp/sigma0_color.tiff')).opts(width=600,height=600)\n",
-                "(gv.tile_sources.Wikipedia * gv.Image(tmp2,vdims='sigma0_color',kdims=['x','y']).opts(cmap='magma',colorbar=True)).opts(width=600,height=600)"
+                "(gv.tile_sources.EsriImagery * gv.Image(tmp,vdims='sigma0_color',kdims=['x','y']).opts(cmap='magma',colorbar=True,tools=['hover'])).opts(width=600,height=600) # "
             ]
         },
         {
             "cell_type": "markdown",
             "id": "21a44ee7-e47f-4d95-a29c-2e29198b5cad",
             "metadata": {},
             "source": [
@@ -386,15 +391,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "merged_lonlat = merged_grid.rio.reproject(4326)\n",
                 "(\n",
-                "    gv.tile_sources.Wikipedia * gv.Image(merged_lonlat['spd']).opts(cmap='jet', alpha=0.3) \n",
+                "    gv.tile_sources.EsriImagery * gv.Image(merged_lonlat['spd']).opts(cmap='jet', alpha=0.3) \n",
                 "    * gv.Image(merged_lonlat['sigma0']).opts(cmap='gray', clim=(0,0.05), alpha=0.7)\n",
                 ").opts(width=600,height=600)\n",
                 "                                                           "
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `xsar-2024.4.24/docs/examples/radarsat2.ipynb` & `xsar-2024.5.15/docs/examples/radarsat2.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/examples/rcm.ipynb` & `xsar-2024.5.15/docs/examples/rcm.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/examples/xsar.ipynb` & `xsar-2024.5.15/docs/examples/xsar.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/examples/xsar_advanced.ipynb` & `xsar-2024.5.15/docs/examples/xsar_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/examples/xsar_batch_datarmor.ipynb` & `xsar-2024.5.15/docs/examples/xsar_batch_datarmor.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/examples/xsar_multiple.ipynb` & `xsar-2024.5.15/docs/examples/xsar_multiple.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/examples/xsar_tops_slc.ipynb` & `xsar-2024.5.15/docs/examples/xsar_tops_slc.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980489417989418%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(3, "*

 * *            '"gv.tile_sources.EsriImagery*gv.Polygons(tmp[\'geometry\']).opts(width=800,height=450,alpha=0.5)\\n")], '*

 * *            "delete: [3]}}, 7: {'source': {insert: [(1, "*

 * *            '"gv.tile_sources.EsriImagery*gv.Polygons(tmp2[\'geometry\']).opts(width=800,height=450,alpha=0.2)*gv.Polygons(tmp[\'geometry\']).opts(width=800,height=450,alpha=0.2)\\n")], '*

 * *            "delete: [1]}}, 24: {'source': {insert: [(0, 's1ds.apply_calibration_and_denoising() "*

 * *     […]*

```diff
@@ -79,26 +79,26 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "#gv.tile_sources.Wikipedia*gv.Polygons(multids.bursts(only_valid_location=True)['geometry']).opts(width=800,height=450,alpha=0.5)\n",
                 "import pandas as pd\n",
                 "tmp = pd.concat([xsar.Sentinel1Dataset(onesubswath).get_bursts_polygons(only_valid_location=True) for onesubswath in multids.subdatasets.index])\n",
-                "gv.tile_sources.Wikipedia*gv.Polygons(tmp['geometry']).opts(width=800,height=450,alpha=0.5)\n"
+                "gv.tile_sources.EsriImagery*gv.Polygons(tmp['geometry']).opts(width=800,height=450,alpha=0.5)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e79e91f7-7134-48ff-aa2c-b8ae8fe1d4fe",
             "metadata": {},
             "outputs": [],
             "source": [
                 "tmp2 = pd.concat([xsar.Sentinel1Dataset(onesubswath).get_bursts_polygons(only_valid_location=False) for onesubswath in multids.subdatasets.index])\n",
-                "gv.tile_sources.Wikipedia*gv.Polygons(tmp2['geometry']).opts(width=800,height=450,alpha=0.2)*gv.Polygons(tmp['geometry']).opts(width=800,height=450,alpha=0.2)\n"
+                "gv.tile_sources.EsriImagery*gv.Polygons(tmp2['geometry']).opts(width=800,height=450,alpha=0.2)*gv.Polygons(tmp['geometry']).opts(width=800,height=450,alpha=0.2)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e0fc0776-400c-45fe-b0ac-5a2c73254f1a",
             "metadata": {},
             "source": [
@@ -257,15 +257,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "21c43292-f707-4bf1-9db9-4e2ce5a70c83",
             "metadata": {},
             "outputs": [],
             "source": [
-                "s1ds.apply_calibration_and_denoising()\n",
+                "s1ds.apply_calibration_and_denoising() \n",
                 "s1ds.dataset"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "56ef1c15-ee3f-4cc4-a752-53b91ccdba59",
@@ -424,14 +424,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.9.15"
         },
         "toc-autonumbering": true
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xsar-2024.4.24/docs/index.rst` & `xsar-2024.5.15/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/docs/installing.rst` & `xsar-2024.5.15/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/highlevel-checks/check_s1_xsar_opendataset.py` & `xsar-2024.5.15/highlevel-checks/check_s1_xsar_opendataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/setup.py` & `xsar-2024.5.15/setup.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/scripts/compress_safe.py` & `xsar-2024.5.15/src/scripts/compress_safe.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/base_dataset.py` & `xsar-2024.5.15/src/xsar/base_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/base_meta.py` & `xsar-2024.5.15/src/xsar/base_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/config.yml` & `xsar-2024.5.15/src/xsar/config.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # default data dir for tests and examples
 data_dir: /tmp
 auxiliary_dir:
+path_auxiliary_df: 
 
 auxiliary_names:    
     S1B:     
         v_IPF_36:
             AUX_PP1: 'S1B_AUX_PP1_V20160422T000000_G20220323T140710.SAFE'
             AUX_CAL: 'S1B_AUX_CAL_V20160422T000000_G20210104T140113.SAFE'
             #AUX_INS: 'S1B_AUX_INS_V20160422T000000_G20211027T134314.SAFE'
```

### Comparing `xsar-2024.4.24/src/xsar/ipython_backends.py` & `xsar-2024.5.15/src/xsar/ipython_backends.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/radarsat2_dataset.py` & `xsar-2024.5.15/src/xsar/radarsat2_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/radarsat2_meta.py` & `xsar-2024.5.15/src/xsar/radarsat2_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/raster_readers.py` & `xsar-2024.5.15/src/xsar/raster_readers.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/rcm_dataset.py` & `xsar-2024.5.15/src/xsar/rcm_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/rcm_meta.py` & `xsar-2024.5.15/src/xsar/rcm_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/sentinel1_dataset.py` & `xsar-2024.5.15/src/xsar/sentinel1_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import xarray as xr
 import dask
 import rasterio.features
 from scipy.interpolate import interp1d
 from shapely.geometry import box
 
 from .utils import timing, map_blocks_coords, BlockingActorProxy, merge_yaml, \
-    to_lon180, config
+    to_lon180, config, datetime
 from .sentinel1_meta import Sentinel1Meta
 from .ipython_backends import repr_mimebundle
 import datatree
 from .base_dataset import BaseDataset
 import pandas as pd
 import geopandas as gpd
 
@@ -36,14 +36,15 @@
 mapping_dataset_geoloc = {'latitude': 'latitude',
                           'longitude': 'longitude',
                           'incidence': 'incidenceAngle',
                           'elevation': 'elevationAngle',
                           'altitude': 'height',
                           'azimuth_time': 'azimuthTime',
                           'slant_range_time': 'slantRangeTime',
+                          'offboresight': 'offboresightAngle',
                           }
 
 
 # noinspection PyTypeChecker
 class Sentinel1Dataset(BaseDataset):
     """
     Handle a SAFE subdataset.
@@ -91,19 +92,18 @@
 
     """
 
     def __init__(self, dataset_id, resolution=None,
                  resampling=rasterio.enums.Resampling.rms,
                  luts=False, chunks={'line': 5000, 'sample': 5000},
                  dtypes=None, patch_variable=True, lazyloading=True,
-                 recalibration=False, aux_config_name='v_IPF_36'):
+                 recalibration=False):
         # default dtypes
         if dtypes is not None:
             self._dtypes.update(dtypes)
-
         # default meta for map_blocks output.
         # as asarray is imported from numpy, it's a numpy array.
         # but if later we decide to import asarray from cupy, il will be a cupy.array (gpu)
         self.sar_meta = None
         self.interpolation_func_slc = {}
         """`xsar.Sentinel1Meta` object"""
 
@@ -135,14 +135,24 @@
         self.resolution, DN_tmp = self.sar_meta.reader.load_digital_number(resolution=resolution,
                                                                            resampling=resampling,
                                                                            chunks=chunks)
 
         # geoloc
         geoloc = self.sar_meta.geoloc
         geoloc.attrs['history'] = 'annotations'
+        geoloc["offboresightAngle"] = geoloc.elevationAngle - \
+            (30.1833947 * geoloc.latitude ** 0 + \
+            0.0082998714 * geoloc.latitude ** 1 - \
+            0.00031181534 * geoloc.latitude ** 2 - \
+            0.0943533e-07 * geoloc.latitude ** 3 + \
+            3.0191435e-08 * geoloc.latitude ** 4 + \
+            4.968415428e-12 *geoloc.latitude ** 5 - \
+            9.315371305e-13 * geoloc.latitude ** 6) + 29.45
+        geoloc["offboresightAngle"].attrs['comment']='built from elevation angle and latitude'
+        
         # bursts
         bu = self.sar_meta._bursts
         bu.attrs['history'] = 'annotations'
 
         # azimuth fm rate
         FM = self.sar_meta.azimuth_fmrate
         FM.attrs['history'] = 'annotations'
@@ -183,16 +193,14 @@
                                                      'noise_range': ds_noise_range,
                                                      'noise_azimuth': ds_noise_azi,
                                                      'antenna_pattern': ds_antenna_pattern,
                                                      'swath_merging': ds_swath_merging
                                                      })
 
         # apply recalibration ?
-
-        self.aux_config_name = aux_config_name
         self.apply_recalibration = recalibration
         if self.apply_recalibration and (self.sar_meta.swath != "EW" and self.sar_meta.swath != "IW"):
             self.apply_recalibration = False
             raise ValueError(
                 f"Recalibration in only done for EW/IW modes. You have '{self.sar_meta.swath}'. apply_recalibration is set to False.")
 
         if self.apply_recalibration and np.all(np.isnan(self.datatree.antenna_pattern['roll'].values)):
@@ -281,32 +289,65 @@
         # return
         self._dataset.attrs.update(self.sar_meta.to_dict("all"))
         self.datatree['measurement'] = self.datatree['measurement'].assign(
             self._dataset)
         self.datatree.attrs.update(self.sar_meta.to_dict("all"))
 
         # load land_mask by default for GRD products
+
+        self.add_high_resolution_variables(
+            patch_variable=patch_variable, luts=luts, lazy_loading=lazyloading)
         if 'GRD' in str(self.datatree.attrs['product']):
-            self.add_high_resolution_variables(
-                patch_variable=patch_variable, luts=luts, lazy_loading=lazyloading)
             if self.apply_recalibration:
                 self.select_gains()
             self.apply_calibration_and_denoising()
 
         # added 6 fev 23, to fill  empty attrs
         self.datatree['measurement'].attrs = self.datatree.attrs
+        if self.sar_meta.product == 'SLC' and 'WV' not in self.sar_meta.swath:  # TOPS cases
+            tmp = self.corrected_range_noise_lut(self.datatree)
+            self.datatree['noise_range'].ds = tmp # the corrcted noise_range dataset shold now contain an attrs 'corrected_range_noise_lut'
         self.sliced = False
         """True if dataset is a slice of original L1 dataset"""
 
         self.resampled = resolution is not None
         """True if dataset is not a sensor resolution"""
 
         # save original bbox
         self._bbox_coords_ori = self._bbox_coords
 
+    def corrected_range_noise_lut(self,dt):
+        """
+        Patch F.Nouguier see https://jira-projects.cls.fr/browse/MPCS-3581 and https://github.com/umr-lops/xsar_slc/issues/175
+        Return range noise lut with corrected line numbering. This function should be used only on the full SLC dataset dt
+        Args:
+            dt (xarray.datatree) : datatree returned by xsar corresponding to one subswath
+        Return:
+            (xarray.dataset) : range noise lut with corrected line number
+        """
+        # Detection of azimuthTime jumps (linked to burst changes). Burst sensingTime should NOT be used since they have erroneous value too !
+        line_shift = 0
+        tt = dt['measurement']['time']
+        i_jump = np.ravel(np.argwhere(np.diff(tt)<np.timedelta64(0))+1) # index of jumps
+        line_jump_meas = dt['measurement']['line'][i_jump] # line number of jumps
+        # line_jump_noise = np.ravel(dt['noise_range']['line'][1:-1].data) # annotated line number of burst begining, this one is corrupted for some S1 TOPS product
+        line_jump_noise = np.ravel(dt['noise_range']['line'][1:1+len(line_jump_meas)].data) # annoted line number of burst begining
+        burst_first_lineshift = line_jump_meas-line_jump_noise
+        if len(np.unique(burst_first_lineshift))==1:
+            line_shift = int(np.unique(burst_first_lineshift)[0])
+            logging.debug('line_shift: %s',line_shift)
+        else:
+            raise ValueError('Inconsistency in line shifting : {}'.format(burst_first_lineshift))
+        res = dt['noise_range'].ds.assign_coords({'line':dt['noise_range']['line']+line_shift})
+        if line_shift==0:
+            res.attrs['corrected_range_noise_lut'] = 'no change'
+        else:
+            res.attrs['corrected_range_noise_lut'] = 'shift : %i lines'%line_shift
+        return res
+
     def select_gains(self):
         """
         attribution of the good swath gain by getting the swath number of each pixel 
 
         Returns:
         --------
 
@@ -456,29 +497,43 @@
 
             if luts:
                 ds_merge_list.append(self._luts[self._hidden_vars])
             attrs = self._dataset.attrs
             self._dataset = xr.merge(ds_merge_list)
             self._dataset.attrs = attrs
             geoloc_vars = ['altitude', 'azimuth_time', 'slant_range_time',
-                           'incidence', 'elevation', 'longitude', 'latitude']
+                           'incidence', 'elevation', 'longitude', 'latitude', 'offboresight']
 
             for vv in skip_variables:
                 if vv in geoloc_vars:
                     geoloc_vars.remove(vv)
 
             self._dataset = self._dataset.merge(
                 self._load_from_geoloc(geoloc_vars, lazy_loading=lazy_loading))
-
-            
-            self.add_swath_number()   
+                         
+            if 'GRD' in str(self.datatree.attrs['product']):
+                self.add_swath_number()
                 
-            if self.apply_recalibration:
-                self.add_gains(config["auxiliary_names"][self.sar_meta.short_name.split(":")[-2][0:3]][self.aux_config_name]["AUX_CAL"],
-                               config["auxiliary_names"][self.sar_meta.short_name.split(":")[-2][0:3]][self.aux_config_name]["AUX_PP1"])
+                if self.apply_recalibration:
+                    path_dataframe_aux = config["path_dataframe_aux"]
+                    dataframe_aux = pd.read_csv(path_dataframe_aux)
+
+                    sel_cal = dataframe_aux.loc[(dataframe_aux.sat_name == self.sar_meta.manifest_attrs['satellite']) & 
+                                                (dataframe_aux.aux_type == "CAL") &
+                                                (dataframe_aux.validation_date <= self.sar_meta.start_date)]
+                    sel_cal = sel_cal.sort_values(by = ["validation_date","generation_date"],ascending=False)
+                    path_new_cal = sel_cal.iloc[0].aux_path
+
+                    sel_pp1 = dataframe_aux.loc[(dataframe_aux.sat_name == self.sar_meta.manifest_attrs['satellite']) & 
+                                (dataframe_aux.aux_type == "PP1") 
+                                & (dataframe_aux.validation_date <= self.sar_meta.start_date)]
+                    sel_pp1 = sel_pp1.sort_values(by = ["validation_date","generation_date"],ascending=False)
+                    path_new_pp1 = sel_pp1.iloc[0].aux_path
+
+                    self.add_gains(path_new_cal, path_new_pp1)
 
             rasters = self._load_rasters_vars()
             if rasters is not None:
                 self._dataset = xr.merge([self._dataset, rasters])
             if 'velocity' not in skip_variables:
                 self._dataset = self._dataset.merge(self.get_sensor_velocity())
             if 'range_ground_spacing' not in skip_variables:
@@ -522,22 +577,22 @@
         """
         swath_tab = xr.DataArray(np.full_like(self._dataset.elevation, np.nan, dtype=int), coords={
                                  'line': self._dataset.coords["line"], 'sample': self._dataset.coords["sample"]})
         flag_tab = xr.DataArray(np.zeros_like(self._dataset.elevation, dtype=int), coords={
                                 'line': self._dataset.coords["line"], 'sample': self._dataset.coords["sample"]})
 
         # Supposons que dataset.swaths ait 45 éléments comme mentionné
-        for i in range(len(self.datatree['swath_merging'].swaths)):
+        for i in range(len(self.datatree['swath_merging'].ds['swaths'])):
             y_min, y_max = self.datatree['swath_merging']['firstAzimuthLine'][
                 i], self.datatree['swath_merging']['lastAzimuthLine'][i]
             x_min, x_max = self.datatree['swath_merging']['firstRangeSample'][
                 i], self.datatree['swath_merging']['lastRangeSample'][i]
 
             # Localisation des pixels appartenant à ce swath
-            swath_index = int(self.datatree['swath_merging'].swaths[i])
+            swath_index = int(self.datatree['swath_merging'].ds['swaths'][i])
 
             condition = (self._dataset.line >= y_min) & (self._dataset.line <= y_max) & (
                 self._dataset.sample >= x_min) & (self._dataset.sample <= x_max)
 
             # Marquer les pixels déjà vus
             flag_tab = xr.where((flag_tab == 1) & condition & (
                 swath_tab == swath_index), 2, flag_tab)
@@ -559,19 +614,19 @@
     def add_gains(self, new_aux_cal_name, new_aux_pp1_name):
         from .utils import get_path_aux_cal, get_path_aux_pp1, get_geap_gains, get_gproc_gains
         import os
         from scipy.interpolate import interp1d
         logger.debug(
             f"doing recalibration with AUX_CAL = {new_aux_cal_name} & AUX_PP1 = {new_aux_pp1_name}")
 
-        path_aux_cal_new = get_path_aux_cal(new_aux_cal_name)
+        path_aux_cal_new = get_path_aux_cal(os.path.basename(new_aux_cal_name))
         path_aux_cal_old = get_path_aux_cal(
             os.path.basename(self.sar_meta.manifest_attrs["aux_cal"]))
 
-        path_aux_pp1_new = get_path_aux_pp1(new_aux_pp1_name)
+        path_aux_pp1_new = get_path_aux_pp1(os.path.basename(new_aux_pp1_name))
         path_aux_pp1_old = get_path_aux_pp1(
             os.path.basename(self.sar_meta.manifest_attrs["aux_pp1"]))
 
         #  1 - compute offboresight angle
         roll = self.datatree['antenna_pattern']['roll']
         azimuthTime = self.datatree['antenna_pattern']['azimuthTime']
         interp_roll = interp1d(azimuthTime.values.flatten().astype(
@@ -676,15 +731,19 @@
                                                                                                os.path.dirname(path_aux_pp1_new)),
                                                                                            os.path.basename(path_aux_pp1_new))
                     self._dataset_recalibration[keyf].loc[...,
                                                           pol] = dict_gproc_new[key][idxpol]
 
         self.datatree['recalibration'] = self.datatree['recalibration'].assign(
             self._dataset_recalibration)
-
+        
+        self.datatree['recalibration'].attrs["path_aux_cal_new"] = path_aux_cal_new
+        self.datatree['recalibration'].attrs["path_aux_pp1_new"] = path_aux_pp1_new
+        self.datatree['recalibration'].attrs["path_aux_cal_old"] = path_aux_cal_old
+        self.datatree['recalibration'].attrs["path_aux_pp1_old"] = path_aux_pp1_old
         # return self._dataset
 
     def apply_calibration_and_denoising(self):
         """
         apply calibration and denoising functions to get high resolution sigma0 , beta0 and gamma0 + variables *_raw
 
         Returns:
```

### Comparing `xsar-2024.4.24/src/xsar/sentinel1_meta.py` & `xsar-2024.5.15/src/xsar/sentinel1_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/utils.py` & `xsar-2024.5.15/src/xsar/utils.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/xarray_backends.py` & `xsar-2024.5.15/src/xsar/xarray_backends.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar/xsar.py` & `xsar-2024.5.15/src/xsar/xsar.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/src/xsar.egg-info/PKG-INFO` & `xsar-2024.5.15/src/xsar.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsar
-Version: 2024.4.24
+Version: 2024.5.15
 Summary: xarray L1 SAR mapper
 Home-page: https://github.com/umr-lops/xsar
 Author: Olivier Archer, Alexandre Levieux, Antoine Grouazel
 Author-email: Olivier.Archer@ifremer.fr, Alexandre.Levieux@gmail.com, Antoine.Grouazel@ifremer.fr
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `xsar-2024.4.24/src/xsar.egg-info/SOURCES.txt` & `xsar-2024.5.15/src/xsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xsar-2024.4.24/test/test_raster_readers.py` & `xsar-2024.5.15/test/test_raster_readers.py`

 * *Files identical despite different names*

