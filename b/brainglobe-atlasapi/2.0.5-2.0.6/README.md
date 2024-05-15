# Comparing `tmp/brainglobe-atlasapi-2.0.5.tar.gz` & `tmp/brainglobe_atlasapi-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-atlasapi-2.0.5.tar", last modified: Mon Apr  8 16:12:23 2024, max compression
+gzip compressed data, was "brainglobe_atlasapi-2.0.6.tar", last modified: Wed May 15 15:38:16 2024, max compression
```

## Comparing `brainglobe-atlasapi-2.0.5.tar` & `brainglobe_atlasapi-2.0.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.496846 brainglobe-atlasapi-2.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.496846 brainglobe-atlasapi-2.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.496846 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.500846 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/admba_3d_dev_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_cord.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/azba_zfish.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/example_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/humanatlas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_developmental_ccf_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/mpin_zfish.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/osten_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/perens_lsfm_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/princeton_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/template_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/whs_sd_rat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/main_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/stacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/structure_json_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/validate_atlases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/volume_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/wrapup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/bg_atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/list_atlases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/structure_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/structure_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/update_atlases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:16.672633 brainglobe_atlasapi-2.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:16.660633 brainglobe_atlasapi-2.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:16.664633 brainglobe_atlasapi-2.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-05-15 15:38:16.672633 brainglobe_atlasapi-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:16.664633 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:16.668633 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:16.672633 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/admba_3d_dev_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_cord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/azba_zfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/example_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/humanatlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_developmental_ccf_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/mpin_zfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/osten_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/perens_lsfm_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/princeton_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/template_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/whs_sd_rat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/main_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/stacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/structure_json_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/validate_atlases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/volume_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/wrapup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/bg_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/list_atlases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/structure_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/structure_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/update_atlases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:16.672633 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-05-15 15:38:16.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-15 15:38:16.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:38:16.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 15:38:16.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 15:38:16.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 15:38:16.000000 brainglobe_atlasapi-2.0.6/brainglobe_atlasapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 15:38:10.000000 brainglobe_atlasapi-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:38:16.672633 brainglobe_atlasapi-2.0.6/setup.cfg
```

### Comparing `brainglobe-atlasapi-2.0.5/.github/workflows/test_and_deploy.yml` & `brainglobe_atlasapi-2.0.6/.github/workflows/test_and_deploy.yml`

 * *Files 9% similar despite different names*

```diff
@@ -26,23 +26,26 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         # Run across a mixture of Python versions and operating systems
         include:
         - os: ubuntu-latest
           python-version: "3.11"
-        - os: macos-latest
+        - os: macos-13 # Intel Mac
+          python-version: "3.11"
+        - os: macos-latest # ARM Mac
           python-version: "3.10"
         - os: windows-latest
           python-version: "3.9"
 
     steps:
       - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: ${{ matrix.python-version }}
+          secret-codecov-token: ${{ secrets.CODECOV_TOKEN }}
 
   build_sdist_wheels:
     name: Build source distribution and wheel
     needs: [test]
     if: github.event_name == 'push' && github.ref_type == 'tag'
     runs-on: ubuntu-latest
     steps:
```

### Comparing `brainglobe-atlasapi-2.0.5/.gitignore` & `brainglobe_atlasapi-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/CITATION.cff` & `brainglobe_atlasapi-2.0.6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/LICENSE` & `brainglobe_atlasapi-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/PKG-INFO` & `brainglobe_atlasapi-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-atlasapi
-Version: 2.0.5
+Version: 2.0.6
 Summary: A lightweight python module to interact with and generate atlases for systems neuroscience.
 Author-email: "Luigi Petrucco, Federico Claudi, Adam Tyson" <code@adamltyson.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, BrainGlobe
         All rights reserved.
```

### Comparing `brainglobe-atlasapi-2.0.5/README.md` & `brainglobe_atlasapi-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/admba_3d_dev_mouse.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/admba_3d_dev_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_cord.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_cord.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_mouse.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/azba_zfish.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/azba_zfish.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/example_mouse.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/example_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/humanatlas.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/humanatlas.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import treelib
 import urllib3
 from allensdk.core.structure_tree import StructureTree
