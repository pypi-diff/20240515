# Comparing `tmp/cellfinder-1.1.3.tar.gz` & `tmp/cellfinder-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-1.1.3.tar", last modified: Fri Apr 12 16:04:04 2024, max compression
+gzip compressed data, was "cellfinder-1.2.0.tar", last modified: Wed May 15 16:11:09 2024, max compression
```

## Comparing `cellfinder-1.1.3.tar` & `cellfinder-1.2.0.tar`

### file list

```diff
@@ -1,94 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.178807 cellfinder-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.162807 cellfinder-1.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-12 16:03:57.000000 cellfinder-1.1.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-12 16:03:57.000000 cellfinder-1.1.3/.github/workflows/test_include_guard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-12 16:03:57.000000 cellfinder-1.1.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/.napari/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 16:03:57.000000 cellfinder-1.1.3/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-12 16:03:57.000000 cellfinder-1.1.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-12 16:03:57.000000 cellfinder-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 16:03:57.000000 cellfinder-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-12 16:04:04.178807 cellfinder-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-12 16:03:57.000000 cellfinder-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/cellfinder/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/cli_migration_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/cellfinder/core/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/cellfinder/core/classify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/cube_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/config/cellfinder.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/detect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/detect/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/classical_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/plane_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/tile_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/setup_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/ball_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/structure_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/volume_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/download/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/download/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/download/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/core/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/IO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/array_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/source_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/core/train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/train/train_yml.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/napari/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/curation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/napari/detect/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/detect/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/detect/detect_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/detect/thread_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/napari/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/images/brainglobe.png
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/input_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/napari/train/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/train/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/train/train_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-12 16:04:04.000000 cellfinder-1.1.3/cellfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-12 16:03:57.000000 cellfinder-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:04:04.178807 cellfinder-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.346486 cellfinder-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-15 16:11:03.000000 cellfinder-1.2.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-15 16:11:03.000000 cellfinder-1.2.0/.github/workflows/test_include_guard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-15 16:11:03.000000 cellfinder-1.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/.napari/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-15 16:11:03.000000 cellfinder-1.2.0/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-15 16:11:03.000000 cellfinder-1.2.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-15 16:11:03.000000 cellfinder-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 16:11:03.000000 cellfinder-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-15 16:11:09.358486 cellfinder-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-15 16:11:03.000000 cellfinder-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/cli_migration_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/core/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/cube_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/classify/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/config/cellfinder.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.350486 cellfinder-1.2.0/cellfinder/core/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/detect/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/classical_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/plane_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/plane/tile_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/setup_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/ball_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/structure_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/detect/filters/volume/volume_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/download/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/array_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/source_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.354486 cellfinder-1.2.0/cellfinder/core/train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13139 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/train/train_yml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/cellfinder/napari/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/curation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/cellfinder/napari/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/detect/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/detect/detect_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/detect/thread_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/input_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/cellfinder/napari/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/train/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/train/train_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 16:11:03.000000 cellfinder-1.2.0/cellfinder/napari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:09.358486 cellfinder-1.2.0/cellfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-15 16:11:09.000000 cellfinder-1.2.0/cellfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 16:11:08.000000 cellfinder-1.2.0/cellfinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-15 16:11:03.000000 cellfinder-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:11:09.358486 cellfinder-1.2.0/setup.cfg
```

### Comparing `cellfinder-1.1.3/.github/workflows/test_and_deploy.yml` & `cellfinder-1.2.0/.github/workflows/test_and_deploy.yml`

 * *Files 12% similar despite different names*

```diff
@@ -38,75 +38,81 @@
     timeout-minutes: 60
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         # Run all supported Python versions on linux
         os: [ubuntu-latest]
         python-version: ["3.9", "3.10"]
-        # Include one windows, one macos run
+        # Include one windows, one macos run each for M1 (latest) and Intel (13)
         include:
-        - os: macos-latest
-          python-version: "3.10"
-        - os: windows-latest
-          python-version: "3.10"
+          - os: macos-13
+            python-version: "3.10"
+          - os: macos-latest
+            python-version: "3.10"
+          - os: windows-latest
+            python-version: "3.10"
 
     steps:
       # Cache the tensorflow model so we don't have to remake it every time
       - name: Cache tensorflow model
         uses: actions/cache@v3
         with:
           path: "~/.cellfinder"
-          key: models-${{ hashFiles('~/.cellfinder/**') }}
+          key: models-${{ hashFiles('~/.brainglobe/**') }}
       # Setup pyqt libraries
       - name: Setup qtpy libraries
         uses: tlambert03/setup-qt-libs@v1
       # Setup VTK with headless display
       - uses: pyvista/setup-headless-display-action@v2
       # Run all tests
       - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: ${{ matrix.python-version }}
+          secret-codecov-token: ${{ secrets.CODECOV_TOKEN }}
           use-xvfb: true
 
   test_numba_disabled:
     needs: [linting, manifest]
     name: Run tests with numba disabled
+    timeout-minutes: 60
     runs-on: ubuntu-latest
     env:
        NUMBA_DISABLE_JIT: "1"
 
     steps:
       - name: Cache tensorflow model
         uses: actions/cache@v3
         with:
           path: "~/.cellfinder"
-          key: models-${{ hashFiles('~/.cellfinder/**') }}
+          key: models-${{ hashFiles('~/.brainglobe/**') }}
       # Setup pyqt libraries
       - name: Setup qtpy libraries
         uses: tlambert03/setup-qt-libs@v1
       # Setup VTK with headless display
       - uses: pyvista/setup-headless-display-action@v2
       # Run test suite with numba disabled
       - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: "3.10"
+          secret-codecov-token: ${{ secrets.CODECOV_TOKEN }}
           codecov-flags: "numba"
 
   # Run brainglobe-workflows brainmapper-CLI tests to check for
   # breakages
   test_brainmapper_cli:
     needs: [linting, manifest]
     name: Run brainmapper tests to check for breakages
+    timeout-minutes: 60
     runs-on: ubuntu-latest
     steps:
       - name: Cache tensorflow model
         uses: actions/cache@v3
         with:
           path: "~/.cellfinder"
-          key: models-${{ hashFiles('~/.cellfinder/**') }}
+          key: models-${{ hashFiles('~/.brainglobe/**') }}
 
       - name: Checkout brainglobe-workflows
         uses: actions/checkout@v3
         with:
           repository: 'brainglobe/brainglobe-workflows'
 
       - name: Set up Python 3.10
```

### Comparing `cellfinder-1.1.3/.github/workflows/test_include_guard.yaml` & `cellfinder-1.2.0/.github/workflows/test_include_guard.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -31,15 +31,20 @@
         uses: jannekem/run-python-script-action@v1
         with:
           fail-on-error: true
           script: |
             import cellfinder.core
             import cellfinder.napari
 
-      - name: Uninstall tensorflow
+      - name: Uninstall tensorflow-macos on Mac M1
+        if: matrix.os == 'macos-latest'
+        run: python -m pip uninstall -y tensorflow-macos
+
+      - name: Uninstall tensorflow on Ubuntu
+        if: matrix.os == 'ubuntu-latest'
         run: python -m pip uninstall -y tensorflow
 
       - name: Test (broken) import
         id: broken_import
         uses: jannekem/run-python-script-action@v1
         with:
           fail-on-error: false
```

### Comparing `cellfinder-1.1.3/.gitignore` & `cellfinder-1.2.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -126,19 +126,14 @@
 
 pip-wheel-metadata/
 
 mprofile*.dat
 
 *.DS_Store
 
-# asv
-.asv
-benchmarks/results
-benchmarks/html
-benchmarks/env
 
 # OS
 .DS_Store
 
 # written by setuptools_scm
 */_version.py
```

### Comparing `cellfinder-1.1.3/CITATION.cff` & `cellfinder-1.2.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/LICENSE` & `cellfinder-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/PKG-INFO` & `cellfinder-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.1.3
+Version: 1.2.0
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: brainglobe-utils>=0.4.2
+Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: brainglobe-napari-io>=0.3.4
 Requires-Dist: dask[array]
 Requires-Dist: fancylog>=0.0.7
 Requires-Dist: natsort
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: scikit-image
@@ -50,25 +50,25 @@
 Requires-Dist: magicgui; extra == "napari"
 Requires-Dist: napari-ndtiffs; extra == "napari"
 Requires-Dist: napari-plugin-engine>=0.1.4; extra == "napari"
 Requires-Dist: napari[pyqt5]; extra == "napari"
 Requires-Dist: pooch>=1; extra == "napari"
 Requires-Dist: qtpy; extra == "napari"
 
