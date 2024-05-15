# Comparing `tmp/brie-2.2.2.tar.gz` & `tmp/brie-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brie-2.2.2.tar", last modified: Fri Nov  4 06:07:08 2022, max compression
+gzip compressed data, was "brie-2.2.3.tar", last modified: Wed May 15 04:29:50 2024, max compression
```

## Comparing `brie-2.2.2.tar` & `brie-2.2.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1184 2022-03-22 05:13:16.000000 brie-2.2.2/.gitignore
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      316 2022-03-22 05:13:16.000000 brie-2.2.2/.readthedocs.yml
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      122 2022-03-22 05:13:16.000000 brie-2.2.2/.travis.yml
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    11393 2022-03-22 05:13:16.000000 brie-2.2.2/LICENSE
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     4869 2022-11-04 06:07:08.000000 brie-2.2.2/PKG-INFO
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     4482 2022-05-29 14:29:34.000000 brie-2.2.2/README.rst
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/brie/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      708 2022-05-29 14:29:34.000000 brie-2.2.2/brie/__init__.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/brie/_cli/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)       40 2022-03-22 05:13:16.000000 brie-2.2.2/brie/_cli/__init__.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      989 2022-03-22 05:13:16.000000 brie-2.2.2/brie/_cli/_cli.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1363 2022-03-22 05:13:16.000000 brie-2.2.2/brie/_cli/count.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      474 2022-03-22 05:13:16.000000 brie-2.2.2/brie/_cli/download.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      403 2022-03-22 05:13:16.000000 brie-2.2.2/brie/_cli/extract.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      497 2022-03-22 05:13:16.000000 brie-2.2.2/brie/_cli/quant.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/brie/bin/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      104 2022-05-29 14:29:34.000000 brie-2.2.2/brie/bin/__init__.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      375 2022-03-22 05:13:16.000000 brie-2.2.2/brie/bin/brie_main.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    11871 2022-07-14 08:24:05.000000 brie-2.2.2/brie/bin/count.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     9323 2022-11-04 03:33:16.000000 brie-2.2.2/brie/bin/quant.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/brie/models/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      142 2022-03-22 05:13:16.000000 brie-2.2.2/brie/models/__init__.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1512 2022-03-22 05:13:16.000000 brie-2.2.2/brie/models/base_model.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     3331 2022-03-22 05:13:16.000000 brie-2.2.2/brie/models/hypothesis_tests.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     8055 2022-03-22 05:13:16.000000 brie-2.2.2/brie/models/model_Beta.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    10251 2022-11-04 02:12:03.000000 brie-2.2.2/brie/models/model_TFProb.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     9656 2022-03-22 05:13:16.000000 brie-2.2.2/brie/models/model_TFProb_dev.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    11532 2022-11-04 02:06:03.000000 brie-2.2.2/brie/models/model_wrap.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     2783 2022-03-22 05:13:16.000000 brie-2.2.2/brie/models/simulator.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      112 2022-03-22 05:13:16.000000 brie-2.2.2/brie/models/tools.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/brie/plot/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     4224 2022-03-22 05:13:16.000000 brie-2.2.2/brie/plot/LRtest_plot.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)       52 2022-03-22 05:13:16.000000 brie-2.2.2/brie/plot/__init__.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     3895 2022-03-22 05:13:16.000000 brie-2.2.2/brie/plot/base_plot.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)       93 2022-03-22 05:13:16.000000 brie-2.2.2/brie/settings.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/brie/utils/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      221 2022-03-22 05:13:16.000000 brie-2.2.2/brie/utils/__init__.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1756 2022-03-22 05:13:16.000000 brie-2.2.2/brie/utils/base_utils.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    15312 2022-03-22 05:13:16.000000 brie-2.2.2/brie/utils/bias_utils.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     9870 2022-05-29 14:29:34.000000 brie-2.2.2/brie/utils/count.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     9325 2022-05-29 14:29:34.000000 brie-2.2.2/brie/utils/count_droplet.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     7957 2022-03-22 05:13:16.000000 brie-2.2.2/brie/utils/fasta_utils.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    11869 2022-03-22 05:13:16.000000 brie-2.2.2/brie/utils/gtf_utils.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     6251 2022-05-29 14:29:34.000000 brie-2.2.2/brie/utils/io_utils.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     3689 2022-03-22 05:13:16.000000 brie-2.2.2/brie/utils/preprocessing.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     7427 2022-03-22 05:13:16.000000 brie-2.2.2/brie/utils/run_utils.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     7928 2022-05-29 14:29:34.000000 brie-2.2.2/brie/utils/sam_utils.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    14267 2022-03-22 05:13:16.000000 brie-2.2.2/brie/utils/tran_utils.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)       23 2022-11-04 06:01:38.000000 brie-2.2.2/brie/version.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/brie/version1/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    10781 2022-03-22 05:13:16.000000 brie-2.2.2/brie/version1/brie.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     9419 2022-03-22 05:13:16.000000 brie-2.2.2/brie/version1/brie_diff.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    15651 2022-03-22 05:13:16.000000 brie-2.2.2/brie/version1/model_brie.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/brie.egg-info/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     4869 2022-11-04 06:07:07.000000 brie-2.2.2/brie.egg-info/PKG-INFO
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1841 2022-11-04 06:07:07.000000 brie-2.2.2/brie.egg-info/SOURCES.txt
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)        1 2022-11-04 06:07:07.000000 brie-2.2.2/brie.egg-info/dependency_links.txt
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      190 2022-11-04 06:07:07.000000 brie-2.2.2/brie.egg-info/entry_points.txt
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      256 2022-11-04 06:07:07.000000 brie-2.2.2/brie.egg-info/requires.txt
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)        5 2022-11-04 06:07:07.000000 brie-2.2.2/brie.egg-info/top_level.txt
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/doc/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     6762 2022-03-22 05:13:16.000000 brie-2.2.2/doc/Makefile
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     8664 2022-03-22 05:13:16.000000 brie-2.2.2/doc/brie1.rst
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     4719 2022-05-29 14:29:34.000000 brie-2.2.2/doc/brie_count.rst
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     8838 2022-05-29 14:29:34.000000 brie-2.2.2/doc/brie_quant.rst
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    12033 2022-05-29 14:29:34.000000 brie-2.2.2/doc/conf.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/doc/image/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)   271871 2022-05-29 14:29:34.000000 brie-2.2.2/doc/image/BRIE2_roadmap.png
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     4232 2022-05-29 14:29:34.000000 brie-2.2.2/doc/index.rst
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     3755 2022-03-22 05:13:16.000000 brie-2.2.2/doc/install.rst
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     6401 2022-05-29 14:29:34.000000 brie-2.2.2/doc/quick_start.rst
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     4811 2022-11-04 04:32:33.000000 brie-2.2.2/doc/release.rst
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      237 2022-03-22 05:13:16.000000 brie-2.2.2/doc/requirements.txt
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)       44 2022-03-22 05:13:16.000000 brie-2.2.2/doc/tutorial.rst
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/examples/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1139 2022-05-29 14:29:34.000000 brie-2.2.2/examples/brie2_demo.sh
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/examples/demo_v1/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     3413 2022-03-22 05:13:16.000000 brie-2.2.2/examples/demo_v1/anno_maker.sh
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1217 2022-03-22 05:13:16.000000 brie-2.2.2/examples/demo_v1/brie_demo.sh
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/examples/gastrulation/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)    11771 2022-03-22 05:13:16.000000 brie-2.2.2/examples/gastrulation/E-MTAB-4079.130cells.txt
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      718 2022-03-22 05:13:16.000000 brie-2.2.2/examples/gastrulation/brie_sashimi.sh
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1971 2022-03-22 05:13:16.000000 brie-2.2.2/examples/gastrulation/gastrulation_130cells.sh
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      724 2022-03-22 05:13:16.000000 brie-2.2.2/examples/gastrulation/prepare_anno.sh
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1775 2022-03-22 05:13:16.000000 brie-2.2.2/examples/gastrulation/sashimi_setting.txt
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      239 2022-03-22 05:13:16.000000 brie-2.2.2/examples/make_list.sh
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      323 2022-03-22 05:13:16.000000 brie-2.2.2/requirements.txt
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)       38 2022-11-04 06:07:08.000000 brie-2.2.2/setup.cfg
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     2255 2022-05-29 14:29:34.000000 brie-2.2.2/setup.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/simulator/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     5784 2022-03-22 05:13:16.000000 brie-2.2.2/simulator/README.rst
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     7707 2022-03-22 05:13:16.000000 brie-2.2.2/simulator/simuDropout.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     7423 2022-03-22 05:13:16.000000 brie-2.2.2/simulator/simuPSI.py
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     1944 2022-03-22 05:13:16.000000 brie-2.2.2/simulator/spanki_demo.sh
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)     2159 2022-03-22 05:13:16.000000 brie-2.2.2/simulator/utils.py
-drwxr-xr-x   0 yuanhua   (1005) yuanhua   (1006)        0 2022-11-04 06:07:08.000000 brie-2.2.2/tests/
--rw-r--r--   0 yuanhua   (1005) yuanhua   (1006)      101 2022-05-29 14:29:34.000000 brie-2.2.2/tests/README.rst
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.207789 brie-2.2.3/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1196 2024-05-15 03:52:43.000000 brie-2.2.3/.gitignore
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      316 2024-04-21 03:22:55.000000 brie-2.2.3/.readthedocs.yml
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      122 2024-04-21 03:22:55.000000 brie-2.2.3/.travis.yml
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    11393 2024-04-21 03:22:55.000000 brie-2.2.3/LICENSE
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     5339 2024-05-15 04:29:50.207789 brie-2.2.3/PKG-INFO
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     4482 2024-04-21 03:22:55.000000 brie-2.2.3/README.rst
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.195789 brie-2.2.3/brie/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      708 2024-04-21 03:22:55.000000 brie-2.2.3/brie/__init__.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.199789 brie-2.2.3/brie/_cli/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)       40 2024-04-21 03:22:55.000000 brie-2.2.3/brie/_cli/__init__.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      989 2024-04-21 03:22:55.000000 brie-2.2.3/brie/_cli/_cli.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1363 2024-04-21 03:22:55.000000 brie-2.2.3/brie/_cli/count.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      474 2024-04-21 03:22:55.000000 brie-2.2.3/brie/_cli/download.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      403 2024-04-21 03:22:55.000000 brie-2.2.3/brie/_cli/extract.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      497 2024-04-21 03:22:55.000000 brie-2.2.3/brie/_cli/quant.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.199789 brie-2.2.3/brie/bin/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      104 2024-04-21 03:22:55.000000 brie-2.2.3/brie/bin/__init__.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      375 2024-04-21 03:22:55.000000 brie-2.2.3/brie/bin/brie_main.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    11871 2024-04-21 03:22:55.000000 brie-2.2.3/brie/bin/count.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     9323 2024-04-21 03:22:55.000000 brie-2.2.3/brie/bin/quant.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.199789 brie-2.2.3/brie/models/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      142 2024-04-21 03:22:55.000000 brie-2.2.3/brie/models/__init__.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1512 2024-04-21 03:22:55.000000 brie-2.2.3/brie/models/base_model.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     3331 2024-04-21 03:22:55.000000 brie-2.2.3/brie/models/hypothesis_tests.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     8055 2024-04-21 03:22:55.000000 brie-2.2.3/brie/models/model_Beta.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    10251 2024-04-21 03:22:55.000000 brie-2.2.3/brie/models/model_TFProb.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     9656 2024-04-21 03:22:55.000000 brie-2.2.3/brie/models/model_TFProb_dev.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    11532 2024-04-21 03:22:55.000000 brie-2.2.3/brie/models/model_wrap.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     2783 2024-04-21 03:22:55.000000 brie-2.2.3/brie/models/simulator.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      112 2024-04-21 03:22:55.000000 brie-2.2.3/brie/models/tools.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.199789 brie-2.2.3/brie/plot/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     4224 2024-05-15 03:41:13.000000 brie-2.2.3/brie/plot/LRtest_plot.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)       52 2024-04-21 03:22:55.000000 brie-2.2.3/brie/plot/__init__.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     3900 2024-05-15 03:37:42.000000 brie-2.2.3/brie/plot/base_plot.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)       93 2024-04-21 03:22:55.000000 brie-2.2.3/brie/settings.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.203789 brie-2.2.3/brie/utils/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      221 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/__init__.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1756 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/base_utils.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    15312 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/bias_utils.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     9870 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/count.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     9325 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/count_droplet.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     7957 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/fasta_utils.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    11869 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/gtf_utils.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     6251 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/io_utils.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     3689 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/preprocessing.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     7427 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/run_utils.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     7928 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/sam_utils.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    14267 2024-04-21 03:22:55.000000 brie-2.2.3/brie/utils/tran_utils.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)       23 2024-05-15 04:23:28.000000 brie-2.2.3/brie/version.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.203789 brie-2.2.3/brie/version1/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    10781 2024-04-21 03:22:55.000000 brie-2.2.3/brie/version1/brie.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     9419 2024-04-21 03:22:55.000000 brie-2.2.3/brie/version1/brie_diff.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    15651 2024-04-21 03:22:55.000000 brie-2.2.3/brie/version1/model_brie.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.199789 brie-2.2.3/brie.egg-info/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     5339 2024-05-15 04:29:50.000000 brie-2.2.3/brie.egg-info/PKG-INFO
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1841 2024-05-15 04:29:50.000000 brie-2.2.3/brie.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)        1 2024-05-15 04:29:50.000000 brie-2.2.3/brie.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      189 2024-05-15 04:29:50.000000 brie-2.2.3/brie.egg-info/entry_points.txt
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      256 2024-05-15 04:29:50.000000 brie-2.2.3/brie.egg-info/requires.txt
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)        5 2024-05-15 04:29:50.000000 brie-2.2.3/brie.egg-info/top_level.txt
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.203789 brie-2.2.3/doc/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     6762 2024-04-21 03:22:55.000000 brie-2.2.3/doc/Makefile
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     8664 2024-04-21 03:22:55.000000 brie-2.2.3/doc/brie1.rst
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     4719 2024-04-21 03:22:55.000000 brie-2.2.3/doc/brie_count.rst
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     9045 2024-05-15 04:22:58.000000 brie-2.2.3/doc/brie_quant.rst
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    12033 2024-04-21 03:22:55.000000 brie-2.2.3/doc/conf.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.203789 brie-2.2.3/doc/image/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)   271871 2024-04-21 03:22:55.000000 brie-2.2.3/doc/image/BRIE2_roadmap.png
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     4232 2024-04-21 03:22:55.000000 brie-2.2.3/doc/index.rst
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     3858 2024-05-15 04:20:31.000000 brie-2.2.3/doc/install.rst
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     6401 2024-04-21 03:22:55.000000 brie-2.2.3/doc/quick_start.rst
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     4948 2024-05-15 04:29:34.000000 brie-2.2.3/doc/release.rst
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      237 2024-04-21 03:22:55.000000 brie-2.2.3/doc/requirements.txt
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)       44 2024-04-21 03:22:55.000000 brie-2.2.3/doc/tutorial.rst
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.203789 brie-2.2.3/examples/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1139 2024-04-21 03:22:55.000000 brie-2.2.3/examples/brie2_demo.sh
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.203789 brie-2.2.3/examples/demo_v1/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     3413 2024-04-21 03:22:55.000000 brie-2.2.3/examples/demo_v1/anno_maker.sh
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1217 2024-04-21 03:22:55.000000 brie-2.2.3/examples/demo_v1/brie_demo.sh
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.207789 brie-2.2.3/examples/gastrulation/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)    11771 2024-04-21 03:22:55.000000 brie-2.2.3/examples/gastrulation/E-MTAB-4079.130cells.txt
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      718 2024-04-21 03:22:55.000000 brie-2.2.3/examples/gastrulation/brie_sashimi.sh
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1971 2024-04-21 03:22:55.000000 brie-2.2.3/examples/gastrulation/gastrulation_130cells.sh
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      724 2024-04-21 03:22:55.000000 brie-2.2.3/examples/gastrulation/prepare_anno.sh
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1775 2024-04-21 03:22:55.000000 brie-2.2.3/examples/gastrulation/sashimi_setting.txt
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      239 2024-04-21 03:22:55.000000 brie-2.2.3/examples/make_list.sh
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      323 2024-04-21 03:22:55.000000 brie-2.2.3/requirements.txt
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)       38 2024-05-15 04:29:50.207789 brie-2.2.3/setup.cfg
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     2255 2024-04-21 03:22:55.000000 brie-2.2.3/setup.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.207789 brie-2.2.3/simulator/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     5784 2024-04-21 03:22:55.000000 brie-2.2.3/simulator/README.rst
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     7707 2024-04-21 03:22:55.000000 brie-2.2.3/simulator/simuDropout.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     7423 2024-04-21 03:22:55.000000 brie-2.2.3/simulator/simuPSI.py
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     1944 2024-04-21 03:22:55.000000 brie-2.2.3/simulator/spanki_demo.sh
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)     2159 2024-04-21 03:22:55.000000 brie-2.2.3/simulator/utils.py
+drwxr-xr-x   0 yuanhua   (1005) yhlab     (1007)        0 2024-05-15 04:29:50.207789 brie-2.2.3/tests/
+-rw-r--r--   0 yuanhua   (1005) yhlab     (1007)      101 2024-04-21 03:22:55.000000 brie-2.2.3/tests/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `brie-2.2.2/.gitignore` & `brie-2.2.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .DS_Store*
 .vscode/
 temp/
+doc/*.ipynb
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `brie-2.2.2/LICENSE` & `brie-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/PKG-INFO` & `brie-2.2.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: brie
-Version: 2.2.2
-Summary: BRIE: Bayesian regression for isoform estimate
-Home-page: https://brie.readthedocs.io
-Author: Yuanhua Huang
-Author-email: yuanhua@hku.hk
-License: Apache-2.0
-Keywords: RNA splicing,Bayesian regression,single cell RNA-seq,variantional inference
-Platform: UNKNOWN
-Requires-Python: >=3.5
-Provides-Extra: docs
-License-File: LICENSE
-
 |PyPI| |Docs| |Build Status|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/brie.svg
     :target: https://pypi.org/project/brie
 .. |Docs| image:: https://readthedocs.org/projects/brie/badge/?version=latest
    :target: https://brie.readthedocs.io
 .. |Build Status| image:: https://travis-ci.org/huangyh09/brie.svg?branch=master
