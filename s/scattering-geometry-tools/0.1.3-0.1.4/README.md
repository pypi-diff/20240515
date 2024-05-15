# Comparing `tmp/scattering-geometry-tools-0.1.3.tar.gz` & `tmp/scattering-geometry-tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scattering-geometry-tools-0.1.3.tar", last modified: Wed May  3 04:48:40 2023, max compression
+gzip compressed data, was "scattering-geometry-tools-0.1.4.tar", last modified: Wed May 15 13:48:52 2024, max compression
```

## Comparing `scattering-geometry-tools-0.1.3.tar` & `scattering-geometry-tools-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 snaka      (501) staff       (20)        0 2023-05-03 04:48:40.800397 scattering-geometry-tools-0.1.3/
--rw-r--r--   0 snaka      (501) staff       (20)     1066 2022-08-19 02:56:27.000000 scattering-geometry-tools-0.1.3/LICENSE
--rw-r--r--   0 snaka      (501) staff       (20)     1833 2023-05-03 04:48:40.800114 scattering-geometry-tools-0.1.3/PKG-INFO
--rw-r--r--   0 snaka      (501) staff       (20)      124 2022-12-12 14:20:07.000000 scattering-geometry-tools-0.1.3/README.md
--rw-r--r--   0 snaka      (501) staff       (20)      700 2023-05-03 04:47:05.000000 scattering-geometry-tools-0.1.3/pyproject.toml
--rw-r--r--   0 snaka      (501) staff       (20)       38 2023-05-03 04:48:40.800463 scattering-geometry-tools-0.1.3/setup.cfg
--rw-r--r--   0 snaka      (501) staff       (20)      433 2022-12-05 13:44:09.000000 scattering-geometry-tools-0.1.3/setup.py
-drwxr-xr-x   0 snaka      (501) staff       (20)        0 2023-05-03 04:48:40.790861 scattering-geometry-tools-0.1.3/src/
-drwxr-xr-x   0 snaka      (501) staff       (20)        0 2023-05-03 04:48:40.794429 scattering-geometry-tools-0.1.3/src/scattering_geometry_tools.egg-info/
--rw-r--r--   0 snaka      (501) staff       (20)     1833 2023-05-03 04:48:40.000000 scattering-geometry-tools-0.1.3/src/scattering_geometry_tools.egg-info/PKG-INFO
--rw-r--r--   0 snaka      (501) staff       (20)      519 2023-05-03 04:48:40.000000 scattering-geometry-tools-0.1.3/src/scattering_geometry_tools.egg-info/SOURCES.txt
--rw-r--r--   0 snaka      (501) staff       (20)        1 2023-05-03 04:48:40.000000 scattering-geometry-tools-0.1.3/src/scattering_geometry_tools.egg-info/dependency_links.txt
--rw-r--r--   0 snaka      (501) staff       (20)       25 2023-05-03 04:48:40.000000 scattering-geometry-tools-0.1.3/src/scattering_geometry_tools.egg-info/requires.txt
--rw-r--r--   0 snaka      (501) staff       (20)        4 2023-05-03 04:48:40.000000 scattering-geometry-tools-0.1.3/src/scattering_geometry_tools.egg-info/top_level.txt
-drwxr-xr-x   0 snaka      (501) staff       (20)        0 2023-05-03 04:48:40.799152 scattering-geometry-tools-0.1.3/src/sgt/
--rw-r--r--   0 snaka      (501) staff       (20)     9602 2023-05-03 04:47:30.000000 scattering-geometry-tools-0.1.3/src/sgt/__init__.py
--rw-r--r--   0 snaka      (501) staff       (20)   979316 2022-11-25 12:35:18.000000 scattering-geometry-tools-0.1.3/src/sgt/_cpolarize.c
--rw-r--r--   0 snaka      (501) staff       (20)   868651 2022-12-05 14:22:10.000000 scattering-geometry-tools-0.1.3/src/sgt/_crefine.c
--rw-r--r--   0 snaka      (501) staff       (20)     4678 2022-11-25 09:54:43.000000 scattering-geometry-tools-0.1.3/src/sgt/_pypolarize.py
--rw-r--r--   0 snaka      (501) staff       (20)    13019 2022-11-30 13:49:56.000000 scattering-geometry-tools-0.1.3/src/sgt/core.py
--rw-r--r--   0 snaka      (501) staff       (20)     1428 2022-12-12 12:57:09.000000 scattering-geometry-tools-0.1.3/src/sgt/crystal.py
--rw-r--r--   0 snaka      (501) staff       (20)     3350 2023-05-03 04:43:55.000000 scattering-geometry-tools-0.1.3/src/sgt/npzimage.py
--rw-r--r--   0 snaka      (501) staff       (20)     7404 2022-11-30 13:36:08.000000 scattering-geometry-tools-0.1.3/src/sgt/pilatus.py
--rw-r--r--   0 snaka      (501) staff       (20)     3358 2023-05-02 19:21:37.000000 scattering-geometry-tools-0.1.3/src/sgt/refine.py
-drwxr-xr-x   0 snaka      (501) staff       (20)        0 2023-05-03 04:48:40.799751 scattering-geometry-tools-0.1.3/test/
--rw-r--r--   0 snaka      (501) staff       (20)      545 2023-05-03 04:46:13.000000 scattering-geometry-tools-0.1.3/test/test_npzimage.py
--rw-r--r--   0 snaka      (501) staff       (20)     3185 2023-03-01 12:43:32.000000 scattering-geometry-tools-0.1.3/test/test_opt.py
+drwxr-xr-x   0 snaka      (501) staff       (20)        0 2024-05-15 13:48:52.418474 scattering-geometry-tools-0.1.4/
+-rw-r--r--   0 snaka      (501) staff       (20)     1066 2022-08-19 02:56:27.000000 scattering-geometry-tools-0.1.4/LICENSE
+-rw-r--r--   0 snaka      (501) staff       (20)     1833 2024-05-15 13:48:52.417973 scattering-geometry-tools-0.1.4/PKG-INFO
+-rw-r--r--   0 snaka      (501) staff       (20)      124 2022-12-12 14:20:07.000000 scattering-geometry-tools-0.1.4/README.md
+-rw-r--r--   0 snaka      (501) staff       (20)      700 2024-05-15 13:42:14.000000 scattering-geometry-tools-0.1.4/pyproject.toml
+-rw-r--r--   0 snaka      (501) staff       (20)       38 2024-05-15 13:48:52.418524 scattering-geometry-tools-0.1.4/setup.cfg
+-rw-r--r--   0 snaka      (501) staff       (20)      433 2022-12-05 13:44:09.000000 scattering-geometry-tools-0.1.4/setup.py
+drwxr-xr-x   0 snaka      (501) staff       (20)        0 2024-05-15 13:48:52.404699 scattering-geometry-tools-0.1.4/src/
+drwxr-xr-x   0 snaka      (501) staff       (20)        0 2024-05-15 13:48:52.408486 scattering-geometry-tools-0.1.4/src/scattering_geometry_tools.egg-info/
+-rw-r--r--   0 snaka      (501) staff       (20)     1833 2024-05-15 13:48:52.000000 scattering-geometry-tools-0.1.4/src/scattering_geometry_tools.egg-info/PKG-INFO
+-rw-r--r--   0 snaka      (501) staff       (20)      519 2024-05-15 13:48:52.000000 scattering-geometry-tools-0.1.4/src/scattering_geometry_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 snaka      (501) staff       (20)        1 2024-05-15 13:48:52.000000 scattering-geometry-tools-0.1.4/src/scattering_geometry_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 snaka      (501) staff       (20)       25 2024-05-15 13:48:52.000000 scattering-geometry-tools-0.1.4/src/scattering_geometry_tools.egg-info/requires.txt
+-rw-r--r--   0 snaka      (501) staff       (20)        4 2024-05-15 13:48:52.000000 scattering-geometry-tools-0.1.4/src/scattering_geometry_tools.egg-info/top_level.txt
+drwxr-xr-x   0 snaka      (501) staff       (20)        0 2024-05-15 13:48:52.416368 scattering-geometry-tools-0.1.4/src/sgt/
+-rw-r--r--   0 snaka      (501) staff       (20)     9602 2024-05-15 13:42:52.000000 scattering-geometry-tools-0.1.4/src/sgt/__init__.py
+-rw-r--r--   0 snaka      (501) staff       (20)   979316 2022-11-25 12:35:18.000000 scattering-geometry-tools-0.1.4/src/sgt/_cpolarize.c
+-rw-r--r--   0 snaka      (501) staff       (20)   868651 2022-12-05 14:22:10.000000 scattering-geometry-tools-0.1.4/src/sgt/_crefine.c
+-rw-r--r--   0 snaka      (501) staff       (20)     4678 2022-11-25 09:54:43.000000 scattering-geometry-tools-0.1.4/src/sgt/_pypolarize.py
+-rw-r--r--   0 snaka      (501) staff       (20)    13019 2022-11-30 13:49:56.000000 scattering-geometry-tools-0.1.4/src/sgt/core.py
+-rw-r--r--   0 snaka      (501) staff       (20)     1428 2023-05-10 11:45:01.000000 scattering-geometry-tools-0.1.4/src/sgt/crystal.py
+-rw-r--r--   0 snaka      (501) staff       (20)     3350 2023-05-03 04:43:55.000000 scattering-geometry-tools-0.1.4/src/sgt/npzimage.py
+-rw-r--r--   0 snaka      (501) staff       (20)     7404 2022-11-30 13:36:08.000000 scattering-geometry-tools-0.1.4/src/sgt/pilatus.py
+-rw-r--r--   0 snaka      (501) staff       (20)     3358 2023-05-02 19:21:37.000000 scattering-geometry-tools-0.1.4/src/sgt/refine.py
+drwxr-xr-x   0 snaka      (501) staff       (20)        0 2024-05-15 13:48:52.417418 scattering-geometry-tools-0.1.4/test/
+-rw-r--r--   0 snaka      (501) staff       (20)      545 2023-05-03 04:46:13.000000 scattering-geometry-tools-0.1.4/test/test_npzimage.py
+-rw-r--r--   0 snaka      (501) staff       (20)     3185 2023-03-01 12:43:32.000000 scattering-geometry-tools-0.1.4/test/test_opt.py
```

### Comparing `scattering-geometry-tools-0.1.3/LICENSE` & `scattering-geometry-tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/PKG-INFO` & `scattering-geometry-tools-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scattering-geometry-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for calculations of geometries in scattering experiments. 
 Author-email: Shintaro Nakagawa <shntrnkgw@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 shntrnkgw
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `scattering-geometry-tools-0.1.3/pyproject.toml` & `scattering-geometry-tools-0.1.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "numpy>=1.23"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scattering-geometry-tools"
-version = "0.1.3"
+version = "0.1.4"
 description = "Tools for calculations of geometries in scattering experiments. "
 readme = "README.md"
 authors = [{name = "Shintaro Nakagawa", email = "shntrnkgw@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
```

