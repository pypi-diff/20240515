# Comparing `tmp/local_determinacy-0.1.2.tar.gz` & `tmp/local_determinacy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_determinacy-0.1.2.tar", last modified: Mon May 13 08:04:44 2024, max compression
+gzip compressed data, was "local_determinacy-0.1.3.tar", last modified: Wed May 15 11:56:08 2024, max compression
```

## Comparing `local_determinacy-0.1.2.tar` & `local_determinacy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:04:44.516808 local_determinacy-0.1.2/
--rw-r--r--   0 alfredlov   (502) staff       (20)     1092 2024-05-06 07:04:05.000000 local_determinacy-0.1.2/LICENSE
--rw-r--r--   0 alfredlov   (502) staff       (20)     5902 2024-05-13 08:04:44.516428 local_determinacy-0.1.2/PKG-INFO
--rw-r--r--   0 alfredlov   (502) staff       (20)     5269 2024-05-13 07:59:53.000000 local_determinacy-0.1.2/README.md
--rw-r--r--   0 alfredlov   (502) staff       (20)      856 2024-05-13 08:04:30.000000 local_determinacy-0.1.2/pyproject.toml
--rw-r--r--   0 alfredlov   (502) staff       (20)       38 2024-05-13 08:04:44.516875 local_determinacy-0.1.2/setup.cfg
-drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:04:44.511890 local_determinacy-0.1.2/src/
-drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:04:44.513530 local_determinacy-0.1.2/src/local_determinacy/
--rw-r--r--   0 alfredlov   (502) staff       (20)       24 2024-05-10 13:00:49.000000 local_determinacy-0.1.2/src/local_determinacy/__init__.py
--rw-r--r--   0 alfredlov   (502) staff       (20)     4747 2024-05-13 08:04:24.000000 local_determinacy-0.1.2/src/local_determinacy/functions.py
-drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:04:44.516084 local_determinacy-0.1.2/src/local_determinacy.egg-info/
--rw-r--r--   0 alfredlov   (502) staff       (20)     5902 2024-05-13 08:04:44.000000 local_determinacy-0.1.2/src/local_determinacy.egg-info/PKG-INFO
--rw-r--r--   0 alfredlov   (502) staff       (20)      281 2024-05-13 08:04:44.000000 local_determinacy-0.1.2/src/local_determinacy.egg-info/SOURCES.txt
--rw-r--r--   0 alfredlov   (502) staff       (20)        1 2024-05-13 08:04:44.000000 local_determinacy-0.1.2/src/local_determinacy.egg-info/dependency_links.txt
--rw-r--r--   0 alfredlov   (502) staff       (20)       18 2024-05-13 08:04:44.000000 local_determinacy-0.1.2/src/local_determinacy.egg-info/top_level.txt
+drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-15 11:56:08.819737 local_determinacy-0.1.3/
+-rw-r--r--   0 alfredlov   (502) staff       (20)     1092 2024-05-06 07:04:05.000000 local_determinacy-0.1.3/LICENSE
+-rw-r--r--   0 alfredlov   (502) staff       (20)     5886 2024-05-15 11:56:08.819358 local_determinacy-0.1.3/PKG-INFO
+-rw-r--r--   0 alfredlov   (502) staff       (20)     5253 2024-05-15 11:53:39.000000 local_determinacy-0.1.3/README.md
+-rw-r--r--   0 alfredlov   (502) staff       (20)      856 2024-05-15 11:55:58.000000 local_determinacy-0.1.3/pyproject.toml
+-rw-r--r--   0 alfredlov   (502) staff       (20)       38 2024-05-15 11:56:08.819879 local_determinacy-0.1.3/setup.cfg
+drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-15 11:56:08.814460 local_determinacy-0.1.3/src/
+drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-15 11:56:08.815933 local_determinacy-0.1.3/src/local_determinacy/
+-rw-r--r--   0 alfredlov   (502) staff       (20)       24 2024-05-10 13:00:49.000000 local_determinacy-0.1.3/src/local_determinacy/__init__.py
+-rw-r--r--   0 alfredlov   (502) staff       (20)     4747 2024-05-13 08:04:24.000000 local_determinacy-0.1.3/src/local_determinacy/functions.py
+drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-15 11:56:08.818979 local_determinacy-0.1.3/src/local_determinacy.egg-info/
+-rw-r--r--   0 alfredlov   (502) staff       (20)     5886 2024-05-15 11:56:08.000000 local_determinacy-0.1.3/src/local_determinacy.egg-info/PKG-INFO
+-rw-r--r--   0 alfredlov   (502) staff       (20)      281 2024-05-15 11:56:08.000000 local_determinacy-0.1.3/src/local_determinacy.egg-info/SOURCES.txt
+-rw-r--r--   0 alfredlov   (502) staff       (20)        1 2024-05-15 11:56:08.000000 local_determinacy-0.1.3/src/local_determinacy.egg-info/dependency_links.txt
+-rw-r--r--   0 alfredlov   (502) staff       (20)       18 2024-05-15 11:56:08.000000 local_determinacy-0.1.3/src/local_determinacy.egg-info/top_level.txt
```

### Comparing `local_determinacy-0.1.2/LICENSE` & `local_determinacy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `local_determinacy-0.1.2/PKG-INFO` & `local_determinacy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local_determinacy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for assessing local determinacy in incomplete markets models.
 Author-email: Alfred Løvgren <alfred.lovgren@econ.uio.no>, Marcus Hagedorn <marcus.hagedorn@econ.uio.no>
 Project-URL: Homepage, https://github.com/alfredlov/local-determinacy/
 Project-URL: Issues, https://github.com/alfredlov/local-determinacy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,21 +52,21 @@
 	- No Solution if winding number is larger than zero.
 
 
 ## Requirements and installation
 
 LD runs on Python 3.7 or newer, and requires Python's core numerical libraries (NumPy, SciPy, Numba).
 
-LD uses the methodology developped in  Auclert, Bardóczy, Rognlie, Straub (2021): "Using the Sequence-Space Jacobian to Solve and Estimate Heterogeneous-Agent Models" ([link to paper](https://www.bencebardoczy.com/publication/sequence-jacobian/sequence-jacobian.pdf)) to obtain the Jacobian matrix of the incomplete-markets model.
+LD uses the methodology developed in  Auclert, Bardóczy, Rognlie, Straub (2021): "Using the Sequence-Space Jacobian to Solve and Estimate Heterogeneous-Agent Models" ([link to paper](https://www.bencebardoczy.com/publication/sequence-jacobian/sequence-jacobian.pdf)) to obtain the Jacobian matrix of the incomplete-markets model.
 
 LD uses the SSJ package of Bence Bardóczy, Michael Cai, Matthew Rognlie, Adrien Auclert, Martin Souchier and Ludwig Straub. The latest version is available at https://github.com/shade-econ/sequence-jacobian. Note that all required packages will be installed automatically.
 
 To install LD, open a terminal and type
 ```