-from brainio import brainio
+from brainglobe_utils.IO.image.load import load_any
 from rich.progress import track
 
-# import sys
-# sys.path.append("./")
 from brainglobe_atlasapi.atlas_generation.mesh_utils import (
     Region,
     create_region_mesh,
     inspect_meshes_folder,
 )
 from brainglobe_atlasapi.atlas_generation.wrapup import wrapup_atlas_from_data
 from brainglobe_atlasapi.structure_tree_util import get_structures_tree
@@ -95,16 +93,16 @@
     # Temporary folder for files before compressing:
     uncompr_atlas_path = temp_path / ATLAS_NAME
     uncompr_atlas_path.mkdir(exist_ok=True)
 
     # ---------------- #
     #   GET TEMPLATE   #
     # ---------------- #
-    annotation = brainio.load_any(annotations_image)  # shape (394, 466, 378)
-    anatomy = brainio.load_any(anatomy_image)  # shape (394, 466, 378)
+    annotation = load_any(annotations_image)  # shape (394, 466, 378)
+    anatomy = load_any(anatomy_image)  # shape (394, 466, 378)
 
     # Remove weird artefact
     annotation = annotation[:200, :, :]
     anatomy = anatomy[:200, :, :]
 
     # show(Volume(root_annotation), axes=1)
```

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_developmental_ccf_mouse.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_developmental_ccf_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_mouse.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/osten_mouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-__version__ = "1"
+__version__ = "0"
 
 import json
 import multiprocessing as mp
 import tarfile
 import time
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import tifffile
 from allensdk.core.reference_space_cache import ReferenceSpaceCache
 from rich.progress import track
 from scipy.ndimage import zoom
 
-# import sys
-# sys.path.append("./")
 from brainglobe_atlasapi import utils
 from brainglobe_atlasapi.atlas_generation.mesh_utils import (
     Region,
     create_region_mesh,
 )
 from brainglobe_atlasapi.atlas_generation.wrapup import wrapup_atlas_from_data
 from brainglobe_atlasapi.structure_tree_util import get_structures_tree
 
 PARALLEL = False  # disable parallel mesh extraction for easier debugging
 
 
 def create_atlas(working_dir, resolution):
-    ATLAS_NAME = "kim_mouse"
+    ATLAS_NAME = "osten_mouse"
     SPECIES = "Mus musculus"
-    ATLAS_LINK = "https://kimlab.io/brain-map/atlas/"
-    CITATION = "Chon et al. 2019, https://doi.org/10.1038/s41467-019-13057-w"
+    ATLAS_LINK = "https://doi.org/10.1016/j.celrep.2014.12.014"
+    CITATION = "Kim et al. 2015, https://doi.org/10.1016/j.celrep.2014.12.014"
     ORIENTATION = "asr"
     ROOT_ID = 997
     ANNOTATIONS_RES_UM = 10
-    ATLAS_FILE_URL = "https://gin.g-node.org/brainglobe/kim_atlas_materials/raw/master/kim_atlas_materials.tar.gz"
+    ATLAS_FILE_URL = "https://gin.g-node.org/brainglobe/osten_atlas_materials/raw/master/osten_atlas_materials.tar.gz"
 
     # Temporary folder for  download:
     download_dir_path = working_dir / "downloads"
     download_dir_path.mkdir(exist_ok=True)
     atlas_files_dir = download_dir_path / "atlas_files"
 
     # Download atlas_file
@@ -49,16 +47,16 @@
 
     tar = tarfile.open(destination_path)
     tar.extractall(path=atlas_files_dir)
     tar.close()
 
     destination_path.unlink()
 
-    structures_file = atlas_files_dir / "kim_atlas" / "structures.csv"
-    annotations_file = atlas_files_dir / "kim_atlas" / "annotation.tiff"
+    structures_file = atlas_files_dir / "osten_atlas" / "structures.csv"
+    annotations_file = atlas_files_dir / "osten_atlas" / "annotation.tiff"
 
     # ---------------- #
     #   GET TEMPLATE   #
     # ---------------- #
 
     # Load (and possibly downsample) annotated volume:
     scaling = ANNOTATIONS_RES_UM / resolution
@@ -85,25 +83,25 @@
     # ------------------------ #
     #   STRUCTURES HIERARCHY   #
     # ------------------------ #
 
     # Parse region names & hierarchy
     # ##############################
     df = pd.read_csv(structures_file)
-    df = df.drop(columns=["Unnamed: 0", "parent_id", "parent_acronym"])
+    df = df.drop(columns=["parent_id"])
 
     # split by "/" and convert list of strings to list of ints
     df["structure_id_path"] = (
         df["structure_id_path"]
         .str.split(pat="/")
         .map(lambda x: [int(i) for i in x])
     )
-
+    df["structure_id_path"] = df["structure_id_path"].map(lambda x: x[:-1])
     structures = df.to_dict("records")
-
+    structures[0000]["structure_id_path"] = [997]
     for structure in structures:
         structure.update({"rgb_triplet": [255, 255, 255]})
         # root doesn't have a parent
         if structure["id"] != 997:
             structure["structure_id_path"].append(structure["id"])
 
     # save regions list json:
@@ -128,15 +126,14 @@
 
         node.data = Region(is_label)
 
     # Mesh creation
     closing_n_iters = 2
     decimate_fraction = 0.2
     smooth = False  # smooth meshes after creation
-
     start = time.time()
     if PARALLEL:
         pool = mp.Pool(mp.cpu_count() - 2)
 
         try:
             pool.map(
                 create_region_mesh,
@@ -233,13 +230,13 @@
         scale_meshes=True,
     )
 
     return output_filename
 
 
 if __name__ == "__main__":
-    resolution = 10  # some resolution, in microns (10, 25, 50, 100)
+    resolution = 100  # some resolution, in microns
 
     # Generated atlas path:
-    bg_root_dir = Path.home() / "brainglobe_workingdir" / "kim_mouse"
+    bg_root_dir = Path.home() / "brainglobe_workingdir" / "osten_mouse"
     bg_root_dir.mkdir(exist_ok=True, parents=True)
     create_atlas(bg_root_dir, resolution)
```

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/mpin_zfish.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/mpin_zfish.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/osten_mouse.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_mouse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-__version__ = "0"
+__version__ = "1"
 
