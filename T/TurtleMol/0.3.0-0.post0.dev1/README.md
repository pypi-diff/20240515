# Comparing `tmp/turtlemol-0.3.0.tar.gz` & `tmp/TurtleMol-0.post0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turtlemol-0.3.0.tar", last modified: Wed May 15 02:29:01 2024, max compression
+gzip compressed data, was "TurtleMol-0.post0.dev1.tar", last modified: Mon Nov 13 20:28:28 2023, max compression
```

## Comparing `turtlemol-0.3.0.tar` & `TurtleMol-0.post0.dev1.tar`

### file list

```diff
@@ -1,44 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:29:01.781302 turtlemol-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-15 02:28:57.000000 turtlemol-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 02:28:57.000000 turtlemol-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-15 02:29:01.781302 turtlemol-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-05-15 02:28:57.000000 turtlemol-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:29:01.781302 turtlemol-0.3.0/TurtleMol/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/Box3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/Sphere3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 02:29:01.785302 turtlemol-0.3.0/TurtleMol/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:29:01.781302 turtlemol-0.3.0/TurtleMol/data/
--rw-r--r--   0 runner    (1001) docker     (127)    19943 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/data/ElementData.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/defaultParams.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/drawMol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/isOverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/makeStruc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/mesh3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/readWriteFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/setAtomProp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/shiftBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/shiftDensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/shiftMesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/shiftSphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-15 02:28:57.000000 turtlemol-0.3.0/TurtleMol/shiftUnitCell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:29:01.781302 turtlemol-0.3.0/TurtleMol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-15 02:29:01.000000 turtlemol-0.3.0/TurtleMol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-15 02:29:01.000000 turtlemol-0.3.0/TurtleMol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 02:29:01.000000 turtlemol-0.3.0/TurtleMol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 02:29:01.000000 turtlemol-0.3.0/TurtleMol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 02:29:01.000000 turtlemol-0.3.0/TurtleMol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 02:29:01.000000 turtlemol-0.3.0/TurtleMol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-15 02:29:01.781302 turtlemol-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-15 02:28:57.000000 turtlemol-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:29:01.781302 turtlemol-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-15 02:28:57.000000 turtlemol-0.3.0/tests/test_BaseStruc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-15 02:28:57.000000 turtlemol-0.3.0/tests/test_atomFill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-15 02:28:57.000000 turtlemol-0.3.0/tests/test_atomRandomPlace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-15 02:28:57.000000 turtlemol-0.3.0/tests/test_moleculeFill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-15 02:28:57.000000 turtlemol-0.3.0/tests/test_moleculeRandomPlace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-15 02:28:57.000000 turtlemol-0.3.0/tests/test_randOrient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-15 02:28:57.000000 turtlemol-0.3.0/tests/test_readWritePDB.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-15 02:28:57.000000 turtlemol-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:28:28.283516 TurtleMol-0.post0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2023-11-13 20:28:28.283516 TurtleMol-0.post0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:28:28.283516 TurtleMol-0.post0.dev1/TurtleMol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/Box3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/Sphere3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2023-11-13 20:28:28.287515 TurtleMol-0.post0.dev1/TurtleMol/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:28:28.283516 TurtleMol-0.post0.dev1/TurtleMol/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    19943 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/data/ElementData.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/defaultParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/drawMol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/isOverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/makeStruc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/readWriteFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/setAtomProp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/shiftBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/TurtleMol/shiftSphere.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:28:28.283516 TurtleMol-0.post0.dev1/TurtleMol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2023-11-13 20:28:28.000000 TurtleMol-0.post0.dev1/TurtleMol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-11-13 20:28:28.000000 TurtleMol-0.post0.dev1/TurtleMol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 20:28:28.000000 TurtleMol-0.post0.dev1/TurtleMol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 20:28:28.000000 TurtleMol-0.post0.dev1/TurtleMol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-13 20:28:28.000000 TurtleMol-0.post0.dev1/TurtleMol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-13 20:28:28.000000 TurtleMol-0.post0.dev1/TurtleMol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2023-11-13 20:28:28.287515 TurtleMol-0.post0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:28:28.283516 TurtleMol-0.post0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/tests/test_BaseStruc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/tests/test_atomFill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/tests/test_atomRandomPlace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/tests/test_moleculeFill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/tests/test_moleculeRandomPlace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/tests/test_randOrient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/tests/test_readWritePDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2023-11-13 20:28:18.000000 TurtleMol-0.post0.dev1/versioneer.py
```

### Comparing `turtlemol-0.3.0/LICENSE` & `TurtleMol-0.post0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `turtlemol-0.3.0/PKG-INFO` & `TurtleMol-0.post0.dev1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: TurtleMol
-Version: 0.3.0
+Version: 0.post0.dev1
 Summary: Design, create, and generate unique, complex molecular structures of any shape and size!
 Author: Dominick Filonowich
 Author-email: filonowichd74@gmail.com
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: trimesh
-Requires-Dist: rtree
-Requires-Dist: scipy
 Requires-Dist: pytest
 
 <h1 align='center'>TurtleMol</h1>
 <h4 align='center'>Design, create, and generate unique, complex molecular structures of any shape and size!</h4>
 
 
 
@@ -76,31 +80,15 @@
 
 You can install the latest development version of TurtleMol from the [Github Repository](https://github.com/Dfilono/TurtleMol).
 
     git clone https://github.com/Dfilono/TurtleMol
     cd TurtleMol
     pip install .
 
-Or you can download it from PyPi:
-
-    pip install TurtleMol
-
-TurtleMol is also available as a plugin for [Avogadro2](https://www.openchemistry.org/projects/avogadro2/)
-and can be installed via the following instructions.
-
-<img src="https://github.com/Dfilono/TurtleMol/blob/main/docs/images/installationPart1.png">
-
-<img src="https://github.com/Dfilono/TurtleMol/blob/main/docs/images/installationPart2.png">
-
-Note that for the plugin to function, the TurtleMol python package and its dependecies must also be installed
-in the same Python environment that is referenced by Avogadro.
-
-## Contributing
-
-We have a lot of wishlist features that can be seen [HERE](https://github.com/Dfilono/TurtleMol/blob/main/WISHLIST.md). If you want to help add any of these features, or others you think TurtleMol would benefit from, let me know! Submit a pull request with your update (please test it in your own fork first), and I'll check it!
+A PyPI version is in progress!
 
 ## Citation
 
 If you find this code helpful, please consider referencing it! We don't currently have a released article to cite,
 but any reference to our work helps acknowledge the effort put into developing and maintaining this code base, 
 provides support for further development!
```

#### html2text {}

