# Comparing `tmp/dfm_tools-0.22.0.tar.gz` & `tmp/dfm_tools-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfm_tools-0.22.0.tar", last modified: Tue Apr  9 17:27:47 2024, max compression
+gzip compressed data, was "dfm_tools-0.23.0.tar", last modified: Wed May 15 15:36:15 2024, max compression
```

## Comparing `dfm_tools-0.22.0.tar` & `dfm_tools-0.23.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:47.313413 dfm_tools-0.22.0/dfm_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/bathymetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/coastlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/energy_dissipation.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    27388 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/get_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/get_nc_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    30674 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/hydrolib_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    35052 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/interpolate_grid2bnd.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/linebuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/meshkernel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/modelbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    23869 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/modplot.py
--rw-r--r--   0 runner    (1001) docker     (127)    47235 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)    16201 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/xarray_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28439 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/xugrid_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/dfm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_bathymetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_coastlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21328 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_dfm_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_external_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_get_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_hydrolib_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22937 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_interpolate_grid2bnd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_meshkernel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_modelbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_observations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_xarray_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_xugrid_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:36:15.843960 dfm_tools-0.23.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-15 15:36:15.843960 dfm_tools-0.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:36:15.839960 dfm_tools-0.23.0/dfm_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/bathymetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/coastlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21907 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/energy_dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27386 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/get_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/get_nc_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30674 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/hydrolib_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34789 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/interpolate_grid2bnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/linebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/meshkernel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18717 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/modelbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23869 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/modplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47235 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15757 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/xarray_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/dfm_tools/xugrid_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:36:15.843960 dfm_tools-0.23.0/dfm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-15 15:36:15.000000 dfm_tools-0.23.0/dfm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 15:36:15.000000 dfm_tools-0.23.0/dfm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:36:15.000000 dfm_tools-0.23.0/dfm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-15 15:36:15.000000 dfm_tools-0.23.0/dfm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 15:36:15.000000 dfm_tools-0.23.0/dfm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:36:15.843960 dfm_tools-0.23.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:36:15.843960 dfm_tools-0.23.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_bathymetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_coastlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21328 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_dfm_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_external_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_get_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_hydrolib_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22937 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_interpolate_grid2bnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_meshkernel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_modelbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_xarray_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-05-15 15:35:16.000000 dfm_tools-0.23.0/tests/test_xugrid_helpers.py
```

### Comparing `dfm_tools-0.22.0/LICENSE` & `dfm_tools-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/PKG-INFO` & `dfm_tools-0.23.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfm_tools
-Version: 0.22.0
+Version: 0.23.0
 Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
 Maintainer-email: Jelmer Veenstra <jelmer.veenstra@deltares.nl>
 License: LGPLv3
 Project-URL: Home, https://github.com/deltares/dfm_tools
 Project-URL: Code, https://github.com/deltares/dfm_tools
 Project-URL: Issues, https://github.com/deltares/dfm_tools/issues
 Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles,modelbuilder
@@ -31,35 +31,34 @@
 Requires-Dist: fiona>=1.9
 Requires-Dist: contextily>=1.0.0
 Requires-Dist: xarray>=2023.9.0
 Requires-Dist: dask>=2023.9.0
 Requires-Dist: netcdf4>=1.5.4
 Requires-Dist: bottleneck>=1.3.3
 Requires-Dist: xugrid>=0.9.0
-Requires-Dist: cdsapi>=0.6.1
+Requires-Dist: cdsapi>=0.7.0
 Requires-Dist: pydap>=3.4.0
 Requires-Dist: erddapy>=2.0.0
-Requires-Dist: copernicusmarine>=1.1.0
+Requires-Dist: copernicusmarine>=1.2.0
 Requires-Dist: rws-ddlpy>=0.4.0
 Requires-Dist: pooch>=1.1.0
 Requires-Dist: hydrolib-core>=0.7.0
 Requires-Dist: meshkernel>=4.1.0
 Provides-Extra: dev
 Requires-Dist: bump2version>=0.5.11; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: mkdocs; extra == "docs"