### Comparing `scattering-geometry-tools-0.1.3/src/scattering_geometry_tools.egg-info/PKG-INFO` & `scattering-geometry-tools-0.1.4/src/scattering_geometry_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scattering-geometry-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for calculations of geometries in scattering experiments. 
 Author-email: Shintaro Nakagawa <shntrnkgw@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 shntrnkgw
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `scattering-geometry-tools-0.1.3/src/scattering_geometry_tools.egg-info/SOURCES.txt` & `scattering-geometry-tools-0.1.4/src/scattering_geometry_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/src/sgt/__init__.py` & `scattering-geometry-tools-0.1.4/src/sgt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 from typing import List, IO, Tuple
 import numpy as np
 import json
 from sgt import core, _cpolarize
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 class geometry:
     """Interface class for scattering geometry manipulation. 
 
     Example:
         To create a `geometry` instance,
```

### Comparing `scattering-geometry-tools-0.1.3/src/sgt/_cpolarize.c` & `scattering-geometry-tools-0.1.4/src/sgt/_cpolarize.c`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/src/sgt/_crefine.c` & `scattering-geometry-tools-0.1.4/src/sgt/_crefine.c`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/src/sgt/_pypolarize.py` & `scattering-geometry-tools-0.1.4/src/sgt/_pypolarize.py`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/src/sgt/core.py` & `scattering-geometry-tools-0.1.4/src/sgt/core.py`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/src/sgt/crystal.py` & `scattering-geometry-tools-0.1.4/src/sgt/crystal.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
     return avec, bvec, cvec
 
 def make_reciprocal_primitive_vectors(
     avec: np.ndarray, bvec: np.ndarray, cvec: np.ndarray
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
 
-    pref: float = 2.0*np.pi*np.dot(avec, np.outer(bvec, cvec))
+    pref: float = 2.0*np.pi/np.dot(avec, np.cross(bvec, cvec))
 
-    return pref*np.outer(bvec, cvec), pref*np.outer(cvec, avec), pref*np.outer(avec, bvec)
+    return pref*np.cross(bvec, cvec), pref*np.cross(cvec, avec), pref*np.cross(avec, bvec)
 
 def make_reciprocal_lattice_vector(
     h: int, k: int, l: int, 
     astar: np.ndarray, bstar: np.ndarray, cstar: np.ndarray
     ) -> np.ndarray:
 
     return h*astar + k*bstar + l*cstar
```

### Comparing `scattering-geometry-tools-0.1.3/src/sgt/npzimage.py` & `scattering-geometry-tools-0.1.4/src/sgt/npzimage.py`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/src/sgt/pilatus.py` & `scattering-geometry-tools-0.1.4/src/sgt/pilatus.py`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/src/sgt/refine.py` & `scattering-geometry-tools-0.1.4/src/sgt/refine.py`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/test/test_npzimage.py` & `scattering-geometry-tools-0.1.4/test/test_npzimage.py`

 * *Files identical despite different names*

### Comparing `scattering-geometry-tools-0.1.3/test/test_opt.py` & `scattering-geometry-tools-0.1.4/test/test_opt.py`

 * *Files identical despite different names*

