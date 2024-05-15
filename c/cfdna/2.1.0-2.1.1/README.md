# Comparing `tmp/cfdna-2.1.0.tar.gz` & `tmp/cfdna-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdna-2.1.0.tar", max compression
+gzip compressed data, was "cfdna-2.1.1.tar", max compression
```

## Comparing `cfdna-2.1.0.tar` & `cfdna-2.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rwxr-xr-x   0        0        0    17895 2022-07-20 16:09:08.000000 cfdna-2.1.0/LICENSE.md
--rwxr-xr-x   0        0        0     1341 2023-11-21 14:09:42.209706 cfdna-2.1.0/README.md
--rw-r--r--   0        0        0     8196 2024-05-14 15:11:34.093762 cfdna-2.1.0/cfdna/.DS_Store
--rwxr-xr-x   0        0        0      638 2024-05-08 14:59:14.786741 cfdna-2.1.0/cfdna/__init__.py
--rwxr-xr-x   0        0        0     4486 2024-04-16 02:05:12.659608 cfdna-2.1.0/cfdna/__main__.py
--rwxr-xr-x   0        0        0       69 2022-07-20 16:09:08.000000 cfdna-2.1.0/cfdna/commandline/__init__.py
--rwxr-xr-x   0        0        0     8737 2024-05-14 15:12:01.217023 cfdna-2.1.0/cfdna/commandline/commands.py
--rwxr-xr-x   0        0        0       64 2022-08-30 19:13:58.000000 cfdna-2.1.0/cfdna/core/__init__.py
--rwxr-xr-x   0        0        0     2918 2023-11-06 18:52:38.951861 cfdna-2.1.0/cfdna/core/core.py
--rw-r--r--   0        0        0     6148 2023-11-06 14:19:28.230169 cfdna-2.1.0/cfdna/io/.DS_Store
--rwxr-xr-x   0        0        0      281 2022-07-20 16:09:09.000000 cfdna-2.1.0/cfdna/io/__init__.py
--rwxr-xr-x   0        0        0      184 2022-07-20 16:09:09.000000 cfdna-2.1.0/cfdna/io/read/__init__.py
--rwxr-xr-x   0        0        0     1762 2023-02-03 15:34:27.663648 cfdna-2.1.0/cfdna/io/read/read_bam.py
--rwxr-xr-x   0        0        0      491 2023-11-06 18:42:33.912191 cfdna-2.1.0/cfdna/io/read/read_h5.py
--rwxr-xr-x   0        0        0      190 2022-07-20 16:09:09.000000 cfdna-2.1.0/cfdna/io/write/__init__.py
--rwxr-xr-x   0        0        0      511 2023-11-06 18:43:44.583371 cfdna-2.1.0/cfdna/io/write/write_h5.py
--rwxr-xr-x   0        0        0      849 2022-07-20 16:09:09.000000 cfdna-2.1.0/cfdna/io/write/write_text.py
--rwxr-xr-x   0        0        0       67 2022-07-20 16:09:08.000000 cfdna-2.1.0/cfdna/plot/__init__.py
--rwxr-xr-x   0        0        0     7663 2022-07-20 16:09:09.000000 cfdna-2.1.0/cfdna/plot/plot_bokeh.py
--rwxr-xr-x   0        0        0      990 2023-11-07 16:01:23.498388 cfdna-2.1.0/cfdna/plot/plot_plt.py
--rwxr-xr-x   0        0        0      391 2022-10-05 14:16:05.000000 cfdna-2.1.0/cfdna/tools/__init__.py
--rwxr-xr-x   0        0        0      167 2023-11-06 18:36:25.971444 cfdna-2.1.0/cfdna/tools/cnv/__init__.py
--rwxr-xr-x   0        0        0     3563 2023-11-06 18:44:12.544286 cfdna-2.1.0/cfdna/tools/cnv/segmentation.py
--rw-r--r--   0        0        0     1334 2024-03-21 21:01:17.622900 cfdna-2.1.0/cfdna/tools/coverage/gene_activity.py
--rwxr-xr-x   0        0        0      165 2022-07-20 16:09:08.000000 cfdna-2.1.0/cfdna/tools/fragmentation/__init__.py
--rwxr-xr-x   0        0        0     2418 2022-08-30 16:29:27.000000 cfdna-2.1.0/cfdna/tools/fragmentation/frag_pattern.py
--rwxr-xr-x   0        0        0      175 2022-07-20 16:09:08.000000 cfdna-2.1.0/cfdna/tools/nucleosome/__init__.py
--rw-r--r--   0        0        0     4281 2022-10-20 20:27:47.000000 cfdna-2.1.0/cfdna/tools/nucleosome/gene_activity.py
--rwxr-xr-x   0        0        0     8696 2022-08-30 16:32:05.000000 cfdna-2.1.0/cfdna/tools/nucleosome/nfr.py
--rw-r--r--   0        0        0     5375 2022-10-21 19:39:37.000000 cfdna-2.1.0/cfdna/tools/nucleosome/relative_window.py
--rwxr-xr-x   0        0        0     8490 2024-05-09 17:45:05.523659 cfdna-2.1.0/cfdna/tools/nucleosome/wps.py
--rw-r--r--   0        0        0     7053 2022-10-05 14:45:53.000000 cfdna-2.1.0/cfdna/tools/nucleosome/wps_functions.py
--rwxr-xr-x   0        0        0      162 2022-07-20 16:09:08.000000 cfdna-2.1.0/cfdna/tools/summarize/__init__.py
--rw-r--r--   0        0        0     3551 2022-08-30 19:26:15.000000 cfdna-2.1.0/cfdna/tools/summarize/multi_sample.py
--rwxr-xr-x   0        0        0     3417 2023-11-06 18:46:14.639312 cfdna-2.1.0/cfdna/tools/summarize/summarize.py
--rwxr-xr-x   0        0        0      143 2022-07-20 16:09:09.000000 cfdna-2.1.0/cfdna/utilities/__init__.py
--rwxr-xr-x   0        0        0     4289 2022-08-30 19:22:16.000000 cfdna-2.1.0/cfdna/utilities/h5_utilities.py
--rw-r--r--   0        0        0     2474 2024-05-14 15:12:34.623293 cfdna-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 cfdna-2.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2022-07-20 16:09:08.000000 cfdna-2.1.1/LICENSE.md
+-rwxr-xr-x   0        0        0     1341 2023-11-21 14:09:42.209706 cfdna-2.1.1/README.md
+-rw-r--r--   0        0        0     8196 2024-05-14 15:11:34.093762 cfdna-2.1.1/cfdna/.DS_Store
+-rwxr-xr-x   0        0        0      638 2024-05-15 18:27:16.441217 cfdna-2.1.1/cfdna/__init__.py
+-rwxr-xr-x   0        0        0     4486 2024-04-16 02:05:12.659608 cfdna-2.1.1/cfdna/__main__.py
+-rwxr-xr-x   0        0        0       69 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/commandline/__init__.py
+-rwxr-xr-x   0        0        0     8733 2024-05-15 18:27:00.233103 cfdna-2.1.1/cfdna/commandline/commands.py
+-rwxr-xr-x   0        0        0       64 2022-08-30 19:13:58.000000 cfdna-2.1.1/cfdna/core/__init__.py
+-rwxr-xr-x   0        0        0     2918 2023-11-06 18:52:38.951861 cfdna-2.1.1/cfdna/core/core.py
+-rw-r--r--   0        0        0     6148 2023-11-06 14:19:28.230169 cfdna-2.1.1/cfdna/io/.DS_Store
+-rwxr-xr-x   0        0        0      281 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/io/__init__.py
+-rwxr-xr-x   0        0        0      184 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/io/read/__init__.py
+-rwxr-xr-x   0        0        0     1762 2023-02-03 15:34:27.663648 cfdna-2.1.1/cfdna/io/read/read_bam.py
+-rwxr-xr-x   0        0        0      491 2023-11-06 18:42:33.912191 cfdna-2.1.1/cfdna/io/read/read_h5.py
+-rwxr-xr-x   0        0        0      190 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/io/write/__init__.py
+-rwxr-xr-x   0        0        0      511 2023-11-06 18:43:44.583371 cfdna-2.1.1/cfdna/io/write/write_h5.py
+-rwxr-xr-x   0        0        0      849 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/io/write/write_text.py
+-rwxr-xr-x   0        0        0       67 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/plot/__init__.py
+-rwxr-xr-x   0        0        0     7663 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/plot/plot_bokeh.py
+-rwxr-xr-x   0        0        0      990 2023-11-07 16:01:23.498388 cfdna-2.1.1/cfdna/plot/plot_plt.py
+-rwxr-xr-x   0        0        0      391 2022-10-05 14:16:05.000000 cfdna-2.1.1/cfdna/tools/__init__.py
+-rwxr-xr-x   0        0        0      167 2023-11-06 18:36:25.971444 cfdna-2.1.1/cfdna/tools/cnv/__init__.py
+-rwxr-xr-x   0        0        0     3563 2023-11-06 18:44:12.544286 cfdna-2.1.1/cfdna/tools/cnv/segmentation.py
+-rw-r--r--   0        0        0     1334 2024-03-21 21:01:17.622900 cfdna-2.1.1/cfdna/tools/coverage/gene_activity.py
+-rwxr-xr-x   0        0        0      165 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/tools/fragmentation/__init__.py
+-rwxr-xr-x   0        0        0     2418 2022-08-30 16:29:27.000000 cfdna-2.1.1/cfdna/tools/fragmentation/frag_pattern.py
+-rwxr-xr-x   0        0        0      175 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/tools/nucleosome/__init__.py
+-rw-r--r--   0        0        0     4281 2022-10-20 20:27:47.000000 cfdna-2.1.1/cfdna/tools/nucleosome/gene_activity.py
+-rwxr-xr-x   0        0        0     8696 2022-08-30 16:32:05.000000 cfdna-2.1.1/cfdna/tools/nucleosome/nfr.py
+-rw-r--r--   0        0        0     5375 2022-10-21 19:39:37.000000 cfdna-2.1.1/cfdna/tools/nucleosome/relative_window.py
+-rwxr-xr-x   0        0        0     8490 2024-05-09 17:45:05.523659 cfdna-2.1.1/cfdna/tools/nucleosome/wps.py
+-rw-r--r--   0        0        0     7053 2022-10-05 14:45:53.000000 cfdna-2.1.1/cfdna/tools/nucleosome/wps_functions.py
+-rwxr-xr-x   0        0        0      162 2022-07-20 16:09:08.000000 cfdna-2.1.1/cfdna/tools/summarize/__init__.py
+-rw-r--r--   0        0        0     3551 2022-08-30 19:26:15.000000 cfdna-2.1.1/cfdna/tools/summarize/multi_sample.py
+-rwxr-xr-x   0        0        0     3417 2023-11-06 18:46:14.639312 cfdna-2.1.1/cfdna/tools/summarize/summarize.py
+-rwxr-xr-x   0        0        0      143 2022-07-20 16:09:09.000000 cfdna-2.1.1/cfdna/utilities/__init__.py
+-rwxr-xr-x   0        0        0     4289 2022-08-30 19:22:16.000000 cfdna-2.1.1/cfdna/utilities/h5_utilities.py
+-rw-r--r--   0        0        0     2474 2024-05-15 18:27:26.456858 cfdna-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 cfdna-2.1.1/PKG-INFO
```

### Comparing `cfdna-2.1.0/LICENSE.md` & `cfdna-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/README.md` & `cfdna-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/.DS_Store` & `cfdna-2.1.1/cfdna/.DS_Store`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/__init__.py` & `cfdna-2.1.1/cfdna/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from . import commandline as cmd
 from . import tools as tl
 
 from ngsfragments import Fragments
 
 
 # This is extracted automatically by the top-level setup.py.
-__version__ = '2.0.8'
+__version__ = '2.1.1'
 
 __author__ = "Kyle S. Smith"
 
 __doc__ = """\
 
 API
 ======
```