@@ -121,9 +107,7 @@
   <https://genomebiology.biomedcentral.com/articles/10.1186/s13059-021-02461-5>`_.
   \ **Genome Biology**\, 2021; 22(1):251.
 
 * Yuanhua Huang and Guido Sanguinetti. `BRIE: transcriptome-wide splicing 
   quantification in single cells 
   <https://genomebiology.biomedcentral.com/articles/10.1186/s13059-017-1248-5>`_. 
   \ **Genome Biology**\, 2017; 18(1):123.
-
-
```

### Comparing `brie-2.2.2/README.rst` & `brie-2.2.3/doc/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/brie.svg
     :target: https://pypi.org/project/brie
 .. |Docs| image:: https://readthedocs.org/projects/brie/badge/?version=latest
    :target: https://brie.readthedocs.io
 .. |Build Status| image:: https://travis-ci.org/huangyh09/brie.svg?branch=master
    :target: https://travis-ci.org/huangyh09/brie
-
-
-BRIE: Bayesian Regression for Isoform Estimate
-==============================================
+   
+====
+Home
+====
 
 Top News
---------
+========
 * [29/05/2022] We have released v2.2 that fully supports counting droplet-based 
   data for both Skipping Exon events and other types of splcing events. See the
   `brie-count manual <https://brie.readthedocs.io/en/latest/brie_count.html>`_
 
 * [29/05/2022] We have include small-sized test data sets (15MB) for both 
   smart-seq2 and 10x Genomics. See data in `brie-tutorials/tests repo 
   <https://github.com/huangyh09/brie-tutorials/tree/main/tests>`_
 
 
 About BRIE
