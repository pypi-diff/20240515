# Comparing `tmp/yaml_designer-0.1.0.tar.gz` & `tmp/yaml_designer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_designer-0.1.0.tar", last modified: Tue May 14 22:00:22 2024, max compression
+gzip compressed data, was "yaml_designer-0.1.1.tar", last modified: Tue May 14 22:09:34 2024, max compression
```

## Comparing `yaml_designer-0.1.0.tar` & `yaml_designer-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-14 22:00:22.736161 yaml_designer-0.1.0/
--rw-r--r--   0 user      (1000) vboxusers   (136)     1493 2024-05-14 21:52:08.000000 yaml_designer-0.1.0/LICENSE
--rw-r--r--   0 user      (1000) vboxusers   (136)     3240 2024-05-14 22:00:22.736161 yaml_designer-0.1.0/PKG-INFO
--rw-r--r--   0 user      (1000) vboxusers   (136)      484 2024-05-14 21:52:55.000000 yaml_designer-0.1.0/README.rst
--rw-r--r--   0 user      (1000) vboxusers   (136)     1101 2024-05-14 22:00:10.000000 yaml_designer-0.1.0/pyproject.toml
--rw-r--r--   0 user      (1000) vboxusers   (136)       38 2024-05-14 22:00:22.736161 yaml_designer-0.1.0/setup.cfg
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-14 22:00:22.732161 yaml_designer-0.1.0/src/
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-14 22:00:22.732161 yaml_designer-0.1.0/src/yaml_designer/
--rw-r--r--   0 user      (1000) vboxusers   (136)        0 2024-05-14 21:12:50.000000 yaml_designer-0.1.0/src/yaml_designer/__init__.py
--rw-r--r--   0 user      (1000) vboxusers   (136)      801 2024-05-14 21:30:57.000000 yaml_designer-0.1.0/src/yaml_designer/yaml_designer.py
-drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-14 22:00:22.736161 yaml_designer-0.1.0/src/yaml_designer.egg-info/
--rw-r--r--   0 user      (1000) vboxusers   (136)     3240 2024-05-14 22:00:22.000000 yaml_designer-0.1.0/src/yaml_designer.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) vboxusers   (136)      302 2024-05-14 22:00:22.000000 yaml_designer-0.1.0/src/yaml_designer.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)        1 2024-05-14 22:00:22.000000 yaml_designer-0.1.0/src/yaml_designer.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-14 22:00:22.000000 yaml_designer-0.1.0/src/yaml_designer.egg-info/requires.txt
--rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-14 22:00:22.000000 yaml_designer-0.1.0/src/yaml_designer.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-14 22:09:34.721243 yaml_designer-0.1.1/
+-rw-r--r--   0 user      (1000) vboxusers   (136)     1493 2024-05-14 21:52:08.000000 yaml_designer-0.1.1/LICENSE
+-rw-r--r--   0 user      (1000) vboxusers   (136)     3240 2024-05-14 22:09:34.721243 yaml_designer-0.1.1/PKG-INFO
+-rw-r--r--   0 user      (1000) vboxusers   (136)      484 2024-05-14 21:52:55.000000 yaml_designer-0.1.1/README.rst
+-rw-r--r--   0 user      (1000) vboxusers   (136)     1165 2024-05-14 22:09:29.000000 yaml_designer-0.1.1/pyproject.toml
+-rw-r--r--   0 user      (1000) vboxusers   (136)       38 2024-05-14 22:09:34.721243 yaml_designer-0.1.1/setup.cfg
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-14 22:09:34.717243 yaml_designer-0.1.1/src/
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-14 22:09:34.717243 yaml_designer-0.1.1/src/yaml_designer/
+-rw-r--r--   0 user      (1000) vboxusers   (136)        0 2024-05-14 21:12:50.000000 yaml_designer-0.1.1/src/yaml_designer/__init__.py
+-rw-r--r--   0 user      (1000) vboxusers   (136)      801 2024-05-14 21:30:57.000000 yaml_designer-0.1.1/src/yaml_designer/yaml_designer.py
+drwxr-xr-x   0 user      (1000) vboxusers   (136)        0 2024-05-14 22:09:34.721243 yaml_designer-0.1.1/src/yaml_designer.egg-info/
+-rw-r--r--   0 user      (1000) vboxusers   (136)     3240 2024-05-14 22:09:34.000000 yaml_designer-0.1.1/src/yaml_designer.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) vboxusers   (136)      346 2024-05-14 22:09:34.000000 yaml_designer-0.1.1/src/yaml_designer.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)        1 2024-05-14 22:09:34.000000 yaml_designer-0.1.1/src/yaml_designer.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       62 2024-05-14 22:09:34.000000 yaml_designer-0.1.1/src/yaml_designer.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-14 22:09:34.000000 yaml_designer-0.1.1/src/yaml_designer.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) vboxusers   (136)       14 2024-05-14 22:09:34.000000 yaml_designer-0.1.1/src/yaml_designer.egg-info/top_level.txt
```

### Comparing `yaml_designer-0.1.0/LICENSE` & `yaml_designer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_designer-0.1.0/PKG-INFO` & `yaml_designer-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-designer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A plugin that allows users to dynamically create yaml classes and convert into a yaml file when done
 Author-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 Maintainer-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 License: 
         Copyright (c) 2024, Babak Michael Engheta
         All rights reserved.
```

### Comparing `yaml_designer-0.1.0/pyproject.toml` & `yaml_designer-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [project]
 name = "yaml-designer"
 description = "A plugin that allows users to dynamically create yaml classes and convert into a yaml file when done"
-version = "0.1.0"
+version = "0.1.1"
 readme = {file = "README.rst", content-type = "text/markdown"}
 requires-python = ">=3.8"
 authors = [
     { name = "Babak Michael Engheta", email = "michaelengheta55@gmail.com" },
 ]
 maintainers = [
     { name = "Babak Michael Engheta", email = "michaelengheta55@gmail.com" },
@@ -23,9 +23,11 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: BSD License",
 ]
 dependencies = [
     "pyyaml>=6.0.1",
 ]
+[project.scripts]
+yaml-designer = "yaml_designer.yaml_designer"
 [project.urls]
 Repository = "https://github.com/MichaelE55/yaml-designer"
```

### Comparing `yaml_designer-0.1.0/src/yaml_designer/yaml_designer.py` & `yaml_designer-0.1.1/src/yaml_designer/yaml_designer.py`

 * *Files identical despite different names*

### Comparing `yaml_designer-0.1.0/src/yaml_designer.egg-info/PKG-INFO` & `yaml_designer-0.1.1/src/yaml_designer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-designer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A plugin that allows users to dynamically create yaml classes and convert into a yaml file when done
 Author-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 Maintainer-email: Babak Michael Engheta <michaelengheta55@gmail.com>
 License: 
         Copyright (c) 2024, Babak Michael Engheta
         All rights reserved.
```