+import argparse
 import json
 import multiprocessing as mp
 import tarfile
 import time
 from pathlib import Path
 
 import numpy as np
@@ -21,22 +22,22 @@
 from brainglobe_atlasapi.atlas_generation.wrapup import wrapup_atlas_from_data
 from brainglobe_atlasapi.structure_tree_util import get_structures_tree
 
 PARALLEL = False  # disable parallel mesh extraction for easier debugging
 
 
 def create_atlas(working_dir, resolution):
-    ATLAS_NAME = "osten_mouse"
+    ATLAS_NAME = "kim_mouse"
     SPECIES = "Mus musculus"
-    ATLAS_LINK = "https://doi.org/10.1016/j.celrep.2014.12.014"
-    CITATION = "Kim et al. 2015, https://doi.org/10.1016/j.celrep.2014.12.014"
+    ATLAS_LINK = "https://kimlab.io/brain-map/atlas/"
+    CITATION = "Chon et al. 2019, https://doi.org/10.1038/s41467-019-13057-w"
     ORIENTATION = "asr"
     ROOT_ID = 997
     ANNOTATIONS_RES_UM = 10
-    ATLAS_FILE_URL = "https://gin.g-node.org/brainglobe/osten_atlas_materials/raw/master/osten_atlas_materials.tar.gz"
+    ATLAS_FILE_URL = "https://gin.g-node.org/brainglobe/kim_atlas_materials/raw/master/kim_atlas_materials.tar.gz"
 
     # Temporary folder for  download:
     download_dir_path = working_dir / "downloads"
     download_dir_path.mkdir(exist_ok=True)
     atlas_files_dir = download_dir_path / "atlas_files"
 
     # Download atlas_file
@@ -47,16 +48,16 @@
 
     tar = tarfile.open(destination_path)
     tar.extractall(path=atlas_files_dir)
     tar.close()
 
     destination_path.unlink()
 
