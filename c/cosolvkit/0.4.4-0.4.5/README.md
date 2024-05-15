# Comparing `tmp/cosolvkit-0.4.4.tar.gz` & `tmp/cosolvkit-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosolvkit-0.4.4.tar", last modified: Tue May 14 17:33:53 2024, max compression
+gzip compressed data, was "cosolvkit-0.4.5.tar", last modified: Tue May 14 21:19:05 2024, max compression
```

## Comparing `cosolvkit-0.4.4.tar` & `cosolvkit-0.4.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.807404 cosolvkit-0.4.4/cosolvkit/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    58843 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/cosolvent_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/cosolvkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/aromatic.json
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/cosolvents.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/forcefields.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/h_bonding.json
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/lipophilic.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/negative.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/data/positive.json
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/cosolvkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/cosolvkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 17:33:53.000000 cosolvkit-0.4.4/cosolvkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/scripts/create_cosolvent_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/scripts/post_simulation_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:33:53.811404 cosolvkit-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-14 17:33:46.000000 cosolvkit-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.777874 cosolvkit-0.4.5/cosolvkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58983 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/cosolvent_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/cosolvkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/aromatic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/cosolvents.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/forcefields.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/h_bonding.json
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/lipophilic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/negative.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/positive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/cosolvkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/scripts/create_cosolvent_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/scripts/post_simulation_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/setup.py
```

### Comparing `cosolvkit-0.4.4/LICENSE` & `cosolvkit-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/README.md` & `cosolvkit-0.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) [![PyPI - Version](https://img.shields.io/pypi/v/cosolvkit)](https://pypi.org/project/cosolvkit/0.4.4/) [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) [![PyPI - Version](https://img.shields.io/pypi/v/cosolvkit)](https://pypi.org/project/cosolvkit/0.4.5/) [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
 [![Documentation Status](https://readthedocs.org/projects/cosolvkit/badge/?version=latest)](https://cosolvkit.readthedocs.io/en/latest/?badge=latest)
       
     
 
 # CosolvKit
 The python package for creating cosolvent system.
```

### Comparing `cosolvkit-0.4.4/cosolvkit/analysis.py` & `cosolvkit-0.4.5/cosolvkit/analysis.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/cosolvkit/config.py` & `cosolvkit-0.4.5/cosolvkit/config.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/cosolvkit/cosolvent_system.py` & `cosolvkit-0.4.5/cosolvkit/cosolvent_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 import sys
 import io
 from collections import defaultdict
+from typing import Union
 import numpy as np
 from scipy import spatial
 from scipy.stats import qmc
 import math 
 from itertools import product
 import parmed
 from openmm import Vec3, unit, XmlSerializer, System, CustomNonbondedForce, NonbondedForce, OpenMMException
@@ -631,30 +632,30 @@
                                          hydrogenMass=3.0*openmmunit.amu)
         return system 
 #endregion
 #region FillTheVoid
     def add_cosolvents(self, 
                        cosolvents: dict, 
                        vectors: tuple[Vec3, Vec3, Vec3], 
-                       lowerBound: openmmunit.Quantity | Vec3, 
-                       upperBound: openmmunit.Quantity | Vec3,
+                       lowerBound: Union[openmmunit.Quantity, Vec3], 
+                       upperBound: Union[openmmunit.Quantity, Vec3],
                        receptor_positions: list) -> dict:
         """This function adds the desired number of cosolvent molecules using the halton sequence
         to generate random uniformly distributed points inside the grid where to place the cosolvent molecules.
         At first, if a receptor/protein is present the halton sequence points that would clash with the protein
         are pruned.
 
         :param cosolvents: keys are cosolvent molecules and values are 3D coordinates of the molecule
         :type cosolvents: dict
         :param vectors: vectors defining the simulation box
         :type vectors: tuple[openmm.Vec3, openmm.Vec3, openmm.Vec3]
         :param lowerBound: lower bound of the simulation box
-        :type lowerBound: openmm.unit.Quantity | Vec3
+        :type lowerBound: Union[openmm.unit.Quantity, Vec3]
         :param upperBound: upper bound of the simulation box
-        :type upperBound: openmm.unit.Quantity | Vec3
+        :type upperBound: [openmm.unit.Quantity, Vec3]
         :param receptor_positions: list of 3D coordinates of the receptor
         :type receptor_positions: list
         :return: keys are cosolvent molecules and values are 3D coordinates of the newly added cosolvent molecules
         :rtype: dict
         """
         edge_cutoff = 2.5*openmmunit.angstrom
         prot_kdtree = None
@@ -754,16 +755,16 @@
             return self.is_in_box(new_coords, self.lowerBound, self.vectors)
 
     def accept_reject(self, 
                       xyz: np.ndarray, 
                       halton: list, 
                       kdtree: spatial.cKDTree, 
                       valid_ids: list, 
-                      lowerBound: openmmunit.Quantity | Vec3, 
-                      upperBound: openmmunit.Quantity | Vec3, 
+                      lowerBound: Union[openmmunit.Quantity, Vec3], 
+                      upperBound: Union[openmmunit.Quantity, Vec3], 
                       protein_kdtree: spatial.cKDTree) -> tuple[np.ndarray, list]:
         """Accepts or reject the halton move. A random halton point is selected and checked, if accepted
         the cosolvent is placed there, otherwise a local search is performed in the neighbors of the point 
         (1 tile). If the local search produces no clashes the new position is accepted, otherwise a new 
         random halton point is selected and the old one is marked as not good. The algorithm stops
         when a move is accepted or 1000000 of trials are done and no move is accepted.
 
@@ -772,17 +773,17 @@
         :param halton: halton sequence
         :type halton: list
         :param kdtree: tree of the cosolvent molecules positions already placed in the box
         :type kdtree: spatial.cKDTree
         :param valid_ids: valid halton indices
         :type valid_ids: list
         :param lowerBound: lower bound of the box
-        :type lowerBound: openmm.unit.Quantity | Vec3
+        :type lowerBound: Union[openmm.unit.Quantity, Vec3]
         :param upperBound: upper bound of the box
-        :type upperBound: openmm.unit.Quantity | Vec3
+        :type upperBound: Union[openmm.unit.Quantity, Vec3]
         :param protein_kdtree: tree of the protein's positions
         :type protein_kdtree: spatial.cKDTree
         :return: accepted coordinates for the cosolvent and the used halton ids
         :rtype: tuple[np.ndarray, list]
         """        
         trial = 0
         accepted = False
@@ -808,24 +809,24 @@
                             coords_to_return = cosolv_xyz
                             break
                     trial += 1
         return coords_to_return, valid_ids
 
     def is_in_box(self, 
                   xyzs: np.ndarray, 
-                  lowerBound: openmmunit.Quantity | Vec3, 
-                  upperBound: openmmunit.Quantity | Vec3) -> bool:
+                  lowerBound: Union[openmmunit.Quantity, Vec3], 
+                  upperBound: Union[openmmunit.Quantity, Vec3]) -> bool:
         """Checks if the coordinates are in the box or not
 
         :param xyzs: coordinates to check
         :type xyzs: np.ndarray
         :param lowerBound: lower bound of the box
-        :type lowerBound: openmmunit.Quantity | Vec3
+        :type lowerBound: Union[openmmunit.Quantity, Vec3]
         :param upperBound: upper bound of the box
-        :type upperBound: openmmunit.Quantity | Vec3
+        :type upperBound: Union[openmmunit.Quantity, Vec3]
         :return: True if all the coordinates are in the box, Flase otherwise
         :rtype: bool
         """
         # cutoff = (1.5*openmmunit.angstrom).value_in_unit(openmmunit.nanometer)
         xyzs = np.atleast_2d(xyzs)
         x, y, z = xyzs[:, 0], xyzs[:, 1], xyzs[:, 2]
 
@@ -898,21 +899,21 @@
         X, Y, Z = np.meshgrid(x, y, z)
         center_xyzs = np.stack((X.ravel(), Y.ravel(), Z.ravel()), axis=-1)
         kdtree = spatial.cKDTree(center_xyzs)
         query = kdtree.query_ball_point(mol_positions, offset)
         points = np.unique(np.hstack(query)).astype(int)
         return round(len(points)*mesh_step**3, 2)
 
-    def fitting_checks(self) -> float | None:
+    def fitting_checks(self) -> Union[float, None]:
         """Checks if the required cosolvents can fit in the box and 
         do not exceed the 50% of the available fillable volume 
         (volume not occupied by the receptor, if present).
 
         :return: available volume if the cosolvents can fit, None otherwise
-        :rtype: float | None
+        :rtype: Union[float, None]
         """
         prot_volume = 0
         if self.receptor:
             prot_volume = self.calculate_mol_volume(self.modeller.positions)
             prot_volume = prot_volume
             print(f"Volume protein: {prot_volume*1000} A^3")
         empty_volume = self.cubic_nanometers_to_liters(self.box_volume - prot_volume)
@@ -924,19 +925,19 @@
         empty_available_volume = round(self.liters_to_cubic_nanometers(empty_volume)/2., 3)
         print(f"Volume requested for cosolvents: {volume_occupied_by_cosolvent} nm**3")
         print(f"Volume available for cosolvents: {empty_available_volume} nm**3")
         if volume_occupied_by_cosolvent > empty_available_volume:
             return None
         return empty_available_volume
 
-    def liters_to_cubic_nanometers(self, liters: float | openmmunit.Quantity) -> float:
+    def liters_to_cubic_nanometers(self, liters: Union[float, openmmunit.Quantity]) -> float:
         """Converts liters in cubic nanometers
 
         :param liters: volume to convert
-        :type liters: float | openmm.unit.Quantity
+        :type liters: Union[float, openmm.unit.Quantity]
         :return: converted volume
         :rtype: float
         """
         if isinstance(liters, openmmunit.Quantity):
             liters = liters.value_in_unit(openmmunit.liters)
         value = liters * 1e+24
         return value
@@ -1002,30 +1003,30 @@
     
 #region SimulationBox
     def _build_box(self, 
                    positions: np.ndarray, 
                    padding: openmmunit.Quantity, 
                    radius: openmmunit.Quantity = None) -> tuple[tuple[Vec3, Vec3, Vec3], 
                                                                 Vec3, 
-                                                                openmmunit.Quantity | Vec3,
-                                                                openmmunit.Quantity | Vec3]:
+                                                                Union[openmmunit.Quantity, Vec3],
+                                                                Union[openmmunit.Quantity, Vec3]]:
         """Builds the simulation box. If a receptor is passed it is used alongside with the padding
         parameter to build the box automatically, otherwise a radius has to be passed. If no receptor
         the box is centered on the point [0, 0, 0].
 
         :param positions: coordinates of the receptor if present
         :type positions: np.ndarray
         :param padding: padding to be used
         :type padding: openmm.unit.Quantity
         :param radius: radius specified if no receptor is passed, defaults to None
         :type radius: openmm.unit.Quantity, optional
         :return: The first element returned is a tuple containing the three vectors describing the simulation box.
                 The second element is the box itself.
                 Third and fourth elements are the lower and upper bound of the simulation box.
-        :rtype: tuple[tuple[Vec3, Vec3, Vec3], Vec3, openmmunit.Quantity | Vec3, openmmunit.Quantity | Vec3]
+        :rtype: tuple[tuple[Vec3, Vec3, Vec3], Vec3, Union[openmmunit.Quantity, Vec3], Union[openmmunit.Quantity, Vec3]]
         """
         padding = padding.value_in_unit(openmmunit.nanometer)
         if positions is not None:
             positions = positions.value_in_unit(openmmunit.nanometer)
             minRange = Vec3(*(min((pos[i] for pos in positions)) for i in range(3)))
             maxRange = Vec3(*(max((pos[i] for pos in positions)) for i in range(3)))
             center = 0.5*(minRange+maxRange)
```

### Comparing `cosolvkit-0.4.4/cosolvkit/data/config.json` & `cosolvkit-0.4.5/cosolvkit/data/config.json`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/cosolvkit/data/cosolvents.json` & `cosolvkit-0.4.5/cosolvkit/data/cosolvents.json`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/cosolvkit/simulation.py` & `cosolvkit-0.4.5/cosolvkit/simulation.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/cosolvkit/utils.py` & `cosolvkit-0.4.5/cosolvkit/utils.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/cosolvkit.egg-info/SOURCES.txt` & `cosolvkit-0.4.5/cosolvkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/scripts/create_cosolvent_system.py` & `cosolvkit-0.4.5/scripts/create_cosolvent_system.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/scripts/post_simulation_processing.py` & `cosolvkit-0.4.5/scripts/post_simulation_processing.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.4/setup.py` & `cosolvkit-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         for filename in fnmatch.filter(filenames, '*'):
             matches.append(os.path.join(root, filename))
 
     return matches
 
 
 setup(name="cosolvkit",
-      version='0.4.4',
+      version='0.4.5',
       description="CosolvKit",
       author="Niccolo Bruciaferri, Jerome Eberhardt",
       author_email="forli@scripps.edu",
       url="https://github.com/forlilab/cosolvkit",
       packages=find_packages(exclude=['docs']),
       package_data={"cosolvkit" : ["data/*"]},
       data_files=[("", ["README.md", "LICENSE"])],
```