-----------
+==========
 
 Welcome to the new BRIE (>=2.0 or BRIE2), Bayesian Regression for Isoform 
 Estimate, a scalable Bayesian method to accurately identify splicing phenotypes 
 in single-cell RNA-seq experiments and quantify isoform proportions and their 
 uncertainty.
 
 BRIE2 supports the analysis of splicing processes at two molecular levels, 
@@ -46,68 +46,81 @@
 2. **Differential momentum genes (DMG):** This task is to quantify the 
    proportions of unspliced and spliced RNAs in each gene and each cell. 
    Similar to DAS, the DMG is a principled selection of genes that capture 
    heterogeneity in transcriptional kinetics between cell groups, e.g., cell 
    types, or continuous cell covariates, hence may enhance the RNA velocity 
    analyses by focusing on dynamics informed genes.
 
+.. note::
+   Though we highly recommend using BRIE v2 for a coherent way for splicing 
+   phenotype selection, `BRIE1 CLI`_ (MCMC based & gene feature only) 
+   is still available but the CLIs are changed to `brie1` and `brie1-diff`.
 
-Installation
-============
-
-BRIE2 is available through PyPI_. To install, type the following command 
-line, and add ``-U`` for upgrading:
-
-.. code-block:: bash
-
-  pip install -U brie
+.. _BRIE1 CLI: https://brie.readthedocs.io/en/latest/brie1.html
 