-pip install local-determinacy
+pip install local_determinacy
 ```
 ## Functions
 
 The LD package has four main functions:
 1) The onatski values of a jacobian
 ```
 >>> onatski(targets, endogenous, scale, T, ss0, H_U)
@@ -110,16 +110,16 @@
 windingNumber = ld.onatskiWindingNumber(onatski)
 
 windingNumber = ld.onatskiWindingNumber(onatski)
 print(ld.checkSolutions(windingNumber))
 
 ld.plot(onatski)
 ```
-If government bonds are nominal, an addtional elasticity decscibing valuation effects need to be added.
-The default setting assumes that all variables (for example lagged inflation) are predetermined. In general, LD requires specifying predetermined and Nnon-predetermnined variables.
+If government bonds are nominal, an addtional elasticity decscibing valuation effects needs to be added.
+The default setting assumes that all variables (for example lagged inflation) are predetermined. In general, LD requires specifying lagged/predetermined variables.
 The notebook examples illustrate these options.
 
 <!-- ## Toolbox
 
 The Toolbox allows using the package without a Python compiler. The toolbox offers several model classes and parameters (right now policy parameters) can be chosen by the user:
 
 - One asset incomplete-markets model with flexible prices and real bonds
@@ -129,9 +129,10 @@
 - One asset incomplete-markets model with flexible prices and FTPL tax rule
 - One asset incomplete-markets model with sticky prices and FTPL tax rule
 - ... -->
 
 ## Authors
 
 This package was written by
-- Alfred Løvgren
 - Marcus Hagedorn
+- Alfred Løvgren
+
```