```diff
@@ -1,13 +1,17 @@
-Metadata-Version: 2.1 Name: TurtleMol Version: 0.3.0 Summary: Design, create,
-and generate unique, complex molecular structures of any shape and size!
-Author: Dominick Filonowich Author-email: filonowichd74@gmail.com Requires-
-Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: trimesh Requires-
-Dist: rtree Requires-Dist: scipy Requires-Dist: pytest
+Metadata-Version: 2.1 Name: TurtleMol Version: 0.post0.dev1 Summary: Design,
+create, and generate unique, complex molecular structures of any shape and
+size! Author: Dominick Filonowich Author-email: filonowichd74@gmail.com
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Science/Research Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Chemistry Requires-Python: >=3.7 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist:
+pandas Requires-Dist: pytest
                             ************ TTuurrttlleeMMooll ************
  ****** DDeessiiggnn,, ccrreeaattee,, aanndd ggeenneerraattee uunniiqquuee,, ccoommpplleexx mmoolleeccuullaarr ssttrruuccttuurreess ooff aannyy
                               sshhaappee aanndd ssiizzee!! ******
     _[_B_u_i_l_d_ _S_t_a_t_u_s_ _]_[_C_o_d_e_c_o_v_]_[_L_i_c_e_n_s_e_]_[_R_e_p_o_ _s_i_z_e_]_[_B_l_a_c_k_ _s_t_y_l_e_]_[_B_l_a_c_k_ _s_t_y_l_e_]
 ## Introduction The goal of TurtleMol is to ease the process of generating
 unique and complex molecular structures for computational chemistry. Available
 as a standalone python-package, or as a plugin for [Avogadro2](https://
@@ -28,28 +32,16 @@
 molecules - Generate a box or sphere of molecules around an existing molecular
 structure - Fill a volume, or place a specfied number of molecules in space -
 Randomly orient molecules to better represent an equilibrium structure - Read/
 Write structures from XYZ and PDB formats ## Features in Progress - Generate
 structures based on meshes defined from outside software/packagaes such as
 Blender ## Installation You can install the latest development version of
 TurtleMol from the [Github Repository](https://github.com/Dfilono/TurtleMol).
-git clone https://github.com/Dfilono/TurtleMol cd TurtleMol pip install . Or
-you can download it from PyPi: pip install TurtleMol TurtleMol is also
-available as a plugin for [Avogadro2](https://www.openchemistry.org/projects/
-avogadro2/) and can be installed via the following instructions. [https://
-github.com/Dfilono/TurtleMol/blob/main/docs/images/installationPart1.png]
-[https://github.com/Dfilono/TurtleMol/blob/main/docs/images/
-installationPart2.png]Note that for the plugin to function, the TurtleMol
-python package and its dependecies must also be installed in the same Python
-environment that is referenced by Avogadro. ## Contributing We have a lot of
-wishlist features that can be seen [HERE](https://github.com/Dfilono/TurtleMol/
-blob/main/WISHLIST.md). If you want to help add any of these features, or
-others you think TurtleMol would benefit from, let me know! Submit a pull
-request with your update (please test it in your own fork first), and I'll
-check it! ## Citation If you find this code helpful, please consider
-referencing it! We don't currently have a released article to cite, but any
-reference to our work helps acknowledge the effort put into developing and
-maintaining this code base, provides support for further development! ##
+git clone https://github.com/Dfilono/TurtleMol cd TurtleMol pip install . A
+PyPI version is in progress! ## Citation If you find this code helpful, please
+consider referencing it! We don't currently have a released article to cite,
+but any reference to our work helps acknowledge the effort put into developing
+and maintaining this code base, provides support for further development! ##
 License Distributed under the MIT License. See [LICENSE](https://github.com/
 Dfilono/TurtleMol/blob/main/LICENSE) for more information. ## Documentation
 Documentation is in progress.[https://github.com/Dfilono/TurtleMol/blob/main/
 docs/images/logo.png]
```

### Comparing `turtlemol-0.3.0/README.md` & `TurtleMol-0.post0.dev1/TurtleMol.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: TurtleMol
+Version: 0.post0.dev1
+Summary: Design, create, and generate unique, complex molecular structures of any shape and size!
+Author: Dominick Filonowich
+Author-email: filonowichd74@gmail.com
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pytest
+
 <h1 align='center'>TurtleMol</h1>
 <h4 align='center'>Design, create, and generate unique, complex molecular structures of any shape and size!</h4>
 
 
 
 <p align="center">
     <a href="https://github.com/Dfilono/TurtleMol/actions/workflows/python-package.yml">