-Alternatively, you can install from this GitHub repository for the latest (often 
-development) version with the following command line
 
-.. code-block:: bash
+Questions and Issues
+====================
+If you find any technical issues in the codes, 
+we will appreciate your report. Please write them in the GitHub issues: 
+https://github.com/huangyh09/brie/issues
 
-  pip install -U git+https://github.com/huangyh09/brie
+If you have other specific questions on using BRIE, feel free to get in touch 
+with us: yuanhua <at> hku.hk
 
-In either case, add ``--user`` if you don't have the write permission for your 
-Python environment.
 
-For more instructions, see the installation_ manual.
+Quick Resources
+===============
 
-.. _PyPI: https://pypi.org/project/brie
-.. _installation: https://brie.readthedocs.io/en/latest/install.html
+* **Code on GitHub:**
+  https://github.com/huangyh09/brie
 
+* **Preprocessed splicing events annotations (GFT/GFF3):**
+  http://sourceforge.net/projects/brie-rna/files/annotation/
 
-Manual and examples
-===================
+* **Example datasets:**
+  https://github.com/huangyh09/brie-tutorials
 
-* The full manual is at https://brie.readthedocs.io 
-* More examples and tutorials: https://github.com/huangyh09/brie-tutorials
+* **All releases:**
+  https://pypi.org/project/brie/#history
 
-In short, there are two steps for running BRIE2. 
-First, obtain cell-by-gene or cell-by-event count matrices for each isoform. 
-For the exon-skipping event, you can run ``brie-count``, which will return count 
-matrices and hdf5 file for AnnData. 
-For spliced and unspliced matrices, we listed a few options in the manual_.
+* **Issue reports:**
+  https://github.com/huangyh09/brie/issues
 