### Comparing `local_determinacy-0.1.2/README.md` & `local_determinacy-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,21 @@
 	- No Solution if winding number is larger than zero.
 
 
 ## Requirements and installation
 
 LD runs on Python 3.7 or newer, and requires Python's core numerical libraries (NumPy, SciPy, Numba).
 
-LD uses the methodology developped in  Auclert, Bardóczy, Rognlie, Straub (2021): "Using the Sequence-Space Jacobian to Solve and Estimate Heterogeneous-Agent Models" ([link to paper](https://www.bencebardoczy.com/publication/sequence-jacobian/sequence-jacobian.pdf)) to obtain the Jacobian matrix of the incomplete-markets model.
+LD uses the methodology developed in  Auclert, Bardóczy, Rognlie, Straub (2021): "Using the Sequence-Space Jacobian to Solve and Estimate Heterogeneous-Agent Models" ([link to paper](https://www.bencebardoczy.com/publication/sequence-jacobian/sequence-jacobian.pdf)) to obtain the Jacobian matrix of the incomplete-markets model.
 
 LD uses the SSJ package of Bence Bardóczy, Michael Cai, Matthew Rognlie, Adrien Auclert, Martin Souchier and Ludwig Straub. The latest version is available at https://github.com/shade-econ/sequence-jacobian. Note that all required packages will be installed automatically.
 
 To install LD, open a terminal and type
 ```
-pip install local-determinacy
+pip install local_determinacy
 ```
 ## Functions
 
 The LD package has four main functions:
 1) The onatski values of a jacobian
 ```
 >>> onatski(targets, endogenous, scale, T, ss0, H_U)
@@ -96,16 +96,16 @@
 windingNumber = ld.onatskiWindingNumber(onatski)
 
 windingNumber = ld.onatskiWindingNumber(onatski)
 print(ld.checkSolutions(windingNumber))
 
 ld.plot(onatski)
 ```
-If government bonds are nominal, an addtional elasticity decscibing valuation effects need to be added.
-The default setting assumes that all variables (for example lagged inflation) are predetermined. In general, LD requires specifying predetermined and Nnon-predetermnined variables.
+If government bonds are nominal, an addtional elasticity decscibing valuation effects needs to be added.
+The default setting assumes that all variables (for example lagged inflation) are predetermined. In general, LD requires specifying lagged/predetermined variables.
 The notebook examples illustrate these options.
 
 <!-- ## Toolbox
 
 The Toolbox allows using the package without a Python compiler. The toolbox offers several model classes and parameters (right now policy parameters) can be chosen by the user:
 
 - One asset incomplete-markets model with flexible prices and real bonds
@@ -115,9 +115,10 @@
 - One asset incomplete-markets model with flexible prices and FTPL tax rule
 - One asset incomplete-markets model with sticky prices and FTPL tax rule
 - ... -->
 
 ## Authors
 
 This package was written by
-- Alfred Løvgren
 - Marcus Hagedorn
+- Alfred Løvgren
+
```

### Comparing `local_determinacy-0.1.2/pyproject.toml` & `local_determinacy-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "matplotlib>=1.16.0"
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "local_determinacy"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Alfred Løvgren", email="alfred.lovgren@econ.uio.no" },
   { name="Marcus Hagedorn", email="marcus.hagedorn@econ.uio.no" },
 ]
 description = "A python package for assessing local determinacy in incomplete markets models."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `local_determinacy-0.1.2/src/local_determinacy/functions.py` & `local_determinacy-0.1.3/src/local_determinacy/functions.py`

 * *Files identical despite different names*

### Comparing `local_determinacy-0.1.2/src/local_determinacy.egg-info/PKG-INFO` & `local_determinacy-0.1.3/src/local_determinacy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local_determinacy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for assessing local determinacy in incomplete markets models.
 Author-email: Alfred Løvgren <alfred.lovgren@econ.uio.no>, Marcus Hagedorn <marcus.hagedorn@econ.uio.no>
 Project-URL: Homepage, https://github.com/alfredlov/local-determinacy/
 Project-URL: Issues, https://github.com/alfredlov/local-determinacy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,21 +52,21 @@
 	- No Solution if winding number is larger than zero.
 
 
 ## Requirements and installation
 
 LD runs on Python 3.7 or newer, and requires Python's core numerical libraries (NumPy, SciPy, Numba).
 
-LD uses the methodology developped in  Auclert, Bardóczy, Rognlie, Straub (2021): "Using the Sequence-Space Jacobian to Solve and Estimate Heterogeneous-Agent Models" ([link to paper](https://www.bencebardoczy.com/publication/sequence-jacobian/sequence-jacobian.pdf)) to obtain the Jacobian matrix of the incomplete-markets model.
+LD uses the methodology developed in  Auclert, Bardóczy, Rognlie, Straub (2021): "Using the Sequence-Space Jacobian to Solve and Estimate Heterogeneous-Agent Models" ([link to paper](https://www.bencebardoczy.com/publication/sequence-jacobian/sequence-jacobian.pdf)) to obtain the Jacobian matrix of the incomplete-markets model.
 
 LD uses the SSJ package of Bence Bardóczy, Michael Cai, Matthew Rognlie, Adrien Auclert, Martin Souchier and Ludwig Straub. The latest version is available at https://github.com/shade-econ/sequence-jacobian. Note that all required packages will be installed automatically.
 
 To install LD, open a terminal and type
 ```
-pip install local-determinacy
+pip install local_determinacy
 ```
 ## Functions
 
 The LD package has four main functions:
 1) The onatski values of a jacobian
 ```
 >>> onatski(targets, endogenous, scale, T, ss0, H_U)
@@ -110,16 +110,16 @@
 windingNumber = ld.onatskiWindingNumber(onatski)
 
 windingNumber = ld.onatskiWindingNumber(onatski)
 print(ld.checkSolutions(windingNumber))
 
 ld.plot(onatski)
 ```
-If government bonds are nominal, an addtional elasticity decscibing valuation effects need to be added.
-The default setting assumes that all variables (for example lagged inflation) are predetermined. In general, LD requires specifying predetermined and Nnon-predetermnined variables.
+If government bonds are nominal, an addtional elasticity decscibing valuation effects needs to be added.
+The default setting assumes that all variables (for example lagged inflation) are predetermined. In general, LD requires specifying lagged/predetermined variables.
 The notebook examples illustrate these options.
 
 <!-- ## Toolbox
 
 The Toolbox allows using the package without a Python compiler. The toolbox offers several model classes and parameters (right now policy parameters) can be chosen by the user:
 
 - One asset incomplete-markets model with flexible prices and real bonds
@@ -129,9 +129,10 @@
 - One asset incomplete-markets model with flexible prices and FTPL tax rule
 - One asset incomplete-markets model with sticky prices and FTPL tax rule
 - ... -->
 
 ## Authors
 
 This package was written by
-- Alfred Løvgren
 - Marcus Hagedorn
+- Alfred Løvgren
+
```

