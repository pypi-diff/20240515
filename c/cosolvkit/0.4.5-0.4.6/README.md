# Comparing `tmp/cosolvkit-0.4.5.tar.gz` & `tmp/cosolvkit-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosolvkit-0.4.5.tar", last modified: Tue May 14 21:19:05 2024, max compression
+gzip compressed data, was "cosolvkit-0.4.6.tar", last modified: Wed May 15 00:18:02 2024, max compression
```

## Comparing `cosolvkit-0.4.5.tar` & `cosolvkit-0.4.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.777874 cosolvkit-0.4.5/cosolvkit/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    58983 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/cosolvent_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/cosolvkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/aromatic.json
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/cosolvents.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/forcefields.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/h_bonding.json
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/lipophilic.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/negative.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/data/positive.json
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/cosolvkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/cosolvkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 21:19:05.000000 cosolvkit-0.4.5/cosolvkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/scripts/create_cosolvent_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/scripts/post_simulation_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:19:05.781874 cosolvkit-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-14 21:18:52.000000 cosolvkit-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:18:02.032217 cosolvkit-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-15 00:18:02.032217 cosolvkit-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:18:02.028217 cosolvkit-0.4.6/cosolvkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58990 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/cosolvent_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:18:02.032217 cosolvkit-0.4.6/cosolvkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/data/aromatic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/data/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/data/cosolvents.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/data/forcefields.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/data/h_bonding.json
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/data/lipophilic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/data/negative.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/data/positive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/cosolvkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:18:02.032217 cosolvkit-0.4.6/cosolvkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-15 00:18:01.000000 cosolvkit-0.4.6/cosolvkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-15 00:18:02.000000 cosolvkit-0.4.6/cosolvkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:18:01.000000 cosolvkit-0.4.6/cosolvkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-15 00:18:01.000000 cosolvkit-0.4.6/cosolvkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:18:01.000000 cosolvkit-0.4.6/cosolvkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 00:18:01.000000 cosolvkit-0.4.6/cosolvkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:18:02.032217 cosolvkit-0.4.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/scripts/create_cosolvent_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/scripts/post_simulation_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:18:02.032217 cosolvkit-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-15 00:17:53.000000 cosolvkit-0.4.6/setup.py
```

### Comparing `cosolvkit-0.4.5/LICENSE` & `cosolvkit-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.5/README.md` & `cosolvkit-0.4.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) [![PyPI - Version](https://img.shields.io/pypi/v/cosolvkit)](https://pypi.org/project/cosolvkit/0.4.5/) [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) [![PyPI - Version](https://img.shields.io/pypi/v/cosolvkit)](https://pypi.org/project/cosolvkit/0.4.6/) [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
 [![Documentation Status](https://readthedocs.org/projects/cosolvkit/badge/?version=latest)](https://cosolvkit.readthedocs.io/en/latest/?badge=latest)
       
     
 
 # CosolvKit
 The python package for creating cosolvent system.
```

### Comparing `cosolvkit-0.4.5/cosolvkit/analysis.py` & `cosolvkit-0.4.6/cosolvkit/analysis.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.5/cosolvkit/config.py` & `cosolvkit-0.4.6/cosolvkit/config.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.5/cosolvkit/cosolvent_system.py` & `cosolvkit-0.4.6/cosolvkit/cosolvent_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import sys
 import io
 from collections import defaultdict
-from typing import Union
+from typing import Union, Tuple
 import numpy as np
 from scipy import spatial
 from scipy.stats import qmc
 import math 
 from itertools import product
 import parmed
 from openmm import Vec3, unit, XmlSerializer, System, CustomNonbondedForce, NonbondedForce, OpenMMException
@@ -631,27 +631,27 @@
                                          constraints=app.HBonds,
                                          hydrogenMass=3.0*openmmunit.amu)
         return system 
 #endregion
 #region FillTheVoid
     def add_cosolvents(self, 
                        cosolvents: dict, 
-                       vectors: tuple[Vec3, Vec3, Vec3], 
+                       vectors: Tuple[Vec3, Vec3, Vec3], 
                        lowerBound: Union[openmmunit.Quantity, Vec3], 
                        upperBound: Union[openmmunit.Quantity, Vec3],
                        receptor_positions: list) -> dict:
         """This function adds the desired number of cosolvent molecules using the halton sequence
         to generate random uniformly distributed points inside the grid where to place the cosolvent molecules.
         At first, if a receptor/protein is present the halton sequence points that would clash with the protein
         are pruned.
 
         :param cosolvents: keys are cosolvent molecules and values are 3D coordinates of the molecule
         :type cosolvents: dict
         :param vectors: vectors defining the simulation box
-        :type vectors: tuple[openmm.Vec3, openmm.Vec3, openmm.Vec3]
+        :type vectors: Tuple[openmm.Vec3, openmm.Vec3, openmm.Vec3]
         :param lowerBound: lower bound of the simulation box
         :type lowerBound: Union[openmm.unit.Quantity, Vec3]
         :param upperBound: upper bound of the simulation box
         :type upperBound: [openmm.unit.Quantity, Vec3]
         :param receptor_positions: list of 3D coordinates of the receptor
         :type receptor_positions: list
         :return: keys are cosolvent molecules and values are 3D coordinates of the newly added cosolvent molecules
@@ -757,15 +757,15 @@
     def accept_reject(self, 
                       xyz: np.ndarray, 
                       halton: list, 
                       kdtree: spatial.cKDTree, 
                       valid_ids: list, 
                       lowerBound: Union[openmmunit.Quantity, Vec3], 
                       upperBound: Union[openmmunit.Quantity, Vec3], 
-                      protein_kdtree: spatial.cKDTree) -> tuple[np.ndarray, list]:
+                      protein_kdtree: spatial.cKDTree) -> Tuple[np.ndarray, list]:
         """Accepts or reject the halton move. A random halton point is selected and checked, if accepted
         the cosolvent is placed there, otherwise a local search is performed in the neighbors of the point 
         (1 tile). If the local search produces no clashes the new position is accepted, otherwise a new 
         random halton point is selected and the old one is marked as not good. The algorithm stops
         when a move is accepted or 1000000 of trials are done and no move is accepted.
 
         :param xyz: 3D coordinates of the cosolvent molecule
@@ -779,15 +779,15 @@
         :param lowerBound: lower bound of the box
         :type lowerBound: Union[openmm.unit.Quantity, Vec3]
         :param upperBound: upper bound of the box
         :type upperBound: Union[openmm.unit.Quantity, Vec3]
         :param protein_kdtree: tree of the protein's positions
         :type protein_kdtree: spatial.cKDTree
         :return: accepted coordinates for the cosolvent and the used halton ids
-        :rtype: tuple[np.ndarray, list]
+        :rtype: Tuple[np.ndarray, list]
         """        
         trial = 0
         accepted = False
         coords_to_return = 0
         moves = self.local_search()
         while not accepted and trial < 1000000:
             halton_idx = np.random.choice(len(valid_ids))
@@ -1001,15 +1001,15 @@
         return small_ff
 #endregion
     
 #region SimulationBox
     def _build_box(self, 
                    positions: np.ndarray, 
                    padding: openmmunit.Quantity, 
-                   radius: openmmunit.Quantity = None) -> tuple[tuple[Vec3, Vec3, Vec3], 
+                   radius: openmmunit.Quantity = None) -> Tuple[Tuple[Vec3, Vec3, Vec3], 
                                                                 Vec3, 
                                                                 Union[openmmunit.Quantity, Vec3],
                                                                 Union[openmmunit.Quantity, Vec3]]:
         """Builds the simulation box. If a receptor is passed it is used alongside with the padding
         parameter to build the box automatically, otherwise a radius has to be passed. If no receptor
         the box is centered on the point [0, 0, 0].
```

### Comparing `cosolvkit-0.4.5/cosolvkit/data/config.json` & `cosolvkit-0.4.6/cosolvkit/data/config.json`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.5/cosolvkit/data/cosolvents.json` & `cosolvkit-0.4.6/cosolvkit/data/cosolvents.json`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.5/cosolvkit/simulation.py` & `cosolvkit-0.4.6/cosolvkit/simulation.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.5/cosolvkit/utils.py` & `cosolvkit-0.4.6/cosolvkit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import contextlib
 import os
 import tempfile
 import shutil
 import subprocess
 import importlib
+from typing import List, Tuple
 from collections import defaultdict
 
 import numpy as np
 import mdtraj
 from MDAnalysis import Universe
 from openmm.app import *
 from openmm import *
@@ -85,15 +86,15 @@
 #     """
 #     # Tranform constant to the right unit
 #     k = k * unit.kilocalories_per_mole / unit.angstroms**2
 #     k = k.value_in_unit_system(unit.md_unit_system)
     
 #     simulation.context.setParameter('k', k)
 
-def fix_pdb(pdbfile: str, pdbxfile: str, keep_heterogens: bool=False) -> tuple[Topology, list]:
+def fix_pdb(pdbfile: str, pdbxfile: str, keep_heterogens: bool=False) -> Tuple[Topology, List]:
     """Fixes common problems in PDB such as:
             - missing atoms
             - missing residues
             - missing hydrogens
             - remove nonstandard residues
 
     :param pdbfile: pdb string old format
@@ -119,15 +120,15 @@
         fixer.removeHeterogens(keepWater=True)
 
     fixer.findMissingAtoms() 
     fixer.addMissingAtoms()
     fixer.addMissingHydrogens(7)
     return fixer.topology, fixer.positions
     
-def add_variants(topology: Topology, positions: list, variants: list=list()) -> tuple[Topology, list]:
+def add_variants(topology: Topology, positions: list, variants: list=list()) -> Tuple[Topology, List]:
     """Adds variants for specific protonation states.
 
     :param topology: openmm topology
     :type topology: Topology
     :param positions: openmm positions
     :type positions: list
     :param variants: list of variants to apply for the protonation states, defaults to list()
```

### Comparing `cosolvkit-0.4.5/cosolvkit.egg-info/SOURCES.txt` & `cosolvkit-0.4.6/cosolvkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.5/scripts/create_cosolvent_system.py` & `cosolvkit-0.4.6/scripts/create_cosolvent_system.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.5/scripts/post_simulation_processing.py` & `cosolvkit-0.4.6/scripts/post_simulation_processing.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.5/setup.py` & `cosolvkit-0.4.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,25 +14,24 @@
         for filename in fnmatch.filter(filenames, '*'):
             matches.append(os.path.join(root, filename))
 
     return matches
 
 
 setup(name="cosolvkit",
-      version='0.4.5',
+      version='0.4.6',
       description="CosolvKit",
       author="Niccolo Bruciaferri, Jerome Eberhardt",
       author_email="forli@scripps.edu",
       url="https://github.com/forlilab/cosolvkit",
       packages=find_packages(exclude=['docs']),
       package_data={"cosolvkit" : ["data/*"]},
       data_files=[("", ["README.md", "LICENSE"])],
       include_package_data=True,
       zip_safe=False,
-      python_requires=">=3.9",
       license="LGPL-2.1",
       keywords=["molecular modeling", "drug design",
                 "cosolvent", "MD simulations"],
       classifiers=["Programming Language :: Python",
                    "Operating System :: Unix",
                    "Operating System :: MacOS",
                    "Topic :: Scientific/Engineering"],
```