-[![Python Version](https://img.shields.io/pypi/pyversions/cellfinder-core.svg)](https://pypi.org/project/cellfinder)
-[![PyPI](https://img.shields.io/pypi/v/cellfinder-core.svg)](https://pypi.org/project/cellfinder)
-[![Downloads](https://pepy.tech/badge/cellfinder-core)](https://pepy.tech/project/cellfinder)
-[![Wheel](https://img.shields.io/pypi/wheel/cellfinder-core.svg)](https://pypi.org/project/cellfinder)
-[![Development Status](https://img.shields.io/pypi/status/cellfinder-core.svg)](https://github.com/brainglobe/cellfinder)
+[![Python Version](https://img.shields.io/pypi/pyversions/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![PyPI](https://img.shields.io/pypi/v/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Downloads](https://pepy.tech/badge/cellfinder)](https://pepy.tech/project/cellfinder)
+[![Wheel](https://img.shields.io/pypi/wheel/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Development Status](https://img.shields.io/pypi/status/cellfinder.svg)](https://github.com/brainglobe/cellfinder)
 [![Tests](https://img.shields.io/github/actions/workflow/status/brainglobe/cellfinder/test_and_deploy.yml?branch=main)](https://github.com/brainglobe/cellfinder/actions)
-[![codecov](https://codecov.io/gh/brainglobe/cellfinder-core/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder)
+[![codecov](https://codecov.io/gh/brainglobe/cellfinder/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/developers/index.html)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/community/developers/index.html)
 [![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
 
 # cellfinder
 
 cellfinder is software for automated 3D cell detection in very large 3D images (e.g., serial two-photon or lightsheet volumes of whole mouse brains).
 There are three different ways to interact and use it, each with different user interfaces and objectives in mind.
 For more details, head over to [the documentation website](https://brainglobe.info/documentation/cellfinder/index.html).
```

### Comparing `cellfinder-1.1.3/README.md` & `cellfinder-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-[![Python Version](https://img.shields.io/pypi/pyversions/cellfinder-core.svg)](https://pypi.org/project/cellfinder)
-[![PyPI](https://img.shields.io/pypi/v/cellfinder-core.svg)](https://pypi.org/project/cellfinder)
-[![Downloads](https://pepy.tech/badge/cellfinder-core)](https://pepy.tech/project/cellfinder)
-[![Wheel](https://img.shields.io/pypi/wheel/cellfinder-core.svg)](https://pypi.org/project/cellfinder)
-[![Development Status](https://img.shields.io/pypi/status/cellfinder-core.svg)](https://github.com/brainglobe/cellfinder)
+[![Python Version](https://img.shields.io/pypi/pyversions/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![PyPI](https://img.shields.io/pypi/v/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Downloads](https://pepy.tech/badge/cellfinder)](https://pepy.tech/project/cellfinder)
+[![Wheel](https://img.shields.io/pypi/wheel/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Development Status](https://img.shields.io/pypi/status/cellfinder.svg)](https://github.com/brainglobe/cellfinder)
 [![Tests](https://img.shields.io/github/actions/workflow/status/brainglobe/cellfinder/test_and_deploy.yml?branch=main)](https://github.com/brainglobe/cellfinder/actions)
-[![codecov](https://codecov.io/gh/brainglobe/cellfinder-core/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder)
+[![codecov](https://codecov.io/gh/brainglobe/cellfinder/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/developers/index.html)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/community/developers/index.html)
 [![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
 
 # cellfinder
 
 cellfinder is software for automated 3D cell detection in very large 3D images (e.g., serial two-photon or lightsheet volumes of whole mouse brains).
 There are three different ways to interact and use it, each with different user interfaces and objectives in mind.
 For more details, head over to [the documentation website](https://brainglobe.info/documentation/cellfinder/index.html).
```

### Comparing `cellfinder-1.1.3/cellfinder/__init__.py` & `cellfinder-1.2.0/cellfinder/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from importlib.metadata import PackageNotFoundError, version
+from pathlib import Path
 
 try:
     __version__ = version("cellfinder")
 except PackageNotFoundError as e:
     raise PackageNotFoundError("cellfinder package not installed") from e
 
 # If tensorflow is not present, tools cannot be used.
@@ -18,7 +19,9 @@
             f"Please install tensorflow into your environment to use cellfinder tools. "
             f"For more information, please see "
             f"https://github.com/brainglobe/brainglobe-meta#readme."
         ) from e
 
 __author__ = "Adam Tyson, Christian Niedworok, Charly Rousseau"
 __license__ = "BSD-3-Clause"
+
+DEFAULT_CELLFINDER_DIRECTORY = Path.home() / ".brainglobe" / "cellfinder"
```

### Comparing `cellfinder-1.1.3/cellfinder/cli_migration_warning.py` & `cellfinder-1.2.0/cellfinder/cli_migration_warning.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/classify/augment.py` & `cellfinder-1.2.0/cellfinder/core/classify/augment.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/classify/classify.py` & `cellfinder-1.2.0/cellfinder/core/classify/classify.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/classify/cube_generator.py` & `cellfinder-1.2.0/cellfinder/core/classify/cube_generator.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/classify/resnet.py` & `cellfinder-1.2.0/cellfinder/core/classify/resnet.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/classify/tools.py` & `cellfinder-1.2.0/cellfinder/core/classify/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/detect/detect.py` & `cellfinder-1.2.0/cellfinder/core/detect/detect.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from queue import Queue
 from threading import Lock
 from typing import Callable, List, Optional, Sequence, Tuple, TypeVar
 
 import numpy as np
 from brainglobe_utils.cells.cells import Cell
 from brainglobe_utils.general.system import get_num_processes
+from numba import set_num_threads
 
 from cellfinder.core import logger, types
 from cellfinder.core.detect.filters.plane import TileProcessor
 from cellfinder.core.detect.filters.setup_filters import setup_tile_filtering
 from cellfinder.core.detect.filters.volume.volume_filter import VolumeFilter
 
 
@@ -153,14 +154,21 @@
     if not np.issubdtype(signal_array.dtype, np.integer):
         raise ValueError(
             "signal_array must be integer datatype, but has datatype "
             f"{signal_array.dtype}"
         )
     n_processes = get_num_processes(min_free_cpu_cores=n_free_cpus)
     n_ball_procs = max(n_processes - 1, 1)
+
+    # we parallelize 2d filtering, which typically lags behind the 3d
+    # processing so for n_ball_procs 2d filtering threads, ball_z_size will
+    # typically be in use while the others stall waiting for 3d processing
+    # so we can use those for other things, such as numba threading
+    set_num_threads(max(n_ball_procs - int(ball_z_size), 1))
+
     start_time = datetime.now()
 
     (
         soma_diameter,
         max_cluster_size,
         ball_xy_size,
         ball_z_size,
@@ -232,15 +240,18 @@
 
         # Start 3D filter
         #
         # This runs in the main thread, and blocks until the all the 2D and
         # then 3D filtering has finished. As batches of planes are filtered
         # by the 3D filter, it releases the locks of subsequent 2D filter
         # processes.
-        cells = mp_3d_filter.process(async_results, locks, callback=callback)
+        mp_3d_filter.process(async_results, locks, callback=callback)
+
+        # it's now done filtering, get results with pool
+        cells = mp_3d_filter.get_results(worker_pool)
 
     time_elapsed = datetime.now() - start_time
     logger.debug(
         f"All Planes done. Found {len(cells)} cells in {format(time_elapsed)}"
     )
     print("Detection complete - all planes done in : {}".format(time_elapsed))
     return cells
```

### Comparing `cellfinder-1.1.3/cellfinder/core/detect/filters/plane/classical_filter.py` & `cellfinder-1.2.0/cellfinder/core/detect/filters/plane/classical_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/detect/filters/plane/plane_filter.py` & `cellfinder-1.2.0/cellfinder/core/detect/filters/plane/plane_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/detect/filters/plane/tile_walker.py` & `cellfinder-1.2.0/cellfinder/core/detect/filters/plane/tile_walker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/detect/filters/setup_filters.py` & `cellfinder-1.2.0/cellfinder/core/detect/filters/setup_filters.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/detect/filters/volume/ball_filter.py` & `cellfinder-1.2.0/cellfinder/core/detect/filters/volume/ball_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,87 @@
+from functools import lru_cache
+
 import numpy as np
-from numba import njit
+from numba import njit, objmode, prange
+from numba.core import types
+from numba.experimental import jitclass
 
 from cellfinder.core.tools.array_operations import bin_mean_3d
 from cellfinder.core.tools.geometry import make_sphere
 
 DEBUG = False
 
+uint32_3d_type = types.uint32[:, :, :]
+bool_3d_type = types.bool_[:, :, :]
+float_3d_type = types.float64[:, :, :]
+
+
+@lru_cache(maxsize=50)
+def get_kernel(ball_xy_size: int, ball_z_size: int) -> np.ndarray:
+    # Create a spherical kernel.
+    #
+    # This is done by:
+    # 1. Generating a binary sphere at a resolution *upscale_factor* larger
+    #    than desired.
+    # 2. Downscaling the binary sphere to get a 'fuzzy' sphere at the
+    #    original intended scale
+    upscale_factor: int = 7
+    upscaled_kernel_shape = (
+        upscale_factor * ball_xy_size,
+        upscale_factor * ball_xy_size,
+        upscale_factor * ball_z_size,
+    )
+    upscaled_ball_centre_position = (
+        np.floor(upscaled_kernel_shape[0] / 2),
+        np.floor(upscaled_kernel_shape[1] / 2),
+        np.floor(upscaled_kernel_shape[2] / 2),
+    )
+    upscaled_ball_radius = upscaled_kernel_shape[0] / 2.0
+
+    sphere_kernel = make_sphere(
+        upscaled_kernel_shape,
+        upscaled_ball_radius,
+        upscaled_ball_centre_position,
+    )
+    sphere_kernel = sphere_kernel.astype(np.float64)
+    kernel = bin_mean_3d(
+        sphere_kernel,
+        bin_height=upscale_factor,
+        bin_width=upscale_factor,
+        bin_depth=upscale_factor,
+    )
+
+    assert (
+        kernel.shape[2] == ball_z_size
+    ), "Kernel z dimension should be {}, got {}".format(
+        ball_z_size, kernel.shape[2]
+    )
+
+    return kernel
+
+
+# volume indices/size is 64 bit for very large brains(!)
+spec = [
+    ("ball_xy_size", types.uint32),
+    ("ball_z_size", types.uint32),
+    ("tile_step_width", types.uint64),
+    ("tile_step_height", types.uint64),
+    ("THRESHOLD_VALUE", types.uint32),
+    ("SOMA_CENTRE_VALUE", types.uint32),
+    ("overlap_fraction", types.float64),
+    ("overlap_threshold", types.float64),
+    ("middle_z_idx", types.uint32),
+    ("_num_z_added", types.uint32),
+    ("kernel", float_3d_type),
+    ("volume", uint32_3d_type),
+    ("inside_brain_tiles", bool_3d_type),
+]
+
 
+@jitclass(spec=spec)
 class BallFilter:
     """
     A 3D ball filter.
 
     This runs a spherical kernel across the (x, y) dimensions
     of a *ball_z_size* stack of planes, and marks pixels in the middle
     plane of the stack that have a high enough intensity within the
@@ -58,195 +129,201 @@
         self.overlap_fraction = overlap_fraction
         self.tile_step_width = tile_step_width
         self.tile_step_height = tile_step_height
 
         self.THRESHOLD_VALUE = threshold_value
         self.SOMA_CENTRE_VALUE = soma_centre_value
 
-        # Create a spherical kernel.
-        #
-        # This is done by:
-        # 1. Generating a binary sphere at a resolution *upscale_factor* larger
-        #    than desired.
-        # 2. Downscaling the binary sphere to get a 'fuzzy' sphere at the
-        #    original intended scale
-        upscale_factor: int = 7
-        upscaled_kernel_shape = (
-            upscale_factor * ball_xy_size,
-            upscale_factor * ball_xy_size,
-            upscale_factor * ball_z_size,
-        )
-        upscaled_ball_centre_position = (
-            np.floor(upscaled_kernel_shape[0] / 2),
-            np.floor(upscaled_kernel_shape[1] / 2),
-            np.floor(upscaled_kernel_shape[2] / 2),
-        )
-        upscaled_ball_radius = upscaled_kernel_shape[0] / 2.0
-        sphere_kernel = make_sphere(
-            upscaled_kernel_shape,
-            upscaled_ball_radius,
-            upscaled_ball_centre_position,
-        )
-        sphere_kernel = sphere_kernel.astype(np.float64)
-        self.kernel = bin_mean_3d(
-            sphere_kernel,
-            bin_height=upscale_factor,
-            bin_width=upscale_factor,
-            bin_depth=upscale_factor,
-        )
-
-        assert (
-            self.kernel.shape[2] == ball_z_size
-        ), "Kernel z dimension should be {}, got {}".format(
-            ball_z_size, self.kernel.shape[2]
-        )
+        # getting kernel is not jitted
+        with objmode(kernel=float_3d_type):
+            kernel = get_kernel(ball_xy_size, ball_z_size)
+        self.kernel = kernel
 
         self.overlap_threshold = np.sum(self.overlap_fraction * self.kernel)
 
         # Stores the current planes that are being filtered
+        # first axis is z for faster rotating the z-axis
         self.volume = np.empty(
-            (plane_width, plane_height, ball_z_size), dtype=np.uint32
+            (ball_z_size, plane_width, plane_height),
+            dtype=np.uint32,
         )
         # Index of the middle plane in the volume
         self.middle_z_idx = int(np.floor(ball_z_size / 2))
+        self._num_z_added = 0
 
-        # TODO: lazy initialisation
+        # first axis is z
         self.inside_brain_tiles = np.empty(
             (
+                ball_z_size,
                 int(np.ceil(plane_width / tile_step_width)),
                 int(np.ceil(plane_height / tile_step_height)),
-                ball_z_size,
             ),
-            dtype=bool,
+            dtype=np.bool_,
         )
-        # Stores the z-index in volume at which new planes are inserted when
-        # append() is called
-        self.__current_z = -1
 
     @property
     def ready(self) -> bool:
         """
         Return `True` if enough planes have been appended to run the filter.
         """
-        return self.__current_z == self.ball_z_size - 1
+        return self._num_z_added >= self.ball_z_size
 
     def append(self, plane: np.ndarray, mask: np.ndarray) -> None:
         """
         Add a new 2D plane to the filter.
         """
         if DEBUG:
             assert [e for e in plane.shape[:2]] == [
-                e for e in self.volume.shape[:2]
+                e for e in self.volume.shape[1:]
             ], 'plane shape mismatch, expected "{}", got "{}"'.format(
-                [e for e in self.volume.shape[:2]],
+                [e for e in self.volume.shape[1:]],
                 [e for e in plane.shape[:2]],
             )
             assert [e for e in mask.shape[:2]] == [
-                e for e in self.inside_brain_tiles.shape[:2]
+                e for e in self.inside_brain_tiles.shape[1:]
             ], 'mask shape mismatch, expected"{}", got {}"'.format(
-                [e for e in self.inside_brain_tiles.shape[:2]],
+                [e for e in self.inside_brain_tiles.shape[1:]],
                 [e for e in mask.shape[:2]],
             )
-        if not self.ready:
-            self.__current_z += 1
-        else:
+
+        if self.ready:
             # Shift everything down by one to make way for the new plane
-            self.volume = np.roll(
-                self.volume, -1, axis=2
-            )  # WARNING: not in place
-            self.inside_brain_tiles = np.roll(
-                self.inside_brain_tiles, -1, axis=2
-            )
+            # this is faster than np.roll, especially with z-axis first
+            self.volume[:-1, :, :] = self.volume[1:, :, :]
+            self.inside_brain_tiles[:-1, :, :] = self.inside_brain_tiles[
+                1:, :, :
+            ]
+
+        # index for *next* slice is num we added *so far* until max
+        idx = min(self._num_z_added, self.ball_z_size - 1)
+        self._num_z_added += 1
+
         # Add the new plane to the top of volume and inside_brain_tiles
-        self.volume[:, :, self.__current_z] = plane[:, :]
-        self.inside_brain_tiles[:, :, self.__current_z] = mask[:, :]
+        self.volume[idx, :, :] = plane
+        self.inside_brain_tiles[idx, :, :] = mask
 
     def get_middle_plane(self) -> np.ndarray:
         """
         Get the plane in the middle of self.volume.
         """
-        z = self.middle_z_idx
-        return np.array(self.volume[:, :, z], dtype=np.uint32)
+        return self.volume[self.middle_z_idx, :, :].copy()
 
-    def walk(self) -> None:  # Highly optimised because most time critical
+    def walk(self, parallel: bool = False) -> None:
+        # **don't** pass parallel as keyword arg - numba struggles with it
+        # Highly optimised because most time critical
         ball_radius = self.ball_xy_size // 2
         # Get extents of image that are covered by tiles
         tile_mask_covered_img_width = (
-            self.inside_brain_tiles.shape[0] * self.tile_step_width
+            self.inside_brain_tiles.shape[1] * self.tile_step_width
         )
         tile_mask_covered_img_height = (
-            self.inside_brain_tiles.shape[1] * self.tile_step_height
+            self.inside_brain_tiles.shape[2] * self.tile_step_height
         )
         # Get maximum offsets for the ball
         max_width = tile_mask_covered_img_width - self.ball_xy_size
         max_height = tile_mask_covered_img_height - self.ball_xy_size
 
-        _walk(
-            max_height,
-            max_width,
-            self.tile_step_width,
-            self.tile_step_height,
-            self.inside_brain_tiles,
-            self.volume,
-            self.kernel,
-            ball_radius,
-            self.middle_z_idx,
-            self.overlap_threshold,
-            self.THRESHOLD_VALUE,
-            self.SOMA_CENTRE_VALUE,
-        )
+        # we have to pass the raw volume so walk doesn't use its edits as it
+        # processes the volume. self.volume is the one edited in place
+        input_volume = self.volume.copy()
+
+        if parallel:
+            _walk_parallel(
+                max_height,
+                max_width,
+                self.tile_step_width,
+                self.tile_step_height,
+                self.inside_brain_tiles,
+                input_volume,
+                self.volume,
+                self.kernel,
+                ball_radius,
+                self.middle_z_idx,
+                self.overlap_threshold,
+                self.THRESHOLD_VALUE,
+                self.SOMA_CENTRE_VALUE,
+            )
+        else:
+            _walk_single(
+                max_height,
+                max_width,
+                self.tile_step_width,
+                self.tile_step_height,
+                self.inside_brain_tiles,
+                input_volume,
+                self.volume,
+                self.kernel,
+                ball_radius,
+                self.middle_z_idx,
+                self.overlap_threshold,
+                self.THRESHOLD_VALUE,
+                self.SOMA_CENTRE_VALUE,
+            )
 
 
 @njit(cache=True)
 def _cube_overlaps(
-    cube: np.ndarray,
+    volume: np.ndarray,
+    x_start: int,
+    x_end: int,
+    y_start: int,
+    y_end: int,
     overlap_threshold: float,
-    THRESHOLD_VALUE: int,
+    threshold_value: int,
     kernel: np.ndarray,
 ) -> bool:  # Highly optimised because most time critical
     """
-    For each pixel in cube that is greater than THRESHOLD_VALUE, sum
+    For each pixel in cube in volume that is greater than THRESHOLD_VALUE, sum
     up the corresponding pixels in *kernel*. If the total is less than
     overlap_threshold, return False, otherwise return True.
 
     Halfway through scanning the z-planes, if the total overlap is
     less than 0.4 * overlap_threshold, this will return False early
     without scanning the second half of the z-planes.
 
     Parameters
     ----------
-    cube :
+    volume :
         3D array.
+    x_start, x_end, y_start, y_end :
+        The start and end indices in volume that form the cube. End is
+        exclusive
     overlap_threshold :
         Threshold above which to return True.
-    THRESHOLD_VALUE :
+    threshold_value :
         Value above which a pixel is marked as being part of a cell.
     kernel :
-        3D array, with the same shape as *cube*.
+        3D array, with the same shape as *cube* in the volume.
     """
-    current_overlap_value = 0
+    current_overlap_value = 0.0
 
-    middle = np.floor(cube.shape[2] / 2) + 1
+    middle = np.floor(volume.shape[0] / 2) + 1
     halfway_overlap_thresh = (
         overlap_threshold * 0.4
     )  # FIXME: do not hard code value
 
-    for z in range(cube.shape[2]):
+    for z in range(volume.shape[0]):
         # TODO: OPTIMISE: step from middle to outer boundaries to check
         # more data first
         #
         # If halfway through the array, and the overlap value isn't more than
         # 0.4 * the overlap threshold, return
         if z == middle and current_overlap_value < halfway_overlap_thresh:
             return False  # DEBUG: optimisation attempt
-        for y in range(cube.shape[1]):
-            for x in range(cube.shape[0]):
+
+        for y in range(y_start, y_end):
+            for x in range(x_start, x_end):
                 # includes self.SOMA_CENTRE_VALUE
-                if cube[x, y, z] >= THRESHOLD_VALUE:
-                    current_overlap_value += kernel[x, y, z]
+                if volume[z, x, y] >= threshold_value:
+                    # x/y must be shifted in kernel because we x/y is relative
+                    # to the full volume, so shift it to relative to the cube
+                    current_overlap_value += kernel[
+                        x - x_start, y - y_start, z
+                    ]
+
     return current_overlap_value > overlap_threshold
 
 
 @njit
 def _is_tile_to_check(
     x: int,
     y: int,
@@ -256,77 +333,85 @@
     inside_brain_tiles: np.ndarray,
 ) -> bool:  # Highly optimised because most time critical
     """
     Check if the tile containing pixel (x, y) is a tile that needs checking.
     """
     x_in_mask = x // tile_step_width  # TEST: test bounds (-1 range)
     y_in_mask = y // tile_step_height  # TEST: test bounds (-1 range)
-    return inside_brain_tiles[x_in_mask, y_in_mask, middle_z]
+    return inside_brain_tiles[middle_z, x_in_mask, y_in_mask]
 
 
-@njit
-def _walk(
+def _walk_base(
     max_height: int,
     max_width: int,
     tile_step_width: int,
     tile_step_height: int,
     inside_brain_tiles: np.ndarray,
+    input_volume: np.ndarray,
     volume: np.ndarray,
     kernel: np.ndarray,
     ball_radius: int,
     middle_z: int,
     overlap_threshold: float,
-    THRESHOLD_VALUE: int,
-    SOMA_CENTRE_VALUE: int,
+    threshold_value: int,
+    soma_centre_value: int,
 ) -> None:
     """
     Scan through *volume*, and mark pixels where there are enough surrounding
     pixels with high enough intensity.
 
     The surrounding area is defined by the *kernel*.
 
     Parameters
     ----------
     max_height, max_width :
         Maximum offsets for the ball filter.
     inside_brain_tiles :
-        Array containing information on whether a tile is inside the brain
-        or not. Tiles outside the brain are skipped.
+        3d array containing information on whether a tile is
+        inside the brain or not. Tiles outside the brain are skipped.
+    input_volume :
+        3D array containing the plane-filtered data passed to the function
+        before walking. volume is edited in place, so this is the original
+        volume to prevent the changes for some cubes affective other cubes
+        during a single walk call.
     volume :
-        3D array containing the plane-filtered data.
+        3D array containing the plane-filtered data - edited in place.
     kernel :
         3D array
     ball_radius :
         Radius of the ball in the xy plane.
-    SOMA_CENTRE_VALUE :
+    soma_centre_value :
         Value that is used to mark pixels in *volume*.
 
     Notes
     -----
     Warning: modifies volume in place!
     """
-    for y in range(max_height):
-        for x in range(max_width):
+    for y in prange(max_height):
+        for x in prange(max_width):
             ball_centre_x = x + ball_radius
             ball_centre_y = y + ball_radius
             if _is_tile_to_check(
                 ball_centre_x,
                 ball_centre_y,
                 middle_z,
                 tile_step_width,
                 tile_step_height,
                 inside_brain_tiles,
             ):
-                cube = volume[
-                    x : x + kernel.shape[0],
-                    y : y + kernel.shape[1],
-                    :,
-                ]
                 if _cube_overlaps(
-                    cube,
+                    input_volume,
+                    x,
+                    x + kernel.shape[0],
+                    y,
+                    y + kernel.shape[1],
                     overlap_threshold,
-                    THRESHOLD_VALUE,
+                    threshold_value,
                     kernel,
                 ):
-                    volume[ball_centre_x, ball_centre_y, middle_z] = (
-                        SOMA_CENTRE_VALUE
+                    volume[middle_z, ball_centre_x, ball_centre_y] = (
+                        soma_centre_value
                     )
+
+
+_walk_parallel = njit(parallel=True)(_walk_base)
+_walk_single = njit(parallel=False)(_walk_base)
```

### Comparing `cellfinder-1.1.3/cellfinder/core/detect/filters/volume/structure_detection.py` & `cellfinder-1.2.0/cellfinder/core/detect/filters/volume/structure_detection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from dataclasses import dataclass
-from typing import Dict, Optional, TypeVar
+from typing import Dict, Optional, Tuple, TypeVar, Union
 
 import numba.typed
 import numpy as np
 import numpy.typing as npt
-from numba import njit
+from numba import njit, typed
 from numba.core import types
 from numba.experimental import jitclass
 from numba.types import DictType
 
+T = TypeVar("T")
+# type used for the domain of the volume - the size of the vol
+vol_np_type = np.int64
+vol_numba_type = types.int64
+# type used for the structure id
+sid_np_type = np.int64
+sid_numba_type = types.int64
+
 
 @dataclass
 class Point:
     x: int
     y: int
     z: int
 
@@ -28,60 +36,74 @@
     min_val = np.iinfo(values.dtype).max
     for v in values:
         if v != 0 and v < min_val:
             min_val = v
     return min_val
 
 
-T = TypeVar("T")
-
-
 @njit
 def traverse_dict(d: Dict[T, T], a: T) -> T:
     """
     Traverse d, until a is not present as a key.
     """
-    if a in d:
-        return traverse_dict(d, d[a])
-    else:
-        return a
+    value = a
+    while value in d:
+        value = d[value]
+    return value
 
 
 @njit
 def get_structure_centre(structure: np.ndarray) -> np.ndarray:
     """
     Get the pixel coordinates of the centre of a structure.
 
     Centre calculated as the mean of each pixel coordinate,
     rounded to the nearest integer.
     """
-    # can't do np.mean(structure, axis=0)
-    # because axis is not supported by numba
+    # numba support axis for sum, but not mean
+    return np.round(np.sum(structure, axis=0) / structure.shape[0])
+
+
+@njit
+def _get_structure_centre(structure: types.ListType) -> np.ndarray:
+    # See get_structure_centre.
+    # this is for our own points stored as list optimized by numba
+    a_sum = 0.0
+    b_sum = 0.0
+    c_sum = 0.0
+    for a, b, c in structure:
+        a_sum += a
+        b_sum += b
+        c_sum += c
+
     return np.round(
         np.array(
             [
-                np.mean(structure[:, 0]),
-                np.mean(structure[:, 1]),
-                np.mean(structure[:, 2]),
+                a_sum / len(structure),
+                b_sum / len(structure),
+                c_sum / len(structure),
             ]
         )
     )
 
 
 # Type declaration has to come outside of the class,
 # see https://github.com/numba/numba/issues/8808
-uint_2d_type = types.uint64[:, :]
+tuple_point_type = types.Tuple(
+    (vol_numba_type, vol_numba_type, vol_numba_type)
+)
+list_of_points_type = types.ListType(tuple_point_type)
 
 
 spec = [
-    ("z", types.uint64),
-    ("next_structure_id", types.uint64),
-    ("shape", types.UniTuple(types.int64, 2)),
-    ("obsolete_ids", DictType(types.int64, types.int64)),
-    ("coords_maps", DictType(types.uint64, uint_2d_type)),
+    ("z", vol_numba_type),
+    ("next_structure_id", sid_numba_type),
+    ("shape", types.UniTuple(vol_numba_type, 2)),
+    ("obsolete_ids", DictType(sid_numba_type, sid_numba_type)),
+    ("coords_maps", DictType(sid_numba_type, list_of_points_type)),
 ]
 
 
 @jitclass(spec=spec)
 class CellDetector:
     """
     A class to detect connected structures within a series of
@@ -99,16 +121,20 @@
     obsolete_ids :
         Mapping from obsolete structure IDs to the structure ID they
         have been replaced with. This is used to keep track of structures
         that were initially disconnected, but later connected as the planes
         are scanned.
     coords_maps :
         Mapping from structure ID to the coordinates of pixels within that
-        structure. Coordinates are stored in a 2D array, with the second
-        axis indexing (x, y, z) coordinates.
+        structure. Coordinates are stored in a list of (x, y, z) tuples of
+        the coordinates.
+
+        Use `get_structures` to get it as a dict whose values are each
+        a 2D array, where rows are points, and columns x, y, z of the
+        points.
     """
 
     def __init__(self, width: int, height: int, start_z: int):
         """
         Parameters
         ----------
         width, height
@@ -119,28 +145,28 @@
         self.shape = width, height
         self.z = start_z
         self.next_structure_id = 1
 
         # Mapping from obsolete IDs to the IDs that they have been
         # made obsolete by
         self.obsolete_ids = numba.typed.Dict.empty(
-            key_type=types.int64, value_type=types.int64
+            key_type=sid_numba_type, value_type=sid_numba_type
         )
         # Mapping from IDs to list of points in that structure
         self.coords_maps = numba.typed.Dict.empty(
-            key_type=types.int64, value_type=uint_2d_type
+            key_type=sid_numba_type, value_type=list_of_points_type
         )
 
     def process(
         self, plane: np.ndarray, previous_plane: Optional[np.ndarray]
     ) -> np.ndarray:
         """
         Process a new plane.
         """
-        if [e for e in plane.shape[:2]] != [e for e in self.shape]:
+        if plane.shape[:2] != self.shape:
             raise ValueError("plane does not have correct shape")
 
         plane = self.connect_four(plane, previous_plane)
         self.z += 1
         return plane
 
     def connect_four(
@@ -162,15 +188,15 @@
             with their structure ID.
         """
         SOMA_CENTRE_VALUE = np.iinfo(plane.dtype).max
         for y in range(plane.shape[1]):
             for x in range(plane.shape[0]):
                 if plane[x, y] == SOMA_CENTRE_VALUE:
                     # Labels of structures below, left and behind
-                    neighbour_ids = np.zeros(3, dtype=np.uint64)
+                    neighbour_ids = np.zeros(3, dtype=sid_np_type)
                     # If in bounds look at neighbours
                     if x > 0:
                         neighbour_ids[0] = plane[x - 1, y]
                     if y > 0:
                         neighbour_ids[1] = plane[x, y - 1]
                     if previous_plane is not None:
                         neighbour_ids[2] = previous_plane[x, y]
@@ -187,49 +213,85 @@
                 plane[x, y] = struct_id
 
         return plane
 
     def get_cell_centres(self) -> np.ndarray:
         return self.structures_to_cells()
 
-    def get_coords_dict(self) -> Dict:
-        return self.coords_maps
+    def get_structures(self) -> Dict[int, np.ndarray]:
+        """
+        Gets the structures as a dict of structure IDs mapped to the 2D array
+        of structure points.
+        """
+        d = {}
+        for sid, points in self.coords_maps.items():
+            # numba silliness - it cannot handle
+            # `item = np.array(points, dtype=vol_np_type)` so we need to create
+            # array and then fill in the point
+            item = np.empty((len(points), 3), dtype=vol_np_type)
+            d[sid] = item
+
+            for i, point in enumerate(points):
+                item[i, :] = point
+
+        return d
+
+    def add_point(
+        self, sid: int, point: Union[tuple, list, np.ndarray]
+    ) -> None:
+        """
+        Add single 3d *point* to the structure with the given *sid*.
+        """
+        if sid not in self.coords_maps:
+            self.coords_maps[sid] = typed.List.empty_list(tuple_point_type)
+
+        self._add_point(sid, (int(point[0]), int(point[1]), int(point[2])))
 
-    def add_point(self, sid: int, point: np.ndarray) -> None:
+    def add_points(self, sid: int, points: np.ndarray):
         """
-        Add *point* to the structure with the given *sid*.
+        Adds ndarray of *points* to the structure with the given *sid*.
+        Each row is a 3d point.
         """
-        self.coords_maps[sid] = np.row_stack((self.coords_maps[sid], point))
+        if sid not in self.coords_maps:
+            self.coords_maps[sid] = typed.List.empty_list(tuple_point_type)
+
+        append = self.coords_maps[sid].append
+        pts = np.round(points).astype(vol_np_type)
+        for point in pts:
+            append((point[0], point[1], point[2]))
+
+    def _add_point(self, sid: int, point: Tuple[int, int, int]) -> None:
+        # sid must exist
+        self.coords_maps[sid].append(point)
 
     def add(
-        self, x: int, y: int, z: int, neighbour_ids: npt.NDArray[np.uint64]
+        self, x: int, y: int, z: int, neighbour_ids: npt.NDArray[sid_np_type]
     ) -> int:
         """
         For the current coordinates takes all the neighbours and find the
         minimum structure including obsolete structures mapping to any of
         the neighbours recursively.
 
         Once the correct structure id is found, append a point with the
         current coordinates to the coordinates map entry for the correct
         structure. Hence each entry of the map will be a vector of all the
         pertaining points.
         """
         updated_id = self.sanitise_ids(neighbour_ids)
         if updated_id not in self.coords_maps:
-            self.coords_maps[updated_id] = np.zeros(
-                shape=(0, 3), dtype=np.uint64
+            self.coords_maps[updated_id] = typed.List.empty_list(
+                tuple_point_type
             )
         self.merge_structures(updated_id, neighbour_ids)
 
         # Add point for that structure
-        point = np.array([[x, y, z]], dtype=np.uint64)
-        self.add_point(updated_id, point)
+        self._add_point(updated_id, (int(x), int(y), int(z)))
         return updated_id
 
-    def sanitise_ids(self, neighbour_ids: npt.NDArray[np.uint64]) -> int:
+    def sanitise_ids(self, neighbour_ids: npt.NDArray[sid_np_type]) -> int:
         """
         Get the smallest ID of all the structures that are connected to IDs
         in `neighbour_ids`.
 
         For all the neighbour ids, walk up the chain of obsolescence (self.
         obsolete_ids) to reassign the corresponding most obsolete structure
         to the current neighbour.
@@ -242,37 +304,39 @@
             neighbour_ids[i] = neighbour_id
 
         # Get minimum of all non-obsolete IDs
         updated_id = get_non_zero_dtype_min(neighbour_ids)
         return int(updated_id)
 
     def merge_structures(
-        self, updated_id: int, neighbour_ids: npt.NDArray[np.uint64]
+        self, updated_id: int, neighbour_ids: npt.NDArray[sid_np_type]
     ) -> None:
         """
         For all the neighbours, reassign all the points of neighbour to
         updated_id. Then deletes the now obsolete entry from the points
         map and add that entry to the obsolete_ids.
 
         Updates:
         - self.coords_maps
         - self.obsolete_ids
         """
         for neighbour_id in np.unique(neighbour_ids):
             # minimise ID so if neighbour with higher ID, reassign its points
             # to current
             if neighbour_id > updated_id:
-                self.add_point(updated_id, self.coords_maps[neighbour_id])
+                self.coords_maps[updated_id].extend(
+                    self.coords_maps[neighbour_id]
+                )
                 self.coords_maps.pop(neighbour_id)
                 self.obsolete_ids[neighbour_id] = updated_id
 
     def structures_to_cells(self) -> np.ndarray:
-        cell_centres = np.empty((len(self.coords_maps.keys()), 3))
+        cell_centres = np.empty((len(self.coords_maps), 3))
         for idx, structure in enumerate(self.coords_maps.values()):
-            p = get_structure_centre(structure)
+            p = _get_structure_centre(structure)
             cell_centres[idx] = p
         return cell_centres
 
 
 @njit
 def is_new_structure(neighbour_ids: np.ndarray) -> bool:
     for i in range(len(neighbour_ids)):
```

### Comparing `cellfinder-1.1.3/cellfinder/core/detect/filters/volume/structure_splitting.py` & `cellfinder-1.2.0/cellfinder/core/detect/filters/volume/structure_splitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     Returns:
         Tuple[np.ndarray, np.ndarray]:
             A tuple containing the filtered volume and the cell centres.
 
     """
     # OPTIMISE: reuse ball filter instance
 
-    good_tiles_mask = np.ones((1, 1, volume.shape[2]), dtype=bool)
+    good_tiles_mask = np.ones((1, 1, volume.shape[2]), dtype=np.bool_)
 
     plane_width, plane_height = volume.shape[:2]
 
     bf = BallFilter(
         plane_width,
         plane_height,
         ball_xy_size,
```

### Comparing `cellfinder-1.1.3/cellfinder/core/detect/filters/volume/volume_filter.py` & `cellfinder-1.2.0/cellfinder/core/detect/filters/volume/volume_filter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import math
+import multiprocessing.pool
 import os
+from functools import partial
 from queue import Queue
 from threading import Lock
 from typing import Any, Callable, List, Optional, Tuple
 
 import numpy as np
 from brainglobe_utils.cells.cells import Cell
 from tifffile import tifffile
@@ -73,15 +75,15 @@
 
     def process(
         self,
         async_result_queue: Queue,
         locks: List[Lock],
         *,
         callback: Callable[[int], None],
-    ) -> List[Cell]:
+    ) -> None:
         progress_bar = tqdm(total=self.n_planes, desc="Processing planes")
         for z in range(self.n_planes):
             # Get result from the queue.
             #
             # It is important to remove the result from the queue here
             # to free up memory once this plane has been processed by
             # the 3D filter here
@@ -104,19 +106,21 @@
 
             callback(self.z)
             self.z += 1
             progress_bar.update()
 
         progress_bar.close()
         logger.debug("3D filter done")
-        return self.get_results()
 
     def _run_filter(self) -> None:
         logger.debug(f"🏐 Ball filtering plane {self.z}")
-        self.ball_filter.walk()
+        # filtering original images, the images should be large enough in x/y
+        # to benefit from parallelization. Note: don't pass arg as keyword arg
+        # because numba gets stuck (probably b/c class jit is new)
+        self.ball_filter.walk(True)
 
         middle_plane = self.ball_filter.get_middle_plane()
         if self.save_planes:
             self.save_plane(middle_plane)
 
         logger.debug(f"🏫 Detecting structures for plane {self.z}")
         self.previous_plane = self.cell_detector.process(
@@ -130,74 +134,69 @@
             raise ValueError(
                 "plane_directory must be set to save planes to file"
             )
         plane_name = f"plane_{str(self.z).zfill(4)}.tif"
         f_path = os.path.join(self.plane_directory, plane_name)
         tifffile.imsave(f_path, plane.T)
 
-    def get_results(self) -> List[Cell]:
+    def get_results(self, worker_pool: multiprocessing.Pool) -> List[Cell]:
         logger.info("Splitting cell clusters and writing results")
 
         max_cell_volume = sphere_volume(
             self.soma_size_spread_factor * self.soma_diameter / 2
         )
 
         cells = []
+        needs_split = []
+        structures = self.cell_detector.get_structures().items()
+        logger.debug(f"Processing {len(structures)} found cells")
 
-        logger.debug(
-            f"Processing {len(self.cell_detector.coords_maps.items())} cells"
-        )
-        for cell_id, cell_points in self.cell_detector.coords_maps.items():
+        # first get all the cells that are not clusters
+        for cell_id, cell_points in structures:
             cell_volume = len(cell_points)
 
             if cell_volume < max_cell_volume:
                 cell_centre = get_structure_centre(cell_points)
-                cells.append(
-                    Cell(
-                        (
-                            cell_centre[0],
-                            cell_centre[1],
-                            cell_centre[2],
-                        ),
-                        Cell.UNKNOWN,
-                    )
-                )
+                cells.append(Cell(cell_centre.tolist(), Cell.UNKNOWN))
             else:
                 if cell_volume < self.max_cluster_size:
-                    try:
-                        cell_centres = split_cells(
-                            cell_points, outlier_keep=self.outlier_keep
-                        )
-                    except (ValueError, AssertionError) as err:
-                        raise StructureSplitException(
-                            f"Cell {cell_id}, error; {err}"
-                        )
-                    for cell_centre in cell_centres:
-                        cells.append(
-                            Cell(
-                                (
-                                    cell_centre[0],
-                                    cell_centre[1],
-                                    cell_centre[2],
-                                ),
-                                Cell.UNKNOWN,
-                            )
-                        )
+                    needs_split.append((cell_id, cell_points))
                 else:
                     cell_centre = get_structure_centre(cell_points)
-                    cells.append(
-                        Cell(
-                            (
-                                cell_centre[0],
-                                cell_centre[1],
-                                cell_centre[2],
-                            ),
-                            Cell.ARTIFACT,
-                        )
-                    )
+                    cells.append(Cell(cell_centre.tolist(), Cell.ARTIFACT))
+
+        if not needs_split:
+            logger.debug("Finished splitting cell clusters - none found")
+            return cells
+
+        # now split clusters into cells
+        logger.debug(f"Splitting {len(needs_split)} clusters")
+        progress_bar = tqdm(
+            total=len(needs_split), desc="Splitting cell clusters"
+        )
+
+        # we are not returning Cell instances from func because it'd be pickled
+        # by multiprocess which slows it down
+        func = partial(_split_cells, outlier_keep=self.outlier_keep)
+        for cell_centres in worker_pool.imap_unordered(func, needs_split):
+            for cell_centre in cell_centres:
+                cells.append(Cell(cell_centre.tolist(), Cell.UNKNOWN))
+            progress_bar.update()
+
+        progress_bar.close()
+        logger.debug(
+            f"Finished splitting cell clusters. Found {len(cells)} total cells"
+        )
 
-        logger.debug("Finished splitting cell clusters.")
         return cells
 
 
+def _split_cells(arg, outlier_keep):
+    cell_id, cell_points = arg
+    try:
+        return split_cells(cell_points, outlier_keep=outlier_keep)
+    except (ValueError, AssertionError) as err:
+        raise StructureSplitException(f"Cell {cell_id}, error; {err}")
+
+
 def sphere_volume(radius: float) -> float:
     return (4 / 3) * math.pi * radius**3
```

### Comparing `cellfinder-1.1.3/cellfinder/core/main.py` & `cellfinder-1.2.0/cellfinder/core/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 it's warnings are silenced
 """
 
 import os
 from typing import Callable, List, Optional, Tuple
 
 import numpy as np
+from brainglobe_utils.cells.cells import Cell
 from brainglobe_utils.general.logging import suppress_specific_logs
 
 from cellfinder.core import logger
-from cellfinder.core.download.models import model_type
+from cellfinder.core.download.download import model_type
 from cellfinder.core.train.train_yml import depth_type
 
 tf_suppress_log_messages = [
     "multiprocessing can interact badly with TensorFlow"
 ]
 
 
@@ -38,14 +39,17 @@
     n_sds_above_mean_thresh: int = 10,
     soma_spread_factor: float = 1.4,
     max_cluster_size: int = 100000,
     cube_width: int = 50,
     cube_height: int = 50,
     cube_depth: int = 20,
     network_depth: depth_type = "50",
+    skip_detection: bool = False,
+    skip_classification: bool = False,
+    detected_cells: List[Cell] = None,
     *,
     detect_callback: Optional[Callable[[int], None]] = None,
     classify_callback: Optional[Callable[[int], None]] = None,
     detect_finished_callback: Optional[Callable[[list], None]] = None,
 ) -> List:
     """
     Parameters
@@ -61,60 +65,66 @@
     """
     suppress_tf_logging(tf_suppress_log_messages)
 
     from cellfinder.core.classify import classify
     from cellfinder.core.detect import detect
     from cellfinder.core.tools import prep
 
-    logger.info("Detecting cell candidates")
+    if not skip_detection:
+        logger.info("Detecting cell candidates")
 
-    points = detect.main(
-        signal_array,
-        start_plane,
-        end_plane,
-        voxel_sizes,
-        soma_diameter,
-        max_cluster_size,
-        ball_xy_size,
-        ball_z_size,
-        ball_overlap_fraction,
-        soma_spread_factor,
-        n_free_cpus,
-        log_sigma_size,
-        n_sds_above_mean_thresh,
-        callback=detect_callback,
-    )
-
-    if detect_finished_callback is not None:
-        detect_finished_callback(points)
-
-    install_path = None
-    model_weights = prep.prep_model_weights(
-        model_weights, install_path, model, n_free_cpus
-    )
-    if len(points) > 0:
-        logger.info("Running classification")
-        points = classify.main(
-            points,
+        points = detect.main(
             signal_array,
-            background_array,
-            n_free_cpus,
+            start_plane,
+            end_plane,
             voxel_sizes,
-            network_voxel_sizes,
-            batch_size,
-            cube_height,
-            cube_width,
-            cube_depth,
-            trained_model,
-            model_weights,
-            network_depth,
-            callback=classify_callback,
+            soma_diameter,
+            max_cluster_size,
+            ball_xy_size,
+            ball_z_size,
+            ball_overlap_fraction,
+            soma_spread_factor,
+            n_free_cpus,
+            log_sigma_size,
+            n_sds_above_mean_thresh,
+            callback=detect_callback,
         )
+
+        if detect_finished_callback is not None:
+            detect_finished_callback(points)
     else:
-        logger.info("No candidates, skipping classification")
+        points = detected_cells or []  # if None
+        detect_finished_callback(points)
+
+    if not skip_classification:
+        install_path = None
+        model_weights = prep.prep_model_weights(
+            model_weights, install_path, model, n_free_cpus
+        )
+        if len(points) > 0:
+            logger.info("Running classification")
+            points = classify.main(
+                points,
+                signal_array,
+                background_array,
+                n_free_cpus,
+                voxel_sizes,
+                network_voxel_sizes,
+                batch_size,
+                cube_height,
+                cube_width,
+                cube_depth,
+                trained_model,
+                model_weights,
+                network_depth,
+                callback=classify_callback,
+            )
+        else:
+            logger.info("No candidates, skipping classification")
+
     return points
 
 
 def suppress_tf_logging(tf_suppress_log_messages: List[str]) -> None:
     """
     Prevents many lines of logs such as:
     "2019-10-24 16:54:41.363978: I tensorflow/stream_executor/platform/default
```

### Comparing `cellfinder-1.1.3/cellfinder/core/tools/array_operations.py` & `cellfinder-1.2.0/cellfinder/core/tools/array_operations.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/tools/geometry.py` & `cellfinder-1.2.0/cellfinder/core/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/tools/image_processing.py` & `cellfinder-1.2.0/cellfinder/core/tools/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/tools/prep.py` & `cellfinder-1.2.0/cellfinder/core/tools/prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 from typing import Optional
 
 from brainglobe_utils.general.config import get_config_obj
 from brainglobe_utils.general.system import get_num_processes
 
 import cellfinder.core.tools.tf as tf_tools
 from cellfinder.core import logger
-from cellfinder.core.download import models as model_download
-from cellfinder.core.download.download import amend_user_configuration
+from cellfinder.core.download.download import (
+    DEFAULT_DOWNLOAD_DIRECTORY,
+    amend_user_configuration,
+    download_models,
+    model_type,
+)
 from cellfinder.core.tools.source_files import user_specific_configuration_path
 
-home = Path.home()
-DEFAULT_INSTALL_PATH = home / ".cellfinder"
-
 
 def prep_model_weights(
     model_weights: Optional[os.PathLike],
     install_path: Optional[os.PathLike],
-    model_name: model_download.model_type,
+    model_name: model_type,
     n_free_cpus: int,
 ) -> Path:
     n_processes = get_num_processes(min_free_cpu_cores=n_free_cpus)
     prep_tensorflow(n_processes)
     model_weights = prep_models(model_weights, install_path, model_name)
 
     return model_weights
@@ -38,32 +39,32 @@
     tf_tools.set_tf_threads(max_threads)
     tf_tools.allow_gpu_memory_growth()
 
 
 def prep_models(
     model_weights_path: Optional[os.PathLike],
     install_path: Optional[os.PathLike],
-    model_name: model_download.model_type,
+    model_name: model_type,
 ) -> Path:
-    install_path = install_path or DEFAULT_INSTALL_PATH
+    install_path = install_path or DEFAULT_DOWNLOAD_DIRECTORY
     # if no model or weights, set default weights
     if model_weights_path is None:
         logger.debug("No model supplied, so using the default")
 
         config_file = user_specific_configuration_path()
 
         if not Path(config_file).exists():
             logger.debug("Custom config does not exist, downloading models")
-            model_path = model_download.main(model_name, install_path)
+            model_path = download_models(model_name, install_path)
             amend_user_configuration(new_model_path=model_path)
 
         model_weights = get_model_weights(config_file)
         if not model_weights.exists():
             logger.debug("Model weights do not exist, downloading")
-            model_path = model_download.main(model_name, install_path)
+            model_path = download_models(model_name, install_path)
             amend_user_configuration(new_model_path=model_path)
             model_weights = get_model_weights(config_file)
     else:
         model_weights = Path(model_weights_path)
     return model_weights
```

### Comparing `cellfinder-1.1.3/cellfinder/core/tools/source_files.py` & `cellfinder-1.2.0/cellfinder/core/tools/source_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from pathlib import Path
 
+from cellfinder import DEFAULT_CELLFINDER_DIRECTORY
+
 
 def default_configuration_path():
     """
     Returns the default configuration path for cellfinder.
 
     Returns:
         Path: The default configuration path.
@@ -13,15 +15,15 @@
 
 def user_specific_configuration_path():
     """
     Returns the path to the user-specific configuration file for cellfinder.
 
     This function returns the path to the user-specific configuration file
     for cellfinder. The user-specific configuration file is located in the
-    user's home directory under the ".cellfinder" folder and is named
-    "cellfinder.conf.custom".
+    user's home directory under the ".brainglobe/cellfinder" folder
+    and is named "cellfinder.conf.custom".
 
     Returns:
         Path: The path to the custom configuration file.
 
     """
-    return Path.home() / ".cellfinder" / "cellfinder.conf.custom"
+    return DEFAULT_CELLFINDER_DIRECTORY / "cellfinder.conf.custom"
```

### Comparing `cellfinder-1.1.3/cellfinder/core/tools/system.py` & `cellfinder-1.2.0/cellfinder/core/tools/system.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/tools/tf.py` & `cellfinder-1.2.0/cellfinder/core/tools/tf.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/tools/tiff.py` & `cellfinder-1.2.0/cellfinder/core/tools/tiff.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/tools/tools.py` & `cellfinder-1.2.0/cellfinder/core/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/core/train/train_yml.py` & `cellfinder-1.2.0/cellfinder/core/train/train_yml.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from brainglobe_utils.IO.yaml import read_yaml_section
 from fancylog import fancylog
 from sklearn.model_selection import train_test_split
 
 import cellfinder.core as program_for_log
 from cellfinder.core import logger
 from cellfinder.core.classify.resnet import layer_type
-from cellfinder.core.tools.prep import DEFAULT_INSTALL_PATH
+from cellfinder.core.download.download import DEFAULT_DOWNLOAD_DIRECTORY
 
 tf_suppress_log_messages = [
     "sample_weight modes were coerced from",
     "multiprocessing can interact badly with TensorFlow",
 ]
 
 depth_type = Literal["18", "34", "50", "101", "152"]
@@ -108,16 +108,15 @@
         "not purely alphabetically",
     )
     return parser
 
 
 def training_parse():
     from cellfinder.core.download.cli import (
-        download_directory_parser,
-        model_parser,
+        download_parser,
     )
 
     training_parser = ArgumentParser(
         formatter_class=ArgumentDefaultsHelpFormatter
     )
     training_parser.add_argument(
         "-y",
@@ -219,16 +218,15 @@
         "--save-progress",
         dest="save_progress",
         action="store_true",
         help="Save training progress to a .csv file",
     )
 
     training_parser = misc_parse(training_parser)
-    training_parser = model_parser(training_parser)
-    training_parser = download_directory_parser(training_parser)
+    training_parser = download_parser(training_parser)
     args = training_parser.parse_args()
 
     return args
 
 
 def parse_yaml(yaml_files, section="data"):
     data = []
@@ -302,15 +300,15 @@
 
 def run(
     output_dir,
     yaml_file,
     n_free_cpus=2,
     trained_model=None,
     model_weights=None,
-    install_path=DEFAULT_INSTALL_PATH,
+    install_path=DEFAULT_DOWNLOAD_DIRECTORY,
     model="resnet50_tv",
     network_depth="50",
     learning_rate=0.0001,
     continue_training=False,
     test_fraction=0.1,
     batch_size=16,
     no_augment=False,
```

### Comparing `cellfinder-1.1.3/cellfinder/napari/curation.py` & `cellfinder-1.2.0/cellfinder/napari/curation.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/napari/detect/detect_containers.py` & `cellfinder-1.2.0/cellfinder/napari/detect/detect_containers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Optional
+from typing import List, Optional
 
 import numpy
+from brainglobe_utils.cells.cells import Cell
 
 from cellfinder.napari.input_container import InputContainer
 from cellfinder.napari.utils import html_label_widget
 
 
 @dataclass
 class DataInputs(InputContainer):
@@ -55,14 +56,16 @@
         )
 
 
 @dataclass
 class DetectionInputs(InputContainer):
     """Container for cell candidate detection inputs."""
 
+    skip_detection: bool = False
+    detected_cells: Optional[List[Cell]] = None
     soma_diameter: float = 16.0
     ball_xy_size: float = 6
     ball_z_size: float = 15
     ball_overlap_fraction: float = 0.6
     log_sigma_size: float = 0.2
     n_sds_above_mean_thresh: int = 10
     soma_spread_factor: float = 1.4
@@ -71,14 +74,15 @@
     def as_core_arguments(self) -> dict:
         return super().as_core_arguments()
 
     @classmethod
     def widget_representation(cls) -> dict:
         return dict(
             detection_options=html_label_widget("Detection:"),
+            skip_detection=dict(value=cls.defaults()["skip_detection"]),
             soma_diameter=cls._custom_widget("soma_diameter"),
             ball_xy_size=cls._custom_widget(
                 "ball_xy_size", custom_label="Ball filter (xy)"
             ),
             ball_z_size=cls._custom_widget(
                 "ball_z_size", custom_label="Ball filter (z)"
             ),
@@ -103,14 +107,15 @@
         )
 
 
 @dataclass
 class ClassificationInputs(InputContainer):
     """Container for classification inputs."""
 
+    skip_classification: bool = False
     use_pre_trained_weights: bool = True
     trained_model: Optional[Path] = Path.home()
 
     def as_core_arguments(self) -> dict:
         args = super().as_core_arguments()
         del args["use_pre_trained_weights"]
         return args
@@ -119,14 +124,17 @@
     def widget_representation(cls) -> dict:
         return dict(
             classification_options=html_label_widget("Classification:"),
             use_pre_trained_weights=dict(
                 value=cls.defaults()["use_pre_trained_weights"]
             ),
             trained_model=dict(value=cls.defaults()["trained_model"]),
+            skip_classification=dict(
+                value=cls.defaults()["skip_classification"]
+            ),
         )
 
 
 @dataclass
 class MiscInputs(InputContainer):
     """Container for miscellaneous inputs."""
```

### Comparing `cellfinder-1.1.3/cellfinder/napari/detect/thread_worker.py` & `cellfinder-1.2.0/cellfinder/napari/detect/thread_worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from magicgui.widgets import ProgressBar
 from napari.qt.threading import WorkerBase, WorkerBaseSignals
 from qtpy.QtCore import Signal
 
 from cellfinder.core.main import main as cellfinder_run
 
 from .detect_containers import (
     ClassificationInputs,
@@ -37,14 +38,27 @@
     ):
         super().__init__(SignalsClass=MyWorkerSignals)
         self.data_inputs = data_inputs
         self.detection_inputs = detection_inputs
         self.classification_inputs = classification_inputs
         self.misc_inputs = misc_inputs
 
+    def connect_progress_bar_callback(self, progress_bar: ProgressBar):
+        """
+        Connects the progress bar to the work so that updates are shown on
+        the bar.
+        """
+
+        def update_progress_bar(label: str, max: int, value: int):
+            progress_bar.label = label
+            progress_bar.max = max
+            progress_bar.value = value
+
+        self.update_progress_bar.connect(update_progress_bar)
+
     def work(self) -> list:
         self.update_progress_bar.emit("Setting up detection...", 1, 0)
 
         def detect_callback(plane: int) -> None:
             self.update_progress_bar.emit(
                 "Detecting cells",
                 self.data_inputs.nplanes,
```

### Comparing `cellfinder-1.1.3/cellfinder/napari/input_container.py` & `cellfinder-1.2.0/cellfinder/napari/input_container.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/napari/napari.yaml` & `cellfinder-1.2.0/cellfinder/napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/napari/sample_data.py` & `cellfinder-1.2.0/cellfinder/napari/sample_data.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.3/cellfinder/napari/train/train.py` & `cellfinder-1.2.0/cellfinder/napari/train/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 from magicgui import magicgui
 from magicgui.widgets import FunctionGui, PushButton
 from napari.qt.threading import thread_worker
 from napari.utils.notifications import show_info
 from qtpy.QtWidgets import QScrollArea
 
 from cellfinder.core.train.train_yml import run as train_yml
-from cellfinder.napari.utils import (
-    header_label_widget,
-    html_label_widget,
-    widget_header,
-)
+from cellfinder.napari.utils import cellfinder_header, html_label_widget
 
 from .train_containers import (
     MiscTrainingInputs,
     OptionalNetworkInputs,
     OptionalTrainingInputs,
     TrainingDataInputs,
 )
@@ -37,26 +33,24 @@
         **misc_training_inputs.as_core_arguments(),
     )
     print("Finished!")
 
 
 def training_widget() -> FunctionGui:
     @magicgui(
-        header=header_label_widget,
         training_label=html_label_widget("Network training", tag="h3"),
         **TrainingDataInputs.widget_representation(),
         **OptionalNetworkInputs.widget_representation(),
         **OptionalTrainingInputs.widget_representation(),
         **MiscTrainingInputs.widget_representation(),
         call_button=True,
         reset_button=dict(widget_type="PushButton", text="Reset defaults"),
         scrollable=True,
     )
     def widget(
-        header: dict,
         training_label: dict,
         data_options: dict,
         yaml_files: Path,
         output_directory: Path,
         network_options: dict,
         trained_model: Optional[Path],
         model_weights: Optional[Path],
@@ -157,16 +151,15 @@
                 training_data_inputs,
                 optional_network_inputs,
                 optional_training_inputs,
                 misc_training_inputs,
             )
             worker.start()
 
-    widget.header.value = widget_header
-    widget.header.native.setOpenExternalLinks(True)
+    widget.native.layout().insertWidget(0, cellfinder_header())
 
     @widget.reset_button.changed.connect
     def restore_defaults():
         defaults = {
             **TrainingDataInputs.defaults(),
             **OptionalNetworkInputs.defaults(),
             **OptionalTrainingInputs.defaults(),
```

### Comparing `cellfinder-1.1.3/cellfinder/napari/train/train_containers.py` & `cellfinder-1.2.0/cellfinder/napari/train/train_containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 
 from magicgui.types import FileDialogMode
 
-from cellfinder.core.download.models import model_weight_urls
+from cellfinder.core.download.download import model_filenames
 from cellfinder.core.train.train_yml import models
 from cellfinder.napari.input_container import InputContainer
 from cellfinder.napari.utils import html_label_widget
 
 
 @dataclass
 class TrainingDataInputs(InputContainer):
@@ -42,15 +42,15 @@
 @dataclass
 class OptionalNetworkInputs(InputContainer):
     """Container for Optional Network input widgets"""
 
     trained_model: Optional[Path] = Path.home()
     model_weights: Optional[Path] = Path.home()
     model_depth: str = list(models.keys())[2]
-    pretrained_model: str = str(list(model_weight_urls.keys())[0])
+    pretrained_model: str = str(list(model_filenames.keys())[0])
 
     def as_core_arguments(self) -> dict:
         arguments = super().as_core_arguments()
         arguments["model"] = arguments.pop("pretrained_model")
         arguments["network_depth"] = arguments.pop("model_depth")
         return arguments
 
@@ -61,15 +61,15 @@
             trained_model=cls._custom_widget("trained_model"),
             model_weights=cls._custom_widget("model_weights"),
             model_depth=cls._custom_widget(
                 "model_depth", choices=list(models.keys())
             ),
             pretrained_model=cls._custom_widget(
                 "pretrained_model",
-                choices=list(model_weight_urls.keys()),
+                choices=list(model_filenames.keys()),
             ),
         )
 
 
 @dataclass
 class OptionalTrainingInputs(InputContainer):
     continue_training: bool = False
```

### Comparing `cellfinder-1.1.3/cellfinder.egg-info/PKG-INFO` & `cellfinder-1.2.0/cellfinder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.1.3
+Version: 1.2.0
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: brainglobe-utils>=0.4.2
+Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: brainglobe-napari-io>=0.3.4
 Requires-Dist: dask[array]
 Requires-Dist: fancylog>=0.0.7
 Requires-Dist: natsort
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: scikit-image
@@ -50,25 +50,25 @@
 Requires-Dist: magicgui; extra == "napari"
 Requires-Dist: napari-ndtiffs; extra == "napari"
 Requires-Dist: napari-plugin-engine>=0.1.4; extra == "napari"
 Requires-Dist: napari[pyqt5]; extra == "napari"
 Requires-Dist: pooch>=1; extra == "napari"
 Requires-Dist: qtpy; extra == "napari"
 
-[![Python Version](https://img.shields.io/pypi/pyversions/cellfinder-core.svg)](https://pypi.org/project/cellfinder)
-[![PyPI](https://img.shields.io/pypi/v/cellfinder-core.svg)](https://pypi.org/project/cellfinder)
-[![Downloads](https://pepy.tech/badge/cellfinder-core)](https://pepy.tech/project/cellfinder)
-[![Wheel](https://img.shields.io/pypi/wheel/cellfinder-core.svg)](https://pypi.org/project/cellfinder)
-[![Development Status](https://img.shields.io/pypi/status/cellfinder-core.svg)](https://github.com/brainglobe/cellfinder)
+[![Python Version](https://img.shields.io/pypi/pyversions/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![PyPI](https://img.shields.io/pypi/v/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Downloads](https://pepy.tech/badge/cellfinder)](https://pepy.tech/project/cellfinder)
+[![Wheel](https://img.shields.io/pypi/wheel/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Development Status](https://img.shields.io/pypi/status/cellfinder.svg)](https://github.com/brainglobe/cellfinder)
 [![Tests](https://img.shields.io/github/actions/workflow/status/brainglobe/cellfinder/test_and_deploy.yml?branch=main)](https://github.com/brainglobe/cellfinder/actions)
-[![codecov](https://codecov.io/gh/brainglobe/cellfinder-core/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder)
+[![codecov](https://codecov.io/gh/brainglobe/cellfinder/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/developers/index.html)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/community/developers/index.html)
 [![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
 
 # cellfinder
 
 cellfinder is software for automated 3D cell detection in very large 3D images (e.g., serial two-photon or lightsheet volumes of whole mouse brains).
 There are three different ways to interact and use it, each with different user interfaces and objectives in mind.
 For more details, head over to [the documentation website](https://brainglobe.info/documentation/cellfinder/index.html).
```

### Comparing `cellfinder-1.1.3/cellfinder.egg-info/SOURCES.txt` & `cellfinder-1.2.0/cellfinder.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,14 @@
 cellfinder/core/detect/filters/volume/ball_filter.py
 cellfinder/core/detect/filters/volume/structure_detection.py
 cellfinder/core/detect/filters/volume/structure_splitting.py
 cellfinder/core/detect/filters/volume/volume_filter.py
 cellfinder/core/download/__init__.py
 cellfinder/core/download/cli.py
 cellfinder/core/download/download.py
-cellfinder/core/download/models.py
-cellfinder/core/tools/IO.py
 cellfinder/core/tools/__init__.py
 cellfinder/core/tools/array_operations.py
 cellfinder/core/tools/geometry.py
 cellfinder/core/tools/image_processing.py
 cellfinder/core/tools/prep.py
 cellfinder/core/tools/source_files.py
 cellfinder/core/tools/system.py
@@ -62,11 +60,10 @@
 cellfinder/napari/napari.yaml
 cellfinder/napari/sample_data.py
 cellfinder/napari/utils.py
 cellfinder/napari/detect/__init__.py
 cellfinder/napari/detect/detect.py
 cellfinder/napari/detect/detect_containers.py
 cellfinder/napari/detect/thread_worker.py
-cellfinder/napari/images/brainglobe.png
 cellfinder/napari/train/__init__.py
 cellfinder/napari/train/train.py
 cellfinder/napari/train/train_containers.py
```

### Comparing `cellfinder-1.1.3/cellfinder.egg-info/requires.txt` & `cellfinder-1.2.0/cellfinder.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-brainglobe-utils>=0.4.2
+brainglobe-utils>=0.5.0
 brainglobe-napari-io>=0.3.4
 dask[array]
 fancylog>=0.0.7
 natsort
 numba
 numpy
 scikit-image
```

### Comparing `cellfinder-1.1.3/pyproject.toml` & `cellfinder-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Image Recognition",
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "brainglobe-utils>=0.4.2",
+    "brainglobe-utils>=0.5.0",
     "brainglobe-napari-io>=0.3.4",
     "dask[array]",
     "fancylog>=0.0.7",
     "natsort",
     "numba",
     "numpy",
     "scikit-image",
@@ -116,15 +116,15 @@
 
 [gh-actions]
 python =
     3.9: py39
     3.10: py310
 
 [testenv]
-commands = python -m pytest -v --color=yes
+commands = python -m pytest -v --color=yes --cov=cellfinder --cov-report=xml
 deps =
     pytest
     pytest-cov
     pytest-mock
     pytest-timeout
     # Even though napari is a requirement for cellfinder.napari, we have to
     # ensure it is installed with the default Qt backend here.
```

