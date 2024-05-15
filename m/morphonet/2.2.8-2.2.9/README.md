# Comparing `tmp/morphonet-2.2.8.tar.gz` & `tmp/morphonet-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphonet-2.2.8.tar", last modified: Wed Feb 21 19:58:47 2024, max compression
+gzip compressed data, was "morphonet-2.2.9.tar", last modified: Thu Feb 22 16:20:20 2024, max compression
```

## Comparing `morphonet-2.2.8.tar` & `morphonet-2.2.9.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.334237 morphonet-2.2.8/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    21782 2023-02-23 16:33:02.000000 morphonet-2.2.8/LICENSE
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       82 2023-07-17 12:17:44.000000 morphonet-2.2.8/MANIFEST.in
--rw-r--r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2506 2024-02-21 19:58:47.334237 morphonet-2.2.8/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1781 2023-02-23 16:53:03.000000 morphonet-2.2.8/README.md
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.062221 morphonet-2.2.8/morphonet/
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.070221 morphonet-2.2.8/morphonet/ImageHandling/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3860 2023-04-17 06:32:31.000000 morphonet-2.2.8/morphonet/ImageHandling/IO.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       72 2023-02-23 16:33:15.000000 morphonet-2.2.8/morphonet/ImageHandling/__init__.py
--rwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)     8046 2023-02-23 16:33:15.000000 morphonet-2.2.8/morphonet/ImageHandling/inrimage.py
--rwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)     7863 2023-04-17 06:32:31.000000 morphonet-2.2.8/morphonet/ImageHandling/metaimage.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7023 2023-02-23 16:33:15.000000 morphonet-2.2.8/morphonet/ImageHandling/spatial_image.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      339 2023-07-07 14:31:32.000000 morphonet-2.2.8/morphonet/__init__.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     9014 2023-02-23 16:33:15.000000 morphonet-2.2.8/morphonet/lineage_communication.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    70317 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/net.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.090222 morphonet-2.2.8/morphonet/plot/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      334 2023-07-07 14:31:32.000000 morphonet-2.2.8/morphonet/plot/Annotation.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    68081 2024-02-21 18:41:11.000000 morphonet-2.2.8/morphonet/plot/Dataset.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1745 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plot/Object.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    12251 2024-02-08 14:58:25.000000 morphonet-2.2.8/morphonet/plot/Property.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2247 2024-02-21 16:07:51.000000 morphonet-2.2.8/morphonet/plot/ScikitProperty.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     9895 2024-02-13 15:05:38.000000 morphonet-2.2.8/morphonet/plot/Server.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      215 2023-07-07 14:31:32.000000 morphonet-2.2.8/morphonet/plot/__init__.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    43516 2024-02-20 12:20:52.000000 morphonet-2.2.8/morphonet/plot/plot.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.094223 morphonet-2.2.8/morphonet/plugins/
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.106223 morphonet-2.2.8/morphonet/plugins/CreateSeeds/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4658 2024-02-20 15:39:28.000000 morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedax.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5005 2024-02-08 14:58:25.000000 morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedero.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5086 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedin.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7290 2024-02-21 17:58:52.000000 morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedio.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4465 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedis.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      346 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/CreateSeeds/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.118224 morphonet-2.2.8/morphonet/plugins/CreateSegmentation/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5166 2024-02-21 15:46:59.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentation/Binarize.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     9262 2024-02-20 12:58:11.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentation/CellPoseTrain.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10366 2024-02-20 09:00:04.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentation/Cellpose.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5905 2024-02-15 07:20:49.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentation/Mars.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5215 2024-02-20 09:00:04.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentation/Stardist.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      377 2024-02-21 15:01:20.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentation/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.126225 morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7245 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/Wata.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     8365 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/Wati.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6926 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/Watio.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5867 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/Wato.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      265 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.138225 morphonet-2.2.8/morphonet/plugins/EditObjects/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6378 2024-02-20 15:46:33.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/CopyPaste.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5618 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deform.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.154226 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1894 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/DeformationAPI.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2066 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/DeformationImage.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2742 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/GridVolume.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5687 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/GridVolumeFromDeformation.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    13580 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/MVC.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4258 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/Mesh.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1043 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/MeshVolume.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4025 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/TetrahedralVolume.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      406 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/Volume.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/__init__.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10665 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/utils.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    18172 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/utils_threads.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3002 2024-02-19 13:10:39.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Delete.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7118 2024-02-21 16:07:51.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Deli.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4267 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Disco.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4412 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Fuse.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5521 2024-02-20 09:00:04.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Gaumi.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3504 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/Splax.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      564 2024-02-13 14:42:15.000000 morphonet-2.2.8/morphonet/plugins/EditObjects/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.158227 morphonet-2.2.8/morphonet/plugins/EditTemporalLinks/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2779 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditTemporalLinks/Addlink.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2049 2024-02-21 11:48:51.000000 morphonet-2.2.8/morphonet/plugins/EditTemporalLinks/Delink.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6821 2024-02-20 15:10:43.000000 morphonet-2.2.8/morphonet/plugins/EditTemporalLinks/Tracko.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      226 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/EditTemporalLinks/__init__.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10595 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/MorphoPlugin.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.158227 morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     9235 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/Propa.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4727 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/Propi.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3629 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/Propro.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      219 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/__init__.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10763 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/seed_propagation_lib.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      591 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/__init__.py
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5835 2024-02-20 15:39:28.000000 morphonet-2.2.8/morphonet/plugins/functions.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.214230 morphonet-2.2.8/morphonet/plugins/icons/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4130 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Addlink.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6954 2024-02-21 17:31:30.000000 morphonet-2.2.8/morphonet/plugins/icons/Binarize.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7527 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Cellpose.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    15946 2024-02-20 12:58:11.000000 morphonet-2.2.8/morphonet/plugins/icons/CellposeTrain.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5451 2024-02-20 12:58:11.000000 morphonet-2.2.8/morphonet/plugins/icons/CopyPaste.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3297 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Deform.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     8947 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Delete.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3855 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Deli.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3136 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Delink.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     8549 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Disco.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5653 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Fuse.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5714 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Gaumi.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10275 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Mars.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5804 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Propa.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5389 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Propi.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3626 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Propo.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4589 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Seedax.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5399 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Seedero.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4420 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Seedin.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4403 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Seedio.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5414 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Seedis.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3980 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Splax.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    17430 2023-07-07 14:31:32.000000 morphonet-2.2.8/morphonet/plugins/icons/Stardist.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6524 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Tracko.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3801 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Wata.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5818 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Wati.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5416 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Watio.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4845 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/icons/Wato.png
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.330237 morphonet-2.2.8/morphonet/plugins/images/
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    66749 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Addlink.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   242508 2024-02-21 17:31:30.000000 morphonet-2.2.8/morphonet/plugins/images/Binarize.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)  1852735 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Cellpose.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   303861 2024-02-20 12:58:11.000000 morphonet-2.2.8/morphonet/plugins/images/CellposeTrain.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   261847 2024-02-20 12:58:11.000000 morphonet-2.2.8/morphonet/plugins/images/CopyPaste.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    80577 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Deform.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   150506 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Delete.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    66595 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Deli.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    67539 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Delink.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    90594 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Disco.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    69172 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Fuse.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   113434 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Gaumi.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   405313 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Mars.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   125806 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Propa.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   135844 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Propi.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   112099 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Propo.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   110379 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Seedax.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    87395 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Seedero.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   135212 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Seedin.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   157913 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Seedio.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   209697 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Seedis.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    98054 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Splax.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)  1332373 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Stardist.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   106626 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Tracko.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   187644 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Wata.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   367017 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Wati.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   116209 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Watio.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    81578 2024-02-08 14:46:20.000000 morphonet-2.2.8/morphonet/plugins/images/Wato.png
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    75422 2024-02-21 18:41:11.000000 morphonet-2.2.8/morphonet/tools.py
-drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-21 19:58:47.330237 morphonet-2.2.8/morphonet.egg-info/
--rw-r--r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2506 2024-02-21 19:58:47.000000 morphonet-2.2.8/morphonet.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5076 2024-02-21 19:58:47.000000 morphonet-2.2.8/morphonet.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)        1 2024-02-21 19:58:47.000000 morphonet-2.2.8/morphonet.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       58 2024-02-21 19:58:47.000000 morphonet-2.2.8/morphonet.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       10 2024-02-21 19:58:47.000000 morphonet-2.2.8/morphonet.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       38 2024-02-21 19:58:47.334237 morphonet-2.2.8/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1071 2024-02-21 19:58:42.000000 morphonet-2.2.8/setup.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.390064 morphonet-2.2.9/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    21782 2023-02-23 16:33:02.000000 morphonet-2.2.9/LICENSE
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       82 2023-07-17 12:17:44.000000 morphonet-2.2.9/MANIFEST.in
+-rw-r--r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2506 2024-02-22 16:20:20.390064 morphonet-2.2.9/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1781 2023-02-23 16:53:03.000000 morphonet-2.2.9/README.md
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.062045 morphonet-2.2.9/morphonet/
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.062045 morphonet-2.2.9/morphonet/ImageHandling/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3860 2023-04-17 06:32:31.000000 morphonet-2.2.9/morphonet/ImageHandling/IO.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       72 2023-02-23 16:33:15.000000 morphonet-2.2.9/morphonet/ImageHandling/__init__.py
+-rwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)     8046 2023-02-23 16:33:15.000000 morphonet-2.2.9/morphonet/ImageHandling/inrimage.py
+-rwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)     7863 2023-04-17 06:32:31.000000 morphonet-2.2.9/morphonet/ImageHandling/metaimage.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7023 2023-02-23 16:33:15.000000 morphonet-2.2.9/morphonet/ImageHandling/spatial_image.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      339 2023-07-07 14:31:32.000000 morphonet-2.2.9/morphonet/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     9014 2023-02-23 16:33:15.000000 morphonet-2.2.9/morphonet/lineage_communication.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    70317 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/net.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.070046 morphonet-2.2.9/morphonet/plot/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      334 2023-07-07 14:31:32.000000 morphonet-2.2.9/morphonet/plot/Annotation.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    68688 2024-02-22 14:52:06.000000 morphonet-2.2.9/morphonet/plot/Dataset.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1745 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plot/Object.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    12251 2024-02-08 14:58:25.000000 morphonet-2.2.9/morphonet/plot/Property.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2247 2024-02-21 16:07:51.000000 morphonet-2.2.9/morphonet/plot/ScikitProperty.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     9895 2024-02-13 15:05:38.000000 morphonet-2.2.9/morphonet/plot/Server.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      215 2023-07-07 14:31:32.000000 morphonet-2.2.9/morphonet/plot/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    43798 2024-02-22 08:56:37.000000 morphonet-2.2.9/morphonet/plot/plot.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.074046 morphonet-2.2.9/morphonet/plugins/
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.090047 morphonet-2.2.9/morphonet/plugins/CreateSeeds/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4658 2024-02-20 15:39:28.000000 morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedax.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5005 2024-02-08 14:58:25.000000 morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedero.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5086 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedin.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7290 2024-02-21 17:58:52.000000 morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedio.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4465 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedis.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      346 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/CreateSeeds/__init__.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.130049 morphonet-2.2.9/morphonet/plugins/CreateSegmentation/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5166 2024-02-21 15:46:59.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentation/Binarize.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     9262 2024-02-20 12:58:11.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentation/CellPoseTrain.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10366 2024-02-20 09:00:04.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentation/Cellpose.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5905 2024-02-15 07:20:49.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentation/Mars.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5215 2024-02-20 09:00:04.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentation/Stardist.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      377 2024-02-21 15:01:20.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentation/__init__.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.138049 morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7245 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/Wata.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     8365 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/Wati.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6926 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/Watio.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5867 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/Wato.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      265 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/__init__.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.142049 morphonet-2.2.9/morphonet/plugins/EditObjects/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6378 2024-02-20 15:46:33.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/CopyPaste.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5661 2024-02-22 08:56:37.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deform.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.146050 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1894 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/DeformationAPI.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2066 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/DeformationImage.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2742 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/GridVolume.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5687 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/GridVolumeFromDeformation.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    13580 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/MVC.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4258 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/Mesh.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1043 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/MeshVolume.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4025 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/TetrahedralVolume.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      406 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/Volume.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10665 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/utils.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    18172 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/utils_threads.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3002 2024-02-19 13:10:39.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Delete.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7118 2024-02-21 16:07:51.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Deli.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4242 2024-02-22 14:52:06.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Disco.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4412 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Fuse.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5521 2024-02-20 09:00:04.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Gaumi.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3504 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/Splax.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      564 2024-02-13 14:42:15.000000 morphonet-2.2.9/morphonet/plugins/EditObjects/__init__.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.146050 morphonet-2.2.9/morphonet/plugins/EditTemporalLinks/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2779 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditTemporalLinks/Addlink.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2049 2024-02-21 11:48:51.000000 morphonet-2.2.9/morphonet/plugins/EditTemporalLinks/Delink.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6821 2024-02-20 15:10:43.000000 morphonet-2.2.9/morphonet/plugins/EditTemporalLinks/Tracko.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      226 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/EditTemporalLinks/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10595 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/MorphoPlugin.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.146050 morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     9235 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/Propa.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4727 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/Propi.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3629 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/Propro.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      219 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10763 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/seed_propagation_lib.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)      591 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5835 2024-02-20 15:39:28.000000 morphonet-2.2.9/morphonet/plugins/functions.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.194053 morphonet-2.2.9/morphonet/plugins/icons/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4130 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Addlink.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6954 2024-02-21 17:31:30.000000 morphonet-2.2.9/morphonet/plugins/icons/Binarize.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     7527 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Cellpose.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    15946 2024-02-20 12:58:11.000000 morphonet-2.2.9/morphonet/plugins/icons/CellposeTrain.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5451 2024-02-20 12:58:11.000000 morphonet-2.2.9/morphonet/plugins/icons/CopyPaste.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    69112 2024-02-22 08:56:37.000000 morphonet-2.2.9/morphonet/plugins/icons/Deform.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     8947 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Delete.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3855 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Deli.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3136 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Delink.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     8549 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Disco.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5653 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Fuse.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5714 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Gaumi.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    10275 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Mars.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5804 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Propa.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5389 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Propi.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3626 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Propo.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4589 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Seedax.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5399 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Seedero.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4420 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Seedin.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4403 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Seedio.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5414 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Seedis.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3980 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Splax.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    17430 2023-07-07 14:31:32.000000 morphonet-2.2.9/morphonet/plugins/icons/Stardist.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     6524 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Tracko.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     3801 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Wata.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5818 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Wati.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5416 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Watio.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     4845 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/icons/Wato.png
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.378063 morphonet-2.2.9/morphonet/plugins/images/
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    66749 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Addlink.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   242508 2024-02-21 17:31:30.000000 morphonet-2.2.9/morphonet/plugins/images/Binarize.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)  1852735 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Cellpose.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   303861 2024-02-20 12:58:11.000000 morphonet-2.2.9/morphonet/plugins/images/CellposeTrain.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   261847 2024-02-20 12:58:11.000000 morphonet-2.2.9/morphonet/plugins/images/CopyPaste.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    80577 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Deform.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   150506 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Delete.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    66595 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Deli.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    67539 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Delink.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    90594 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Disco.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    69172 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Fuse.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   113434 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Gaumi.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   405313 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Mars.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   125806 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Propa.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   135844 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Propi.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   112099 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Propo.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   110379 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Seedax.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    87395 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Seedero.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   135212 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Seedin.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   157913 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Seedio.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   209697 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Seedis.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    98054 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Splax.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)  1332373 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Stardist.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   106626 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Tracko.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   187644 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Wata.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   367017 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Wati.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)   116209 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Watio.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    81578 2024-02-08 14:46:20.000000 morphonet-2.2.9/morphonet/plugins/images/Wato.png
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)    75422 2024-02-21 18:41:11.000000 morphonet-2.2.9/morphonet/tools.py
+drwxrwxr-x   0 gitlab-runner  (1002) gitlab-runner  (1003)        0 2024-02-22 16:20:20.386063 morphonet-2.2.9/morphonet.egg-info/
+-rw-r--r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     2506 2024-02-22 16:20:20.000000 morphonet-2.2.9/morphonet.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     5076 2024-02-22 16:20:20.000000 morphonet-2.2.9/morphonet.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)        1 2024-02-22 16:20:20.000000 morphonet-2.2.9/morphonet.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       58 2024-02-22 16:20:20.000000 morphonet-2.2.9/morphonet.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       10 2024-02-22 16:20:20.000000 morphonet-2.2.9/morphonet.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)       38 2024-02-22 16:20:20.390064 morphonet-2.2.9/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1002) gitlab-runner  (1003)     1071 2024-02-22 16:20:13.000000 morphonet-2.2.9/setup.py
```

### Comparing `morphonet-2.2.8/LICENSE` & `morphonet-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/PKG-INFO` & `morphonet-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphonet
-Version: 2.2.8
+Version: 2.2.9
 Summary: Python API to interact with MorphoNet
 Home-page: https://gitlab.inria.fr/efaure/MorphoNet
 Author: Emmanuel Faure
 Author-email: api@morphonet.org
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
```

### Comparing `morphonet-2.2.8/README.md` & `morphonet-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/ImageHandling/IO.py` & `morphonet-2.2.9/morphonet/ImageHandling/IO.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/ImageHandling/inrimage.py` & `morphonet-2.2.9/morphonet/ImageHandling/inrimage.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/ImageHandling/metaimage.py` & `morphonet-2.2.9/morphonet/ImageHandling/metaimage.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/ImageHandling/spatial_image.py` & `morphonet-2.2.9/morphonet/ImageHandling/spatial_image.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/lineage_communication.py` & `morphonet-2.2.9/morphonet/lineage_communication.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/net.py` & `morphonet-2.2.9/morphonet/net.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plot/Dataset.py` & `morphonet-2.2.9/morphonet/plot/Dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,23 @@
         bc = 0
         while isdir(join(self.temp_path, str(bc))):
             bc += 1
         if bc == 0:
             return 0
         return bc - 1
 
