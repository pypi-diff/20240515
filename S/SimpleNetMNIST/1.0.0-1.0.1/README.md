# Comparing `tmp/simplenetmnist-1.0.0.tar.gz` & `tmp/simplenetmnist-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplenetmnist-1.0.0.tar", last modified: Tue May 14 20:19:56 2024, max compression
+gzip compressed data, was "simplenetmnist-1.0.1.tar", last modified: Wed May 15 02:55:09 2024, max compression
```

## Comparing `simplenetmnist-1.0.0.tar` & `simplenetmnist-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-14 20:19:56.652284 simplenetmnist-1.0.0/
--rw-r--r--   0 dane      (1000) dane      (1000)     1066 2024-03-16 20:05:16.000000 simplenetmnist-1.0.0/LICENSE
--rw-r--r--   0 dane      (1000) dane      (1000)     2147 2024-05-14 20:19:56.652284 simplenetmnist-1.0.0/PKG-INFO
--rw-r--r--   0 dane      (1000) dane      (1000)      219 2024-03-16 20:05:16.000000 simplenetmnist-1.0.0/README.md
-drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-14 20:19:56.652284 simplenetmnist-1.0.0/SimpleNetMNIST/
--rw-r--r--   0 dane      (1000) dane      (1000)     3114 2024-03-16 20:05:16.000000 simplenetmnist-1.0.0/SimpleNetMNIST/predict.py
--rw-r--r--   0 dane      (1000) dane      (1000)     6959 2024-03-18 17:07:44.000000 simplenetmnist-1.0.0/SimpleNetMNIST/simpnet.py
--rw-r--r--   0 dane      (1000) dane      (1000)     4634 2024-03-16 20:05:16.000000 simplenetmnist-1.0.0/SimpleNetMNIST/train.py
--rw-r--r--   0 dane      (1000) dane      (1000)     1592 2024-03-16 20:05:16.000000 simplenetmnist-1.0.0/SimpleNetMNIST/utils.py
-drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-14 20:19:56.652284 simplenetmnist-1.0.0/SimpleNetMNIST.egg-info/
--rw-r--r--   0 dane      (1000) dane      (1000)     2147 2024-05-14 20:19:56.000000 simplenetmnist-1.0.0/SimpleNetMNIST.egg-info/PKG-INFO
--rw-r--r--   0 dane      (1000) dane      (1000)      330 2024-05-14 20:19:56.000000 simplenetmnist-1.0.0/SimpleNetMNIST.egg-info/SOURCES.txt
--rw-r--r--   0 dane      (1000) dane      (1000)        1 2024-05-14 20:19:56.000000 simplenetmnist-1.0.0/SimpleNetMNIST.egg-info/dependency_links.txt
--rw-r--r--   0 dane      (1000) dane      (1000)       13 2024-05-14 20:19:56.000000 simplenetmnist-1.0.0/SimpleNetMNIST.egg-info/requires.txt
--rw-r--r--   0 dane      (1000) dane      (1000)       15 2024-05-14 20:19:56.000000 simplenetmnist-1.0.0/SimpleNetMNIST.egg-info/top_level.txt
--rw-r--r--   0 dane      (1000) dane      (1000)      830 2024-05-14 20:10:14.000000 simplenetmnist-1.0.0/pyproject.toml
--rw-r--r--   0 dane      (1000) dane      (1000)       38 2024-05-14 20:19:56.652284 simplenetmnist-1.0.0/setup.cfg
--rw-r--r--   0 dane      (1000) dane      (1000)      160 2024-03-16 21:53:55.000000 simplenetmnist-1.0.0/setup.py
+drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-15 02:55:09.172152 simplenetmnist-1.0.1/
+-rw-r--r--   0 dane      (1000) dane      (1000)     1066 2024-03-16 20:05:16.000000 simplenetmnist-1.0.1/LICENSE
+-rw-r--r--   0 dane      (1000) dane      (1000)     2145 2024-05-15 02:55:09.172152 simplenetmnist-1.0.1/PKG-INFO
+-rw-r--r--   0 dane      (1000) dane      (1000)      219 2024-03-16 20:05:16.000000 simplenetmnist-1.0.1/README.md
+drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-15 02:55:09.172152 simplenetmnist-1.0.1/SimpleNetMNIST/
+-rw-r--r--   0 dane      (1000) dane      (1000)     3114 2024-03-16 20:05:16.000000 simplenetmnist-1.0.1/SimpleNetMNIST/predict.py
+-rw-r--r--   0 dane      (1000) dane      (1000)     6959 2024-03-18 17:07:44.000000 simplenetmnist-1.0.1/SimpleNetMNIST/simpnet.py
+-rw-r--r--   0 dane      (1000) dane      (1000)     4634 2024-03-16 20:05:16.000000 simplenetmnist-1.0.1/SimpleNetMNIST/train.py
+-rw-r--r--   0 dane      (1000) dane      (1000)     1592 2024-03-16 20:05:16.000000 simplenetmnist-1.0.1/SimpleNetMNIST/utils.py
+drwxr-xr-x   0 dane      (1000) dane      (1000)        0 2024-05-15 02:55:09.172152 simplenetmnist-1.0.1/SimpleNetMNIST.egg-info/
+-rw-r--r--   0 dane      (1000) dane      (1000)     2145 2024-05-15 02:55:09.000000 simplenetmnist-1.0.1/SimpleNetMNIST.egg-info/PKG-INFO
+-rw-r--r--   0 dane      (1000) dane      (1000)      330 2024-05-15 02:55:09.000000 simplenetmnist-1.0.1/SimpleNetMNIST.egg-info/SOURCES.txt
+-rw-r--r--   0 dane      (1000) dane      (1000)        1 2024-05-15 02:55:09.000000 simplenetmnist-1.0.1/SimpleNetMNIST.egg-info/dependency_links.txt
+-rw-r--r--   0 dane      (1000) dane      (1000)       11 2024-05-15 02:55:09.000000 simplenetmnist-1.0.1/SimpleNetMNIST.egg-info/requires.txt
+-rw-r--r--   0 dane      (1000) dane      (1000)       15 2024-05-15 02:55:09.000000 simplenetmnist-1.0.1/SimpleNetMNIST.egg-info/top_level.txt
+-rw-r--r--   0 dane      (1000) dane      (1000)      828 2024-05-15 02:54:55.000000 simplenetmnist-1.0.1/pyproject.toml
+-rw-r--r--   0 dane      (1000) dane      (1000)       38 2024-05-15 02:55:09.172152 simplenetmnist-1.0.1/setup.cfg
+-rw-r--r--   0 dane      (1000) dane      (1000)      160 2024-03-16 21:53:55.000000 simplenetmnist-1.0.1/setup.py
```

### Comparing `simplenetmnist-1.0.0/LICENSE` & `simplenetmnist-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.0/PKG-INFO` & `simplenetmnist-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleNetMNIST
-Version: 1.0.0
+Version: 1.0.1
 Summary: SimpleNetMNIST.  Based off an implementation of a simple neural network for MNIST classification in PyTorch. Created by Edward Ji (https://github.com/Edward-Ji).
 Author-email: Edward Ji <jiziao6@gmail.com>, Daniel Elliott <danelliottster@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Edward Ji
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: pytorch,mnist,neural network
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch>=2.2.1
+Requires-Dist: torch>=2.0
 
 ---
 title: SimpleNetMNSIT
 emoji: ✍️
 colorFrom: indigo
 colorTo: indigo
 sdk: gradio
```

### Comparing `simplenetmnist-1.0.0/SimpleNetMNIST/predict.py` & `simplenetmnist-1.0.1/SimpleNetMNIST/predict.py`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.0/SimpleNetMNIST/simpnet.py` & `simplenetmnist-1.0.1/SimpleNetMNIST/simpnet.py`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.0/SimpleNetMNIST/train.py` & `simplenetmnist-1.0.1/SimpleNetMNIST/train.py`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.0/SimpleNetMNIST/utils.py` & `simplenetmnist-1.0.1/SimpleNetMNIST/utils.py`

 * *Files identical despite different names*

### Comparing `simplenetmnist-1.0.0/SimpleNetMNIST.egg-info/PKG-INFO` & `simplenetmnist-1.0.1/SimpleNetMNIST.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleNetMNIST
-Version: 1.0.0
+Version: 1.0.1
 Summary: SimpleNetMNIST.  Based off an implementation of a simple neural network for MNIST classification in PyTorch. Created by Edward Ji (https://github.com/Edward-Ji).
 Author-email: Edward Ji <jiziao6@gmail.com>, Daniel Elliott <danelliottster@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Edward Ji
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: pytorch,mnist,neural network
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch>=2.2.1
+Requires-Dist: torch>=2.0
 
 ---
 title: SimpleNetMNSIT
 emoji: ✍️
 colorFrom: indigo
 colorTo: indigo
 sdk: gradio
```

### Comparing `simplenetmnist-1.0.0/pyproject.toml` & `simplenetmnist-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SimpleNetMNIST"
-version = "1.0.0"
+version = "1.0.1"
 description = "SimpleNetMNIST.  Based off an implementation of a simple neural network for MNIST classification in PyTorch. Created by Edward Ji (https://github.com/Edward-Ji)."
 authors = [ {name="Edward Ji", email="jiziao6@gmail.com"} , {name="Daniel Elliott", email="danelliottster@gmail.com"} ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["pytorch", "mnist", "neural network"]
 license = { file="LICENSE" }
 readme = "README.md"
 dependencies = [
-    "torch>=2.2.1"
+    "torch>=2.0"
 ]
 requires-python = ">=3.11"
 
 [project.urls]
 homepage = "https://github.com/danelliottster/SimpleNetMNIST"
```

