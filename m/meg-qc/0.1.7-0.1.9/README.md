# Comparing `tmp/meg_qc-0.1.7.tar.gz` & `tmp/meg_qc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meg_qc-0.1.7.tar", last modified: Tue Apr 30 09:32:26 2024, max compression
+gzip compressed data, was "meg_qc-0.1.9.tar", last modified: Wed May 15 13:29:05 2024, max compression
```

## Comparing `meg_qc-0.1.7.tar` & `meg_qc-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.585735 meg_qc-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-30 09:32:16.000000 meg_qc-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-30 09:32:26.585735 meg_qc-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-30 09:32:16.000000 meg_qc-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.585735 meg_qc-0.1.7/meg_qc/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 09:32:26.585735 meg_qc-0.1.7/meg_qc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.581735 meg_qc-0.1.7/meg_qc/calculation/
--rw-r--r--   0 runner    (1001) docker     (127)    26343 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/initial_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/meg_qc_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.585735 meg_qc-0.1.7/meg_qc/calculation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)   112596 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/Head_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    53766 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/PSD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18689 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25659 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/STD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/calculation/metrics/muscle_meg_qc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.585735 meg_qc-0.1.7/meg_qc/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/plotting/meg_qc_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/plotting/universal_html_report.py
--rw-r--r--   0 runner    (1001) docker     (127)   130403 2024-04-30 09:32:16.000000 meg_qc-0.1.7/meg_qc/plotting/universal_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:32:26.581735 meg_qc-0.1.7/meg_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-30 09:32:26.000000 meg_qc-0.1.7/meg_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-30 09:32:26.000000 meg_qc-0.1.7/meg_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:32:26.000000 meg_qc-0.1.7/meg_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 09:32:26.000000 meg_qc-0.1.7/meg_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 09:32:16.000000 meg_qc-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-30 09:32:26.585735 meg_qc-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-30 09:32:16.000000 meg_qc-0.1.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-30 09:32:16.000000 meg_qc-0.1.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 13:28:51.000000 meg_qc-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-15 13:29:05.391676 meg_qc-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-15 13:28:51.000000 meg_qc-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.395676 meg_qc-0.1.9/meg_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 13:29:05.395676 meg_qc-0.1.9/meg_qc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/meg_qc/calculation/
+-rw-r--r--   0 runner    (1001) docker     (127)    26343 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/initial_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20755 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/meg_qc_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/meg_qc/calculation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)   112596 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/Head_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53766 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/PSD_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18689 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25659 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/STD_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/muscle_meg_qc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/meg_qc/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/plotting/meg_qc_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/plotting/universal_html_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130403 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/plotting/universal_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/meg_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-15 13:29:05.000000 meg_qc-0.1.9/meg_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 13:29:05.000000 meg_qc-0.1.9/meg_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:29:05.000000 meg_qc-0.1.9/meg_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 13:29:05.000000 meg_qc-0.1.9/meg_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 13:28:51.000000 meg_qc-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-15 13:29:05.395676 meg_qc-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-15 13:28:51.000000 meg_qc-0.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-05-15 13:28:51.000000 meg_qc-0.1.9/versioneer.py
```

### Comparing `meg_qc-0.1.7/LICENSE` & `meg_qc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/PKG-INFO` & `meg_qc-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meg_qc
-Version: 0.1.7
+Version: 0.1.9
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.1.7/README.md` & `meg_qc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/__main__.py` & `meg_qc-0.1.9/meg_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/calculation/initial_meg_qc.py` & `meg_qc-0.1.9/meg_qc/calculation/initial_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/calculation/meg_qc_pipeline.py` & `meg_qc-0.1.9/meg_qc/calculation/meg_qc_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         # entities = dataset.query_entities()
         # print('___MEGqc___: ', 'entities', entities)
 
         # list_of_subs = list(entities["sub"])
         if all_qc_params['default']['subjects'][0] != 'all':
             list_of_subs = all_qc_params['default']['subjects']
         elif all_qc_params['default']['subjects'][0] == 'all':
-            list_of_subs = sorted(list(dataset.query_entities()["sub"]))
+            list_of_subs = sorted(list(dataset.query_entities()["subject"]))
             print('___MEGqc___: ', 'list_of_subs', list_of_subs)
             if not list_of_subs:
                 print('___MEGqc___: ', 'No subjects found by ANCP BIDS. Check your data set and directory path in config.')
                 return
         else:
             print('___MEGqc___: ', 'Something went wrong with the subjects list. Check parameter "subjects" in config file or simply set it to "all".')
             return
@@ -124,15 +124,15 @@
         avg_eog=[]
 
         print('___MEGqc___: ', 'TOTAL subs', len(list_of_subs))
         print('___MEGqc___: ', 'EMPTY room?', sorted(list_of_subs)[0], sorted(list_of_subs)[-1])
         #list_of_subs = ['009', '012', '019', '020', '021', '022', '023', '024', '025'] #especially 23 in ds 83! There doesnt detect all the ecg peaks and says bad ch, but it s good.
         
         raw=None #preassign in case no calculation will be successful
-        for sid in list_of_subs[2:3]: #[0:4]: 
+        for sid in list_of_subs: #[0:4]: 
             print('___MEGqc___: ', 'Dataset: ', dataset_path)
             print('___MEGqc___: ', 'Take SID: ', sid)
             
             subject_folder = derivative.create_folder(type_=schema.Subject, name='sub-'+sid)
 
             list_of_fifs = sorted(list(dataset.query(suffix='meg', extension='.fif', return_type='filename', subj=sid)))
             print('___MEGqc___: ', 'list_of_fifs', list_of_fifs)
```

### Comparing `meg_qc-0.1.7/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py` & `meg_qc-0.1.9/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/calculation/metrics/Head_meg_qc.py` & `meg_qc-0.1.9/meg_qc/calculation/metrics/Head_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/calculation/metrics/PSD_meg_qc.py` & `meg_qc-0.1.9/meg_qc/calculation/metrics/PSD_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py` & `meg_qc-0.1.9/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py` & `meg_qc-0.1.9/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/calculation/metrics/STD_meg_qc.py` & `meg_qc-0.1.9/meg_qc/calculation/metrics/STD_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/calculation/metrics/muscle_meg_qc.py` & `meg_qc-0.1.9/meg_qc/calculation/metrics/muscle_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/plotting/meg_qc_plots.py` & `meg_qc-0.1.9/meg_qc/plotting/meg_qc_plots.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/plotting/universal_html_report.py` & `meg_qc-0.1.9/meg_qc/plotting/universal_html_report.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc/plotting/universal_plots.py` & `meg_qc-0.1.9/meg_qc/plotting/universal_plots.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/meg_qc.egg-info/PKG-INFO` & `meg_qc-0.1.9/meg_qc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meg-qc
-Version: 0.1.7
+Version: 0.1.9
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.1.7/meg_qc.egg-info/SOURCES.txt` & `meg_qc-0.1.9/meg_qc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/setup.cfg` & `meg_qc-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/setup.py` & `meg_qc-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.7/versioneer.py` & `meg_qc-0.1.9/versioneer.py`

 * *Files identical despite different names*

