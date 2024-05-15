# Comparing `tmp/cmsml-0.2.5.tar.gz` & `tmp/cmsml-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmsml-0.2.5.tar", last modified: Wed Mar 27 15:09:40 2024, max compression
+gzip compressed data, was "cmsml-0.2.6.tar", last modified: Wed May 15 16:30:02 2024, max compression
```

## Comparing `cmsml-0.2.5.tar` & `cmsml-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:09:40.989501 cmsml-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-27 15:09:28.000000 cmsml-0.2.5/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-27 15:09:28.000000 cmsml-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-27 15:09:28.000000 cmsml-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-03-27 15:09:40.989501 cmsml-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-27 15:09:28.000000 cmsml-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:09:40.985501 cmsml-0.2.5/cmsml/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/__meta__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:09:40.985501 cmsml-0.2.5/cmsml/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/keras/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/lazy_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:09:40.985501 cmsml-0.2.5/cmsml/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/scripts/check_aot_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/scripts/compile_tf_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/scripts/open_tf_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:09:40.985501 cmsml-0.2.5/cmsml/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/tensorflow/aot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/tensorflow/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-03-27 15:09:28.000000 cmsml-0.2.5/cmsml/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:09:40.985501 cmsml-0.2.5/cmsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-03-27 15:09:40.000000 cmsml-0.2.5/cmsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-27 15:09:40.000000 cmsml-0.2.5/cmsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:09:40.000000 cmsml-0.2.5/cmsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-27 15:09:40.000000 cmsml-0.2.5/cmsml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-27 15:09:40.000000 cmsml-0.2.5/cmsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 15:09:40.000000 cmsml-0.2.5/cmsml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-27 15:09:28.000000 cmsml-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-27 15:09:28.000000 cmsml-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-27 15:09:28.000000 cmsml-0.2.5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:09:40.989501 cmsml-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:30:02.928198 cmsml-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 16:29:50.000000 cmsml-0.2.6/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-15 16:29:50.000000 cmsml-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 16:29:50.000000 cmsml-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-15 16:30:02.928198 cmsml-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-15 16:29:50.000000 cmsml-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:30:02.924198 cmsml-0.2.6/cmsml/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/__meta__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:30:02.924198 cmsml-0.2.6/cmsml/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/keras/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/lazy_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:30:02.924198 cmsml-0.2.6/cmsml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/scripts/check_aot_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/scripts/compile_tf_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/scripts/open_tf_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:30:02.924198 cmsml-0.2.6/cmsml/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/tensorflow/aot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/tensorflow/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-05-15 16:29:50.000000 cmsml-0.2.6/cmsml/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:30:02.924198 cmsml-0.2.6/cmsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-15 16:30:02.000000 cmsml-0.2.6/cmsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 16:30:02.000000 cmsml-0.2.6/cmsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:30:02.000000 cmsml-0.2.6/cmsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-15 16:30:02.000000 cmsml-0.2.6/cmsml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-15 16:30:02.000000 cmsml-0.2.6/cmsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 16:30:02.000000 cmsml-0.2.6/cmsml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-15 16:29:50.000000 cmsml-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 16:29:50.000000 cmsml-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 16:29:50.000000 cmsml-0.2.6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:30:02.928198 cmsml-0.2.6/setup.cfg
```

### Comparing `cmsml-0.2.5/LICENSE` & `cmsml-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/PKG-INFO` & `cmsml-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsml
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python package of the CMS Machine Learning Group
 Author-email: Marcel Rieger <marcel.rieger@cern.ch>
 License: Copyright (c) 2020 - 2023, CMS Machine Learning Group
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmsml Version: 0.2.5 Summary: Python package of the
+Metadata-Version: 2.1 Name: cmsml Version: 0.2.6 Summary: Python package of the
 CMS Machine Learning Group Author-email: Marcel Rieger
 cern.ch> License: Copyright (c) 2020 - 2023, CMS Machine Learning Group All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. * Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
```

### Comparing `cmsml-0.2.5/README.md` & `cmsml-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/cmsml/keras/callbacks.py` & `cmsml-0.2.6/cmsml/keras/callbacks.py`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/cmsml/lazy_loader.py` & `cmsml-0.2.6/cmsml/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/cmsml/scripts/check_aot_compatibility.py` & `cmsml-0.2.6/cmsml/scripts/check_aot_compatibility.py`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/cmsml/scripts/compile_tf_graph.py` & `cmsml-0.2.6/cmsml/scripts/compile_tf_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,21 +149,21 @@
     # ammend the env when xla flags were passed
     env = os.environ.copy()
     if xla_flags:
         xla_flags = make_list(xla_flags)
         xla_flags_orig = env.get("XLA_FLAGS", "")
         if xla_flags_orig:
             xla_flags = [xla_flags_orig.rstrip(",")] + xla_flags
-        env["XLA_FLAGS"] = ",".join(map(str, xla_flags))
+        env["XLA_FLAGS"] = " ".join(map(str, xla_flags))
     if tf_xla_flags:
         tf_xla_flags = make_list(tf_xla_flags)
         tf_xla_flags_orig = env.get("TF_XLA_FLAGS", "")
         if tf_xla_flags_orig:
             tf_xla_flags = [tf_xla_flags_orig.rstrip(",")] + tf_xla_flags
-        env["TF_XLA_FLAGS"] = ",".join(map(str, tf_xla_flags))
+        env["TF_XLA_FLAGS"] = " ".join(map(str, tf_xla_flags))
 
     # prepare additional flags
     additional_flags_str = " ".join(make_list(additional_flags)) if additional_flags else ""
 
     # compile for each batch size
     for bs in sorted(set(map(int, batch_sizes))):
         cmd = (
```

### Comparing `cmsml-0.2.5/cmsml/scripts/open_tf_graph.py` & `cmsml-0.2.6/cmsml/scripts/open_tf_graph.py`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/cmsml/tensorflow/__init__.py` & `cmsml-0.2.6/cmsml/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/cmsml/tensorflow/aot.py` & `cmsml-0.2.6/cmsml/tensorflow/aot.py`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/cmsml/tensorflow/tools.py` & `cmsml-0.2.6/cmsml/tensorflow/tools.py`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/cmsml/util.py` & `cmsml-0.2.6/cmsml/util.py`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/cmsml.egg-info/PKG-INFO` & `cmsml-0.2.6/cmsml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsml
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python package of the CMS Machine Learning Group
 Author-email: Marcel Rieger <marcel.rieger@cern.ch>
 License: Copyright (c) 2020 - 2023, CMS Machine Learning Group
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmsml Version: 0.2.5 Summary: Python package of the
+Metadata-Version: 2.1 Name: cmsml Version: 0.2.6 Summary: Python package of the
 CMS Machine Learning Group Author-email: Marcel Rieger
 cern.ch> License: Copyright (c) 2020 - 2023, CMS Machine Learning Group All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. * Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
```

### Comparing `cmsml-0.2.5/cmsml.egg-info/SOURCES.txt` & `cmsml-0.2.6/cmsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmsml-0.2.5/pyproject.toml` & `cmsml-0.2.6/pyproject.toml`

 * *Files identical despite different names*

