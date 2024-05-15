# Comparing `tmp/avclass-malicialab-2.8.7.tar.gz` & `tmp/avclass_malicialab-2.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avclass-malicialab-2.8.7.tar", last modified: Sun Jul 23 08:27:17 2023, max compression
+gzip compressed data, was "avclass_malicialab-2.8.8.tar", last modified: Wed May 15 09:18:31 2024, max compression
```

## Comparing `avclass-malicialab-2.8.7.tar` & `avclass_malicialab-2.8.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-23 08:27:17.977305 avclass-malicialab-2.8.7/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.7/LICENSE
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.7/MANIFEST.in
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-07-23 08:27:17.977305 avclass-malicialab-2.8.7/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.7/README.md
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-23 08:27:17.977305 avclass-malicialab-2.8.7/avclass/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.7/avclass/__init__.py
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    20596 2023-05-05 15:16:06.000000 avclass-malicialab-2.8.7/avclass/common.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-23 08:27:17.977305 avclass-malicialab-2.8.7/avclass/data/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.7/avclass/data/andropup.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-07-20 10:20:10.000000 avclass-malicialab-2.8.7/avclass/data/default.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    56816 2023-07-23 08:23:32.000000 avclass-malicialab-2.8.7/avclass/data/default.tagging
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    41799 2023-07-23 08:23:32.000000 avclass-malicialab-2.8.7/avclass/data/default.taxonomy
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.7/avclass/evaluate.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23609 2023-05-26 13:02:48.000000 avclass-malicialab-2.8.7/avclass/labeler.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.7/avclass/misp.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.7/avclass/normalize.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.7/avclass/update.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-23 08:27:17.977305 avclass-malicialab-2.8.7/avclass_malicialab.egg-info/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-07-23 08:27:17.000000 avclass-malicialab-2.8.7/avclass_malicialab.egg-info/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-07-23 08:27:17.000000 avclass-malicialab-2.8.7/avclass_malicialab.egg-info/SOURCES.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-07-23 08:27:17.000000 avclass-malicialab-2.8.7/avclass_malicialab.egg-info/dependency_links.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-07-23 08:27:17.000000 avclass-malicialab-2.8.7/avclass_malicialab.egg-info/entry_points.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-07-23 08:27:17.000000 avclass-malicialab-2.8.7/avclass_malicialab.egg-info/top_level.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-07-23 08:26:29.000000 avclass-malicialab-2.8.7/pyproject.toml
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-07-23 08:27:17.977305 avclass-malicialab-2.8.7/setup.cfg
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2024-05-15 09:18:31.295905 avclass_malicialab-2.8.8/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass_malicialab-2.8.8/LICENSE
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass_malicialab-2.8.8/MANIFEST.in
+-rw-r--r--   0 juanca    (1000) juanca    (1000)    17117 2024-05-15 09:18:31.295905 avclass_malicialab-2.8.8/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass_malicialab-2.8.8/README.md
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2024-05-15 09:18:31.295905 avclass_malicialab-2.8.8/avclass/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass_malicialab-2.8.8/avclass/__init__.py
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    20596 2023-05-05 15:16:06.000000 avclass_malicialab-2.8.8/avclass/common.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2024-05-15 09:18:31.295905 avclass_malicialab-2.8.8/avclass/data/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass_malicialab-2.8.8/avclass/data/andropup.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-07-20 10:20:10.000000 avclass_malicialab-2.8.8/avclass/data/default.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    56816 2024-03-04 10:57:03.000000 avclass_malicialab-2.8.8/avclass/data/default.tagging
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    41799 2024-03-04 10:57:03.000000 avclass_malicialab-2.8.8/avclass/data/default.taxonomy
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass_malicialab-2.8.8/avclass/evaluate.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23715 2024-05-15 09:13:33.000000 avclass_malicialab-2.8.8/avclass/labeler.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass_malicialab-2.8.8/avclass/misp.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass_malicialab-2.8.8/avclass/normalize.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass_malicialab-2.8.8/avclass/update.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2024-05-15 09:18:31.295905 avclass_malicialab-2.8.8/avclass_malicialab.egg-info/
+-rw-r--r--   0 juanca    (1000) juanca    (1000)    17117 2024-05-15 09:18:31.000000 avclass_malicialab-2.8.8/avclass_malicialab.egg-info/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2024-05-15 09:18:31.000000 avclass_malicialab-2.8.8/avclass_malicialab.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2024-05-15 09:18:31.000000 avclass_malicialab-2.8.8/avclass_malicialab.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2024-05-15 09:18:31.000000 avclass_malicialab-2.8.8/avclass_malicialab.egg-info/entry_points.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2024-05-15 09:18:31.000000 avclass_malicialab-2.8.8/avclass_malicialab.egg-info/top_level.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2024-05-15 09:14:09.000000 avclass_malicialab-2.8.8/pyproject.toml
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2024-05-15 09:18:31.295905 avclass_malicialab-2.8.8/setup.cfg
```

### Comparing `avclass-malicialab-2.8.7/LICENSE` & `avclass_malicialab-2.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/PKG-INFO` & `avclass_malicialab-2.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.7
+Version: 2.8.8
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.7/README.md` & `avclass_malicialab-2.8.8/README.md`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/avclass/common.py` & `avclass_malicialab-2.8.8/avclass/common.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/avclass/data/andropup.expansion` & `avclass_malicialab-2.8.8/avclass/data/andropup.expansion`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/avclass/data/default.tagging` & `avclass_malicialab-2.8.8/avclass/data/default.tagging`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/avclass/data/default.taxonomy` & `avclass_malicialab-2.8.8/avclass/data/default.taxonomy`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/avclass/evaluate.py` & `avclass_malicialab-2.8.8/avclass/evaluate.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/avclass/labeler.py` & `avclass_malicialab-2.8.8/avclass/labeler.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,16 +475,19 @@
         frac = float(num_tagged) / float(num_samples) * 100
         fd.write('Tagged (all): %d (%.01f%%)\n' % (num_tagged, frac))
         num_maltagged = self.stats['maltagged']
         frac = float(num_maltagged) / float(num_samples) * 100
         fd.write('Tagged (VT>3): %d (%.01f%%)\n' % (num_maltagged, frac))
         for c in ['FILE','CLASS','BEH','FAM','UNK']:
             count = self.stats[c]