-    structures_file = atlas_files_dir / "osten_atlas" / "structures.csv"
-    annotations_file = atlas_files_dir / "osten_atlas" / "annotation.tiff"
+    structures_file = atlas_files_dir / "kim_atlas" / "structures.csv"
+    annotations_file = atlas_files_dir / "kim_atlas" / "annotation.tiff"
 
     # ---------------- #
     #   GET TEMPLATE   #
     # ---------------- #
 
     # Load (and possibly downsample) annotated volume:
     scaling = ANNOTATIONS_RES_UM / resolution
@@ -83,25 +84,25 @@
     # ------------------------ #
     #   STRUCTURES HIERARCHY   #
     # ------------------------ #
 
     # Parse region names & hierarchy
     # ##############################
     df = pd.read_csv(structures_file)
-    df = df.drop(columns=["parent_id"])
+    df = df.drop(columns=["Unnamed: 0", "parent_id", "parent_acronym"])
 
     # split by "/" and convert list of strings to list of ints
     df["structure_id_path"] = (
         df["structure_id_path"]
         .str.split(pat="/")
         .map(lambda x: [int(i) for i in x])
     )
-    df["structure_id_path"] = df["structure_id_path"].map(lambda x: x[:-1])
+
     structures = df.to_dict("records")
-    structures[0000]["structure_id_path"] = [997]
+
     for structure in structures:
         structure.update({"rgb_triplet": [255, 255, 255]})
         # root doesn't have a parent
         if structure["id"] != 997:
             structure["structure_id_path"].append(structure["id"])
 
     # save regions list json:
@@ -111,43 +112,42 @@
     # Create meshes:
     print(f"Saving atlas data at {download_dir_path}")
     meshes_dir_path = download_dir_path / "meshes"
     meshes_dir_path.mkdir(exist_ok=True)
 
     tree = get_structures_tree(structures)
 
-    rotated_annotations = np.rot90(annotated_volume, axes=(0, 2))
-
-    labels = np.unique(rotated_annotations).astype(np.int32)
+    labels = np.unique(annotated_volume).astype(np.int32)
     for key, node in tree.nodes.items():
         if key in labels:
             is_label = True
         else:
             is_label = False
 
         node.data = Region(is_label)
 
     # Mesh creation
     closing_n_iters = 2
     decimate_fraction = 0.2
     smooth = False  # smooth meshes after creation
+
     start = time.time()
     if PARALLEL:
         pool = mp.Pool(mp.cpu_count() - 2)
 
         try:
             pool.map(
                 create_region_mesh,
                 [
                     (
                         meshes_dir_path,
                         node,
                         tree,
                         labels,
-                        rotated_annotations,
+                        annotated_volume,
                         ROOT_ID,
                         closing_n_iters,
                         decimate_fraction,
                         smooth,
                     )
                     for node in tree.nodes.values()
                 ],
@@ -163,15 +163,15 @@
         ):
             create_region_mesh(
                 (
                     meshes_dir_path,
                     node,
                     tree,
                     labels,
-                    rotated_annotations,
+                    annotated_volume,
                     ROOT_ID,
                     closing_n_iters,
                     decimate_fraction,
                     smooth,
                 )
             )
 
@@ -230,13 +230,25 @@
         scale_meshes=True,
     )
 
     return output_filename
 
 
 if __name__ == "__main__":
-    resolution = 100  # some resolution, in microns
+    # Create argument parser to pass resoulution as an argument
+    parser = argparse.ArgumentParser(
+        description="Create an atlas with a specified resolution."
+    )
+    parser.add_argument(
+        "--resolution",
+        type=int,
+        default=10,
+        help="Resolution in microns (10, 25, 50, 100)",
+    )
+    args = parser.parse_args()
 
     # Generated atlas path:
-    bg_root_dir = Path.home() / "brainglobe_workingdir" / "osten_mouse"
+    bg_root_dir = Path.home() / "brainglobe_workingdir" / "kim_mouse"
     bg_root_dir.mkdir(exist_ok=True, parents=True)
