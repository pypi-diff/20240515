# Comparing `tmp/pydicomutils-0.1.3.tar.gz` & `tmp/pydicomutils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydicomutils-0.1.3.tar", last modified: Mon Dec 11 08:13:53 2023, max compression
+gzip compressed data, was "pydicomutils-0.2.1.tar", last modified: Wed May 15 08:44:41 2024, max compression
```

## Comparing `pydicomutils-0.1.3.tar` & `pydicomutils-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/
--rw-r--r--   0 da-for    (1000) da-for    (1000)     1061 2020-11-25 12:33:10.000000 pydicomutils-0.1.3/LICENSE
--rw-r--r--   0 da-for    (1000) da-for    (1000)       74 2023-01-02 09:43:09.000000 pydicomutils-0.1.3/MANIFEST.in
--rw-r--r--   0 da-for    (1000) da-for    (1000)     2665 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/PKG-INFO
--rw-r--r--   0 da-for    (1000) da-for    (1000)      547 2023-01-04 13:24:24.000000 pydicomutils-0.1.3/README.md
--rw-r--r--   0 da-for    (1000) da-for    (1000)     1496 2023-12-11 08:12:36.000000 pydicomutils-0.1.3/pyproject.toml
--rw-r--r--   0 da-for    (1000) da-for    (1000)       38 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/setup.cfg
--rw-r--r--   0 da-for    (1000) da-for    (1000)       56 2023-01-02 09:04:52.000000 pydicomutils-0.1.3/setup.py
-drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/src/
-drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/src/pydicomutils/
-drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/src/pydicomutils/IODs/
--rw-r--r--   0 da-for    (1000) da-for    (1000)     5712 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/BasicSRText.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     3887 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/CRImage.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)    11439 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/CSPS.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     4812 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/CTImage.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)    49960 2023-12-11 08:05:10.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/EnhancedSRTID1500.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)    17689 2023-12-11 07:50:44.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/EnhancedSRTID4300.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)    11592 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/GSPS.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     8231 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/IOD.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     6593 2021-03-04 16:03:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/KOS.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     4343 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/SCImage.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)    16717 2023-01-02 09:01:59.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/WSMImage.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/__init__.py
-drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/src/pydicomutils/IODs/modules/
--rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/modules/__init__.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     9043 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/modules/general_modules.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     3683 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/modules/specific_image_modules.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     1902 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/modules/specific_presentation_state_modules.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     2706 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/modules/specific_sr_modules.py
-drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/src/pydicomutils/IODs/sequences/
--rw-r--r--   0 da-for    (1000) da-for    (1000)    37002 2023-12-11 07:59:51.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/sequences/Sequences.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/IODs/sequences/__init__.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)       56 2023-12-11 08:12:36.000000 pydicomutils-0.1.3/src/pydicomutils/__init__.py
-drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/src/pydicomutils/external/
--rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/external/__init__.py
-drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/src/pydicomutils/external/icc_profiles/
--rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/external/icc_profiles/__init__.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)      319 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/external/icc_profiles/icc_profiles.py
--rw-r--r--   0 da-for    (1000) da-for    (1000)     3024 2020-11-25 12:33:11.000000 pydicomutils-0.1.3/src/pydicomutils/external/icc_profiles/sRGB2014.icc
-drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2023-12-11 08:13:53.307322 pydicomutils-0.1.3/src/pydicomutils.egg-info/
--rw-r--r--   0 da-for    (1000) da-for    (1000)     2665 2023-12-11 08:13:53.000000 pydicomutils-0.1.3/src/pydicomutils.egg-info/PKG-INFO
--rw-r--r--   0 da-for    (1000) da-for    (1000)     1243 2023-12-11 08:13:53.000000 pydicomutils-0.1.3/src/pydicomutils.egg-info/SOURCES.txt
--rw-r--r--   0 da-for    (1000) da-for    (1000)        1 2023-12-11 08:13:53.000000 pydicomutils-0.1.3/src/pydicomutils.egg-info/dependency_links.txt
--rw-r--r--   0 da-for    (1000) da-for    (1000)       68 2023-12-11 08:13:53.000000 pydicomutils-0.1.3/src/pydicomutils.egg-info/requires.txt
--rw-r--r--   0 da-for    (1000) da-for    (1000)       13 2023-12-11 08:13:53.000000 pydicomutils-0.1.3/src/pydicomutils.egg-info/top_level.txt
+drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2024-05-15 08:44:41.301875 pydicomutils-0.2.1/
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     1061 2020-11-25 12:33:10.000000 pydicomutils-0.2.1/LICENSE
+-rw-r--r--   0 da-for    (1000) da-for    (1000)       74 2023-01-02 09:43:09.000000 pydicomutils-0.2.1/MANIFEST.in
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     2665 2024-05-15 08:44:41.301875 pydicomutils-0.2.1/PKG-INFO
+-rw-r--r--   0 da-for    (1000) da-for    (1000)      547 2023-01-04 13:24:24.000000 pydicomutils-0.2.1/README.md
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     1496 2024-05-15 08:43:29.000000 pydicomutils-0.2.1/pyproject.toml
+-rw-r--r--   0 da-for    (1000) da-for    (1000)       38 2024-05-15 08:44:41.301875 pydicomutils-0.2.1/setup.cfg
+-rw-r--r--   0 da-for    (1000) da-for    (1000)       56 2023-01-02 09:04:52.000000 pydicomutils-0.2.1/setup.py
+drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2024-05-15 08:44:41.291875 pydicomutils-0.2.1/src/
+drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2024-05-15 08:44:41.291875 pydicomutils-0.2.1/src/pydicomutils/
+drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2024-05-15 08:44:41.301875 pydicomutils-0.2.1/src/pydicomutils/IODs/
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     5712 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/BasicSRText.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     3887 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/CRImage.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)    11439 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/CSPS.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     4812 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/CTImage.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)    23374 2024-05-15 08:05:52.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/Comprehensive3DSRTID1500.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)    49960 2023-12-11 08:05:10.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/EnhancedSRTID1500.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)    17689 2024-05-15 08:42:22.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/EnhancedSRTID4300.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)    11592 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/GSPS.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     8486 2024-05-14 17:42:48.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/IOD.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     6593 2021-03-04 16:03:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/KOS.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     4343 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/SCImage.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)    16717 2023-01-02 09:01:59.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/WSMImage.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/__init__.py
+drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2024-05-15 08:44:41.301875 pydicomutils-0.2.1/src/pydicomutils/IODs/modules/
+-rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/modules/__init__.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     9043 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/modules/general_modules.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     3683 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/modules/specific_image_modules.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     1902 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/modules/specific_presentation_state_modules.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     2706 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/modules/specific_sr_modules.py
+drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2024-05-15 08:44:41.301875 pydicomutils-0.2.1/src/pydicomutils/IODs/sequences/
+-rw-r--r--   0 da-for    (1000) da-for    (1000)    39851 2024-05-15 07:49:39.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/sequences/Sequences.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/IODs/sequences/__init__.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)       56 2024-05-15 08:43:29.000000 pydicomutils-0.2.1/src/pydicomutils/__init__.py
+drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2024-05-15 08:44:41.301875 pydicomutils-0.2.1/src/pydicomutils/external/
+-rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/external/__init__.py
+drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2024-05-15 08:44:41.301875 pydicomutils-0.2.1/src/pydicomutils/external/icc_profiles/
+-rw-r--r--   0 da-for    (1000) da-for    (1000)        0 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/external/icc_profiles/__init__.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)      319 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/external/icc_profiles/icc_profiles.py
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     3024 2020-11-25 12:33:11.000000 pydicomutils-0.2.1/src/pydicomutils/external/icc_profiles/sRGB2014.icc
+drwxr-xr-x   0 da-for    (1000) da-for    (1000)        0 2024-05-15 08:44:41.301875 pydicomutils-0.2.1/src/pydicomutils.egg-info/
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     2665 2024-05-15 08:44:41.000000 pydicomutils-0.2.1/src/pydicomutils.egg-info/PKG-INFO
+-rw-r--r--   0 da-for    (1000) da-for    (1000)     1293 2024-05-15 08:44:41.000000 pydicomutils-0.2.1/src/pydicomutils.egg-info/SOURCES.txt
+-rw-r--r--   0 da-for    (1000) da-for    (1000)        1 2024-05-15 08:44:41.000000 pydicomutils-0.2.1/src/pydicomutils.egg-info/dependency_links.txt
+-rw-r--r--   0 da-for    (1000) da-for    (1000)       68 2024-05-15 08:44:41.000000 pydicomutils-0.2.1/src/pydicomutils.egg-info/requires.txt
+-rw-r--r--   0 da-for    (1000) da-for    (1000)       13 2024-05-15 08:44:41.000000 pydicomutils-0.2.1/src/pydicomutils.egg-info/top_level.txt
```

### Comparing `pydicomutils-0.1.3/LICENSE` & `pydicomutils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/PKG-INFO` & `pydicomutils-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydicomutils
-Version: 0.1.3
+Version: 0.2.1
 Summary: Python library for creating DICOM objects
 Author-email: Daniel Forsberg <daniel.forsberg@sectra.com>
 License: Copyright 2020 Sectra AB
         
         Permission is hereby granted, free of charge, to any person obtaining 
         a copy of this software and associated documentation files (the "Software"), 
         to deal in the Software without restriction, including without limitation
