# Comparing `tmp/xarrayutils-2.0.0.tar.gz` & `tmp/xarrayutils-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarrayutils-2.0.0.tar", last modified: Fri Jun  9 18:26:22 2023, max compression
+gzip compressed data, was "xarrayutils-2.0.1.tar", last modified: Wed May 15 17:15:25 2024, max compression
```

## Comparing `xarrayutils-2.0.0.tar` & `xarrayutils-2.0.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.337704 xarrayutils-2.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.337704 xarrayutils-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.github/workflows/pythonpublish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.341704 xarrayutils-2.0.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/ci/environment-upstream-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.345704 xarrayutils-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/contributor_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   689757 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   851989 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/utils.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   246650 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/vertical_coords.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/whats-new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.345704 xarrayutils-2.0.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/notebooks/Untitled.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/notebooks/regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/xarrayutils/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/xarrayutils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/build_grids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/climate_indicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/xarrayutils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_build_grids.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_file_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_xgcm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_xmitgcm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    27953 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/xgcm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/xmitgcm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/xarrayutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:25.442149 xarrayutils-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:25.434149 xarrayutils-2.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:25.434149 xarrayutils-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/.github/workflows/pythonpublish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-15 17:15:25.442149 xarrayutils-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:25.434149 xarrayutils-2.0.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/ci/environment-upstream-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:25.438149 xarrayutils-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/contributor_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   689757 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   851989 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/utils.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   246650 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/vertical_coords.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/docs/whats-new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:25.438149 xarrayutils-2.0.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/notebooks/Untitled.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27015 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/notebooks/regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-15 17:15:25.442149 xarrayutils-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68751 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:25.442149 xarrayutils-2.0.1/xarrayutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-15 17:15:25.442149 xarrayutils-2.0.1/xarrayutils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/build_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/climate_indicies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22170 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:25.442149 xarrayutils-2.0.1/xarrayutils/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/test/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/test/test_build_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/test/test_file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/test/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20504 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/test/test_xgcm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/test/test_xmitgcm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27985 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/xgcm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-15 17:15:16.000000 xarrayutils-2.0.1/xarrayutils/xmitgcm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:15:25.438149 xarrayutils-2.0.1/xarrayutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-15 17:15:25.000000 xarrayutils-2.0.1/xarrayutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-15 17:15:25.000000 xarrayutils-2.0.1/xarrayutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:15:25.000000 xarrayutils-2.0.1/xarrayutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 17:15:25.000000 xarrayutils-2.0.1/xarrayutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 17:15:25.000000 xarrayutils-2.0.1/xarrayutils.egg-info/top_level.txt
```

### Comparing `xarrayutils-2.0.0/.github/workflows/ci.yaml` & `xarrayutils-2.0.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/.github/workflows/pythonpublish.yaml` & `xarrayutils-2.0.1/.github/workflows/pythonpublish.yaml`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/.gitignore` & `xarrayutils-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/LICENSE` & `xarrayutils-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/PKG-INFO` & `xarrayutils-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarrayutils
-Version: 2.0.0
+Version: 2.0.1
 Summary: A collection of various tools for data analysis built on top of xarray and xgcm
 Home-page: https://github.com/jbusecke/xarrayutils
 Author: xarrayutils Developers
 Author-email: julius@ldeo.columbia.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xarrayutils-2.0.0/README.md` & `xarrayutils-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/docs/Makefile` & `xarrayutils-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/docs/conf.py` & `xarrayutils-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/docs/contributor_guide.rst` & `xarrayutils-2.0.1/docs/contributor_guide.rst`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/docs/index.rst` & `xarrayutils-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/docs/plotting.ipynb` & `xarrayutils-2.0.1/docs/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/docs/utils.ipynb` & `xarrayutils-2.0.1/docs/utils.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/docs/vertical_coords.ipynb` & `xarrayutils-2.0.1/docs/vertical_coords.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/docs/whats-new.rst` & `xarrayutils-2.0.1/docs/whats-new.rst`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/notebooks/Untitled.ipynb` & `xarrayutils-2.0.1/notebooks/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/notebooks/regression.ipynb` & `xarrayutils-2.0.1/notebooks/regression.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/setup.py` & `xarrayutils-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/versioneer.py` & `xarrayutils-2.0.1/versioneer.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/build_grids.py` & `xarrayutils-2.0.1/xarrayutils/build_grids.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/climate_indicies.py` & `xarrayutils-2.0.1/xarrayutils/climate_indicies.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/file_handling.py` & `xarrayutils-2.0.1/xarrayutils/file_handling.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/filtering.py` & `xarrayutils-2.0.1/xarrayutils/filtering.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/plotting.py` & `xarrayutils-2.0.1/xarrayutils/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,24 +125,28 @@
         Color of the box behind each letter (the default is None).
     labels: list
         List of strings used as labels (if None (default), uses lowercase alphabet followed by uppercase alphabet)
     **kwargs : type
         kwargs passed to matplotlib.axis.text
 
     """
+    # setting default values
+    kwargs.setdefault("horizontalalignment", "center")
+    kwargs.setdefault("verticalalignment", "center")
+    x = kwargs.pop("x", 0.1)
+    y = kwargs.pop("y", 0.85)
+
     if labels is None:
         labels = list(string.ascii_letters)
 
     for ax, letter in zip(axes.flat, labels[start_idx:]):
         t = ax.text(
-            0.1,
-            0.85,
+            x,
+            y,
             letter + ")",
-            horizontalalignment="center",
-            verticalalignment="center",
             transform=ax.transAxes,
             **kwargs,
         )
         if box_color:
             t.set_bbox(dict(facecolor=box_color, alpha=0.5, edgecolor=None))
```

