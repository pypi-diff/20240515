# Comparing `tmp/ragu-0.1.33.tar.gz` & `tmp/ragu-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragu-0.1.33.tar", last modified: Wed Apr 24 19:10:43 2024, max compression
+gzip compressed data, was "ragu-0.1.34.tar", last modified: Wed May 15 14:33:46 2024, max compression
```

## Comparing `ragu-0.1.33.tar` & `ragu-0.1.34.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.073327 ragu-0.1.33/
--rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.33/LICENSE.txt
--rw-r--r--   0 btober     (501) staff       (20)    47505 2024-04-24 19:10:43.073085 ragu-0.1.33/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     6295 2024-04-19 17:28:40.000000 ragu-0.1.33/README.md
--rw-r--r--   0 btober     (501) staff       (20)      942 2024-04-24 19:09:42.000000 ragu-0.1.33/pyproject.toml
--rw-r--r--   0 btober     (501) staff       (20)       38 2024-04-24 19:10:43.073365 ragu-0.1.33/setup.cfg
--rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.33/setup.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.049736 ragu-0.1.33/src/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.051327 ragu-0.1.33/src/ragu/
--rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/__init__.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.052114 ragu-0.1.33/src/ragu/bin/
--rw-r--r--   0 btober     (501) staff       (20)     2574 2024-02-24 23:44:42.000000 ragu-0.1.33/src/ragu/bin/ragu.py
--rw-r--r--   0 btober     (501) staff       (20)     2112 2024-04-24 18:46:05.000000 ragu-0.1.33/src/ragu/config.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.049889 ragu-0.1.33/src/ragu/dat/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.052230 ragu-0.1.33/src/ragu/dat/mars/
--rw-r--r--   0 btober     (501) staff       (20) 33196562 2024-02-24 23:44:42.000000 ragu-0.1.33/src/ragu/dat/mars/mega90n000eb.tif
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.069625 ragu-0.1.33/src/ragu/ingest/
--rw-r--r--   0 btober     (501) staff       (20)     5750 2024-04-19 16:57:42.000000 ragu-0.1.33/src/ragu/ingest/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     2411 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_cresis_rds.py
--rw-r--r--   0 btober     (501) staff       (20)     2454 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_cresis_snow.py
--rw-r--r--   0 btober     (501) staff       (20)     3089 2024-04-24 18:40:40.000000 ragu-0.1.33/src/ragu/ingest/ingest_groundhog.py
--rw-r--r--   0 btober     (501) staff       (20)     3366 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_gssi.py
--rw-r--r--   0 btober     (501) staff       (20)     2562 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_lrs.py
--rw-r--r--   0 btober     (501) staff       (20)     2896 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_marsis.py
--rw-r--r--   0 btober     (501) staff       (20)     2474 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_marsis_ipc.py
--rw-r--r--   0 btober     (501) staff       (20)     5780 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_oibAK.py
--rw-r--r--   0 btober     (501) staff       (20)    14181 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_pulseekko.py
--rw-r--r--   0 btober     (501) staff       (20)     2537 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_rimfax.py
--rw-r--r--   0 btober     (501) staff       (20)     2931 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_sharad.py
--rw-r--r--   0 btober     (501) staff       (20)     3640 2024-04-19 16:41:20.000000 ragu-0.1.33/src/ragu/ingest/ingest_template.py
--rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/ingest/ingest_uaf_kentech.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.069968 ragu-0.1.33/src/ragu/nav/
--rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/nav/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/nav/gps.py
--rw-r--r--   0 btober     (501) staff       (20)    21420 2024-04-22 00:33:24.000000 ragu-0.1.33/src/ragu/nav/navparse.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.070422 ragu-0.1.33/src/ragu/radar/
--rw-r--r--   0 btober     (501) staff       (20)     7814 2024-04-23 21:24:56.000000 ragu-0.1.33/src/ragu/radar/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/radar/flags.py
--rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/radar/pick.py
--rw-r--r--   0 btober     (501) staff       (20)    14029 2024-04-19 16:55:41.000000 ragu-0.1.33/src/ragu/radar/processing.py
--rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/raguError.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.071391 ragu-0.1.33/src/ragu/recs/
--rw-r--r--   0 btober     (501) staff       (20)  1079564 2024-02-24 23:44:42.000000 ragu-0.1.33/src/ragu/recs/20190928-235534_compiled.jpg
--rw-r--r--   0 btober     (501) staff       (20)    16176 2024-02-24 23:44:42.000000 ragu-0.1.33/src/ragu/recs/basemap_icon.png
--rw-r--r--   0 btober     (501) staff       (20)    92542 2024-02-24 23:44:42.000000 ragu-0.1.33/src/ragu/recs/bulb.jpg
--rw-r--r--   0 btober     (501) staff       (20)    21590 2024-02-24 23:44:42.000000 ragu-0.1.33/src/ragu/recs/ragu_logo.png
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.071809 ragu-0.1.33/src/ragu/tools/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/tools/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/tools/constants.py
--rw-r--r--   0 btober     (501) staff       (20)     9245 2024-04-19 16:56:13.000000 ragu-0.1.33/src/ragu/tools/export.py
--rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/tools/utils.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.072669 ragu-0.1.33/src/ragu/ui/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/ui/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)    16621 2024-02-24 23:44:42.000000 ragu-0.1.33/src/ragu/ui/basemap.py
--rw-r--r--   0 btober     (501) staff       (20)    69074 2024-04-24 19:08:38.000000 ragu-0.1.33/src/ragu/ui/gui.py
--rw-r--r--   0 btober     (501) staff       (20)    71060 2024-04-23 21:19:13.000000 ragu-0.1.33/src/ragu/ui/impick.py
--rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/ui/notepad.py
--rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.33/src/ragu/ui/wvpick.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 19:10:43.051996 ragu-0.1.33/src/ragu.egg-info/
--rw-r--r--   0 btober     (501) staff       (20)    47505 2024-04-24 19:10:43.000000 ragu-0.1.33/src/ragu.egg-info/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     1369 2024-04-24 19:10:43.000000 ragu-0.1.33/src/ragu.egg-info/SOURCES.txt
--rw-r--r--   0 btober     (501) staff       (20)        1 2024-04-24 19:10:43.000000 ragu-0.1.33/src/ragu.egg-info/dependency_links.txt
--rw-r--r--   0 btober     (501) staff       (20)       44 2024-04-24 19:10:43.000000 ragu-0.1.33/src/ragu.egg-info/entry_points.txt
--rw-r--r--   0 btober     (501) staff       (20)       64 2024-04-24 19:10:43.000000 ragu-0.1.33/src/ragu.egg-info/requires.txt
--rw-r--r--   0 btober     (501) staff       (20)       10 2024-04-24 19:10:43.000000 ragu-0.1.33/src/ragu.egg-info/top_level.txt
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.361105 ragu-0.1.34/
+-rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.34/LICENSE.txt
+-rw-r--r--   0 btober     (501) staff       (20)    47505 2024-05-15 14:33:46.360865 ragu-0.1.34/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     6295 2024-04-19 17:28:40.000000 ragu-0.1.34/README.md
+-rw-r--r--   0 btober     (501) staff       (20)      942 2024-05-15 14:33:06.000000 ragu-0.1.34/pyproject.toml
+-rw-r--r--   0 btober     (501) staff       (20)       38 2024-05-15 14:33:46.361145 ragu-0.1.34/setup.cfg
+-rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.34/setup.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.332558 ragu-0.1.34/src/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.333805 ragu-0.1.34/src/ragu/
+-rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/__init__.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.334676 ragu-0.1.34/src/ragu/bin/
+-rw-r--r--   0 btober     (501) staff       (20)     2574 2024-02-24 23:44:42.000000 ragu-0.1.34/src/ragu/bin/ragu.py
+-rw-r--r--   0 btober     (501) staff       (20)     2112 2024-04-24 18:46:05.000000 ragu-0.1.34/src/ragu/config.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.332713 ragu-0.1.34/src/ragu/dat/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.334801 ragu-0.1.34/src/ragu/dat/mars/
+-rw-r--r--   0 btober     (501) staff       (20) 33196562 2024-02-24 23:44:42.000000 ragu-0.1.34/src/ragu/dat/mars/mega90n000eb.tif
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.356326 ragu-0.1.34/src/ragu/ingest/
+-rw-r--r--   0 btober     (501) staff       (20)     5750 2024-05-15 14:31:25.000000 ragu-0.1.34/src/ragu/ingest/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     2411 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_cresis_rds.py
+-rw-r--r--   0 btober     (501) staff       (20)     2454 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_cresis_snow.py
+-rw-r--r--   0 btober     (501) staff       (20)     3190 2024-05-15 14:29:27.000000 ragu-0.1.34/src/ragu/ingest/ingest_groundhog.py
+-rw-r--r--   0 btober     (501) staff       (20)     3366 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_gssi.py
+-rw-r--r--   0 btober     (501) staff       (20)     2562 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_lrs.py
+-rw-r--r--   0 btober     (501) staff       (20)     2896 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_marsis.py
+-rw-r--r--   0 btober     (501) staff       (20)     2474 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_marsis_ipc.py
+-rw-r--r--   0 btober     (501) staff       (20)     5780 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_oibAK.py
+-rw-r--r--   0 btober     (501) staff       (20)    14181 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_pulseekko.py
+-rw-r--r--   0 btober     (501) staff       (20)     2537 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_rimfax.py
+-rw-r--r--   0 btober     (501) staff       (20)     2931 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_sharad.py
+-rw-r--r--   0 btober     (501) staff       (20)     3640 2024-04-19 16:41:20.000000 ragu-0.1.34/src/ragu/ingest/ingest_template.py
+-rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/ingest/ingest_uaf_kentech.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.356634 ragu-0.1.34/src/ragu/nav/
+-rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/nav/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/nav/gps.py
+-rw-r--r--   0 btober     (501) staff       (20)    21420 2024-04-22 00:33:24.000000 ragu-0.1.34/src/ragu/nav/navparse.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.357067 ragu-0.1.34/src/ragu/radar/
+-rw-r--r--   0 btober     (501) staff       (20)     7814 2024-04-23 21:24:56.000000 ragu-0.1.34/src/ragu/radar/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/radar/flags.py
+-rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/radar/pick.py
+-rw-r--r--   0 btober     (501) staff       (20)    14029 2024-04-19 16:55:41.000000 ragu-0.1.34/src/ragu/radar/processing.py
+-rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/raguError.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.359297 ragu-0.1.34/src/ragu/recs/
+-rw-r--r--   0 btober     (501) staff       (20)  1079564 2024-02-24 23:44:42.000000 ragu-0.1.34/src/ragu/recs/20190928-235534_compiled.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    16176 2024-02-24 23:44:42.000000 ragu-0.1.34/src/ragu/recs/basemap_icon.png
+-rw-r--r--   0 btober     (501) staff       (20)    92542 2024-02-24 23:44:42.000000 ragu-0.1.34/src/ragu/recs/bulb.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    21590 2024-02-24 23:44:42.000000 ragu-0.1.34/src/ragu/recs/ragu_logo.png
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.359785 ragu-0.1.34/src/ragu/tools/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/tools/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/tools/constants.py
+-rw-r--r--   0 btober     (501) staff       (20)     9245 2024-04-19 16:56:13.000000 ragu-0.1.34/src/ragu/tools/export.py
+-rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/tools/utils.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.360522 ragu-0.1.34/src/ragu/ui/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/ui/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)    16621 2024-02-24 23:44:42.000000 ragu-0.1.34/src/ragu/ui/basemap.py
+-rw-r--r--   0 btober     (501) staff       (20)    69074 2024-05-15 01:43:36.000000 ragu-0.1.34/src/ragu/ui/gui.py
+-rw-r--r--   0 btober     (501) staff       (20)    71060 2024-04-23 21:19:13.000000 ragu-0.1.34/src/ragu/ui/impick.py
+-rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/ui/notepad.py
+-rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.34/src/ragu/ui/wvpick.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-05-15 14:33:46.334562 ragu-0.1.34/src/ragu.egg-info/
+-rw-r--r--   0 btober     (501) staff       (20)    47505 2024-05-15 14:33:46.000000 ragu-0.1.34/src/ragu.egg-info/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     1369 2024-05-15 14:33:46.000000 ragu-0.1.34/src/ragu.egg-info/SOURCES.txt
+-rw-r--r--   0 btober     (501) staff       (20)        1 2024-05-15 14:33:46.000000 ragu-0.1.34/src/ragu.egg-info/dependency_links.txt
+-rw-r--r--   0 btober     (501) staff       (20)       44 2024-05-15 14:33:46.000000 ragu-0.1.34/src/ragu.egg-info/entry_points.txt
+-rw-r--r--   0 btober     (501) staff       (20)       64 2024-05-15 14:33:46.000000 ragu-0.1.34/src/ragu.egg-info/requires.txt
+-rw-r--r--   0 btober     (501) staff       (20)       10 2024-05-15 14:33:46.000000 ragu-0.1.34/src/ragu.egg-info/top_level.txt
```

### Comparing `ragu-0.1.33/LICENSE.txt` & `ragu-0.1.34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/PKG-INFO` & `ragu-0.1.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.33
+Version: 0.1.34
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ragu-0.1.33/README.md` & `ragu-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/pyproject.toml` & `ragu-0.1.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ragu"
-version = "0.1.33"
+version = "0.1.34"
 description = "Radar Analysis Graphical Utility (RAGU)"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 authors = [
      {name = "Brandon Tober", email = "tobers.brandon@gmail.com"},
      {name = "Michael Christoffersen", email = "mchristo28@gmail.com"},
```

### Comparing `ragu-0.1.33/src/ragu/bin/ragu.py` & `ragu-0.1.34/src/ragu/bin/ragu.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/config.py` & `ragu-0.1.34/src/ragu/config.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/dat/mars/mega90n000eb.tif` & `ragu-0.1.34/src/ragu/dat/mars/mega90n000eb.tif`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/__init__.py` & `ragu-0.1.34/src/ragu/ingest/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,17 @@
         # better ways to do this than an if/else
         # but for a few file types this is easier
         if (self.ftype == "h5"):
             try:
                 self.rdata = ingest_oibAK.read_h5(self.fpath, navcrs, body)
             except:
                 try:
-                    self.rdata = ingest_uaf_kentech.read_h5(self.fpath, navcrs, body)
-                except:
                     self.rdata = ingest_groundhog.read_h5(self.fpath, navcrs, body)
+                except:
+                    self.rdata = ingest_uaf_kentech.read_h5(self.fpath, navcrs, body)
         elif (self.ftype == "mat"):
             try:
                 self.rdata = ingest_cresis_snow.read_mat(self.fpath, navcrs, body)
             except:
                 try:
                     self.rdata = ingest_cresis_rds.read_mat(self.fpath, navcrs, body)
                 except:
```

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_cresis_rds.py` & `ragu-0.1.34/src/ragu/ingest/ingest_cresis_rds.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_cresis_snow.py` & `ragu-0.1.34/src/ragu/ingest/ingest_cresis_snow.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_groundhog.py` & `ragu-0.1.34/src/ragu/ingest/ingest_groundhog.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import scipy as sp
 import sys
 
 # method to ingest groundhog hdf5 data format
 def read_h5(fpath, navcrs, body):
     rdata = garlic(fpath)
     rdata.fn = fpath.split("/")[-1][:-3]
-    rdata.dtype = "groundhog"
 
     # read in .h5 file
     f = h5py.File(rdata.fpath, "r")                      
 
     # pull necessary raw group data
     rdata.fs = f["raw/rx0"].attrs["fs"]                             # sampling frequency
     rdata.dt = 1/rdata.fs
@@ -36,16 +35,23 @@
 
     # pull radar proc and sim arrayss
     if("restack" in f.keys()):
         rdata.set_dat(f["restack/rx0"][:].astype(float))
     else:
         rdata.set_dat(f["raw/rx0"][:].astype(float))
 
-    # want to plot positive and negative amplitude values - don't dB 
-    rdata.dbit = False
+    # get system info
+    try:
+        if "Blue Systems" in f.attrs["system"]:
+            rdata.dtype = "bsi"
+            rdata.dbit = True
+    except KeyError:
+        rdata.dtype = "groundhog"
+        rdata.dbit = False
+
     rdata.set_proc(rdata.get_dat())
     rdata.snum, rdata.tnum = rdata.get_dat().shape
 
     rdata.set_twtt()
 
     # parse nav
     rdata.geocrs = navcrs
```

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_gssi.py` & `ragu-0.1.34/src/ragu/ingest/ingest_gssi.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_lrs.py` & `ragu-0.1.34/src/ragu/ingest/ingest_lrs.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_marsis.py` & `ragu-0.1.34/src/ragu/ingest/ingest_marsis.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_marsis_ipc.py` & `ragu-0.1.34/src/ragu/ingest/ingest_marsis_ipc.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_oibAK.py` & `ragu-0.1.34/src/ragu/ingest/ingest_oibAK.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_pulseekko.py` & `ragu-0.1.34/src/ragu/ingest/ingest_pulseekko.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_rimfax.py` & `ragu-0.1.34/src/ragu/ingest/ingest_rimfax.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_sharad.py` & `ragu-0.1.34/src/ragu/ingest/ingest_sharad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_template.py` & `ragu-0.1.34/src/ragu/ingest/ingest_template.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ingest/ingest_uaf_kentech.py` & `ragu-0.1.34/src/ragu/ingest/ingest_uaf_kentech.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/nav/gps.py` & `ragu-0.1.34/src/ragu/nav/gps.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/nav/navparse.py` & `ragu-0.1.34/src/ragu/nav/navparse.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/radar/__init__.py` & `ragu-0.1.34/src/ragu/radar/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/radar/pick.py` & `ragu-0.1.34/src/ragu/radar/pick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/radar/processing.py` & `ragu-0.1.34/src/ragu/radar/processing.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/recs/20190928-235534_compiled.jpg` & `ragu-0.1.34/src/ragu/recs/20190928-235534_compiled.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/recs/basemap_icon.png` & `ragu-0.1.34/src/ragu/recs/basemap_icon.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/recs/bulb.jpg` & `ragu-0.1.34/src/ragu/recs/bulb.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/recs/ragu_logo.png` & `ragu-0.1.34/src/ragu/recs/ragu_logo.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/tools/export.py` & `ragu-0.1.34/src/ragu/tools/export.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/tools/utils.py` & `ragu-0.1.34/src/ragu/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ui/basemap.py` & `ragu-0.1.34/src/ragu/ui/basemap.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ui/gui.py` & `ragu-0.1.34/src/ragu/ui/gui.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ui/impick.py` & `ragu-0.1.34/src/ragu/ui/impick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ui/notepad.py` & `ragu-0.1.34/src/ragu/ui/notepad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu/ui/wvpick.py` & `ragu-0.1.34/src/ragu/ui/wvpick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.33/src/ragu.egg-info/PKG-INFO` & `ragu-0.1.34/src/ragu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.33
+Version: 0.1.34
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ragu-0.1.33/src/ragu.egg-info/SOURCES.txt` & `ragu-0.1.34/src/ragu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