-Requires-Dist: mkdocs-material; extra == "docs"
-Requires-Dist: mkdocs-jupyter; extra == "docs"
-Requires-Dist: mkdocstrings-python; extra == "docs"
-Requires-Dist: mkdocs-exclude; extra == "docs"
+Requires-Dist: sphinx>=1.8.1; extra == "docs"
+Requires-Dist: sphinx_mdinclude; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Provides-Extra: examples
 Requires-Dist: jupyter; extra == "examples"
 Requires-Dist: notebook; extra == "examples"
 
 [![pytest](https://github.com/Deltares/dfm_tools/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest.yml)
 [![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
```

### Comparing `dfm_tools-0.22.0/README.md` & `dfm_tools-0.23.0/README.md`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/__init__.py` & `dfm_tools-0.23.0/dfm_tools/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
-.. include:: ../README.md
+Pre- and postprocessing D-FlowFM model input and output files
 """
 
 __author__ = """Jelmer Veenstra"""
 __email__ = "jelmer.veenstra@deltares.nl"
-__version__ = "0.22.0"
+__version__ = "0.23.0"
 
 from dfm_tools.deprecated import *
 from dfm_tools.download import *
 from dfm_tools.get_nc import *
 from dfm_tools.get_nc_helpers import *
 from dfm_tools.hydrolib_helpers import *
 from dfm_tools.meshkernel_helpers import *
```

### Comparing `dfm_tools-0.22.0/dfm_tools/bathymetry.py` & `dfm_tools-0.23.0/dfm_tools/bathymetry.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/coastlines.py` & `dfm_tools-0.23.0/dfm_tools/coastlines.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     res : str, optional
         f(ull), h(igh), i(ntermediate), l(ow), c(oarse) resolution. The default is 'h'.
     bbox : tuple, optional
         (minx, miny, maxx, maxy), also includes shapes that are partly in the bbox. The default is (-180, -90, 180, 90).
     min_area : float, optional
         in km2, min_area>0 speeds up process. The default is 0.
     crs : str, optional
-        
+        coordinate reference system
     include_fields : list, optional
         which shapefile fields to include, None gives all. The default is ['area'].
 
     Returns
     -------
     coastlines_gdb : TYPE
         DESCRIPTION.
@@ -93,14 +93,15 @@
     Parameters
     ----------
     res : str, optional
         f(ull), h(igh), i(ntermediate), l(ow), c(oarse) resolution. The default is 'h'.
     bbox : tuple, optional
         (minx, miny, maxx, maxy), also includes shapes that are partly in the bbox. The default is (-180, -90, 180, 90).
     crs : str, optional
+        coordinate reference system
     
     Returns
     -------
     coastlines_gdb : TYPE
         DESCRIPTION.
 
     """
```

### Comparing `dfm_tools-0.22.0/dfm_tools/data.py` & `dfm_tools-0.23.0/dfm_tools/data.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/deprecated.py` & `dfm_tools-0.23.0/dfm_tools/deprecated.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/download.py` & `dfm_tools-0.23.0/dfm_tools/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     #TODO: describe something about the .cdsapirc file
     #TODO: make this function cdsapi generic, instead of ERA5 hardcoded (make flexible for product_type/name/name_output) (variables_dict is not used actively anymore, so this is possible)
     
     # create ~/.cdsapirc if it does not exist
     cds_credentials()
     
     # import cdsapi and create a Client instance # https://cds.climate.copernicus.eu/api-how-to
-    c = cds_client_withargs()
+    c = cdsapi.Client()
 
     #dictionary with ERA5 variables #this is not actively used
     variables_dict = {'ssr':'surface_net_solar_radiation',
                       'sst':'sea_surface_temperature',
                       'strd':'surface_thermal_radiation_downwards',
                       'slhf':'surface_latent_heat_flux',
                       'sshf':'surface_sensible_heat_flux',
@@ -112,15 +112,15 @@
     if os.path.isfile(file_cds_credentials):
         config = cdsapi.api.read_config(file_cds_credentials)
         cds_url = config["url"]
         cds_uid_apikey = config["key"]
     
     try:
         # checks whether CDS apikey is in environment variable or ~/.cdsapirc file and if it is in correct format
-        c = cds_client_withargs()
+        c = cdsapi.Client()
         # checks whether credentials (uid and apikey) are correct
         c.retrieve(name="dummy", request={})
     except Exception as e:
         if "Missing/incomplete configuration file" in str(e):
             # to catch "Exception: Missing/incomplete configuration file"
             # query uid and apikey if not present
             print("Downloading CDS/ERA5 data requires a CDS API key, copy your UID and API-key from https://cds.climate.copernicus.eu/user (first register, login and accept the terms). ")
@@ -160,25 +160,14 @@
             os.environ.pop(key)
     
     file_cds_credentials = cds_get_file()
     if os.path.isfile(file_cds_credentials):
         os.remove(file_cds_credentials)
 
 
-def cds_client_withargs():
-    """
-    Initialize a csdapi client with url and key from os environment variables
-    These are the default values for the url/key arguments, but somehow this 
-    is necessary to use the key/url from environment variables.
-    """
-    c = cdsapi.Client(url=os.environ.get("CDSAPI_URL"),
-                      key=os.environ.get("CDSAPI_KEY"))
-    return c
-
-
 def download_CMEMS(varkey,
                    longitude_min, longitude_max, latitude_min, latitude_max, 
                    date_min, date_max, freq='D',
                    dataset_id=None, buffer=None,
                    dir_output='.', file_prefix='', overwrite=False):
     """
     https://help.marine.copernicus.eu/en/articles/8283072-copernicus-marine-toolbox-api-subset
@@ -323,25 +312,25 @@
     print("Downloading CMEMS data requires a Copernicus Marine username and password, "
           "sign up for free at: https://data.marine.copernicus.eu/register.")
     success = copernicusmarine.login(skip_if_user_logged_in=True)
     if not success:
         raise InvalidUsernameOrPassword("Invalid credentials, please try again")
 
 
-def copernicusmarine_reset(remove_folder=False, overwrite_cache=True, update_package=False):
+def copernicusmarine_reset(update_package=False, remove_folder=False, overwrite_cache=True):
+    if update_package:
+        print("reset copernicusmarine: updating copernicusmarine")
+        subprocess.check_call(f"{sys.executable} -m pip install copernicusmarine -U")
     if remove_folder:
         dir_copernicusmarine = os.path.expanduser("~/.copernicusmarine")
         print(f"reset copernicusmarine: removing {dir_copernicusmarine}, you will have to login again.")
         shutil.rmtree(dir_copernicusmarine, ignore_errors=True)
     if overwrite_cache:
         print("reset copernicusmarine: overwriting copernicusmarine metadata cache (takes some time)")
         subprocess.run("copernicusmarine describe --overwrite-metadata-cache")
-    if update_package:
-        print("reset copernicusmarine: updating copernicusmarine")
-        subprocess.check_call(f"{sys.executable} -m pip install copernicusmarine -U")
 
 
 def copernicusmarine_dataset_timerange(dataset_id):
     ds = copernicusmarine.open_dataset(dataset_id=dataset_id)
     ds_tstart = pd.Timestamp(ds.time.isel(time=0).values)
     ds_tstop = pd.Timestamp(ds.time.isel(time=-1).values)
     return ds_tstart, ds_tstop
```

### Comparing `dfm_tools-0.22.0/dfm_tools/energy_dissipation.py` & `dfm_tools-0.23.0/dfm_tools/energy_dissipation.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/get_nc.py` & `dfm_tools-0.23.0/dfm_tools/get_nc.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
         DESCRIPTION.
     varname : TYPE
         DESCRIPTION.
     ax : matplotlib.axes._subplots.AxesSubplot, optional
         the figure axis. The default is None.
     only_contour : bool, optional
         Wheter to plot contour lines of the dataset. The default is False.
-    **kwargs : TYPE
+    kwargs : TYPE
         properties to give on to the pcolormesh function.
     
     Raises
     ------
     Exception
         DESCRIPTION.
```

### Comparing `dfm_tools-0.22.0/dfm_tools/get_nc_helpers.py` & `dfm_tools-0.23.0/dfm_tools/get_nc_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/hydrolib_helpers.py` & `dfm_tools-0.23.0/dfm_tools/hydrolib_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/interpolate_grid2bnd.py` & `dfm_tools-0.23.0/dfm_tools/interpolate_grid2bnd.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,29 +38,30 @@
     conversion_dict.keys() are the dflowfm quantities and the ncvarname the corresponding netcdf variable name/key
     alternative ncvarnames can be supplied via ncvarname_updates, e.g. get_conversion_dict(ncvarname_updates={'temperaturebnd':'tos'})
     
     interpolate_nc_to_bc() renames netcdf variable like this:
     data_xr = data_xr.rename({ncvarname:quantity})
     
     for CMCC:
-    conversion_dict = { # conversion is phyc in mol/m3 to newvar in g/m3
-                       'tracerbndOXY'        : {'ncvarname': 'o2',          'unit': 'g/m3', 'conversion': 32.0 },
-                       'tracerbndNO3'        : {'ncvarname': 'no3',         'unit': 'g/m3', 'conversion': 14.0 },
-                       'tracerbndPO4'        : {'ncvarname': 'po4',         'unit': 'g/m3', 'conversion': 30.97 },
-                       'tracerbndSi'         : {'ncvarname': 'si',          'unit': 'g/m3', 'conversion': 28.08},
-                       'tracerbndPON1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 14.0}, # Caution: this empirical relation might not be applicable to your use case
-                       'tracerbndPOP1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 30.97}, # Caution: this empirical relation might not be applicable to your use case
-                       'tracerbndPOC1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 14.0 * (106 / 16)}, # Caution: this empirical relation might not be applicable to your use case
-                       'salinitybnd'         : {'ncvarname': 'sos'},         #'1e-3'
-                       'temperaturebnd'      : {'ncvarname': 'tos'},         #'degC'
-                       'ux'                  : {'ncvarname': 'uo'},          #'m/s'
-                       'uy'                  : {'ncvarname': 'vo'},          #'m/s'
-                       'waterlevelbnd'       : {'ncvarname': 'zos'},         #'m' #steric
-                       'tide'                : {'ncvarname': ''},            #'m' #tide (dummy entry)
-                       }
+    conversion_dict = {
+    # conversion is phyc in mol/m3 to newvar in g/m3
+    'tracerbndOXY'        : {'ncvarname': 'o2',          'unit': 'g/m3', 'conversion': 32.0 },
+    'tracerbndNO3'        : {'ncvarname': 'no3',         'unit': 'g/m3', 'conversion': 14.0 },
+    'tracerbndPO4'        : {'ncvarname': 'po4',         'unit': 'g/m3', 'conversion': 30.97 },
+    'tracerbndSi'         : {'ncvarname': 'si',          'unit': 'g/m3', 'conversion': 28.08},
+    'tracerbndPON1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 14.0}, # Caution: this empirical relation might not be applicable to your use case
+    'tracerbndPOP1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 30.97}, # Caution: this empirical relation might not be applicable to your use case
+    'tracerbndPOC1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 14.0 * (106 / 16)}, # Caution: this empirical relation might not be applicable to your use case
+    'salinitybnd'         : {'ncvarname': 'sos'},         #'1e-3'
+    'temperaturebnd'      : {'ncvarname': 'tos'},         #'degC'
+    'ux'                  : {'ncvarname': 'uo'},          #'m/s'
+    'uy'                  : {'ncvarname': 'vo'},          #'m/s'
+    'waterlevelbnd'       : {'ncvarname': 'zos'},         #'m' #steric
+    'tide'                : {'ncvarname': ''},            #'m' #tide (dummy entry)
+    }
     
     
     The below clarification about the CMEMS conversion factors in this function is by Jos van Gils.
     The use of boundary conditions from CMEMS requires some conversion (scaling). 
     In the first place, there is the unit conversion from mmol/m3 in CMEMS to g/m3 in DFM. 
     This involves a factor M/1000, where M is the molar weight of the constituent in question: 
     M = 12 for constituents expressed in gC/m3, 14 for gN/m3, 30.97 for gP/m3, 28.08 for gSi/m3 and 32 for dissolved oxygen. 
@@ -443,15 +444,15 @@
     print(f'>>time passed: {time_passed:.2f} sec')
 
     return data_interp_loaded
 
 
 def interp_uds_to_plipoints(uds:xu.UgridDataset, gdf:geopandas.GeoDataFrame, nPoints:int=None) -> xr.Dataset:
     """
-    To interpolate an unstructured dataset (like a *_map.nc file) read with xugrid to plipoint locations
+    To interpolate an unstructured dataset (like a _map.nc file) read with xugrid to plipoint locations
     
     Parameters
     ----------
     uds : xu.UgridDataset
         dfm model output read using dfm_tools. Dims: mesh2d_nLayers, mesh2d_nInterfaces, time, mesh2d_nNodes, mesh2d_nFaces, mesh2d_nMax_face_nodes, mesh2d_nEdges.
     gdf : geopandas.GeoDataFrame (str/path is also supported)
         gdf with location, geometry (Point) and crs corresponding to model crs.
```

### Comparing `dfm_tools-0.22.0/dfm_tools/linebuilder.py` & `dfm_tools-0.23.0/dfm_tools/linebuilder.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/meshkernel_helpers.py` & `dfm_tools-0.23.0/dfm_tools/meshkernel_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/modelbuilder.py` & `dfm_tools-0.23.0/dfm_tools/modelbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,37 +6,40 @@
 import hydrolib.core.dflowfm as hcdfm
 from hydrolib.core.dimr.models import DIMR, FMComponent, Start
 from hydrolib.core.utils import get_path_style_for_current_operating_system
 from dfm_tools.hydrolib_helpers import get_ncbnd_construct
 
 __all__ = [
     "cmems_nc_to_bc",
-    "preprocess_ini_cmems_to_nc",
     "cmems_nc_to_ini",
+    "preprocess_ini_cmems_to_nc",
     "preprocess_merge_meteofiles_era5",
     "create_model_exec_files",
     "make_paths_relative",
     ]
 
 
-def cmems_nc_to_bc(ext_bnd, list_quantities, tstart, tstop, file_pli, dir_pattern, dir_output, refdate_str=None):
+def cmems_nc_to_bc(ext_bnd, list_quantities, tstart, tstop, file_pli, dir_pattern, dir_output, conversion_dict=None, refdate_str=None):
     #input examples in https://github.com/Deltares/dfm_tools/blob/main/tests/examples/preprocess_interpolate_nc_to_bc.py
     
+    if conversion_dict is None:
+        conversion_dict = dfmt.get_conversion_dict()
+    
     file_bc_basename = os.path.basename(file_pli).replace('.pli','')
     for quantity in list_quantities:
         print(f'processing quantity: {quantity}')
         
         # times in cmems API are at midnight, so round to nearest outer midnight datetime
         tstart = pd.Timestamp(tstart).floor('1d')
         tstop = pd.Timestamp(tstop).ceil('1d')
         
         #open regulargridDataset and do some basic stuff (time selection, renaming depth/lat/lon/varname, converting units, etc)
         data_xr_vars = dfmt.open_dataset_extra(dir_pattern=dir_pattern, quantity=quantity,
                                                tstart=tstart, tstop=tstop,
-                                               conversion_dict=dfmt.get_conversion_dict(),
+                                               conversion_dict=conversion_dict,
                                                refdate_str=refdate_str)
         #interpolate regulargridDataset to plipointsDataset
         data_interp = dfmt.interp_regularnc_to_plipoints(data_xr_reg=data_xr_vars, file_pli=file_pli)
         
         #convert plipointsDataset to hydrolib ForcingModel
         ForcingModel_object = dfmt.plipointsDataset_to_ForcingModel(plipointsDataset=data_interp)
```

### Comparing `dfm_tools-0.22.0/dfm_tools/modplot.py` & `dfm_tools-0.23.0/dfm_tools/modplot.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/observations.py` & `dfm_tools-0.23.0/dfm_tools/observations.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/dfm_tools/xarray_helpers.py` & `dfm_tools-0.23.0/dfm_tools/xarray_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
-from netCDF4 import Dataset
 import xarray as xr
+import dask
 import datetime as dt
 import glob
 import pandas as pd
 import warnings
 import numpy as np
 import netCDF4
 from dfm_tools.errors import OutOfRangeError
@@ -155,73 +155,62 @@
 
     Parameters
     ----------
     file_nc : str
         DESCRIPTION.
     preprocess : TYPE, optional
         DESCRIPTION. The default is None.
-    chunks : dict, optional
-        Prevents large chunks and memory issues. The default is {'time':1}.
     time_slice : slice, optional
         DESCRIPTION. The default is slice(None,None).
     add_global_overlap : bool, optional
         GTSM specific: extend data beyond -180 to 180 longitude. The default is False.
     zerostart : bool, optional
         GTSM specific: extend data with 0-value fields 1 and 2 days before time_slice.start. The default is False.
-
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
+    kwargs : dict, optional
+        arguments for xr.open_mfdataset() like `chunks` to prevent large chunks and resulting memory issues.
 
     Returns
     -------
-    TYPE
-        DESCRIPTION.
+    data_xr : xr.Dataset
+        Merged meteo dataset.
 
     """
     #TODO: add ERA5 conversions and features from hydro_tools\ERA5\ERA52DFM.py (except for varRhoair_alt, request FM support for varying airpressure: https://issuetracker.deltares.nl/browse/UNST-6593)
-    #TODO: request FM support for charnock (etc) separate meteo forcing (currently airpressure_windx_windy_charnock merged file is required): https://issuetracker.deltares.nl/browse/UNST-6453
     #TODO: provide extfile example with fmquantity/ncvarname combinations and cleanup FM code: https://issuetracker.deltares.nl/browse/UNST-6453
     #TODO: add coordinate conversion (only valid for models with multidimensional lat/lon variables like HARMONIE and HIRLAM). This should work: ds_reproj = ds.set_crs(4326).to_crs(28992)
     #TODO: add CMCC etc from gtsmip repos (mainly calendar conversion)
     #TODO: put conversions in separate function?
     #TODO: maybe add renaming like {'salinity':'so', 'water_temp':'thetao'} for hycom
-    
-    if "chunks" not in kwargs.keys():
-        kwargs["chunks"] = {'time':1}
-        
-    
+       
     #woa workaround
     if preprocess == preprocess_woa:
         decode_cf = False
     else:
         decode_cf = True        
 
     file_nc_list = file_to_list(file_nc)
 
     print(f'>> opening multifile dataset of {len(file_nc_list)} files (can take a while with lots of files): ',end='')
     dtstart = dt.datetime.now()
-    data_xr = xr.open_mfdataset(file_nc_list,
-                                #parallel=True, #TODO: speeds up the process, but often "OSError: [Errno -51] NetCDF: Unknown file format" on WCF
-                                preprocess=preprocess,
-                                decode_cf=decode_cf,
-                                **kwargs)
+    with dask.config.set(**{'array.slicing.split_large_chunks': True}):
+        # using dask option to avoid large chunks which speeds up the merging/writing process
+        data_xr = xr.open_mfdataset(file_nc_list,
+                                    preprocess=preprocess,
+                                    decode_cf=decode_cf,
+                                    **kwargs)
     print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
     
     #rename variables
     if 'longitude' not in data_xr.variables: #TODO: make generic, comparable rename in rename_dims_dict in dfmt.open_dataset_extra()
         if 'lon' in data_xr.variables:
             data_xr = data_xr.rename({'lon':'longitude', 'lat':'latitude'})
         elif 'x' in data_xr.variables:
             data_xr = data_xr.rename({'x':'longitude', 'y':'latitude'})
         else:
             raise KeyError('no longitude/latitude, lon/lat or x/y variables found in dataset')
-
-    #data_xr.attrs['comment'] = 'merged with dfm_tools from https://github.com/Deltares/dfm_tools' #TODO: add something like this or other attributes? (some might also be dropped now)
     
     #select time and do checks #TODO: check if calendar is standard/gregorian
     data_xr = data_xr.sel(time=time_slice)
     if data_xr.get_index('time').duplicated().any():
         print('dropping duplicate timesteps')
         data_xr = data_xr.sel(time=~data_xr.get_index('time').duplicated()) #drop duplicate timesteps
```

### Comparing `dfm_tools-0.22.0/dfm_tools/xugrid_helpers.py` & `dfm_tools-0.23.0/dfm_tools/xugrid_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,27 +188,28 @@
         DESCRIPTION.
 
     Returns
     -------
     ds_merged_xu : TYPE
         DESCRIPTION.
     
-    file_nc = 'p:\\1204257-dcsmzuno\\2006-2012\\3D-DCSM-FM\\A18b_ntsu1\\DFM_OUTPUT_DCSM-FM_0_5nm\\DCSM-FM_0_5nm_0*_map.nc' #3D DCSM
-    file_nc = 'p:\\archivedprojects\\11206813-006-kpp2021_rmm-2d\\C_Work\\31_RMM_FMmodel\\computations\\model_setup\\run_207\\results\\RMM_dflowfm_0*_map.nc' #RMM 2D
-    file_nc = 'p:\\1230882-emodnet_hrsm\\GTSMv5.0\\runs\\reference_GTSMv4.1_wiCA_2.20.06_mapformat4\\output\\gtsm_model_0*_map.nc' #GTSM 2D
-    file_nc = 'p:\\11208053-005-kpp2022-rmm3d\\C_Work\\01_saltiMarlein\\RMM_2019_computations_02\\computations\\theo_03\\DFM_OUTPUT_RMM_dflowfm_2019\\RMM_dflowfm_2019_0*_map.nc' #RMM 3D
-    file_nc = 'p:\\archivedprojects\\11203379-005-mwra-updated-bem\\03_model\\02_final\\A72_ntsu0_kzlb2\\DFM_OUTPUT_MB_02\\MB_02_0*_map.nc'
-    Timings (xu.open_dataset/xu.merge_partitions):
-        - DCSM 3D 20 partitions  367 timesteps: 231.5/ 4.5 sec (decode_times=False: 229.0 sec)
-        - RMM  2D  8 partitions  421 timesteps:  55.4/ 4.4 sec (decode_times=False:  56.6 sec)
-        - GTSM 2D  8 partitions  746 timesteps:  71.8/30.0 sec (decode_times=False: 204.8 sec)
-        - RMM  3D 40 partitions  146 timesteps: 168.8/ 6.3 sec (decode_times=False: 158.4 sec)
-        - MWRA 3D 20 partitions 2551 timesteps:  74.4/ 3.4 sec (decode_times=False:  79.0 sec)
-    
     """
+    # TODO: timings
+    # file_nc = 'p:\\1204257-dcsmzuno\\2006-2012\\3D-DCSM-FM\\A18b_ntsu1\\DFM_OUTPUT_DCSM-FM_0_5nm\\DCSM-FM_0_5nm_0*_map.nc' #3D DCSM
+    # file_nc = 'p:\\archivedprojects\\11206813-006-kpp2021_rmm-2d\\C_Work\\31_RMM_FMmodel\\computations\\model_setup\\run_207\\results\\RMM_dflowfm_0*_map.nc' #RMM 2D
+    # file_nc = 'p:\\1230882-emodnet_hrsm\\GTSMv5.0\\runs\\reference_GTSMv4.1_wiCA_2.20.06_mapformat4\\output\\gtsm_model_0*_map.nc' #GTSM 2D
+    # file_nc = 'p:\\11208053-005-kpp2022-rmm3d\\C_Work\\01_saltiMarlein\\RMM_2019_computations_02\\computations\\theo_03\\DFM_OUTPUT_RMM_dflowfm_2019\\RMM_dflowfm_2019_0*_map.nc' #RMM 3D
+    # file_nc = 'p:\\archivedprojects\\11203379-005-mwra-updated-bem\\03_model\\02_final\\A72_ntsu0_kzlb2\\DFM_OUTPUT_MB_02\\MB_02_0*_map.nc'
+    # Timings (xu.open_dataset/xu.merge_partitions):
+    # - DCSM 3D 20 partitions  367 timesteps: 231.5/ 4.5 sec (decode_times=False: 229.0 sec)
+    # - RMM  2D  8 partitions  421 timesteps:  55.4/ 4.4 sec (decode_times=False:  56.6 sec)
+    # - GTSM 2D  8 partitions  746 timesteps:  71.8/30.0 sec (decode_times=False: 204.8 sec)
+    # - RMM  3D 40 partitions  146 timesteps: 168.8/ 6.3 sec (decode_times=False: 158.4 sec)
+    # - MWRA 3D 20 partitions 2551 timesteps:  74.4/ 3.4 sec (decode_times=False:  79.0 sec)
+
     #TODO: add support for multiple grids via keyword? https://github.com/Deltares/dfm_tools/issues/497
     #TODO: speed up open_dataset https://github.com/Deltares/dfm_tools/issues/225 (also remove_ghost)
     
     if 'chunks' not in kwargs:
         kwargs['chunks'] = {'time':1}
     
     dtstart_all = dt.datetime.now()
@@ -431,17 +432,33 @@
                       )
     
     face_dim = grid.face_dimension
     ds_stacked = ds.stack({face_dim:('M','N')}).sel({face_dim:keep_faces_bool})
     ds_stacked = ds_stacked.drop_vars(['M','N','mesh2d_nFaces'])
     uds = xu.UgridDataset(ds_stacked,grids=[grid]) 
     
-    uds = uds.drop_vars(['XCOR','YCOR'])
+    uds = uds.drop_vars(['XCOR','YCOR','grid'])
     uds = uds.drop_dims(['MC','NC']) #clean up dataset by dropping corner dims (drops also variabes with U/V masks and U/V/C bedlevel)
     
+    # convert to xarray.Dataset to update/remove attrs
+    ds_temp = uds.ugrid.to_dataset()
+    
+    # set vertical dimensions attr
+    # TODO: would be more convenient to do within xu.Ugrid2d(): https://github.com/Deltares/xugrid/issues/195#issuecomment-2111841390
+    grid_attrs = {"vertical_dimensions": ds.grid.attrs["vertical_dimensions"]}
+    ds_temp["mesh2d"] = ds_temp["mesh2d"].assign_attrs(grid_attrs)
+
+    # drop attrs pointing to the removed grid variable (topology is now in mesh2d)
+    # TODO: this is not possible on the xu.UgridDataset directly
+    for varn in ds_temp.data_vars:
+        if "grid" in ds_temp[varn].attrs.keys():
+            del ds_temp[varn].attrs["grid"]
+
+    uds = xu.UgridDataset(ds_temp)
+    
     return uds
 
 
 def uda_to_faces(uda : xu.UgridDataArray) -> xu.UgridDataArray:
     """
     Interpolates a ugrid variable (xu.DataArray) with a node or edge dimension to the faces by averaging the 3/4 nodes/edges around each face.
```

### Comparing `dfm_tools-0.22.0/dfm_tools.egg-info/PKG-INFO` & `dfm_tools-0.23.0/dfm_tools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfm_tools
-Version: 0.22.0
+Version: 0.23.0
 Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
 Maintainer-email: Jelmer Veenstra <jelmer.veenstra@deltares.nl>
 License: LGPLv3
 Project-URL: Home, https://github.com/deltares/dfm_tools
 Project-URL: Code, https://github.com/deltares/dfm_tools
 Project-URL: Issues, https://github.com/deltares/dfm_tools/issues
 Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles,modelbuilder
@@ -31,35 +31,34 @@
 Requires-Dist: fiona>=1.9
 Requires-Dist: contextily>=1.0.0
 Requires-Dist: xarray>=2023.9.0
 Requires-Dist: dask>=2023.9.0
 Requires-Dist: netcdf4>=1.5.4
 Requires-Dist: bottleneck>=1.3.3
 Requires-Dist: xugrid>=0.9.0
-Requires-Dist: cdsapi>=0.6.1
+Requires-Dist: cdsapi>=0.7.0
 Requires-Dist: pydap>=3.4.0
 Requires-Dist: erddapy>=2.0.0
-Requires-Dist: copernicusmarine>=1.1.0
+Requires-Dist: copernicusmarine>=1.2.0
 Requires-Dist: rws-ddlpy>=0.4.0
 Requires-Dist: pooch>=1.1.0
 Requires-Dist: hydrolib-core>=0.7.0
 Requires-Dist: meshkernel>=4.1.0
 Provides-Extra: dev
 Requires-Dist: bump2version>=0.5.11; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: mkdocs; extra == "docs"
-Requires-Dist: mkdocs-material; extra == "docs"
-Requires-Dist: mkdocs-jupyter; extra == "docs"
-Requires-Dist: mkdocstrings-python; extra == "docs"
-Requires-Dist: mkdocs-exclude; extra == "docs"
+Requires-Dist: sphinx>=1.8.1; extra == "docs"
+Requires-Dist: sphinx_mdinclude; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Provides-Extra: examples
 Requires-Dist: jupyter; extra == "examples"
 Requires-Dist: notebook; extra == "examples"
 
 [![pytest](https://github.com/Deltares/dfm_tools/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest.yml)
 [![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
```

### Comparing `dfm_tools-0.22.0/dfm_tools.egg-info/SOURCES.txt` & `dfm_tools-0.23.0/dfm_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/pyproject.toml` & `dfm_tools-0.23.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfm_tools"
-version = "0.22.0"
+version = "0.23.0"
 maintainers = [{ name = "Jelmer Veenstra", email = "jelmer.veenstra@deltares.nl" }]
 description = "dfm_tools are pre- and post-processing tools for Delft3D FM"
 readme = "README.md"
 keywords = ["dfm_tools", "D-FlowFM", "D-HYDRO", "post-processing", "pre-processing", "mapfiles", "hisfiles", "modelbuilder"]
 license = { text = "LGPLv3" }
 requires-python = ">=3.9"
 dependencies = [
@@ -34,22 +34,22 @@
 	"dask>=2023.9.0",
 	#netcdf4<1.5.4 pip install fails in py39
 	"netcdf4>=1.5.4",
 	#bottleneck<1.3.3 pip install fails in py39
 	"bottleneck>=1.3.3",
 	#xugrid<0.9.0 does not support partitioned 1d2d grids
 	"xugrid>=0.9.0",
-	#cdsapi<0.6.1 is from Feb 2021 and does not support newer python versions
-	"cdsapi>=0.6.1",
+	#cdsapi<0.7.0 supports credentials from environment variables
+	"cdsapi>=0.7.0",
 	#pydap<3.4.0 is from May 2017 and does not support newer python versions
 	"pydap>=3.4.0",
 	#erddapy<2.0.0 does not support pandas>=2.0.0
 	"erddapy>=2.0.0",
-	#copernicusmarine<1.1.0 does not support insitu data via files service and does not check credentials upon login
-	"copernicusmarine>=1.1.0",
+	#copernicusmarine<1.2.0 returns incorrect time ranges of cmems my/forecast datasets (https://github.com/Deltares/dfm_tools/issues/842)
+	"copernicusmarine>=1.2.0",
 	#rws-ddlpy<0.4.0 does not yet have `ddlpy.dataframe_to_xarray()`
 	"rws-ddlpy>=0.4.0",
 	#pooch<1.1.0 do not have attribute retrieve
 	"pooch>=1.1.0",
 	#hydrolib-core 0.7.0 supports meshkernel>=4.1.0
 	"hydrolib-core>=0.7.0",
 	#meshkernel<4.1.0 does not support contacts_get, no macos support, etc
@@ -80,19 +80,19 @@
 	"flake8",
 	"pytest",
 	"pytest-cov",
 	"twine",
 	"build",
 ]
 docs = [
-	"mkdocs",
-	"mkdocs-material",
-	"mkdocs-jupyter",
-	"mkdocstrings-python",
-	"mkdocs-exclude",
+	"sphinx>=1.8.1",
+	"sphinx_mdinclude",
+	"nbsphinx",
+	"pydata-sphinx-theme",
+	#"pandoc", # installed with choco on github
 ]
 examples = [
 	"jupyter",
 	"notebook",
 ]
 
 [tool.setuptools]
```

### Comparing `dfm_tools-0.22.0/tests/test_bathymetry.py` & `dfm_tools-0.23.0/tests/test_bathymetry.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_coastlines.py` & `dfm_tools-0.23.0/tests/test_coastlines.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_data.py` & `dfm_tools-0.23.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_dfm_tools.py` & `dfm_tools-0.23.0/tests/test_dfm_tools.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_download.py` & `dfm_tools-0.23.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_examples.py` & `dfm_tools-0.23.0/tests/test_examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import glob
 import subprocess
 
 # ACCEPTANCE TESTS VIA EXAMPLE SCRIPTS, these are the ones who are only meant to generate output files
 
 dir_tests = os.path.dirname(__file__) #F9 doesnt work, only F5 (F5 also only method to reload external definition scripts)
 list_configfiles = glob.glob(os.path.join(dir_tests,'examples','*.py'))
-list_configfiles = [x for x in list_configfiles if 'postprocess_xarray_performance' not in x] #ignore this slow script
 dir_output_general = os.path.join(dir_tests,'examples_output')
 os.makedirs(dir_output_general, exist_ok=True)
 
 @pytest.mark.requireslocaldata
 @pytest.mark.acceptance
 @pytest.mark.parametrize("file_config", [pytest.param(file_config, id=os.path.basename(file_config).replace('.py','')) for file_config in list_configfiles])
 def test_run_examples(file_config):
```

### Comparing `dfm_tools-0.22.0/tests/test_external_packages.py` & `dfm_tools-0.23.0/tests/test_external_packages.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_get_nc.py` & `dfm_tools-0.23.0/tests/test_get_nc.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_hydrolib_helpers.py` & `dfm_tools-0.23.0/tests/test_hydrolib_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_interpolate_grid2bnd.py` & `dfm_tools-0.23.0/tests/test_interpolate_grid2bnd.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_meshkernel_helpers.py` & `dfm_tools-0.23.0/tests/test_meshkernel_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_modelbuilder.py` & `dfm_tools-0.23.0/tests/test_modelbuilder.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_observations.py` & `dfm_tools-0.23.0/tests/test_observations.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_xarray_helpers.py` & `dfm_tools-0.23.0/tests/test_xarray_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.22.0/tests/test_xugrid_helpers.py` & `dfm_tools-0.23.0/tests/test_xugrid_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,7 +185,21 @@
     
     uds_rst = dfmt.open_partitioned_dataset(file_nc_rst, preprocess=dfmt.enrich_rst_with_map)
     
     uds_rst.s1.isel(time=0).ugrid.plot()
     
     uda_rst = uds_rst['DetCS1']
     assert "mesh2d_face_x" in uda_rst.coords
+
+
+@pytest.mark.unittest
+def test_open_dataset_delft3d4():
+    file_nc = dfmt.data.d3d_curvedbend_trim(return_filepath=True)
+
+    uds = dfmt.open_dataset_delft3d4(file_nc)
+
+    assert "mesh2d" in uds.grid.to_dataset().data_vars
+    assert "vertical_dimensions" in uds.grid.attrs
+    assert "grid" not in uds.data_vars
+
+    # test if plotting works, this is a basic validation of whether it is a proper ugrid dataset
+    uds.umag.isel(time=-1, KMAXOUT_RESTR=-1).ugrid.plot()
```