-Then you can use ``brie-quant`` to perform quantification of splicing ratio and 
-detect differential alternative splicing or differential momentum genes. 
-
-Type command line ``brie-count -h`` and ``brie-quant -h`` to see the full 
-arguments.
-
-
-.. _manual: https://brie.readthedocs.io/en/latest/quick_start.html#step1-read-counts
 
 
 References
 ==========
 
 * Yuanhua Huang and Guido Sanguinetti. `BRIE2: computational identification of 
   splicing phenotypes from single-cell transcriptomic experiments
   <https://genomebiology.biomedcentral.com/articles/10.1186/s13059-021-02461-5>`_.
   \ **Genome Biology**\, 2021; 22(1):251.
 
 * Yuanhua Huang and Guido Sanguinetti. `BRIE: transcriptome-wide splicing 
   quantification in single cells 
   <https://genomebiology.biomedcentral.com/articles/10.1186/s13059-017-1248-5>`_. 
   \ **Genome Biology**\, 2017; 18(1):123.
+
+
+
+.. toctree::
+   :caption: Main
+   :maxdepth: 1
+   :hidden:
+   
+   index
+   install
+   quick_start
+   brie_count
+   brie_quant
+   release
+
+.. toctree::
+   :caption: Examples
+   :maxdepth: 1
+   :hidden:
+
+   brie2_msEAE
+   brie2_scNTseq
+   brie2_dentateGyrus
+   Prior_distribution_BRIE2
```

### Comparing `brie-2.2.2/brie/__init__.py` & `brie-2.2.3/brie/__init__.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/_cli/_cli.py` & `brie-2.2.3/brie/_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/_cli/count.py` & `brie-2.2.3/brie/_cli/count.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/bin/count.py` & `brie-2.2.3/brie/bin/count.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/bin/quant.py` & `brie-2.2.3/brie/bin/quant.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/models/base_model.py` & `brie-2.2.3/brie/models/base_model.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/models/hypothesis_tests.py` & `brie-2.2.3/brie/models/hypothesis_tests.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/models/model_Beta.py` & `brie-2.2.3/brie/models/model_Beta.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/models/model_TFProb.py` & `brie-2.2.3/brie/models/model_TFProb.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/models/model_TFProb_dev.py` & `brie-2.2.3/brie/models/model_TFProb_dev.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/models/model_wrap.py` & `brie-2.2.3/brie/models/model_wrap.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/models/simulator.py` & `brie-2.2.3/brie/models/simulator.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/plot/LRtest_plot.py` & `brie-2.2.3/brie/plot/LRtest_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             yval = -np.log10(yval)
         else:
             y_label = str(y)
     
     plt.scatter(xval[~idx], yval[~idx], color="gray")
     plt.scatter(xval[idx], yval[idx], color="firebrick")
     
-    lable = adata.var.index if anno_id is 'index' else adata.var[anno_id]
+    lable = adata.var.index if anno_id == 'index' else adata.var[anno_id]
     
     texts = []
     for i in idx_anno:
         _label = lable[i]
         _xx = xval[i]
         _yy = yval[i]
         texts.append(plt.text(_xx, _yy, _label, size=8))
```

### Comparing `brie-2.2.2/brie/plot/base_plot.py` & `brie-2.2.3/brie/plot/base_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # support a single gene input
     if type(genes) == str:
         genes = [genes]
             
     if ncol is None:
         ncol = min(4, len(genes))
     if nrow is None:
-        nrow = np.ceil(len(genes) / ncol)
+        nrow = int(np.ceil(len(genes) / ncol))
     
     if color is None:
         color_use = None
     else:
         try:
             if len(color) == adata.shape[0]:
                 color_use = color
```

### Comparing `brie-2.2.2/brie/utils/base_utils.py` & `brie-2.2.3/brie/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/bias_utils.py` & `brie-2.2.3/brie/utils/bias_utils.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/count.py` & `brie-2.2.3/brie/utils/count.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/count_droplet.py` & `brie-2.2.3/brie/utils/count_droplet.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/fasta_utils.py` & `brie-2.2.3/brie/utils/fasta_utils.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/gtf_utils.py` & `brie-2.2.3/brie/utils/gtf_utils.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/io_utils.py` & `brie-2.2.3/brie/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/preprocessing.py` & `brie-2.2.3/brie/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/run_utils.py` & `brie-2.2.3/brie/utils/run_utils.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/sam_utils.py` & `brie-2.2.3/brie/utils/sam_utils.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/utils/tran_utils.py` & `brie-2.2.3/brie/utils/tran_utils.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/version1/brie.py` & `brie-2.2.3/brie/version1/brie.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/version1/brie_diff.py` & `brie-2.2.3/brie/version1/brie_diff.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie/version1/model_brie.py` & `brie-2.2.3/brie/version1/model_brie.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/brie.egg-info/PKG-INFO` & `brie-2.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 Metadata-Version: 2.1
 Name: brie
-Version: 2.2.2
+Version: 2.2.3
 Summary: BRIE: Bayesian regression for isoform estimate
 Home-page: https://brie.readthedocs.io
 Author: Yuanhua Huang
 Author-email: yuanhua@hku.hk
 License: Apache-2.0
 Keywords: RNA splicing,Bayesian regression,single cell RNA-seq,variantional inference
-Platform: UNKNOWN
 Requires-Python: >=3.5
-Provides-Extra: docs
 License-File: LICENSE
+Requires-Dist: anndata>=0.6
+Requires-Dist: scanpy>=1.5
+Requires-Dist: pysam>=0.15.2
+Requires-Dist: numpy>=1.18.0
+Requires-Dist: scipy>=1.4.1
+Requires-Dist: statsmodels>=0.11
+Requires-Dist: pandas>=0.23.0
+Requires-Dist: h5py>=2.9.0
+Requires-Dist: matplotlib>=3.1.2
+Requires-Dist: seaborn>=0.10.0
+Requires-Dist: tensorflow>=2.0.0
+Requires-Dist: tensorflow-probability>=0.8.0
+Requires-Dist: scikit-learn>=0.23
+Requires-Dist: click>=7.0.0
+Provides-Extra: docs
+Requires-Dist: sphinx_bootstrap_theme; extra == "docs"
 
 |PyPI| |Docs| |Build Status|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/brie.svg
     :target: https://pypi.org/project/brie
 .. |Docs| image:: https://readthedocs.org/projects/brie/badge/?version=latest
    :target: https://brie.readthedocs.io