```

### Comparing `pydicomutils-0.1.3/README.md` & `pydicomutils-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/pyproject.toml` & `pydicomutils-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pydicomutils"
-version = "0.1.3"
+version = "0.2.1"
 description = "Python library for creating DICOM objects"
 readme = "README.md"
 authors = [{ name = "Daniel Forsberg", email = "daniel.forsberg@sectra.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,15 +24,15 @@
 
     [project.urls]
     repository    = "https://github.com/sectra-medical/pydicomutils"
     documentation = "https://github.com/sectra-medical/pydicomutils"
 
 
 [tool.bumpver]
-current_version = "0.1.3"
+current_version = "0.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
     [tool.bumpver.file_patterns]
```

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/BasicSRText.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/BasicSRText.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/CRImage.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/CRImage.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/CSPS.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/CSPS.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/CTImage.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/CTImage.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/EnhancedSRTID1500.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/EnhancedSRTID1500.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/EnhancedSRTID4300.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/EnhancedSRTID4300.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/GSPS.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/GSPS.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/IOD.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/IOD.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 import random
 from datetime import datetime
 from enum import Enum
 
-from pydicom import Dataset, FileDataset, DataElement, Sequence, write_file, read_file, uid
+from pydicom import (
+    Dataset,
+    FileDataset,
+    DataElement,
+    Sequence,
+    write_file,
+    read_file,
+    uid,
+)
 from pydicom.datadict import tag_for_keyword, dictionary_VR
 
 from .modules.general_modules import PatientModule, GeneralStudyModule
-from .modules.general_modules import GeneralSeriesModule, GeneralEquipmentModule, EnhancedGeneralEquipmentModule
+from .modules.general_modules import (
+    GeneralSeriesModule,
+    GeneralEquipmentModule,
+    EnhancedGeneralEquipmentModule,
+)
 from .modules.general_modules import GeneralImageModule, ImagePixelModule
 from .modules.general_modules import SOPCommonModule
 from .sequences.Sequences import generate_sequence
 
+
 class IODTypes(Enum):
-    """Definition of different IODs and their corresponding SOP Class UIDs
-    """
-    CRImage =     "1.2.840.10008.5.1.4.1.1.1"
-    CTImage =     "1.2.840.10008.5.1.4.1.1.2"
-    SCImage =     "1.2.840.10008.5.1.4.1.1.7"
-    GSPS =        "1.2.840.10008.5.1.4.1.1.11.1"
-    CSPS =        "1.2.840.10008.5.1.4.1.1.11.2"
+    """Definition of different IODs and their corresponding SOP Class UIDs"""
+
+    CRImage = "1.2.840.10008.5.1.4.1.1.1"
+    CTImage = "1.2.840.10008.5.1.4.1.1.2"
+    SCImage = "1.2.840.10008.5.1.4.1.1.7"
+    GSPS = "1.2.840.10008.5.1.4.1.1.11.1"
+    CSPS = "1.2.840.10008.5.1.4.1.1.11.2"
     BasicTextSR = "1.2.840.10008.5.1.4.1.1.88.11"
-    EnhancedSR =  "1.2.840.10008.5.1.4.1.1.88.22"
-    KOS =         "1.2.840.10008.5.1.4.1.1.88.59"
-    WSMImage =    "1.2.840.10008.5.1.4.1.1.77.1.6"
+    EnhancedSR = "1.2.840.10008.5.1.4.1.1.88.22"
+    ComprehensiveSR = "1.2.840.10008.5.1.4.1.1.88.33"
+    Comprehensive3DSR = "1.2.840.10008.5.1.4.1.1.88.34"
+    KOS = "1.2.840.10008.5.1.4.1.1.88.59"
+    WSMImage = "1.2.840.10008.5.1.4.1.1.77.1.6"
+
 
 """Dictionary to go from SOPClassUID to Modality code
 """
 SOP_CLASS_UID_MODALITY_DICT = {
     IODTypes.CRImage: "CR",
     IODTypes.CTImage: "CT",
     IODTypes.SCImage: "SC",
     IODTypes.GSPS: "PR",
     IODTypes.CSPS: "PR",
     IODTypes.BasicTextSR: "SR",
     IODTypes.EnhancedSR: "SR",
+    IODTypes.ComprehensiveSR: "SR",
+    IODTypes.Comprehensive3DSR: "SR",
     IODTypes.KOS: "KO",
-    IODTypes.WSMImage: "SM"
+    IODTypes.WSMImage: "SM",
 }
 
+
 class IOD:
-    """Basic IOD class
-    """
+    """Basic IOD class"""
+
     iod_type = None
     dataset = None
 
     def __init__(self, iod_type):
         """
         Parameters
         ----------
@@ -72,108 +91,138 @@
         Parameters
         ----------
         keyword : Name of DICOM tag to set value for
         value : Value to set
         """
         if tag_for_keyword(keyword):
             if keyword in self.dataset:
-                if dictionary_VR(tag_for_keyword(keyword)) == "SQ" and isinstance(value, list):
+                if dictionary_VR(tag_for_keyword(keyword)) == "SQ" and isinstance(
+                    value, list
+                ):
                     value = generate_sequence(keyword, value)
                 self.dataset[tag_for_keyword(keyword)].value = value
             else:
-                if dictionary_VR(tag_for_keyword(keyword)) == "SQ" and isinstance(value, list):
+                if dictionary_VR(tag_for_keyword(keyword)) == "SQ" and isinstance(
+                    value, list
+                ):
                     value = generate_sequence(keyword, value)
-                de = DataElement(tag_for_keyword(keyword), 
-                                 dictionary_VR(tag_for_keyword(keyword)), 
-                                 value)
+                de = DataElement(
+                    tag_for_keyword(keyword),
+                    dictionary_VR(tag_for_keyword(keyword)),
+                    value,
+                )
                 self.dataset[tag_for_keyword(keyword)] = de
         else:
-            print("Keyword", keyword,"is an unknown DICOM attribute")
+            print("Keyword", keyword, "is an unknown DICOM attribute")
 
-    def copy_required_dicom_attributes(self, dataset_to_copy_from, 
-                                       include_optional=True):
+    def copy_required_dicom_attributes(
+        self, dataset_to_copy_from, include_optional=True
+    ):
         """Copies required DICOM attributes from provided dataset
         Parameters
         ----------
         dataset_to_copy_from : Dataset to copy DICOM attributes from
         include_optional : Include optional DICOM attributes in copy
         """
-        general_modules = [PatientModule(),
-                           GeneralStudyModule(),
-                           GeneralEquipmentModule(),
-                           SOPCommonModule()]
+        general_modules = [
+            PatientModule(),
+            GeneralStudyModule(),
+            GeneralEquipmentModule(),
+            SOPCommonModule(),
+        ]
         for module in general_modules:
-            module.copy_required_dicom_attributes(dataset_to_copy_from, 
-                                                  self.dataset)
+            module.copy_required_dicom_attributes(dataset_to_copy_from, self.dataset)
             if include_optional:
-                module.copy_optional_dicom_attributes(dataset_to_copy_from, 
-                                                      self.dataset)
+                module.copy_optional_dicom_attributes(
+                    dataset_to_copy_from, self.dataset
+                )
 
         if self.iod_type in [IODTypes.WSMImage]:
             general_modules = [EnhancedGeneralEquipmentModule()]
             for module in general_modules:
-                module.copy_required_dicom_attributes(dataset_to_copy_from, 
-                                                      self.dataset)
+                module.copy_required_dicom_attributes(
+                    dataset_to_copy_from, self.dataset
+                )
                 if include_optional:
-                    module.copy_optional_dicom_attributes(dataset_to_copy_from, 
-                                                          self.dataset)
-
-        if self.iod_type in [IODTypes.CRImage, IODTypes.CTImage, IODTypes.SCImage, IODTypes.WSMImage]:
-            general_image_modules = [GeneralImageModule(),
-                                     GeneralSeriesModule(),
-                                     ImagePixelModule()]
+                    module.copy_optional_dicom_attributes(
+                        dataset_to_copy_from, self.dataset
+                    )
+
+        if self.iod_type in [
+            IODTypes.CRImage,
+            IODTypes.CTImage,
+            IODTypes.SCImage,
+            IODTypes.WSMImage,
+        ]:
+            general_image_modules = [
+                GeneralImageModule(),
+                GeneralSeriesModule(),
+                ImagePixelModule(),
+            ]
             for module in general_image_modules:
-                module.copy_required_dicom_attributes(dataset_to_copy_from, 
-                                                      self.dataset)
+                module.copy_required_dicom_attributes(
+                    dataset_to_copy_from, self.dataset
+                )
                 if include_optional:
-                    module.copy_optional_dicom_attributes(dataset_to_copy_from, 
-                                                          self.dataset)
+                    module.copy_optional_dicom_attributes(
+                        dataset_to_copy_from, self.dataset
+                    )
 
         if self.iod_type in [IODTypes.GSPS, IODTypes.CSPS]:
             general_series_modules = [GeneralSeriesModule()]
             for module in general_series_modules:
-                module.copy_required_dicom_attributes(dataset_to_copy_from, 
-                                                    self.dataset)
+                module.copy_required_dicom_attributes(
+                    dataset_to_copy_from, self.dataset
+                )
                 if include_optional:
-                    module.copy_optional_dicom_attributes(dataset_to_copy_from, 
-                                                          self.dataset)
+                    module.copy_optional_dicom_attributes(
+                        dataset_to_copy_from, self.dataset
+                    )
 
     def initiate(self):
         """Initiate the IOD by setting some dummy values for
         required attributes
         """
         # patient module
-        self.dataset.PatientID = ''.join(random.choice('0123456789ABCDEF') for i in range(16))
+        self.dataset.PatientID = "".join(
+            random.choice("0123456789ABCDEF") for i in range(16)
+        )
         # general study module
         self.dataset.StudyInstanceUID = uid.generate_uid()
         self.dataset.StudyDate = datetime.now().strftime("%Y%m%d")
         self.dataset.StudyTime = datetime.now().strftime("%H%M%S")
-        self.dataset.StudyID = ''.join(random.choice('0123456789ABCDEF') for i in range(16))
+        self.dataset.StudyID = "".join(
+            random.choice("0123456789ABCDEF") for i in range(16)
+        )
         self.dataset.AccessionNumber = self.dataset.StudyID
         # sop common module
         self.dataset.SOPClassUID = self.iod_type.value
         self.dataset.SOPInstanceUID = uid.generate_uid()
 
-        if self.iod_type in [IODTypes.CRImage, IODTypes.CTImage, IODTypes.SCImage, IODTypes.WSMImage]:
+        if self.iod_type in [
+            IODTypes.CRImage,
+            IODTypes.CTImage,
+            IODTypes.SCImage,
+            IODTypes.WSMImage,
+        ]:
             # general series module
             self.dataset.Modality = SOP_CLASS_UID_MODALITY_DICT[self.iod_type]
             self.dataset.SeriesInstanceUID = uid.generate_uid()
             self.dataset.SeriesNumber = str(100)
             # general image module
             self.dataset.InstanceNumber = str(1)
             self.dataset.ContentDate = datetime.now().strftime("%Y%m%d")
             self.dataset.ContentTime = datetime.now().strftime("%H%M%S")
 
         if self.iod_type in [IODTypes.GSPS, IODTypes.CSPS]:
             # general series module
             self.dataset.Modality = SOP_CLASS_UID_MODALITY_DICT[self.iod_type]
             self.dataset.SeriesInstanceUID = uid.generate_uid()
             self.dataset.SeriesNumber = str(100)
-            
-        
+
     def write_to_file(self, output_file, write_like_original=False):
         """Writes the current IOD to file
         Parameters
         ----------
         output_file : Complete path of file to write to
         """
         write_file(output_file, self.dataset, write_like_original=write_like_original)
```

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/KOS.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/KOS.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/SCImage.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/SCImage.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/WSMImage.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/WSMImage.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/modules/general_modules.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/modules/general_modules.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/modules/specific_image_modules.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/modules/specific_image_modules.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/modules/specific_presentation_state_modules.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/modules/specific_presentation_state_modules.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/modules/specific_sr_modules.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/modules/specific_sr_modules.py`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils/IODs/sequences/Sequences.py` & `pydicomutils-0.2.1/src/pydicomutils/IODs/sequences/Sequences.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from pydicom import Sequence, Dataset, read_file, DataElement
 from pydicom.datadict import tag_for_keyword, dictionary_VM, dictionary_VR
 from pydicom.uid import generate_uid
 
 
 """Various definitions that can be of good use
 """
@@ -67,14 +69,102 @@
     "US": "Ultrasound",
     "VA": "Visual Acuity",
     "XA": "X-Ray Angiography",
     "XC": "External-camera Photography",
 }
 
 
+class ConceptNameCodeSequenceItem(object):
+    def __init__(
+        self, code_value: str, coding_scheme_designator: str, code_meaning: str
+    ):
+        self.CodeValue = code_value
+        self.CodingSchemeDesignator = coding_scheme_designator
+        self.CodeMeaning = code_meaning
+
+    def CodeValue(self):
+        return self.CodeValue
+
+    def CodingSchemeDesignator(self):
+        return self.CodingSchemeDesignator
+
+    def CodeMeaning(self):
+        return self.CodeMeaning
+
+    def __str__(self):
+        return f"CodeValue: {self.CodeValue}, CodingSchemeDesignator: {self.CodingSchemeDesignator}, CodeMeaning: {self.CodeMeaning}"
+
+    def __repr__(self):
+        return f"CodeValue: {self.CodeValue}, CodingSchemeDesignator: {self.CodingSchemeDesignator}, CodeMeaning: {self.CodeMeaning}"
+
+    def __eq__(self, other):
+        return (
+            self.CodeValue == other.CodeValue
+            and self.CodingSchemeDesignator == other.CodingSchemeDesignator
+            and self.CodeMeaning == other.CodeMeaning
+        )
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def as_dict(self):
+        return {
+            "CodeValue": self.CodeValue,
+            "CodingSchemeDesignator": self.CodingSchemeDesignator,
+            "CodeMeaning": self.CodeMeaning,
+        }
+
+    def as_json(self):
+        return json.dumps(self.as_dict())
+
+
+class ConceptCodeSequenceItem(object):
+    def __init__(
+        self, code_value: str, coding_scheme_designator: str, code_meaning: str
+    ):
+        self.CodeValue = code_value
+        self.CodingSchemeDesignator = coding_scheme_designator
+        self.CodeMeaning = code_meaning
+
+    def CodeValue(self):
+        return self.CodeValue
+
+    def CodingSchemeDesignator(self):
+        return self.CodingSchemeDesignator
+
+    def CodeMeaning(self):
+        return self.CodeMeaning
+
+    def __str__(self):
+        return f"CodeValue: {self.CodeValue}, CodingSchemeDesignator: {self.CodingSchemeDesignator}, CodeMeaning: {self.CodeMeaning}"
+
+    def __repr__(self):
+        return f"CodeValue: {self.CodeValue}, CodingSchemeDesignator: {self.CodingSchemeDesignator}, CodeMeaning: {self.CodeMeaning}"
+
+    def __eq__(self, other):
+        return (
+            self.CodeValue == other.CodeValue
+            and self.CodingSchemeDesignator == other.CodingSchemeDesignator
+            and self.CodeMeaning == other.CodeMeaning
+        )
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def as_dict(self):
+        return {
+            "CodeValue": self.CodeValue,
+            "CodingSchemeDesignator": self.CodingSchemeDesignator,
+            "CodeMeaning": self.CodeMeaning,
+        }
+
+    def as_json(self):
+        return json.dumps(self.as_dict())
+
+
 def update_and_insert_additional_DICOM_attributes_in_ds(ds, keyword_and_value_dict):
     # For every keyword
     for keyword in keyword_and_value_dict:
         # Get corresponding tag and value
         tag = tag_for_keyword(keyword)
         # Verify that it is a valid keyword
         if tag is None:
```

### Comparing `pydicomutils-0.1.3/src/pydicomutils/external/icc_profiles/sRGB2014.icc` & `pydicomutils-0.2.1/src/pydicomutils/external/icc_profiles/sRGB2014.icc`

 * *Files identical despite different names*

### Comparing `pydicomutils-0.1.3/src/pydicomutils.egg-info/PKG-INFO` & `pydicomutils-0.2.1/src/pydicomutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydicomutils
-Version: 0.1.3
+Version: 0.2.1
 Summary: Python library for creating DICOM objects
 Author-email: Daniel Forsberg <daniel.forsberg@sectra.com>
 License: Copyright 2020 Sectra AB
         
         Permission is hereby granted, free of charge, to any person obtaining 
         a copy of this software and associated documentation files (the "Software"), 
         to deal in the Software without restriction, including without limitation
```

### Comparing `pydicomutils-0.1.3/src/pydicomutils.egg-info/SOURCES.txt` & `pydicomutils-0.2.1/src/pydicomutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/pydicomutils.egg-info/dependency_links.txt
 src/pydicomutils.egg-info/requires.txt
 src/pydicomutils.egg-info/top_level.txt
 src/pydicomutils/IODs/BasicSRText.py
 src/pydicomutils/IODs/CRImage.py
 src/pydicomutils/IODs/CSPS.py
 src/pydicomutils/IODs/CTImage.py
+src/pydicomutils/IODs/Comprehensive3DSRTID1500.py
 src/pydicomutils/IODs/EnhancedSRTID1500.py
 src/pydicomutils/IODs/EnhancedSRTID4300.py
 src/pydicomutils/IODs/GSPS.py
 src/pydicomutils/IODs/IOD.py
 src/pydicomutils/IODs/KOS.py
 src/pydicomutils/IODs/SCImage.py
 src/pydicomutils/IODs/WSMImage.py
```