+    def get_first_step_with_seg(self,time):
+        for index_step in range(0,self.step+1): #for all existing step
+            image_path = join(self.temp_path, str(index_step), self.temp_segname.format(int(time), int(
+                self.segmented_channels[0])))
+            if isfile(image_path):
+                return index_step
+        return -1
+
+
     def start_step(self, command, exec_time):
         '''
         Prepare the step folder and save the command to the log file system
         '''
         printv("Increase Step at " + str(self.step + 1), 1)
         self.step += 1  # Increase Step
         self.step_folder = join(self.temp_path, str(self.step))
@@ -384,31 +393,35 @@
         import shutil
         last_step = self.get_last_step()
 
         # EXPORT IMAGES
 
         for t in range(self.begin, self.end + 1):  # List images to restore HERE EXPORT AS ONE IMAGE IF MULTI CHANNEL
             printv("Exporting time point " + str(t), 1)
-            dataTemplate, vsize = _load_seg(join(self.temp_path, str(0), self.temp_segname.format(int(t), int(
+            seg_step = self.get_first_step_with_seg(t)
+            dataTemplate, vsize = _load_seg(join(self.temp_path, str(seg_step), self.temp_segname.format(int(t), int(
                 self.segmented_channels[0]))))
-            data = np.zeros(dataTemplate.shape+(len(self.segmented_channels),),dtype=dataTemplate.dtype) #add channel dims
-            for channel in self.segmented_channels:
-                printv("  adding channel : "+str(channel), 1)
-                s=last_step
-                while s>0 and not isfile(join(self.temp_path, str(s), self.temp_segname.format(int(t),int(channel)))):
-                    s-=1
-                if not isfile(join(self.temp_path, str(s), self.temp_segname.format(int(t),int(channel)))):
-                    printv("ERROR did not find any backup for "+self.temp_segname.format(int(t),int(channel)),1)
-                else:
-                    datachannel, vsize =_load_seg(join(self.temp_path, str(s), self.temp_segname.format(int(t),int(channel))))
-                    data[:,:,:,int(channel)] = datachannel # aggregates channels into image output
-                    self.set_voxel_size(t, vsize)
-            filename=join(export_path,self.temp_segname.replace("_ch{:01d}","").format(int(t)).replace("npz",image_file_type))
-            printv("writing segmented image to "+filename,1)
-            imsave(filename,data,voxel_size=(vsize[0],vsize[1],vsize[2],1.0))
+            if seg_step > -1:
+                data = np.zeros(dataTemplate.shape+(len(self.segmented_channels),),dtype=dataTemplate.dtype) #add channel dims
+                for channel in self.segmented_channels:
+                    printv("  adding channel : "+str(channel), 1)
+                    s=last_step
+                    while s>0 and not isfile(join(self.temp_path, str(s), self.temp_segname.format(int(t),int(channel)))):
+                        s-=1
+                    if not isfile(join(self.temp_path, str(s), self.temp_segname.format(int(t),int(channel)))):
+                        printv("ERROR did not find any backup for "+self.temp_segname.format(int(t),int(channel)),1)
+                    else:
+                        datachannel, vsize =_load_seg(join(self.temp_path, str(s), self.temp_segname.format(int(t),int(channel))))
+                        data[:,:,:,int(channel)] = datachannel # aggregates channels into image output
+                        self.set_voxel_size(t, vsize)
+                filename=join(export_path,self.temp_segname.replace("_ch{:01d}","").format(int(t)).replace("npz",image_file_type))
+                printv("writing segmented image to "+filename,1)
+                imsave(filename,data,voxel_size=(vsize[0],vsize[1],vsize[2],1.0))
+            else :
+                printv("Unable to find a segmentation image at time : "+str(t),1)
         """
         for t in range(self.begin, self.end + 1):  # List images to restore HERE EXPORT AS ONE IMAGE IF MULTI CHANNEL
             for channel in self.segmented_channels:
                 s=last_step
                 while s>0 and not isfile(join(self.temp_path, str(s), self.temp_segname.format(int(t),int(channel)))):
                     s-=1
                 if not isfile(join(self.temp_path, str(s), self.temp_segname.format(int(t),int(channel)))):
```

### Comparing `morphonet-2.2.8/morphonet/plot/Object.py` & `morphonet-2.2.9/morphonet/plot/Object.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plot/Property.py` & `morphonet-2.2.9/morphonet/plot/Property.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plot/ScikitProperty.py` & `morphonet-2.2.9/morphonet/plot/ScikitProperty.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plot/Server.py` & `morphonet-2.2.9/morphonet/plot/Server.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plot/plot.py` & `morphonet-2.2.9/morphonet/plot/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -931,17 +931,21 @@
     def plot_regionprop(self, name):  # PLOT Scikiimage property
         """ Send the specified property with the specified name to browser
 
         Parameters
         ----------
         name : property name
         """
+        printv("Plot scikit property 1 " + name, 2)
         if self.dataset.regionprops is not None:
+            printv("Plot scikit property 2 " + name, 2)
             if name in self.dataset.regionprops:
+                printv("Plot scikit property 3 " + name, 2)
                 if not  self.dataset.regionprops[name].sent:
+                    printv("Plot scikit property 4 " + name, 2)
                     if self.is_all_computed_regionprop(name):
                         self.dataset.wait_regionprops()
                         printv("Plot scikit property " + name, 2)
                         prop_text = self.dataset.regionprops[name].get_txt()
                         self.send("INFO_"+name.replace("_","-"), prop_text)
                         self.dataset.regionprops[name].sent=True
 
@@ -1031,27 +1035,27 @@
         return obj
 
     def get_mesh_object(self,mo):
         """
         Return the mesh (in obj) for a given cell
         (Read the vtk temporart file and convert it to obj)
         """
-        obj_step = self.dataset.get_last_version(str(mo.t) + ".obj", step_only=True) #Look for the location of th last time point
-        obj_mesh_path = join(self.temp_path, str(obj_step),str(mo.t))
+        obj_step = self.dataset.get_last_version(str(mo.t) +"_ch"+str(mo.channel)+".obj", step_only=True) #Look for the location of th last time point
+        obj_mesh_path = join(self.temp_path, str(obj_step),str(mo.t)+","+str(mo.channel))
         if not isdir(obj_mesh_path):
             printv("error did not find the temporary mesh path "+obj_mesh_path, 1)
             return None
         cell_mesh_filename=join(obj_mesh_path,str(mo.t)+'-'+str(mo.id)+'.vtk')
 
         if not isfile(cell_mesh_filename):
             printv("error did not find the temporary cell mesh file " + cell_mesh_filename, 1)
             return None
 
         #Convert VTK in OBJ
-        obj=convert_vtk_file_in_obj(cell_mesh_filename, mo, ch=0, factor=self.factor, center=self.dataset.get_center(), VoxelSize=self.dataset.get_voxel_size(mo.t))
+        obj=convert_vtk_file_in_obj(cell_mesh_filename, mo, ch=mo.channel, factor=self.factor, center=self.dataset.get_center(), VoxelSize=self.dataset.get_voxel_size(mo.t))
         return obj
 
     def recompute_mesh_at_t(self,t,channel):
         data = self.dataset.get_seg(t,channel)
         if data is not None:
             if t not in self.dataset.cells_updated: self.dataset.cells_updated[t]={}
             self.dataset.cells_updated[t][channel] = None
```

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedax.py` & `morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedax.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedero.py` & `morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedero.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedin.py` & `morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedin.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedio.py` & `morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedio.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSeeds/Seedis.py` & `morphonet-2.2.9/morphonet/plugins/CreateSeeds/Seedis.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSegmentation/Binarize.py` & `morphonet-2.2.9/morphonet/plugins/CreateSegmentation/Binarize.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSegmentation/CellPoseTrain.py` & `morphonet-2.2.9/morphonet/plugins/CreateSegmentation/CellPoseTrain.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSegmentation/Cellpose.py` & `morphonet-2.2.9/morphonet/plugins/CreateSegmentation/Cellpose.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSegmentation/Mars.py` & `morphonet-2.2.9/morphonet/plugins/CreateSegmentation/Mars.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSegmentation/Stardist.py` & `morphonet-2.2.9/morphonet/plugins/CreateSegmentation/Stardist.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/Wata.py` & `morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/Wata.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/Wati.py` & `morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/Wati.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/Watio.py` & `morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/Watio.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/CreateSegmentationFromSeeds/Wato.py` & `morphonet-2.2.9/morphonet/plugins/CreateSegmentationFromSeeds/Wato.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/CopyPaste.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/CopyPaste.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deform.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deform.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         if not self.start(t,dataset,objects):
             return None
 
         if len(objects)!=1:
             printv("error : please select only one cell", 0)
         else:
             cells_updated=[]
+            data=None
             for cid in objects:
                 o=dataset.get_object(cid)
                 if o is not None:
                     data = dataset.get_seg(o.t)
                     
                     mesh = dataset.get_mesh_object(o)
 
@@ -97,15 +98,15 @@
                         printv(f"Mesh error : {ex}", 0)
                     except Exception as ex:
                         printv(f"Generic error in deformation : {ex}", 2)
                     else:
                         cells_updated.append(o.id)
                         printv(f"Deformation successful on cell {o.t} {o.id}, processing results...", 0)
 
-            if len(cells_updated) > 0:
+            if len(cells_updated) > 0 and data is not None:
                 dataset.set_seg(o.t, data, cells_updated=cells_updated)
                 printv(f"Computing new mesh{'es' if len(cells_updated) > 1 else ''} ...", 0)
             self.restart()
 
     def computeDeformation(self, data : np.array, mesh : str, mesh_deform : str, mesh_translation, mesh_scaling, background, cell=None, time=None, ):
         printv("Initializing deformation", 0)
         originalData, originalMesh, deformedData, deformedMesh, volume = initializeData(data, mesh, mesh_deform, mesh_translation, mesh_scaling, background, cell, time)
```

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/DeformationAPI.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/DeformationAPI.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/DeformationImage.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/DeformationImage.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/GridVolume.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/GridVolume.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/GridVolumeFromDeformation.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/GridVolumeFromDeformation.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/MVC.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/MVC.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/Mesh.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/Mesh.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/MeshVolume.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/MeshVolume.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/TetrahedralVolume.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/TetrahedralVolume.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/utils.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/utils.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deformation/utils_threads.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deformation/utils_threads.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Delete.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Delete.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Deli.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Deli.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Disco.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Disco.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                              "    Current : Current time point in MorphoNet \n"
                              "    All : will delete all objects at all time points \n ")
 
     def split_unconnected_at(self, t, channel, dataset):
         import numpy as np
         from skimage.measure import label
         data = dataset.get_seg(t)  #Get segmentations at the time
-        lastID = np.max(data) + 1  # new id = max of segmentation +1
+        lastID = dataset.get_last_id(t) + 1
         cells_updated = []
         for o in dataset.get_all_objects_at(t,channel):  # For all objects in segmentation from morphonet
             bb = dataset.get_regionprop("bbox", o)
             data_cell = data[bb[0]:bb[3], bb[1]:bb[4], bb[2]:bb[5]]
             labels = label(data_cell==o.id, background=dataset.background)
             ids, counts = np.unique(labels, return_counts=True)  # Get the differents  connected components
             w=ids!=0 #Remove background (ATTENTION it's not dataset.background !)
```

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Fuse.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Fuse.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Gaumi.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Gaumi.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/Splax.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/Splax.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditObjects/__init__.py` & `morphonet-2.2.9/morphonet/plugins/EditObjects/__init__.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditTemporalLinks/Addlink.py` & `morphonet-2.2.9/morphonet/plugins/EditTemporalLinks/Addlink.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditTemporalLinks/Delink.py` & `morphonet-2.2.9/morphonet/plugins/EditTemporalLinks/Delink.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/EditTemporalLinks/Tracko.py` & `morphonet-2.2.9/morphonet/plugins/EditTemporalLinks/Tracko.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/MorphoPlugin.py` & `morphonet-2.2.9/morphonet/plugins/MorphoPlugin.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/Propa.py` & `morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/Propa.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/Propi.py` & `morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/Propi.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/Propro.py` & `morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/Propro.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/PropagateSegmentation/seed_propagation_lib.py` & `morphonet-2.2.9/morphonet/plugins/PropagateSegmentation/seed_propagation_lib.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/__init__.py` & `morphonet-2.2.9/morphonet/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/functions.py` & `morphonet-2.2.9/morphonet/plugins/functions.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Addlink.png` & `morphonet-2.2.9/morphonet/plugins/icons/Addlink.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Binarize.png` & `morphonet-2.2.9/morphonet/plugins/icons/Binarize.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Cellpose.png` & `morphonet-2.2.9/morphonet/plugins/icons/Cellpose.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/CellposeTrain.png` & `morphonet-2.2.9/morphonet/plugins/icons/CellposeTrain.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/CopyPaste.png` & `morphonet-2.2.9/morphonet/plugins/icons/CopyPaste.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Delete.png` & `morphonet-2.2.9/morphonet/plugins/icons/Delete.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Deli.png` & `morphonet-2.2.9/morphonet/plugins/icons/Deli.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Delink.png` & `morphonet-2.2.9/morphonet/plugins/icons/Delink.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Disco.png` & `morphonet-2.2.9/morphonet/plugins/icons/Disco.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Fuse.png` & `morphonet-2.2.9/morphonet/plugins/icons/Fuse.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Gaumi.png` & `morphonet-2.2.9/morphonet/plugins/icons/Gaumi.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Mars.png` & `morphonet-2.2.9/morphonet/plugins/icons/Mars.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Propa.png` & `morphonet-2.2.9/morphonet/plugins/icons/Propa.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Propi.png` & `morphonet-2.2.9/morphonet/plugins/icons/Propi.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Propo.png` & `morphonet-2.2.9/morphonet/plugins/icons/Propo.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Seedax.png` & `morphonet-2.2.9/morphonet/plugins/icons/Seedax.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Seedero.png` & `morphonet-2.2.9/morphonet/plugins/icons/Seedero.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Seedin.png` & `morphonet-2.2.9/morphonet/plugins/icons/Seedin.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Seedio.png` & `morphonet-2.2.9/morphonet/plugins/icons/Seedio.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Seedis.png` & `morphonet-2.2.9/morphonet/plugins/icons/Seedis.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Splax.png` & `morphonet-2.2.9/morphonet/plugins/icons/Splax.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Stardist.png` & `morphonet-2.2.9/morphonet/plugins/icons/Stardist.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Tracko.png` & `morphonet-2.2.9/morphonet/plugins/icons/Tracko.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Wata.png` & `morphonet-2.2.9/morphonet/plugins/icons/Wata.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Wati.png` & `morphonet-2.2.9/morphonet/plugins/icons/Wati.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Watio.png` & `morphonet-2.2.9/morphonet/plugins/icons/Watio.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/icons/Wato.png` & `morphonet-2.2.9/morphonet/plugins/icons/Wato.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Addlink.png` & `morphonet-2.2.9/morphonet/plugins/images/Addlink.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Binarize.png` & `morphonet-2.2.9/morphonet/plugins/images/Binarize.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Cellpose.png` & `morphonet-2.2.9/morphonet/plugins/images/Cellpose.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/CellposeTrain.png` & `morphonet-2.2.9/morphonet/plugins/images/CellposeTrain.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/CopyPaste.png` & `morphonet-2.2.9/morphonet/plugins/images/CopyPaste.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Deform.png` & `morphonet-2.2.9/morphonet/plugins/images/Deform.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Delete.png` & `morphonet-2.2.9/morphonet/plugins/images/Delete.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Deli.png` & `morphonet-2.2.9/morphonet/plugins/images/Deli.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Delink.png` & `morphonet-2.2.9/morphonet/plugins/images/Delink.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Disco.png` & `morphonet-2.2.9/morphonet/plugins/images/Disco.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Fuse.png` & `morphonet-2.2.9/morphonet/plugins/images/Fuse.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Gaumi.png` & `morphonet-2.2.9/morphonet/plugins/images/Gaumi.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Mars.png` & `morphonet-2.2.9/morphonet/plugins/images/Mars.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Propa.png` & `morphonet-2.2.9/morphonet/plugins/images/Propa.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Propi.png` & `morphonet-2.2.9/morphonet/plugins/images/Propi.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Propo.png` & `morphonet-2.2.9/morphonet/plugins/images/Propo.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Seedax.png` & `morphonet-2.2.9/morphonet/plugins/images/Seedax.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Seedero.png` & `morphonet-2.2.9/morphonet/plugins/images/Seedero.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Seedin.png` & `morphonet-2.2.9/morphonet/plugins/images/Seedin.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Seedio.png` & `morphonet-2.2.9/morphonet/plugins/images/Seedio.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Seedis.png` & `morphonet-2.2.9/morphonet/plugins/images/Seedis.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Splax.png` & `morphonet-2.2.9/morphonet/plugins/images/Splax.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Stardist.png` & `morphonet-2.2.9/morphonet/plugins/images/Stardist.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Tracko.png` & `morphonet-2.2.9/morphonet/plugins/images/Tracko.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Wata.png` & `morphonet-2.2.9/morphonet/plugins/images/Wata.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Wati.png` & `morphonet-2.2.9/morphonet/plugins/images/Wati.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Watio.png` & `morphonet-2.2.9/morphonet/plugins/images/Watio.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/plugins/images/Wato.png` & `morphonet-2.2.9/morphonet/plugins/images/Wato.png`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet/tools.py` & `morphonet-2.2.9/morphonet/tools.py`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/morphonet.egg-info/PKG-INFO` & `morphonet-2.2.9/morphonet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphonet
-Version: 2.2.8
+Version: 2.2.9
 Summary: Python API to interact with MorphoNet
 Home-page: https://gitlab.inria.fr/efaure/MorphoNet
 Author: Emmanuel Faure
 Author-email: api@morphonet.org
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
```

### Comparing `morphonet-2.2.8/morphonet.egg-info/SOURCES.txt` & `morphonet-2.2.9/morphonet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphonet-2.2.8/setup.py` & `morphonet-2.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import morphonet
 
 setup(
 
     name='morphonet',
 
-    version="2.2.8",
+    version="2.2.9",
 
     packages=find_packages(),
 
     author="Emmanuel Faure",
 
     author_email="api@morphonet.org",
```