@@ -121,9 +135,7 @@
   <https://genomebiology.biomedcentral.com/articles/10.1186/s13059-021-02461-5>`_.
   \ **Genome Biology**\, 2021; 22(1):251.
 
 * Yuanhua Huang and Guido Sanguinetti. `BRIE: transcriptome-wide splicing 
   quantification in single cells 
   <https://genomebiology.biomedcentral.com/articles/10.1186/s13059-017-1248-5>`_. 
   \ **Genome Biology**\, 2017; 18(1):123.
-
-
```

### Comparing `brie-2.2.2/brie.egg-info/SOURCES.txt` & `brie-2.2.3/brie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/doc/Makefile` & `brie-2.2.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/doc/brie1.rst` & `brie-2.2.3/doc/brie1.rst`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/doc/brie_count.rst` & `brie-2.2.3/doc/brie_count.rst`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/doc/brie_quant.rst` & `brie-2.2.3/doc/brie_quant.rst`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 Based on the cell aggregated imputation, most dimension reduction methods can be
 used, even it doesn't support missing values.
 
 Example command line for mode 2:
 
 .. code-block:: bash
 
+  # keep the following line if you have GPU and want to specify a card
+  CUDA_VISIBLE_DEVICES=1 \
   brie-quant -i out_dir/brie_count.h5ad -o out_dir/brie_quant_aggr.h5ad --interceptMode gene
   
   
 Mode2-diff: Variable splicing detection
 =======================================
 
 This mode requires argument ``-c`` for cell features and ``--LRTindex`` for the 
@@ -173,35 +175,37 @@
       -i IN_FILE, --inFile=IN_FILE
                             Input read count matrices in AnnData h5ad or brie npz format.
       -c CELL_FILE, --cellFile=CELL_FILE
                             File for cell features in tsv[.gz] with cell and feature ids.
       -g GENE_FILE, --geneFile=GENE_FILE
                             File for gene features in tsv[.gz] with gene and feature ids.
       -o OUT_FILE, --out_file=OUT_FILE
-                            Full path of output file for annData in h5ad [default:
-                            $inFile/brie_quant.h5ad]
-      --LRTindex=LRT_INDEX  Index (0-based) of cell features to test with LRT: All, None
-                            or comma separated integers [default: None]
+                            Full path of output file for annData in h5ad
+                            [default: $inFile/brie_quant.h5ad]
+      --LRTindex=LRT_INDEX  Index (0-based) of cell features to test with LRT: 
+                            All, None or comma separated integers [default: None]
       --testBase=TEST_BASE  Features in testing base model: full, null  [default: full]
       --interceptMode=INTERCEPT_MODE
                             Intercept mode: gene, cell or None [default: None]
       --layers=LAYERS       Comma separated layers two or three for estimating Psi
                             [default: isoform1,isoform2,ambiguous]
 
       Gene filtering:
         --minCount=MIN_COUNT
                             Minimum total counts for fitltering genes [default: 50]
         --minUniqCount=MIN_UNIQ_COUNT
                             Minimum unique counts for fitltering genes [default: 10]
         --minCell=MIN_CELL  Minimum number of cells with unique count for fitltering genes
                             [default: 30]
-        --minMIF=MIN_MIF    Minimum minor isoform frequency in unique count [default:
-                            0.001]
+        --minMIF=MIN_MIF    Minimum minor isoform frequency in unique count 
+                            [default: 0.001]
 
       VI Optimization:
         --MCsize=MC_SIZE    Sample size for Monte Carlo Expectation [default: 3]
         --minIter=MIN_ITER  Minimum number of iterations [default: 5000]
         --maxIter=MAX_ITER  Maximum number of iterations [default: 20000]
         --batchSize=BATCH_SIZE
                             Element size per batch: n_gene * total cell [default: 500000]
         --pseudoCount=PSEUDO_COUNT
                             Pseudo count to add on unique count matrices [default: 0.01]
+        -p NPROC, --nproc=NPROC
+                            Number of processes for computing [default: 6]
```

### Comparing `brie-2.2.2/doc/conf.py` & `brie-2.2.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/doc/image/BRIE2_roadmap.png` & `brie-2.2.3/doc/image/BRIE2_roadmap.png`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/doc/index.rst` & `brie-2.2.3/brie.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,61 @@
+Metadata-Version: 2.1
+Name: brie
+Version: 2.2.3
+Summary: BRIE: Bayesian regression for isoform estimate
+Home-page: https://brie.readthedocs.io
+Author: Yuanhua Huang
+Author-email: yuanhua@hku.hk
+License: Apache-2.0
+Keywords: RNA splicing,Bayesian regression,single cell RNA-seq,variantional inference
+Requires-Python: >=3.5
+License-File: LICENSE
+Requires-Dist: anndata>=0.6
+Requires-Dist: scanpy>=1.5
+Requires-Dist: pysam>=0.15.2
+Requires-Dist: numpy>=1.18.0
+Requires-Dist: scipy>=1.4.1
+Requires-Dist: statsmodels>=0.11
+Requires-Dist: pandas>=0.23.0
+Requires-Dist: h5py>=2.9.0
+Requires-Dist: matplotlib>=3.1.2
+Requires-Dist: seaborn>=0.10.0
+Requires-Dist: tensorflow>=2.0.0
+Requires-Dist: tensorflow-probability>=0.8.0
+Requires-Dist: scikit-learn>=0.23
+Requires-Dist: click>=7.0.0
+Provides-Extra: docs
+Requires-Dist: sphinx_bootstrap_theme; extra == "docs"
+
 |PyPI| |Docs| |Build Status|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/brie.svg
     :target: https://pypi.org/project/brie
 .. |Docs| image:: https://readthedocs.org/projects/brie/badge/?version=latest
    :target: https://brie.readthedocs.io
 .. |Build Status| image:: https://travis-ci.org/huangyh09/brie.svg?branch=master
    :target: https://travis-ci.org/huangyh09/brie