-    create_atlas(bg_root_dir, resolution)
+
+    # Use the parsed resolution
+    create_atlas(bg_root_dir, args.resolution)
```

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/perens_lsfm_mouse.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/perens_lsfm_mouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-__version__ = "0"
+__version__ = "2"
 
 import json
 import multiprocessing as mp
 import tarfile
 import time
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import SimpleITK as sitk
 from rich.progress import track
 
-# from allensdk.core.reference_space_cache import ReferenceSpaceCache
 from brainglobe_atlasapi import utils
 from brainglobe_atlasapi.atlas_generation.mesh_utils import (
     Region,
     create_region_mesh,
 )
 from brainglobe_atlasapi.atlas_generation.wrapup import wrapup_atlas_from_data
 from brainglobe_atlasapi.structure_tree_util import get_structures_tree
 
-PARALLEL = False  # disable parallel mesh extraction for easier debugging
+PARALLEL = True  # disable parallel mesh extraction for easier debugging
 
 
 ### Additional functions #####################################################
 
 
 ##############################################################################
 def get_id_from_acronym(df, acronym):
@@ -141,15 +140,15 @@
 
 
 def create_atlas(working_dir, resolution):
     ATLAS_NAME = "perens_lsfm_mouse"
     SPECIES = "Mus musculus"
     ATLAS_LINK = "https://github.com/Gubra-ApS/LSFM-mouse-brain-atlas"
     CITATION = "Perens et al. 2021, https://doi.org/10.1007/s12021-020-09490-8"
-    ORIENTATION = "rai"
+    ORIENTATION = "ial"
     ROOT_ID = 997
     ATLAS_FILE_URL = "https://github.com/Gubra-ApS/LSFM-mouse-brain-atlas/archive/master.tar.gz"
 
     # Temporary folder for  download:
     download_dir_path = working_dir / "downloads"
     download_dir_path.mkdir(exist_ok=True)
     atlas_files_dir = download_dir_path / "atlas_files"
@@ -187,16 +186,14 @@
 
     annotated_volume = sitk.GetArrayFromImage(
         sitk.ReadImage(str(annotations_file))
     )
     template_volume = sitk.GetArrayFromImage(
         sitk.ReadImage(str(reference_file))
     )
-    annotated_volume = np.rot90(annotated_volume, axes=(0, 2))
-    template_volume = np.rot90(template_volume, axes=(0, 2))
 
     print("Download completed...")
 
     # ------------------------ #
     #   STRUCTURES HIERARCHY   #
     # ------------------------ #
 
@@ -244,15 +241,18 @@
             is_label = True
         else:
             is_label = False
 
         node.data = Region(is_label)
 
     # Mesh creation
-    closing_n_iters = 2
+    closing_n_iters = 2  # not used for this atlas
+    decimate_fraction = 0.2  # not used for this atlas
+
+    smooth = False
     start = time.time()
     if PARALLEL:
         pool = mp.Pool(mp.cpu_count() - 2)
 
         try:
             pool.map(
                 create_region_mesh,
@@ -261,14 +261,16 @@
                         meshes_dir_path,
                         node,
                         tree,
                         labels,
                         annotated_volume,
                         ROOT_ID,
                         closing_n_iters,
+                        decimate_fraction,
+                        smooth,
                     )
                     for node in tree.nodes.values()
                 ],
             )
         except mp.pool.MaybeEncodingError:
             # error with returning results from pool.map but we don't care
             pass
@@ -283,14 +285,16 @@
                     meshes_dir_path,
                     node,
                     tree,
                     labels,
                     annotated_volume,
                     ROOT_ID,
                     closing_n_iters,
+                    decimate_fraction,
+                    smooth,
                 )
             )
 
     print(
         "Finished mesh extraction in: ",
         round((time.time() - start) / 60, 2),
         " minutes",
```

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/princeton_mouse.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/princeton_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/template_script.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/template_script.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/whs_sd_rat.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/atlas_scripts/whs_sd_rat.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/main_script.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/main_script.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/mesh_utils.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/metadata_utils.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/stacks.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/stacks.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/structure_json_to_csv.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/structure_json_to_csv.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/structures.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/structures.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/validate_atlases.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/validate_atlases.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/volume_utils.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/volume_utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/wrapup.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/atlas_generation/wrapup.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/bg_atlas.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/bg_atlas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tarfile
 from io import StringIO
 from pathlib import Path