### Comparing `cfdna-2.1.0/cfdna/__main__.py` & `cfdna-2.1.1/cfdna/__main__.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/commandline/commands.py` & `cfdna-2.1.1/cfdna/commandline/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,33 +53,33 @@
                                                                 genome_version=args.genome,
                                                                 cnv_binsize=args.bin_size,
                                                                 hmm_binsize=args.hmm_bin_size,
                                                                 nthreads = nthreads,
                                                                 use_normal = args.use_normal,
                                                                 keep_sex_chroms = args.add_sex,
                                                                 normal = [0.1, 0.25, 0.5, 0.75, 0.9],
-                                                                ploidy = [1,2,3],
+                                                                ploidy = [2,3],
                                                                 estimatePloidy = True,
                                                                 scStates = [1, 3],
-                                                                minSegmentBins = 50,
+                                                                minSegmentBins = 25,
                                                                 maxCN = 5)
             else:
                 cfdna_object = ngs.segment.cnv_pipeline.call_cnv_pipeline(cfdna_object,
                                                             frags,
                                                             genome_version=args.genome,
                                                             cnv_binsize=args.bin_size,
                                                             hmm_binsize=args.hmm_bin_size,
                                                             nthreads = nthreads,
                                                             use_normal = args.use_normal,
                                                             keep_sex_chroms = args.add_sex,
                                                             normal = [0.1, 0.25, 0.5, 0.75, 0.9],
-                                                            ploidy = [1,2,3],
+                                                            ploidy = [2,3],
                                                             estimatePloidy = True,
                                                             scStates = None,
-                                                            minSegmentBins = 50,
+                                                            minSegmentBins = 25,
                                                             maxCN = 5)
             
             # Add WPS
             if args.add_wps:
                 scores = ngs.metrics.wps_windows(frags,
                                                 protection = 120,
                                                 min_length = args.min_length,
```

### Comparing `cfdna-2.1.0/cfdna/core/core.py` & `cfdna-2.1.1/cfdna/core/core.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/io/.DS_Store` & `cfdna-2.1.1/cfdna/io/.DS_Store`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/io/read/read_bam.py` & `cfdna-2.1.1/cfdna/io/read/read_bam.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/io/write/write_text.py` & `cfdna-2.1.1/cfdna/io/write/write_text.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/plot/plot_bokeh.py` & `cfdna-2.1.1/cfdna/plot/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/plot/plot_plt.py` & `cfdna-2.1.1/cfdna/plot/plot_plt.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/cnv/segmentation.py` & `cfdna-2.1.1/cfdna/tools/cnv/segmentation.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/coverage/gene_activity.py` & `cfdna-2.1.1/cfdna/tools/coverage/gene_activity.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/fragmentation/frag_pattern.py` & `cfdna-2.1.1/cfdna/tools/fragmentation/frag_pattern.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/nucleosome/gene_activity.py` & `cfdna-2.1.1/cfdna/tools/nucleosome/gene_activity.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/nucleosome/nfr.py` & `cfdna-2.1.1/cfdna/tools/nucleosome/nfr.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/nucleosome/relative_window.py` & `cfdna-2.1.1/cfdna/tools/nucleosome/relative_window.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/nucleosome/wps.py` & `cfdna-2.1.1/cfdna/tools/nucleosome/wps.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/nucleosome/wps_functions.py` & `cfdna-2.1.1/cfdna/tools/nucleosome/wps_functions.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/summarize/multi_sample.py` & `cfdna-2.1.1/cfdna/tools/summarize/multi_sample.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/tools/summarize/summarize.py` & `cfdna-2.1.1/cfdna/tools/summarize/summarize.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/cfdna/utilities/h5_utilities.py` & `cfdna-2.1.1/cfdna/utilities/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `cfdna-2.1.0/pyproject.toml` & `cfdna-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cfdna"
-version = "2.1.0"
+version = "2.1.1"
 description = "Python package for fragment manipulation for cfDNA"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/cfdna"
 documentation = "https://www.biosciencestack.com/static/cfdna/docs/index.html"
 keywords = ["cython", "interval", "cfdna", "c"]
 readme = 'README.md'
```

### Comparing `cfdna-2.1.0/PKG-INFO` & `cfdna-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdna
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python package for fragment manipulation for cfDNA
 Home-page: https://github.com/kylessmith/cfdna
 License: GPL-2.0-or-later
 Keywords: cython,interval,cfdna,c
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
```