-   
-====
-Home
-====
+
+
+BRIE: Bayesian Regression for Isoform Estimate
+==============================================
 
 Top News
-========
+--------
 * [29/05/2022] We have released v2.2 that fully supports counting droplet-based 
   data for both Skipping Exon events and other types of splcing events. See the
   `brie-count manual <https://brie.readthedocs.io/en/latest/brie_count.html>`_
 
 * [29/05/2022] We have include small-sized test data sets (15MB) for both 
   smart-seq2 and 10x Genomics. See data in `brie-tutorials/tests repo 
   <https://github.com/huangyh09/brie-tutorials/tree/main/tests>`_
 
 
 About BRIE
-==========
+----------
 
 Welcome to the new BRIE (>=2.0 or BRIE2), Bayesian Regression for Isoform 
 Estimate, a scalable Bayesian method to accurately identify splicing phenotypes 
 in single-cell RNA-seq experiments and quantify isoform proportions and their 
 uncertainty.
 
 BRIE2 supports the analysis of splicing processes at two molecular levels, 
@@ -46,81 +74,68 @@
 2. **Differential momentum genes (DMG):** This task is to quantify the 
    proportions of unspliced and spliced RNAs in each gene and each cell. 
    Similar to DAS, the DMG is a principled selection of genes that capture 
    heterogeneity in transcriptional kinetics between cell groups, e.g., cell 
    types, or continuous cell covariates, hence may enhance the RNA velocity 
    analyses by focusing on dynamics informed genes.
 
-.. note::
-   Though we highly recommend using BRIE v2 for a coherent way for splicing 
-   phenotype selection, `BRIE1 CLI`_ (MCMC based & gene feature only) 
-   is still available but the CLIs are changed to `brie1` and `brie1-diff`.
 
-.. _BRIE1 CLI: https://brie.readthedocs.io/en/latest/brie1.html
+Installation
+============
+
+BRIE2 is available through PyPI_. To install, type the following command 
+line, and add ``-U`` for upgrading:
+
+.. code-block:: bash
+
+  pip install -U brie
 
+Alternatively, you can install from this GitHub repository for the latest (often 
+development) version with the following command line
 
-Questions and Issues
-====================
-If you find any technical issues in the codes, 
-we will appreciate your report. Please write them in the GitHub issues: 
-https://github.com/huangyh09/brie/issues
+.. code-block:: bash
 
-If you have other specific questions on using BRIE, feel free to get in touch 
-with us: yuanhua <at> hku.hk
+  pip install -U git+https://github.com/huangyh09/brie
 
+In either case, add ``--user`` if you don't have the write permission for your 
+Python environment.
 
-Quick Resources
-===============
+For more instructions, see the installation_ manual.
 
-* **Code on GitHub:**
-  https://github.com/huangyh09/brie
+.. _PyPI: https://pypi.org/project/brie
+.. _installation: https://brie.readthedocs.io/en/latest/install.html
 
-* **Preprocessed splicing events annotations (GFT/GFF3):**
-  http://sourceforge.net/projects/brie-rna/files/annotation/
 
-* **Example datasets:**
-  https://github.com/huangyh09/brie-tutorials
+Manual and examples
+===================
 
-* **All releases:**
-  https://pypi.org/project/brie/#history
+* The full manual is at https://brie.readthedocs.io 
+* More examples and tutorials: https://github.com/huangyh09/brie-tutorials
 
-* **Issue reports:**
-  https://github.com/huangyh09/brie/issues
+In short, there are two steps for running BRIE2. 
+First, obtain cell-by-gene or cell-by-event count matrices for each isoform. 
+For the exon-skipping event, you can run ``brie-count``, which will return count 
+matrices and hdf5 file for AnnData. 
+For spliced and unspliced matrices, we listed a few options in the manual_.
 
+Then you can use ``brie-quant`` to perform quantification of splicing ratio and 
+detect differential alternative splicing or differential momentum genes. 
+
+Type command line ``brie-count -h`` and ``brie-quant -h`` to see the full 
+arguments.
+
+
+.. _manual: https://brie.readthedocs.io/en/latest/quick_start.html#step1-read-counts
 
 
 References
 ==========
 
 * Yuanhua Huang and Guido Sanguinetti. `BRIE2: computational identification of 
   splicing phenotypes from single-cell transcriptomic experiments
   <https://genomebiology.biomedcentral.com/articles/10.1186/s13059-021-02461-5>`_.
   \ **Genome Biology**\, 2021; 22(1):251.
 
 * Yuanhua Huang and Guido Sanguinetti. `BRIE: transcriptome-wide splicing 
   quantification in single cells 
   <https://genomebiology.biomedcentral.com/articles/10.1186/s13059-017-1248-5>`_. 
   \ **Genome Biology**\, 2017; 18(1):123.