### Comparing `xarrayutils-2.0.0/xarrayutils/test/datasets.py` & `xarrayutils-2.0.1/xarrayutils/test/datasets.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/test/test_build_grids.py` & `xarrayutils-2.0.1/xarrayutils/test/test_build_grids.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/test/test_file_handling.py` & `xarrayutils-2.0.1/xarrayutils/test/test_file_handling.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/test/test_filtering.py` & `xarrayutils-2.0.1/xarrayutils/test/test_filtering.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/test/test_plotting.py` & `xarrayutils-2.0.1/xarrayutils/test/test_plotting.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/test/test_utils.py` & `xarrayutils-2.0.1/xarrayutils/test/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,20 +188,20 @@
     if nans:
         if nans == "all":
             a = xr.ones_like(a) * np.nan
             b = xr.ones_like(b) * np.nan
 
         else:
             # add nans at random positions
-            a.data[
-                np.unravel_index(np.random.randint(0, 5 * 7 * 3, 10), a.shape)
-            ] = np.nan
-            b.data[
-                np.unravel_index(np.random.randint(0, 5 * 7 * 3, 10), b.shape)
-            ] = np.nan
+            a.data[np.unravel_index(np.random.randint(0, 5 * 7 * 3, 10), a.shape)] = (
+                np.nan
+            )
+            b.data[np.unravel_index(np.random.randint(0, 5 * 7 * 3, 10), b.shape)] = (
+                np.nan
+            )
 
     if chunks is not None:
         if variant == 0:
             a = a.chunk(chunks)
         elif variant == 1:
             b = b.chunk(chunks)
         elif variant == 2:
@@ -576,15 +576,15 @@
 @pytest.mark.parametrize(
     "blocks_fail",
     [
         [("i", 3.4), ("j", 2)],
         # non int interval
         [("blah", 2), ("blubb", 3)],
         # no matching labels
-        [(2, 2), ("j", 2)]
+        [(2, 2), ("j", 2)],
         # non str dim label
     ],
 )
 def test_aggregate_input_blocks(dataarray_2d_example, blocks_fail):
     with pytest.raises(RuntimeError):
         aggregate(dataarray_2d_example, blocks_fail, func=np.nanmean)
```

### Comparing `xarrayutils-2.0.0/xarrayutils/test/test_xgcm_utils.py` & `xarrayutils-2.0.1/xarrayutils/test/test_xgcm_utils.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/test/test_xmitgcm_utils.py` & `xarrayutils-2.0.1/xarrayutils/test/test_xmitgcm_utils.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/utils.py` & `xarrayutils-2.0.1/xarrayutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import xarray as xr
-from scipy.signal import filtfilt, gaussian
+from scipy.signal import filtfilt
+from scipy.signal.windows import gaussian
 from scipy import stats
 
 from dask.array import coarsen, ones_like
 from dask.array.core import Array
 import warnings
 from xarrayutils.utilities import detect_dtype
 from xarrayutils.filtering import filter_1D as filter_1D_refactored
```

### Comparing `xarrayutils-2.0.0/xarrayutils/xgcm_utils.py` & `xarrayutils-2.0.1/xarrayutils/xgcm_utils.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils/xmitgcm_utils.py` & `xarrayutils-2.0.1/xarrayutils/xmitgcm_utils.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-2.0.0/xarrayutils.egg-info/PKG-INFO` & `xarrayutils-2.0.1/xarrayutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarrayutils
-Version: 2.0.0
+Version: 2.0.1
 Summary: A collection of various tools for data analysis built on top of xarray and xgcm
 Home-page: https://github.com/jbusecke/xarrayutils
 Author: xarrayutils Developers
 Author-email: julius@ldeo.columbia.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xarrayutils-2.0.0/xarrayutils.egg-info/SOURCES.txt` & `xarrayutils-2.0.1/xarrayutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