+from typing import Optional
 
 import requests
 from rich import print as rprint
 from rich.console import Console
 
 from brainglobe_atlasapi import config, core, descriptors, utils
 from brainglobe_atlasapi.utils import _rich_atlas_metadata
@@ -173,31 +174,49 @@
         # Uncompress in brainglobe path:
         tar = tarfile.open(destination_path)
         tar.extractall(path=self.brainglobe_dir)
         tar.close()
 
         destination_path.unlink()
 
-    def check_latest_version(self):
-        """Checks if the local version is the latest available
+    def check_latest_version(
+        self, print_warning: bool = True
+    ) -> Optional[bool]:
+        """
+        Checks if the local version is the latest available
         and prompts the user to update if not.
+
+        Parameters
+        ----------
+        print_warning : bool, optional
+            If True, prints a message if the local version is not the latest,
+            by default True. Useful to turn off, e.g. when the user is updating
+            the atlas
+
+        Returns
+        -------
+        Optional[bool]
+            Returns False if the local version is not the latest,
+            True if it is, and None if we are offline.
         """
+
         if self.remote_version is None:  # in this case, we are offline
             return
         local = _version_str_from_tuple(self.local_version)
         online = _version_str_from_tuple(self.remote_version)
 
         if local != online:
-            rprint(
-                f"[b][magenta2]brainglobe_atlasapi[/b]: "
-                f"[b]{self.atlas_name}[/b] version [b]{local}[/b]"
-                f"is not the latest available ([b]{online}[/b]). "
-                "To update the atlas run in the terminal:[/magenta2]\n"
-                f"    [gold1]brainglobe update -a {self.atlas_name}[/gold1]"
-            )
+            if print_warning:
+                rprint(
+                    "[b][magenta2]brainglobe_atlasapi[/b]: "
+                    f"[b]{self.atlas_name}[/b] version [b]{local}[/b] "
+                    f"is not the latest available ([b]{online}[/b]). "
+                    "To update the atlas run in the terminal:[/magenta2]\n"
+                    f" [gold1]brainglobe update -a {self.atlas_name}[/gold1]"
+                )
             return False
         return True
 
     def __repr__(self):
         """Fancy print providing atlas information."""
         name_split = self.atlas_name.split("_")
         pretty_name = "{} {} atlas (res. {})".format(*name_split)
```

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/cli.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/cli.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/config.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/config.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/core.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/core.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/descriptors.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/descriptors.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/list_atlases.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/list_atlases.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/structure_class.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/structure_class.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/structure_tree_util.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/structure_tree_util.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/update_atlases.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/update_atlases.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     atlas_name: str
         Name of the atlas to update.
     force: bool
         If False it checks if the atlas is already at the latest version
         and doesn't update if that's the case.
     """
 
-    atlas = BrainGlobeAtlas(atlas_name=atlas_name)
+    atlas = BrainGlobeAtlas(atlas_name=atlas_name, check_latest=False)
 
     # Check if we need to update
     if not force:
-        if atlas.check_latest_version():
+        if atlas.check_latest_version(print_warning=False):
             rprint(
                 f"[b][magenta2]brainglobe_atlasapi: {atlas.atlas_name} "
                 "is already updated "
                 f"(version: {_version_str_from_tuple(atlas.local_version)})"
                 "[/b]"
             )
             return
```

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/utils.py` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi/utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/PKG-INFO` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-atlasapi
-Version: 2.0.5
+Version: 2.0.6
 Summary: A lightweight python module to interact with and generate atlases for systems neuroscience.
 Author-email: "Luigi Petrucco, Federico Claudi, Adam Tyson" <code@adamltyson.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, BrainGlobe
         All rights reserved.
```

### Comparing `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/SOURCES.txt` & `brainglobe_atlasapi-2.0.6/brainglobe_atlasapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.5/pyproject.toml` & `brainglobe_atlasapi-2.0.6/pyproject.toml`

 * *Files identical despite different names*