-
-
-
-.. toctree::
-   :caption: Main
-   :maxdepth: 1
-   :hidden:
-   
-   index
-   install
-   quick_start
-   brie_count
-   brie_quant
-   release
-
-.. toctree::
-   :caption: Examples
-   :maxdepth: 1
-   :hidden:
-
-   brie2_msEAE
-   brie2_scNTseq
-   brie2_dentateGyrus
-   Prior_distribution_BRIE2
```

### Comparing `brie-2.2.2/doc/install.rst` & `brie-2.2.3/doc/install.rst`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 Environment setting (optional)
 ==============================
 For using BRIE2, we recommend creating a separated `conda environment`_ for 
 easier and cleaner management of dependent packages, particularly TensorFlow and 
 TensorFlow-probability, which are under active development.
 
 The following command line in terminal (Linux or MacOS) will create a conda 
-environment with name ``TFProb``, probably in the path ``~/.conda/envs/TFProb``:
+environment with name ``TFProb``, probably in the path ``~/.conda/envs/TFProb``
+(tested on Python 3.7 to 3.11):
 
 .. code-block:: bash
   
-  conda create -n TFProb python=3.7
+  conda create -n TFProb python=3.11
 
 Alternatively, you can create the environment in another path by replacing 
 ``-n TFProb`` with ``-p ANY_PATH/TFProb`` to specify the path for conda 
 environment. Then you can check your environment by ``conda env list`` and 
 activate the environment by ``conda activate TFProb`` or the full path, before 
 start installing brie and other packages.
 
@@ -47,40 +48,37 @@
 
 .. _PYPI: https://pypi.org/project/brie
 
 
 GPU usage
 =========
 One of the key benefits of using TensorFlow backend is its direct support of 
-GPU for substantial speedups (generally >10x). Here is one way to set up GPU 
-configurations with NVIDIA GPU on Ubuntu:
+GPU for substantial speedups (generally >10x). In general, the above 
+installation should directly support GPU use as default by using the newest 
+tensorflow and tensorflow-probability. 
 
-.. code-block:: bash
+To check if the installation is compatible with GPUs, you can print out the 
+detectable GPU cards, as below (it gives `[ ]` if failing to setup properly):
 
-  pip install -U tensorflow-gpu
-  conda install -c anaconda cudatoolkit
+.. code-block:: html
 
-Make sure that you have compatible versions between tensorflow and NVIDIA CUDA. 
-You can check TF's test `here <https://www.tensorflow.org/install/source#gpu>`_.
-For more information on GPU configuration, please refer to the 
-`Tensorflow documentation`_ or `anaconda GPU`_.
+  $ python3 -c "import tensorflow as tf; print(tf.config.list_physical_devices('GPU'))"
+    [PhysicalDevice(name='/physical_device:GPU:0', device_type='GPU'), ...]
 
-.. _Tensorflow documentation: https://www.tensorflow.org/guide/gpu
-.. _anaconda GPU: https://docs.anaconda.com/anaconda/user-guide/tasks/gpu-packages/
+However, occasionally, the newest TensorFlow may not be stable or compatible
+widely, for example the `tensorflow[and-cuda]==2.16.1` is not compatible with GPUs,
+see discussion `here <https://github.com/tensorflow/tensorflow/issues/63362#issuecomment-2053849484>`_.
 
-Once successfully configured, you will see log info like the following when 
-using ``brie-quant``:
+Here is one way to use a lower version for GPU configurations with NVIDIA GPU 
+on Ubuntu (tested on 21/04/2024):
 
-.. code-block:: html
-
-  $ brie-quant
-    I tensorflow/stream_executor/platform/default/dso_loader.cc:53] 
-    Successfully opened dynamic library libcudart.so.11.0
-    Welcome to brie-quant in BRIE v2.0.5!
+.. code-block:: bash
 
+  pip install tensorflow-probability==0.23.0
+  pip install tensorflow[and-cuda]==2.15.1
 
 .. note::
    At the moment, TensorFlow calls all available GPUs, which is not necessary. 
    You can specify the card (e.g., card 3) by adding the below variable before 
    your command line ``CUDA_VISIBLE_DEVICES=3 brie-quant -i my_count.h5ad``
```

### Comparing `brie-2.2.2/doc/quick_start.rst` & `brie-2.2.3/doc/quick_start.rst`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/doc/release.rst` & `brie-2.2.3/doc/release.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 =============
 Release notes
 =============
 
 Release in future
 =================
 
+Release v2.2.3 (15/05/2022)
+===========================
+* minor fix in plotting function brie.pl.count()
+* add submodule brie-tutorials
+
 Release v2.2.2 (04/11/2022)
 ===========================
 * support limit the CPU threads used by tensorflow in brie-quant (default 6)
 
 Release v2.2.1 (14/07/2022)
 ===========================
 * fix a bug for `--eventType=Any` in smart-seq
```

### Comparing `brie-2.2.2/examples/brie2_demo.sh` & `brie-2.2.3/examples/brie2_demo.sh`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/examples/demo_v1/anno_maker.sh` & `brie-2.2.3/examples/demo_v1/anno_maker.sh`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/examples/demo_v1/brie_demo.sh` & `brie-2.2.3/examples/demo_v1/brie_demo.sh`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/examples/gastrulation/E-MTAB-4079.130cells.txt` & `brie-2.2.3/examples/gastrulation/E-MTAB-4079.130cells.txt`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/examples/gastrulation/brie_sashimi.sh` & `brie-2.2.3/examples/gastrulation/brie_sashimi.sh`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/examples/gastrulation/gastrulation_130cells.sh` & `brie-2.2.3/examples/gastrulation/gastrulation_130cells.sh`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/examples/gastrulation/prepare_anno.sh` & `brie-2.2.3/examples/gastrulation/prepare_anno.sh`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/examples/gastrulation/sashimi_setting.txt` & `brie-2.2.3/examples/gastrulation/sashimi_setting.txt`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/setup.py` & `brie-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/simulator/README.rst` & `brie-2.2.3/simulator/README.rst`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/simulator/simuDropout.py` & `brie-2.2.3/simulator/simuDropout.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/simulator/simuPSI.py` & `brie-2.2.3/simulator/simuPSI.py`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/simulator/spanki_demo.sh` & `brie-2.2.3/simulator/spanki_demo.sh`

 * *Files identical despite different names*

### Comparing `brie-2.2.2/simulator/utils.py` & `brie-2.2.3/simulator/utils.py`

 * *Files identical despite different names*