-            frac = float(count) / float(num_maltagged) * 100
-            fd.write('%s: %d (%.01f%%)\n' % (c, self.stats[c], frac))
+            if num_maltagged > 0:
+                frac = float(count) / float(num_maltagged) * 100
+                fd.write('%s: %d (%.01f%%)\n' % (c, count, frac))
+            else:
+                fd.write('%s: %d (-)\n' % (c, count))
         fd.close()
 
     def output_vendor_info(self, filepath):
         fd = open(filepath, 'w')
         for t in sorted(self.avtags_dict.keys()):
             fd.write('%s\t' % t)
             pairs = sorted(self.avtags_dict[t].items(),
```

### Comparing `avclass-malicialab-2.8.7/avclass/misp.py` & `avclass_malicialab-2.8.8/avclass/misp.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/avclass/normalize.py` & `avclass_malicialab-2.8.8/avclass/normalize.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/avclass/update.py` & `avclass_malicialab-2.8.8/avclass/update.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.7/avclass_malicialab.egg-info/PKG-INFO` & `avclass_malicialab-2.8.8/avclass_malicialab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.7
+Version: 2.8.8
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.7/pyproject.toml` & `avclass_malicialab-2.8.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avclass-malicialab"
-version = "2.8.7"
+version = "2.8.8"
 description = "AVClass is a Python package and command line tool to tag / label malware samples."
 readme = "README.md"
 authors = [{ name = "MaliciaLab" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