@@ -60,31 +80,15 @@
 
 You can install the latest development version of TurtleMol from the [Github Repository](https://github.com/Dfilono/TurtleMol).
 
     git clone https://github.com/Dfilono/TurtleMol
     cd TurtleMol
     pip install .
 
-Or you can download it from PyPi:
-
-    pip install TurtleMol
-
-TurtleMol is also available as a plugin for [Avogadro2](https://www.openchemistry.org/projects/avogadro2/)
-and can be installed via the following instructions.
-
-<img src="https://github.com/Dfilono/TurtleMol/blob/main/docs/images/installationPart1.png">
-
-<img src="https://github.com/Dfilono/TurtleMol/blob/main/docs/images/installationPart2.png">
-
-Note that for the plugin to function, the TurtleMol python package and its dependecies must also be installed
-in the same Python environment that is referenced by Avogadro.
-
-## Contributing
-
-We have a lot of wishlist features that can be seen [HERE](https://github.com/Dfilono/TurtleMol/blob/main/WISHLIST.md). If you want to help add any of these features, or others you think TurtleMol would benefit from, let me know! Submit a pull request with your update (please test it in your own fork first), and I'll check it!
+A PyPI version is in progress!
 
 ## Citation
 
 If you find this code helpful, please consider referencing it! We don't currently have a released article to cite,
 but any reference to our work helps acknowledge the effort put into developing and maintaining this code base, 
 provides support for further development!
```

#### html2text {}

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1 Name: TurtleMol Version: 0.post0.dev1 Summary: Design,
+create, and generate unique, complex molecular structures of any shape and
+size! Author: Dominick Filonowich Author-email: filonowichd74@gmail.com
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Science/Research Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Chemistry Requires-Python: >=3.7 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist:
+pandas Requires-Dist: pytest
                             ************ TTuurrttlleeMMooll ************
  ****** DDeessiiggnn,, ccrreeaattee,, aanndd ggeenneerraattee uunniiqquuee,, ccoommpplleexx mmoolleeccuullaarr ssttrruuccttuurreess ooff aannyy
                               sshhaappee aanndd ssiizzee!! ******
     _[_B_u_i_l_d_ _S_t_a_t_u_s_ _]_[_C_o_d_e_c_o_v_]_[_L_i_c_e_n_s_e_]_[_R_e_p_o_ _s_i_z_e_]_[_B_l_a_c_k_ _s_t_y_l_e_]_[_B_l_a_c_k_ _s_t_y_l_e_]
 ## Introduction The goal of TurtleMol is to ease the process of generating
 unique and complex molecular structures for computational chemistry. Available
 as a standalone python-package, or as a plugin for [Avogadro2](https://
@@ -22,28 +32,16 @@
 molecules - Generate a box or sphere of molecules around an existing molecular
 structure - Fill a volume, or place a specfied number of molecules in space -
 Randomly orient molecules to better represent an equilibrium structure - Read/
 Write structures from XYZ and PDB formats ## Features in Progress - Generate
 structures based on meshes defined from outside software/packagaes such as
 Blender ## Installation You can install the latest development version of
 TurtleMol from the [Github Repository](https://github.com/Dfilono/TurtleMol).
-git clone https://github.com/Dfilono/TurtleMol cd TurtleMol pip install . Or
-you can download it from PyPi: pip install TurtleMol TurtleMol is also
-available as a plugin for [Avogadro2](https://www.openchemistry.org/projects/
-avogadro2/) and can be installed via the following instructions. [https://
-github.com/Dfilono/TurtleMol/blob/main/docs/images/installationPart1.png]
-[https://github.com/Dfilono/TurtleMol/blob/main/docs/images/
-installationPart2.png]Note that for the plugin to function, the TurtleMol
-python package and its dependecies must also be installed in the same Python
-environment that is referenced by Avogadro. ## Contributing We have a lot of
-wishlist features that can be seen [HERE](https://github.com/Dfilono/TurtleMol/
-blob/main/WISHLIST.md). If you want to help add any of these features, or
-others you think TurtleMol would benefit from, let me know! Submit a pull
-request with your update (please test it in your own fork first), and I'll
-check it! ## Citation If you find this code helpful, please consider
-referencing it! We don't currently have a released article to cite, but any
-reference to our work helps acknowledge the effort put into developing and
-maintaining this code base, provides support for further development! ##
+git clone https://github.com/Dfilono/TurtleMol cd TurtleMol pip install . A
+PyPI version is in progress! ## Citation If you find this code helpful, please
+consider referencing it! We don't currently have a released article to cite,
+but any reference to our work helps acknowledge the effort put into developing
+and maintaining this code base, provides support for further development! ##
 License Distributed under the MIT License. See [LICENSE](https://github.com/
 Dfilono/TurtleMol/blob/main/LICENSE) for more information. ## Documentation
 Documentation is in progress.[https://github.com/Dfilono/TurtleMol/blob/main/
 docs/images/logo.png]
```

### Comparing `turtlemol-0.3.0/TurtleMol/Box3D.py` & `TurtleMol-0.post0.dev1/TurtleMol/Box3D.py`

 * *Files identical despite different names*

### Comparing `turtlemol-0.3.0/TurtleMol/Sphere3D.py` & `TurtleMol-0.post0.dev1/TurtleMol/Sphere3D.py`

 * *Files identical despite different names*

### Comparing `turtlemol-0.3.0/TurtleMol/__init__.py` & `TurtleMol-0.post0.dev1/TurtleMol/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 # Top level package
 from .Box3D import Box3d, drawBox
 from .defaultParams import defaultParams
-from .drawMol import drawMolBox, drawMolSphere, drawMolMesh
-from .isOverlap import isOverlapAtom, isOverlapMolecule, isOverlapAtomKDTree, isOverlapMoleculeKDTree, buildKDTreeMapping
-from .makeStruc import makeBase, calcCenter, reCenter, shiftPoints, randReorient, calcDensity, calcNumMol, calcDistance
-from .readWriteFiles import getInput, readStrucFile, readPdb, writeOutput, writePdb, writeXYZ, getElementData, readMesh
+from .drawMol import drawMolBox, drawMolSphere
+from .isOverlap import isOverlapAtom, isOverlapMolecule
+from .makeStruc import makeBase, calcCenter, reCenter, shiftPoints, randReorient, calcDensity, calcNumMol
+from .readWriteFiles import getInput, readStrucFile, readPdb, writeOutput, writePdb, writeXYZ, getElementData
 from .setAtomProp import setAtomicMass, setAtomicRadius
 from .shiftBox import atomsFillBox, atomsRandBox, moleculesFillBox, moleculesRandBox, inBox
 from .shiftSphere import atomFillSphere, atomRandSphere, moleculeFillSphere, moleculeRandSphere
 from .Sphere3D import Sphere3d
-from .shiftDensity import placeMols
-from .mesh3D import mesh3D
-from .shiftMesh import atomsFillMesh, moleculesFillMesh, atomsRandMesh, moleculesRandMesh
-from .shiftUnitCell import unitCellBox, unitCellSphere, unitCellMesh
-
 from . import _version
 __version__ = _version.get_versions()['version']
```

### Comparing `turtlemol-0.3.0/TurtleMol/__main__.py` & `TurtleMol-0.post0.dev1/TurtleMol/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''Module contains the main loop'''
 
 import sys
 import argparse
-from drawMol import drawMolBox, drawMolSphere, drawMolMesh
-from readWriteFiles import writeOutput, getInput, readStrucFile
-from defaultParams import defaultParams
+from .drawMol import drawMolBox, drawMolSphere
+from .readWriteFiles import writeOutput, getInput, readStrucFile
+from .defaultParams import defaultParams
 
 def parseCommandLine(dparams):
     '''Parses command line for parameters'''
     parser = argparse.ArgumentParser(description='Tile Fill')
 
     # Command line arguemnnts
     parser.add_argument('-i', '--inputFile', type=str, help="Path to input file")
@@ -39,28 +39,24 @@
     parser.add_argument('-baseCenter', '--baseStrucCenter', nargs='+', type=float,
                         help="X, Y, Z coordinates of the center of the base structure",
                         default=dparams['baseStrucCenter'])
     parser.add_argument('-n', '--numMolecules', type=int,
                         help="Number of molecules", default=dparams['numMolecules'])
     parser.add_argument('-t', '--tol', type=float,
                         help="Minimum distance between molecules", default=dparams['tol'])
-    parser.add_argument('-rho', '--density', type=float,
+    parser.add_argument('-rho', '--denisty', type=float,
                         help="Density in g/mL", default=dparams['density'])
     parser.add_argument('-a', '--maxAttempts', type=int,
                         help="Maximum iterations for finite sized systems",
                         default=dparams['maxAttempts'])
     parser.add_argument('-ar', '--atomRadius', type=str,
                         help="What radius type to be used for atoms",
                         default=dparams['atomRadius'])
     parser.add_argument('-out', '--outputFile', type=str,
                         help="Path for output file if desired")
-    parser.add_argument('-mesh', '--mesh', type=str,
-                        help="Path for mesh file if desired")
-    parser.add_argument('-scale', '--meshScale', type=float,
-                        help="Uniform scale of mesh", default=dparams['meshScale'])
 
     return parser.parse_args()
 
 def main():
     '''The main loop'''
     # Init default params
     dparams = defaultParams()
@@ -82,59 +78,29 @@
     if not iparams['structureFile']:
         print('Please provide an initial structure')
         sys.exit()
 
     print(iparams)
 
     # Get structure
-    struc, unitCell = readStrucFile(iparams['structureFile'])
+    struc = readStrucFile(iparams['structureFile'])
     print(struc)
 
-    if unitCell:
-        iparams['unitCell'] = [unitCell['a'], unitCell['b'], unitCell['c']]
-
     if iparams['baseStrucFile']:
-        baseStruc, baseUnitCell = readStrucFile(iparams['baseStrucFile'])
+        baseStruc = readStrucFile(iparams['baseStrucFile'])
     else:
         baseStruc = None
 
     if iparams['shape'].lower() == 'box' or iparams['shape'].lower() == 'cube':
         # Generate the new structure
-
-        if unitCell:
-            outStruc, strucType, cellParams = drawMolBox(struc, baseStruc, iparams)
-        else:
-            outStruc, strucType = drawMolBox(struc, baseStruc, iparams)
+        outStruc, strucType = drawMolBox(struc, baseStruc, iparams)
+        print(len(outStruc))
 
     elif iparams['shape'].lower() == 'sphere':
         # Generate the new structure
+        outStruc, strucType = drawMolSphere(struc, baseStruc, iparams)
 
-        if unitCell:
-            outStruc, strucType, cellParams = drawMolSphere(struc, baseStruc, iparams)
-        else:
-            outStruc, strucType = drawMolSphere(struc, baseStruc, iparams)
-
-    elif iparams['shape'].lower() == 'mesh' and iparams['mesh'] is not None:
-        # Generate the new structure
-        outStruc = []
-
-#        if isinstance(iparams['mesh'], str):
-#            iparams['mesh'] = [iparams['mesh']]
-#
-#        for i in iparams['mesh']:
-
-        if unitCell:
-            outStrucTemp, strucType, cellParams = drawMolMesh(struc, baseStruc, iparams)
-            outStruc.append(outStrucTemp)
-        else:
-            outStrucTemp, strucType = drawMolMesh(struc, baseStruc, iparams)
-            outStruc.append(outStrucTemp)
-
-        
     if iparams['outputFile']:
-        if unitCell:
-            writeOutput(outStruc, iparams['outputFile'], strucType, cellParams)
-        else:
-            writeOutput(outStruc, iparams['outputFile'], strucType)
+        writeOutput(outStruc, iparams['outputFile'], strucType)
 
 if __name__ == "__main__":
     main()
```

### Comparing `turtlemol-0.3.0/TurtleMol/data/ElementData.csv` & `TurtleMol-0.post0.dev1/TurtleMol/data/ElementData.csv`

 * *Files identical despite different names*

### Comparing `turtlemol-0.3.0/TurtleMol/defaultParams.py` & `TurtleMol-0.post0.dev1/TurtleMol/defaultParams.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,13 +38,10 @@
         'maxAttempts' : 10000,
         'baseStrucCenter' : [0, 0, 0],
         'baseStrucFile' : None,
         'randomizeOrient' : False,
         'randFill' : False,
         'density' : None,
         'atomRadius' : 'AtomicRadius',
-        'mesh' : None,
-        'meshScale' : 1.0,
-        'unitCell' : None
     }
 
     return params
```

### Comparing `turtlemol-0.3.0/TurtleMol/drawMol.py` & `TurtleMol-0.post0.dev1/TurtleMol/drawMol.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,46 +5,35 @@
 A 'Fill' option was also added so that one could just define a space,
 and fill said space with provided structure as many times as it can fit.
 '''
 
 import math
 from .Box3D import Box3d, drawBox
 from .Sphere3D import Sphere3d
-from .mesh3D import mesh3D
 from .shiftBox import atomsFillBox, atomsRandBox, \
                      moleculesFillBox, moleculesRandBox
 from .shiftSphere import atomFillSphere, atomRandSphere, \
                         moleculeRandSphere, moleculeFillSphere
-from .shiftMesh import atomsFillMesh, moleculesFillMesh, atomsRandMesh, moleculesRandMesh
 from .setAtomProp import setAtomicRadius
-from .makeStruc import makeBase, shiftPoints
-from .shiftDensity import placeMols
-from .shiftUnitCell import unitCellBox, unitCellMesh, unitCellSphere
+from .makeStruc import makeBase, calcNumMol, shiftPoints
 
 def drawMolBox(struc, baseStruc, iparams):
     '''Utilized to place molecules in a box'''
     dims = drawBox(iparams)
     box = Box3d(0, 0, 0, dims)
     radii = setAtomicRadius(iparams['atomRadius'])
     numMol = iparams['numMolecules']
     tol = float(iparams['tol'])
 
     originalPoints = makeBase(struc)
 
     originalPoints = shiftPoints(originalPoints, box)
 
-    if iparams['unitCell']:
-        filled, strucType, cellParams = unitCellBox(box, dims, iparams['unitCell'], 
-                                        originalPoints, radii)
-        return filled, strucType, cellParams
-
     if iparams['density']:
-        filled, strucType = placeMols(box, originalPoints, iparams['density'],
-                                 tol, "box", radii, iparams['randomizeOrient'])
-        return filled, strucType
+        numMol = calcNumMol(box, originalPoints, iparams['density'])
 
     if not isinstance(numMol, int) and str(numMol).lower() != "fill":
         numMol = int(numMol)
 
     if iparams['randFill'] == 'False' or iparams['randFill'] is False:
         numXShifts = math.ceil(box.length / tol)
         numYShifts = math.ceil(box.height / tol)
@@ -84,23 +73,17 @@
     radii = setAtomicRadius(iparams['atomRadius'])
     numMol = iparams['numMolecules']
     tol = float(iparams['tol'])
 
     originalPoints = makeBase(struc)
     originalPoints = shiftPoints(originalPoints, sphere)
 
-    if iparams['unitCell']:
-        filled, strucType, cellParams = unitCellSphere(sphere, iparams['unitCell'], 
-                                        originalPoints, radii)
-        return filled, strucType, cellParams
-
     if iparams['density']:
-        filled, strucType = placeMols(sphere, originalPoints, iparams['density'],
-                                 tol, "sphere", radii, iparams['randomizeOrient'])
-        return filled, strucType
+        numMol = calcNumMol(sphere, originalPoints, iparams['density'])
+        print(numMol)
 
     if not isinstance(numMol, int) and str(numMol).lower() != "fill":
         numMol = int(numMol)
 
     if iparams['randFill'] == 'False' or iparams['randFill'] is False:
         numShifts = math.ceil(2*sphere.radius / tol)
 
@@ -127,51 +110,7 @@
         if len(originalPoints) > 1:
             filledAtom = moleculeRandSphere(numMol, iparams['maxAttempts'],
                                                 originalPoints, sphere, radii, tol, baseStruc,
                                                 iparams['randomizeOrient'])
             return list(filledAtom), "molecule"
 
     return "ERROR: No atoms found"
-
-def drawMolMesh(struc, baseStruc, iparams):
-    '''Places molecules in a mesh'''
-    mesh = mesh3D(iparams['mesh'], iparams['meshScale'])
-    radii = setAtomicRadius(iparams['atomRadius'])
-    numMol = iparams['numMolecules']
-    tol = float(iparams['tol'])
-
-    originalPoints = makeBase(struc)
-
-    if iparams['unitCell']:
-        filled, strucType, cellParams = unitCellMesh(mesh, iparams['unitCell'], 
-                                        originalPoints, radii)
-        return filled, strucType, cellParams
-
-    if iparams['density']:
-        filled, strucType = placeMols(mesh, originalPoints, iparams['density'],
-                                 tol, "mesh", radii, iparams['randomizeOrient'])
-        return filled, strucType
-
-    if not isinstance(numMol, int) and str(numMol).lower() != "fill":
-        numMol = int(numMol)
-
-    if iparams['randFill'] == 'False' or iparams['randFill'] is False:
-        if len(originalPoints) == 1:
-            filledAtom = atomsFillMesh(mesh, originalPoints, tol, radii, numMol)
-
-            return list(filledAtom), 'atom'
-        else:
-            filledMol = moleculesFillMesh(mesh, originalPoints, tol,
-                                          radii, numMol, baseStruc, iparams['randomizeOrient'])
-            
-            return list(filledMol), 'molecule'
-
-    elif iparams['randFill'] == 'True' or iparams['randFill'] is True:
-        if len(originalPoints) == 1:
-            filledAtom = atomsRandMesh(mesh, originalPoints, tol, radii, numMol,
-                                       iparams['maxAttempts'])
-            return list(filledAtom), 'atom'
-        else:
-            filledMol = moleculesRandMesh(mesh, originalPoints, tol, radii, numMol,
-                                          baseStruc, iparams['randomizeOrient'],
-                                          iparams['maxAttempts'])
-            return list(filledMol), 'molecule'
```

### Comparing `turtlemol-0.3.0/TurtleMol/readWriteFiles.py` & `TurtleMol-0.post0.dev1/TurtleMol/readWriteFiles.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Since both the input and output files are optional, these functions can be avoided.
 The structure file is required however, and currently the only supported format is xyz files.
 Data on elements is also imported and searchable. Primary use at this time is for the atomic radius
 '''
 
 import os
 import pandas as pd
-import trimesh
 
 def getInput(filePath):
     '''Reads input file if provided'''
     params = {}
     with open(filePath, encoding = 'utf-8') as f:
         for line in f:
             key, value = line.strip().split('=')
@@ -20,41 +19,29 @@
     return params
 
 def readStrucFile(filePath):
     '''Reads structure file'''
     # Reads XYZ
     if filePath[-3:] == 'xyz':
         return pd.read_csv(filePath, delim_whitespace=True,
-                           skiprows=2, names=["Atom", "X", "Y", "Z"]), None
+                           skiprows=2, names=["Atom", "X", "Y", "Z"])
     # Reads PDB
     if filePath[-3:] == 'pdb':
         return readPdb(filePath)
 
     return f"ERROR: Issue generating file to {filePath}"
 
 def readPdb(filePath):
     '''Reads structure file if a pdb'''
     data = []
-    unitCell = None
     symbols = getElementData('AtomicMass')
 
     with open(filePath, 'r', encoding = 'utf-8') as pdbFile:
         for line in pdbFile:
-
-            if line.startswith('CRYST1'):
-                # Extract unit cell parameters from the CRYST1 line
-                a = float(line[6:15].strip())
-                b = float(line[15:24].strip())
-                c = float(line[24:33].strip())
-                alpha = float(line[33:40].strip())
-                beta = float(line[40:47].strip())
-                gamma = float(line[47:54].strip())
-                unitCell = {'a': a, 'b': b, 'c': c, 'alpha': alpha, 'beta': beta, 'gamma': gamma}
-
-            elif line.startswith('ATOM') or line.startswith('HETATM'):
+            if line.startswith('ATOM') or line.startswith('HETATM'):
                 # Parse relevant fields from the PDB format
                 atomName = line[12:16].strip()
                 element = line[76:78].strip()
 
                 if element not in symbols['Symbol']:
                     element = atomName
 
@@ -67,50 +54,38 @@
                 residueName = line[17:20].strip()
                 residueSeq = int(line[22:26].strip())
 
                 data.append([element, x, y, z, residueName, residueSeq])
 
     df = pd.DataFrame(data, columns=['Atom', 'X', 'Y', 'Z', 'Residue', 'ResidueSeq'])
 
-    return df, unitCell
+    return df
 
-def readMesh(filePath):
-    '''Reads mesh files in format like .obj, .stl, .ply'''
-    mesh = trimesh.load(filePath)
-    return mesh
-
-def writeOutput(data, filePath, strucType, cellParams=None):
+def writeOutput(data, filePath, strucType):
     '''Writes data to output file'''
     try:
         # Writes XYZ
         if filePath[-3:] == 'xyz':
             writeXYZ(data, filePath, strucType)
         # Writes PDB
         elif filePath[-3:] == 'pdb':
-            if cellParams != None:
-                writePdb(data, filePath, cellParams)
-            else:
-                writePdb(data, filePath)
+            writePdb(data, filePath)
     except KeyError:
         print(f"Filetype {filePath[-3:]} not supported\n")
 
-def writePdb(data, filePath, cellParams=None):
+def writePdb(data, filePath):
     '''Writes a pdb file from results'''
     template = (
-        "HETATM{atomNum:5d} {atomType:>2}  {residueName:>3} A{resNum: >4d}"
-        "    {x: >8.3f}{y: >8.3f}{z: >8.3f}{occupancy: >6.2f}{tempFactor: >6.2f}\n"
+        "HETATM{atomNum:5d} {atomType:^4}{residueName:<4} A{resNum:4d}"
+        "    {x:8.3f}{y:8.3f}{z:8.3f}{occupancy:6.2f}{tempFactor:6.2f}\n"
         )
 
     with open(filePath, 'w', encoding = 'utf-8') as pdbFile:
         atomNum = 1
         resNum = 1
-        cell = cellParams
-
-        if cell != None:
-            pdbFile.write(cell + '\n')
 
         for mol in data:
             for atom in mol:
                 pdbFile.write(template.format(
                    atomNum = atomNum,
                    atomType = atom[0],
                    residueName = atom[4],
```

### Comparing `turtlemol-0.3.0/TurtleMol/setAtomProp.py` & `TurtleMol-0.post0.dev1/TurtleMol/setAtomProp.py`

 * *Files identical despite different names*

### Comparing `turtlemol-0.3.0/TurtleMol/shiftSphere.py` & `TurtleMol-0.post0.dev1/TurtleMol/shiftSphere.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 '''Module places molecules in a sphere'''
 
 import random
-import scipy.spatial
-import numpy as np
-from .isOverlap import isOverlapAtomKDTree, isOverlapMoleculeKDTree, buildKDTreeMapping
+from .isOverlap import isOverlapAtom, isOverlapMolecule
 from .makeStruc import makeBase, reCenter, randReorient
 
 def atomFillSphere(numShifts, sphere, og, radii, tol, numMol):
     '''Fills sphere with single atoms'''
     filled = []
 
     if str(numMol).lower() == 'fill':
         numMol = 10000000000000
 
-    # Create KD-tree for filledAtoms
-    kdTree, indexToAtom = buildKDTreeMapping(filled, radii)
-
     for zShifts in range(numShifts):
         for yShifts in range(numShifts):
             for xShifts in range(numShifts):
                 for atom in og:
                     # Calculate the relative position of each atom within the molecule
                     relX = atom[1]
                     relY = atom[2]
@@ -37,31 +32,25 @@
                     # Check if the new atom fits within the sphere
                     if sphere.containsPoints(x, y, z, atomRadius):
                         if len(atom) == 5:
                             newAtom = (atom[0], x, y, z, atom[4])
                         else:
                             newAtom = (atom[0], x, y, z)
 
-                        if (kdTree is None or not isOverlapAtomKDTree(newAtom, kdTree, indexToAtom, radii, tol)) and \
+                        if not isOverlapAtom(newAtom, filled, radii, tol) and \
                             numMol > len(filled):
                             filled.append(newAtom)
 
-                            # Rebuild KDTree with newly added atoms
-                            kdTree, indexToAtom = buildKDTreeMapping(filled, radii)
-
     return filled
 
 def atomRandSphere(numMol, maxAttempts, og, sphere, radii, tol):
     '''Places a defined number of atoms in a sphere'''
     filled = []
     attempts = 0
 
-    # Create KD-tree for filledAtoms
-    kdTree, indexToAtom = buildKDTreeMapping(filled, radii)
-
     while len(filled) < numMol and attempts <= maxAttempts:
         for atom in og:
 
             # Calculate the shift for each tile and new point
             newX = atom[1] + random.uniform((sphere.xCoord - sphere.radius),
                                             (sphere.xCoord + sphere.radius))
             newY = atom[2] + random.uniform((sphere.yCoord - sphere.radius),
@@ -76,20 +65,17 @@
             # Check if the new atom fits within the sphere
             if sphere.containsPoints(newX, newY, newZ, atomRadius):
                 if len(atom) == 5:
                     newAtom = (atom[0], newX, newY, newZ, atom[4])
                 else:
                     newAtom = (atom[0], newX, newY, newZ)
 
-                if (kdTree is None or not isOverlapAtomKDTree(newAtom, kdTree, indexToAtom, radii, tol)):
+                if not isOverlapAtom(newAtom, filled, radii, tol):
                     filled.append(newAtom)
 
-                    # Rebuild KDTree with newly added atoms
-                    kdTree, indexToAtom = buildKDTreeMapping(filled, radii)
-
         attempts += 1
 
     return list(filled)
 
 def moleculeFillSphere(numShifts, sphere, og, radii, tol,
                        baseStruc, randOrient, numMol):
     '''Fills sphere with molecules'''
@@ -98,17 +84,14 @@
     if str(numMol).lower() == 'fill':
         numMol = 10000000000000
 
     if baseStruc is not None:
         base = makeBase(baseStruc)
         filled.append(reCenter(base, sphere))
 
-    # Create KD-tree for filledAtoms
-    kdTree, indexToAtom = buildKDTreeMapping(filled, radii)
-
     for zShifts in range(numShifts):
         for yShifts in range(numShifts):
             for xShifts in range(numShifts):
                 newMol = []
 
                 for atom in og:
                     # Calculate the relative position of each atom within the molecule
@@ -134,36 +117,30 @@
                         newMol.append(newAtom)
                     else:
                         break # If any atom doesn't fit, discard the whol molecule
 
                 if randOrient and len(newMol) == len(og):
                     newMol = randReorient(newMol)
 
-                if (kdTree is None or not isOverlapMoleculeKDTree(newMol, kdTree, indexToAtom, radii, tol)) and \
+                if not isOverlapMolecule(newMol, filled, radii, tol) and \
                     numMol > len(filled):
                     if len(newMol) == len(og):
                         filled.append(newMol)
-
-                        # Rebuild KDTree with newly added atoms
-                        kdTree, indexToAtom = buildKDTreeMapping(filled, radii)
     return filled
 
 def moleculeRandSphere(numMol, maxAttempts, og, sphere, radii, tol,
                            baseStruc, randOrient):
     '''Places a defined number of molecules in a sphere'''
     filled = []
     attempts = 0
 
     if baseStruc is not None:
         base = makeBase(baseStruc)
         filled.append(reCenter(base, sphere))
 
-    # Create KD-tree for filledAtoms
-    kdTree, indexToAtom = buildKDTreeMapping(filled, radii)
-
     while len(filled) < numMol and attempts <= maxAttempts:
         newMol = []
 
         shiftX = 0
         shiftY = 0
         shiftZ = 0
 
@@ -192,17 +169,14 @@
                 newMol.append(newAtom)
             else:
                 break # If any atom doesn't fit, discard the whol molecule
 
         if randOrient and len(newMol) == len(og):
             newMol = randReorient(newMol)
 
-        if (kdTree is None or not isOverlapMoleculeKDTree(newMol, kdTree, indexToAtom, radii, tol)):
+        if not isOverlapMolecule(newMol, filled, radii, tol):
             if len(newMol) == len(og):
                 filled.append(newMol)
 
-                # Rebuild KDTree with newly added atoms
-                kdTree, indexToAtom = buildKDTreeMapping(filled, radii)
-
         attempts += 1
 
     return list(filled)
```

### Comparing `turtlemol-0.3.0/TurtleMol.egg-info/SOURCES.txt` & `TurtleMol-0.post0.dev1/TurtleMol.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,18 @@
 TurtleMol/__init__.py
 TurtleMol/__main__.py
 TurtleMol/_version.py
 TurtleMol/defaultParams.py
 TurtleMol/drawMol.py
 TurtleMol/isOverlap.py
 TurtleMol/makeStruc.py
-TurtleMol/mesh3D.py
 TurtleMol/readWriteFiles.py
 TurtleMol/setAtomProp.py
 TurtleMol/shiftBox.py
-TurtleMol/shiftDensity.py
-TurtleMol/shiftMesh.py
 TurtleMol/shiftSphere.py
-TurtleMol/shiftUnitCell.py
 TurtleMol.egg-info/PKG-INFO
 TurtleMol.egg-info/SOURCES.txt
 TurtleMol.egg-info/dependency_links.txt
 TurtleMol.egg-info/not-zip-safe
 TurtleMol.egg-info/requires.txt
 TurtleMol.egg-info/top_level.txt
 TurtleMol/data/ElementData.csv
```

### Comparing `turtlemol-0.3.0/setup.py` & `TurtleMol-0.post0.dev1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from setuptools import setup, find_packages
 import versioneer
 
 requirements = [
     'numpy',
     'pandas',
-    'trimesh',
-    'rtree',
-    'scipy',
 ]
 
 setup_requirements = []
 test_requirements = requirements.append(['pytest'])
 
 setup(
     python_requires = '>=3.7',
```

### Comparing `turtlemol-0.3.0/tests/test_BaseStruc.py` & `TurtleMol-0.post0.dev1/tests/test_BaseStruc.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,18 @@
     for name in dparams:
         if name not in iparamsSphere:
             iparamsSphere[name] = dparams[name]
 
         if name not in iparamsCube:
             iparamsCube[name] = dparams[name]
 
-    struc, unitCell = readStrucFile(iparamsSphere['structureFile'])
+    struc = readStrucFile(iparamsSphere['structureFile'])
 
     if iparamsSphere['baseStrucFile']:
-        baseStruc, baseUnitCell = readStrucFile(iparamsSphere['baseStrucFile'])
+        baseStruc = readStrucFile(iparamsSphere['baseStrucFile'])
     else:
         baseStruc = None
 
     outStrucCube, strucTypeCube = drawMolBox(struc, baseStruc, iparamsCube)
     assert len(outStrucCube) != 0, "Output structure should have some length"
     assert strucTypeCube == "molecule", "Structure type should be an atom"
```

### Comparing `turtlemol-0.3.0/tests/test_atomFill.py` & `TurtleMol-0.post0.dev1/tests/test_atomRandomPlace.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 
 # pylin: skip-file
 
 from TurtleMol.drawMol import drawMolBox, drawMolSphere
 from TurtleMol.readWriteFiles import readStrucFile
 from TurtleMol.defaultParams import defaultParams
 
-def testAtomFill():
+def testRandomPlace():
     iparamsSphere = {
         'shape' : 'sphere',
         'radius' : 5.0,
-        'numMolecules' : 'fill',
+        'numMolecules' : '20',
+        'randFill' : True,
         'structureFile' : "TurtleMol/examples/Argon/argon.xyz"
     }
 
     iparamsCube = {
         'shape' : 'cube',
         'sideLength' : 10.0,
-        'numMolecules' : 'fill',
+        'numMolecules' : '20',
+        'randFill' : True,
         'structureFile' : "TurtleMol/examples/Argon/argon.xyz"
     }
 
     dparams = defaultParams()
 
     for name in dparams:
         if name not in iparamsSphere:
             iparamsSphere[name] = dparams[name]
 
         if name not in iparamsCube:
             iparamsCube[name] = dparams[name]
 
-    struc, unitCell = readStrucFile(iparamsSphere['structureFile'])
+    struc = readStrucFile(iparamsSphere['structureFile'])
 
     if iparamsSphere['baseStrucFile']:
         baseStruc = readStrucFile(iparamsSphere['baseStrucFile'])
     else:
         baseStruc = None
 
-    print(iparamsCube)
-
     outStrucCube, strucTypeCube = drawMolBox(struc, baseStruc, iparamsCube)
     assert len(outStrucCube) != 0, "Output structure should have some length"
     assert strucTypeCube == "atom", "Structure type should be an atom"
 
     outStrucSphere, strucTypeSphere = drawMolSphere(struc, baseStruc, iparamsSphere)
     assert len(outStrucSphere) != 0, "Output structure should have some length"
     assert strucTypeSphere == "atom", "Structure type should be an atom"
```

### Comparing `turtlemol-0.3.0/tests/test_atomRandomPlace.py` & `TurtleMol-0.post0.dev1/tests/test_moleculeFill.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,47 +2,45 @@
 
 # pylin: skip-file
 
 from TurtleMol.drawMol import drawMolBox, drawMolSphere
 from TurtleMol.readWriteFiles import readStrucFile
 from TurtleMol.defaultParams import defaultParams
 
-def testRandomPlace():
+def testMoleculeFill():
     iparamsSphere = {
         'shape' : 'sphere',
         'radius' : 5.0,
-        'numMolecules' : '20',
-        'randFill' : True,
-        'structureFile' : "TurtleMol/examples/Argon/argon.xyz"
+        'numMolecules' : 'fill',
+        'structureFile' : "TurtleMol/examples/Water/water.xyz"
     }
 
     iparamsCube = {
         'shape' : 'cube',
         'sideLength' : 10.0,
-        'numMolecules' : '20',
-        'randFill' : True,
-        'structureFile' : "TurtleMol/examples/Argon/argon.xyz"
+        'numMolecules' : 'fill',
+        'structureFile' : "TurtleMol/examples/Water/water.xyz"
     }
 
     dparams = defaultParams()
 
     for name in dparams:
         if name not in iparamsSphere:
             iparamsSphere[name] = dparams[name]
 
         if name not in iparamsCube:
             iparamsCube[name] = dparams[name]
 
-    struc, unitCell = readStrucFile(iparamsSphere['structureFile'])
+    struc = readStrucFile(iparamsSphere['structureFile'])
 
     if iparamsSphere['baseStrucFile']:
         baseStruc = readStrucFile(iparamsSphere['baseStrucFile'])
     else:
         baseStruc = None
 
     outStrucCube, strucTypeCube = drawMolBox(struc, baseStruc, iparamsCube)
     assert len(outStrucCube) != 0, "Output structure should have some length"
-    assert strucTypeCube == "atom", "Structure type should be an atom"
+    assert strucTypeCube == "molecule", "Structure type should be an atom"
 
     outStrucSphere, strucTypeSphere = drawMolSphere(struc, baseStruc, iparamsSphere)
     assert len(outStrucSphere) != 0, "Output structure should have some length"
-    assert strucTypeSphere == "atom", "Structure type should be an atom"
+    assert strucTypeSphere == "molecule", "Structure type should be an atom"
```

### Comparing `turtlemol-0.3.0/tests/test_moleculeFill.py` & `TurtleMol-0.post0.dev1/tests/test_moleculeRandomPlace.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,39 +2,41 @@
 
 # pylin: skip-file
 
 from TurtleMol.drawMol import drawMolBox, drawMolSphere
 from TurtleMol.readWriteFiles import readStrucFile
 from TurtleMol.defaultParams import defaultParams
 
-def testMoleculeFill():
+def testMoleculeRandomPlace():
     iparamsSphere = {
         'shape' : 'sphere',
         'radius' : 5.0,
-        'numMolecules' : 'fill',
+        'numMolecules' : 20,
+        'randFill' : True,
         'structureFile' : "TurtleMol/examples/Water/water.xyz"
     }
 
     iparamsCube = {
         'shape' : 'cube',
         'sideLength' : 10.0,
-        'numMolecules' : 'fill',
+        'numMolecules' : 20,
+        'randFill' : True,
         'structureFile' : "TurtleMol/examples/Water/water.xyz"
     }
 
     dparams = defaultParams()
 
     for name in dparams:
         if name not in iparamsSphere:
             iparamsSphere[name] = dparams[name]
 
         if name not in iparamsCube:
             iparamsCube[name] = dparams[name]
 
-    struc, unitCell = readStrucFile(iparamsSphere['structureFile'])
+    struc = readStrucFile(iparamsSphere['structureFile'])
 
     if iparamsSphere['baseStrucFile']:
         baseStruc = readStrucFile(iparamsSphere['baseStrucFile'])
     else:
         baseStruc = None
 
     outStrucCube, strucTypeCube = drawMolBox(struc, baseStruc, iparamsCube)
```

### Comparing `turtlemol-0.3.0/tests/test_moleculeRandomPlace.py` & `TurtleMol-0.post0.dev1/tests/test_randOrient.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 
 # pylin: skip-file
 
 from TurtleMol.drawMol import drawMolBox, drawMolSphere
 from TurtleMol.readWriteFiles import readStrucFile
 from TurtleMol.defaultParams import defaultParams
 
-def testMoleculeRandomPlace():
+def testRandOrient():
     iparamsSphere = {
         'shape' : 'sphere',
         'radius' : 5.0,
-        'numMolecules' : 20,
-        'randFill' : True,
+        'numMolecules' : 'fill',
+        'randomizeOrient' : True,
         'structureFile' : "TurtleMol/examples/Water/water.xyz"
     }
 
     iparamsCube = {
         'shape' : 'cube',
         'sideLength' : 10.0,
-        'numMolecules' : 20,
-        'randFill' : True,
+        'numMolecules' : 'fill',
+        'randomizeOrient' : True,
         'structureFile' : "TurtleMol/examples/Water/water.xyz"
     }
 
     dparams = defaultParams()
 
     for name in dparams:
         if name not in iparamsSphere:
             iparamsSphere[name] = dparams[name]
 
         if name not in iparamsCube:
             iparamsCube[name] = dparams[name]
 
-    struc, unitCell = readStrucFile(iparamsSphere['structureFile'])
+    struc = readStrucFile(iparamsSphere['structureFile'])
 
     if iparamsSphere['baseStrucFile']:
-        baseStruc, baseUnitCell = readStrucFile(iparamsSphere['baseStrucFile'])
+        baseStruc = readStrucFile(iparamsSphere['baseStrucFile'])
     else:
         baseStruc = None
 
     outStrucCube, strucTypeCube = drawMolBox(struc, baseStruc, iparamsCube)
     assert len(outStrucCube) != 0, "Output structure should have some length"
     assert strucTypeCube == "molecule", "Structure type should be an atom"
```

### Comparing `turtlemol-0.3.0/tests/test_randOrient.py` & `TurtleMol-0.post0.dev1/tests/test_readWritePDB.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 
 # pylin: skip-file
 
 from TurtleMol.drawMol import drawMolBox, drawMolSphere
 from TurtleMol.readWriteFiles import readStrucFile
 from TurtleMol.defaultParams import defaultParams
 
-def testRandOrient():
+def testReadWritePDB():
     iparamsSphere = {
         'shape' : 'sphere',
         'radius' : 5.0,
         'numMolecules' : 'fill',
-        'randomizeOrient' : True,
-        'structureFile' : "TurtleMol/examples/Water/water.xyz"
+        'structureFile' : "TurtleMol/examples/Water/water.pdb"
     }
 
     iparamsCube = {
         'shape' : 'cube',
         'sideLength' : 10.0,
         'numMolecules' : 'fill',
-        'randomizeOrient' : True,
-        'structureFile' : "TurtleMol/examples/Water/water.xyz"
+        'structureFile' : "TurtleMol/examples/Water/water.pdb"
     }
 
     dparams = defaultParams()
 
     for name in dparams:
         if name not in iparamsSphere:
             iparamsSphere[name] = dparams[name]
 
         if name not in iparamsCube:
             iparamsCube[name] = dparams[name]
 
-    struc, unitCell = readStrucFile(iparamsSphere['structureFile'])
+    struc = readStrucFile(iparamsSphere['structureFile'])
 
     if iparamsSphere['baseStrucFile']:
         baseStruc = readStrucFile(iparamsSphere['baseStrucFile'])
     else:
         baseStruc = None
 
     outStrucCube, strucTypeCube = drawMolBox(struc, baseStruc, iparamsCube)
     assert len(outStrucCube) != 0, "Output structure should have some length"
     assert strucTypeCube == "molecule", "Structure type should be an atom"
+    assert isinstance(outStrucCube[0][0][-1], str), 'Final place should be residue ID'
 
     outStrucSphere, strucTypeSphere = drawMolSphere(struc, baseStruc, iparamsSphere)
     assert len(outStrucSphere) != 0, "Output structure should have some length"
-    assert strucTypeSphere == "molecule", "Structure type should be an atom"
+    assert strucTypeSphere == "molecule", "Structure type should be an atom"
+    assert isinstance(outStrucSphere[0][0][-1], str), 'Final place should be residue ID'
```

### Comparing `turtlemol-0.3.0/versioneer.py` & `TurtleMol-0.post0.dev1/versioneer.py`

 * *Files identical despite different names*

