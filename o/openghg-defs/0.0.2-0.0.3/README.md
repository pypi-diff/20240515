# Comparing `tmp/openghg_defs-0.0.2.tar.gz` & `tmp/openghg_defs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openghg_defs-0.0.2.tar", last modified: Tue Jul 18 15:18:58 2023, max compression
+gzip compressed data, was "openghg_defs-0.0.3.tar", last modified: Wed May 15 19:22:20 2024, max compression
```

## Comparing `openghg_defs-0.0.2.tar` & `openghg_defs-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,33 @@
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.607221 openghg_defs-0.0.2/
--rw-r--r--   0 gar        (501) staff       (20)     1064 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/LICENSE
--rw-r--r--   0 gar        (501) staff       (20)     2632 2023-07-18 15:18:58.607082 openghg_defs-0.0.2/PKG-INFO
--rw-r--r--   0 gar        (501) staff       (20)     2281 2023-07-18 11:11:37.000000 openghg_defs-0.0.2/README.md
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.600551 openghg_defs-0.0.2/openghg_defs/
--rw-r--r--   0 gar        (501) staff       (20)      279 2023-07-18 11:11:37.000000 openghg_defs-0.0.2/openghg_defs/__init__.py
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.602426 openghg_defs-0.0.2/openghg_defs/__pycache__/
--rw-r--r--   0 gar        (501) staff       (20)      571 2023-07-14 11:08:13.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 gar        (501) staff       (20)      791 2023-03-21 14:59:46.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 gar        (501) staff       (20)     1305 2023-03-21 14:54:07.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/_load.cpython-39.pyc
--rw-r--r--   0 gar        (501) staff       (20)      822 2023-03-21 14:54:07.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/_paths.cpython-39.pyc
--rw-r--r--   0 gar        (501) staff       (20)    14392 2023-07-14 11:08:13.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/_version.cpython-310.pyc
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.603667 openghg_defs-0.0.2/openghg_defs/data/
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.606852 openghg_defs-0.0.2/openghg_defs/data/domain/
--rw-r--r--   0 gar        (501) staff       (20)     5750 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/ARCTIC_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)    25879 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/ARCTIC_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     8523 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/EASTASIA_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     9775 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/EASTASIA_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     7325 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/EUROPE_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)    10054 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/EUROPE_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     7714 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/PACIFIC_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)    10300 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/PACIFIC_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     7599 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/SOUTHAFRICA_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     9918 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/SOUTHAFRICA_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     5475 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/USA_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     7436 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/USA_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     2297 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain_info.json
--rw-r--r--   0 gar        (501) staff       (20)    82852 2023-07-18 11:11:37.000000 openghg_defs-0.0.2/openghg_defs/data/site_info.json
--rw-r--r--   0 gar        (501) staff       (20)    18967 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/species_info.json
--rw-r--r--   0 gar        (501) staff       (20)        0 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/py.typed
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.601037 openghg_defs-0.0.2/openghg_defs.egg-info/
--rw-r--r--   0 gar        (501) staff       (20)     2632 2023-07-18 15:18:58.000000 openghg_defs-0.0.2/openghg_defs.egg-info/PKG-INFO
--rw-r--r--   0 gar        (501) staff       (20)     1125 2023-07-18 15:18:58.000000 openghg_defs-0.0.2/openghg_defs.egg-info/SOURCES.txt
--rw-r--r--   0 gar        (501) staff       (20)        1 2023-07-18 15:18:58.000000 openghg_defs-0.0.2/openghg_defs.egg-info/dependency_links.txt
--rw-r--r--   0 gar        (501) staff       (20)       32 2023-07-18 15:18:58.000000 openghg_defs-0.0.2/openghg_defs.egg-info/top_level.txt
--rw-r--r--   0 gar        (501) staff       (20)      578 2023-07-18 11:33:14.000000 openghg_defs-0.0.2/pyproject.toml
--rw-r--r--   0 gar        (501) staff       (20)       38 2023-07-18 15:18:58.607262 openghg_defs-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:22:20.467462 openghg_defs-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-15 19:22:20.467462 openghg_defs-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:22:20.463462 openghg_defs-0.0.3/openghg_defs/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:22:20.463462 openghg_defs-0.0.3/openghg_defs/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:22:20.467462 openghg_defs-0.0.3/openghg_defs/data/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/ARCTIC_latitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/ARCTIC_longitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/EASTASIA_latitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/EASTASIA_longitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/EUROPE_latitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/EUROPE_longitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/PACIFIC_latitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/PACIFIC_longitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/SOUTHAFRICA_latitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/SOUTHAFRICA_longitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/USA_latitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain/USA_longitude.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/domain_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84863 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/site_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/data/species_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/openghg_defs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:22:20.467462 openghg_defs-0.0.3/openghg_defs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-15 19:22:20.000000 openghg_defs-0.0.3/openghg_defs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-15 19:22:20.000000 openghg_defs-0.0.3/openghg_defs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:22:20.000000 openghg_defs-0.0.3/openghg_defs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 19:22:20.000000 openghg_defs-0.0.3/openghg_defs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:22:20.467462 openghg_defs-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:22:20.467462 openghg_defs-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-15 19:22:12.000000 openghg_defs-0.0.3/tests/test_valid.py
```

### Comparing `openghg_defs-0.0.2/LICENSE` & `openghg_defs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/PKG-INFO` & `openghg_defs-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openghg_defs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Supplementary definition data for OpenGHG
 License: MIT License
 Project-URL: Homepage, https://github.com/openghg/openghg_defs
 Project-URL: Bug Tracker, https://github.com/openghg/openghg_defs/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,14 @@
 # openghg_defs
 
 This repository contains the supplementary information / metadata around site, species and domain details. This is used within the OpenGHG project.
 
 ## Installation
 
 Note that `openghg_defs` should be installed in the same virtual environment as OpenGHG.
-There are two ways of installing `openghg_defs`, as an editable install of this git repository or via PyPI. 
 
 ### Editable install
 
 If you feel like you'll want to make changes to the metadata stored you should go for an editable install of the git repository. This will help ensure you always have the latest development changes we make to the repository. It also
 means that you can make changes to your local copy of the metadata and see the results straight away in your
 OpenGHG workflow.
 
@@ -28,15 +27,15 @@
 
 ```console
 git clone https://github.com/openghg/openghg_defs.git
 ```
 
 Next, move into the repository and use pip to create an editable install using the `-e` flag.
 
-> **_NOTE:_**  If you're using OpenGHG, please install `openghg_defs` in the [same virtual environment](https://docs.openghg.org/install.html#id1).
+> **_NOTE:_** If you're using OpenGHG, please install `openghg_defs` in the [same virtual environment](https://docs.openghg.org/install.html#id1).
 
 ```console
 cd openghg_defs
 pip install -e .
 ```
 
 This will create a symbolic link between the folder and your Python environment, meaning any changes you make to
@@ -66,14 +65,56 @@
 import openghg_defs
 
 species_info_file = openghg_defs.species_info_file
 site_info_file = openghg_defs.site_info_file
 domain_info_file = openghg_defs.domain_info_file
 ```
 
-## Updating information
+## Development
+
+### Updating information
 
 We invite users to update the information we have stored. If you find a mistake in the data or want to add something, please
 [open an issue](https://github.com/openghg/supplementary_data/issues/new) and fill out the template that matches your
-problem.
+problem. You're also welcome to submit a pull-request with your fix.
+
+For the recommended development process please see the [OpenGHG documentation](https://docs.openghg.org/development/python_devel.html)
+
+### Run the tests
+
+After making changes to the package please ensure you've added a test if adding new functionality and run the tests making sure they all pass.
+
+```console
+pytest -v tests/
+```
+
+### Release
+
+The package is released using GitHub actions and pushed to conda and PyPI.
+
+#### 1. Update the CHANGELOG
+
+- Update the changelog to add the header for the new version and add the date.
+- Update the Unreleased header to match the version you're releasing and `...HEAD`.
+
+#### 2. Update `pyproject.toml`
+
+For a new release the package version must be updated in the `pyproject.toml` file. Try and follow the [Semantic Versioning](https://semver.org/) method.
+
+#### 3. Tag the commit
+
+Now tag the commit. First we create the tag and add a message (remember to insert correct version numbers here).
+
+```console
+git tag -a x.x.x -m "openghg_defs release vx.x.x"
+```
+
+Next push the tag. This will trigger the automated release by GitHub Actions.
+
+```console
+git push origin x.x.x
+```
+
+#### 4. Check GitHub Actions runners
 
-You're also welcome to submit a pull-request with your fix.
+Check the GitHub Actions [runners](https://github.com/openghg/openghg_defs/actions) to ensure the tests have
+all passed and the build for conda and PyPI has run successfully.
```

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/ARCTIC_latitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/ARCTIC_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/ARCTIC_longitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/ARCTIC_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/EASTASIA_latitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/EASTASIA_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/EASTASIA_longitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/EASTASIA_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/EUROPE_latitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/EUROPE_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/EUROPE_longitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/EUROPE_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/PACIFIC_latitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/PACIFIC_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/PACIFIC_longitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/PACIFIC_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/SOUTHAFRICA_latitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/SOUTHAFRICA_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/SOUTHAFRICA_longitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/SOUTHAFRICA_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/USA_latitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/USA_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain/USA_longitude.dat` & `openghg_defs-0.0.3/openghg_defs/data/domain/USA_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/domain_info.json` & `openghg_defs-0.0.3/openghg_defs/data/domain_info.json`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.2/openghg_defs/data/site_info.json` & `openghg_defs-0.0.3/openghg_defs/data/site_info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735667293233083%*

 * *Differences: {"'AZV'": "OrderedDict([('NIES', OrderedDict([('height', ['50m']), ('height_name', ['50magl']), "*

 * *          "('height_station_masl', 110), ('latitude', 54.705), ('long_name', 'Azovo, Russia'), "*

 * *          "('longitude', 73.0292)]))])",*

 * * "'BRZ'": "OrderedDict([('NIES', OrderedDict([('height', ['80m']), ('height_name', ['80magl']), "*

 * *          "('height_station_masl', 168), ('latitude', 56.1458), ('long_name', 'Berezorechka, "*

 * *          "Russia'), ('longitude', 84.3319)]))])",*

 * * "'BSD'": "{'DECC': {'height_nam […]*

```diff
@@ -250,14 +250,28 @@
             ],
             "height_station_masl": 19.0,
             "latitude": 38.766,
             "long_name": "Terceira Island, Azores, Portugal",
             "longitude": -27.375
         }
     },
+    "AZV": {
+        "NIES": {
+            "height": [
+                "50m"
+            ],
+            "height_name": [
+                "50magl"
+            ],
+            "height_station_masl": 110,
+            "latitude": 54.705,
+            "long_name": "Azovo, Russia",
+            "longitude": 73.0292
+        }
+    },
     "BAL": {
         "NOAA": {
             "height_station_masl": 3.0,
             "latitude": 55.35,
             "long_name": "Baltic Sea, Poland",
             "longitude": 17.22
         }
@@ -486,14 +500,28 @@
             ],
             "height_station_masl": 11.0,
             "latitude": 71.323,
             "long_name": "Barrow, Alaska",
             "longitude": -156.6114
         }
     },
+    "BRZ": {
+        "NIES": {
+            "height": [
+                "80m"
+            ],
+            "height_name": [
+                "80magl"
+            ],
+            "height_station_masl": 168,
+            "latitude": 56.1458,
+            "long_name": "Berezorechka, Russia",
+            "longitude": 84.3319
+        }
+    },
     "BSC": {
         "NOAA": {
             "height_station_masl": 0.0,
             "latitude": 44.1776,
             "long_name": "Black Sea, Constanta, Romania",
             "longitude": 28.6647
         }
@@ -527,19 +555,26 @@
                 }
             ],
             "height": [
                 "248m",
                 "108m",
                 "42m"
             ],
-            "height_name": [
-                "248magl",
-                "108magl",
-                "42magl"
-            ],
+            "height_name": {
+                "108m": [
+                    "108magl"
+                ],
+                "248m": [
+                    "248magl",
+                    "250magl"
+                ],
+                "42m": [
+                    "42magl"
+                ]
+            },
             "height_station_masl": 382,
             "latitude": 54.35861,
             "long_name": "Bilsdale, UK",
             "longitude": -1.15036
         },
         "NOAA": {
             "height": [
@@ -1475,14 +1510,26 @@
         "NOAA": {
             "height_station_masl": 0.0,
             "latitude": 13.386,
             "long_name": "Mariana Islands, Guam",
             "longitude": 144.656
         }
     },
+    "GOSAT-ALASKA": {
+        "GOSAT/GOSAT-ALASKA": {
+            "height": [
+                "column"
+            ],
+            "height_name": [
+                "column"
+            ],
+            "long_name": "GOSAT, Alaska",
+            "platform": "satellite"
+        }
+    },
     "GOSAT-BRAZIL": {
         "GOSAT/GOSAT-BRAZIL": {
             "height": [
                 "column"
             ],
             "height_name": [
                 "column"
@@ -1886,14 +1933,26 @@
             ],
             "height_station_masl": 118.0,
             "latitude": 63.4,
             "long_name": "Storhofdi, Vestmannaeyjar, Iceland",
             "longitude": -20.288
         }
     },
+    "IMP": {
+        "height": [
+            "26m"
+        ],
+        "height_name": [
+            "26magl"
+        ],
+        "height_station_masl": 36.0,
+        "latitude": 51.4988,
+        "long_name": "Imperial College London, London, UK",
+        "longitude": -0.1749
+    },
     "INU": {
         "EC": {
             "height": [
                 "10m"
             ],
             "height_name": [
                 "10magl"
@@ -2195,17 +2254,23 @@
             "long_name": "Key Biscane, Florida",
             "longitude": -80.158
         }
     },
     "KIT": {
         "ICOS": {
             "height": [
+                "30m",
+                "60m",
+                "100m",
                 "200m"
             ],
             "height_name": [
+                "30magl",
+                "60magl",
+                "100magl",
                 "200magl"
             ],
             "height_station_masl": 110.0,
             "latitude": 49.0915,
             "long_name": "Karlsruhe, Germany",
             "longitude": 8.4249
         }
@@ -2268,14 +2333,28 @@
             ],
             "height_station_masl": 534.0,
             "latitude": 49.583,
             "long_name": "Kresin u Pacova, Czech Republic",
             "longitude": 15.083
         }
     },
+    "KRS": {
+        "NIES": {
+            "height": [
+                "67m"
+            ],
+            "height_name": [
+                "67magl"
+            ],
+            "height_station_masl": 76,
+            "latitude": 58.2456,
+            "long_name": "Karasevoe, Russia",
+            "longitude": 82.4244
+        }
+    },
     "KUM": {
         "NOAA": {
             "height": [
                 "10m"
             ],
             "height_name": [
                 "10magl"
@@ -2885,14 +2964,28 @@
             ],
             "height_station_masl": 46.0,
             "latitude": 60.0864,
             "long_name": "Norunda, Sweden",
             "longitude": 17.4794
         }
     },
+    "NOY": {
+        "NIES": {
+            "height": [
+                "43m"
+            ],
+            "height_name": [
+                "43magl"
+            ],
+            "height_station_masl": 108,
+            "latitude": 63.4292,
+            "long_name": "Noyabrsk, Russia",
+            "longitude": 75.78
+        }
+    },
     "NPL": {
         "LGHG": {
             "height": [
                 "NA"
             ],
             "height_name": [
                 "NA"
@@ -4114,14 +4207,38 @@
             ],
             "height_station_masl": 131.0,
             "latitude": 47.9647,
             "long_name": "Trainou, France",
             "longitude": 2.1125
         }
     },
+    "TROPOMI-ALASKA": {
+        "TROPOMI/TROPOMI-ALASKA": {
+            "height": [
+                "column"
+            ],
+            "height_name": [
+                "column"
+            ],
+            "long_name": "TROPOMI, ALASKA",
+            "platform": "satellite"
+        }
+    },
+    "TROPOMI-WFMD-ALASKA": {
+        "TROPOMI/TROPOMI-WFMD-ALASKA": {
+            "height": [
+                "column"
+            ],
+            "height_name": [
+                "column"
+            ],
+            "long_name": "TROPOMI-WFMD, ALASKA",
+            "platform": "satellite"
+        }
+    },
     "TTA": {
         "DECC": {
             "height": [
                 "222m"
             ],
             "height_name": [
                 "222magl"
@@ -4240,14 +4357,28 @@
                 "10magl"
             ],
             "latitude": 51.908,
             "long_name": "Valentia, Ireland",
             "longitude": -10.403
         }
     },
+    "VGN": {
+        "NIES": {
+            "height": [
+                "85m"
+            ],
+            "height_name": [
+                "85magl"
+            ],
+            "height_station_masl": 192,
+            "latitude": 54.4972,
+            "long_name": "Vaganovo, Russia",
+            "longitude": 62.3247
+        }
+    },
     "VGR": {
         "CNR": {
             "height": [
                 "5m"
             ],
             "height_name": [
                 "5magl"
```

### Comparing `openghg_defs-0.0.2/openghg_defs/data/species_info.json` & `openghg_defs-0.0.3/openghg_defs/data/species_info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878048780487805%*

 * *Differences: {"'ClCH2CH2Cl'": "OrderedDict([('alt', ['1,2-DCA', 'EDC', '1,2-dichloroethane']), ('group', "*

 * *                 "'Chloromethanes'), ('name', '1,2-dichloroethane'), ('long_name', "*

 * *                 "'1,2-dichloroethane'), ('mol_mass', '98.959'), ('print_string', "*

 * *                 "'ClCH$_2$CH$_2$Cl'), ('units', 'ppt')])"}*

```diff
@@ -387,14 +387,27 @@
         "group": "CO2",
         "long_name": "Carbon dioxide",
         "mol_mass": "44.01",
         "name": "carbon_dioxide",
         "print_string": "CO$_2$",
         "units": "ppm"
     },
+    "ClCH2CH2Cl": {
+        "alt": [
+            "1,2-DCA",
+            "EDC",
+            "1,2-dichloroethane"
+        ],
+        "group": "Chloromethanes",
+        "long_name": "1,2-dichloroethane",
+        "mol_mass": "98.959",
+        "name": "1,2-dichloroethane",
+        "print_string": "ClCH$_2$CH$_2$Cl",
+        "units": "ppt"
+    },
     "DCH4C13": {
         "alt": [
             "d13ch4",
             "delta_ch4_c13",
             "CH4C13"
         ],
         "group": "CH4",
```

### Comparing `openghg_defs-0.0.2/openghg_defs.egg-info/PKG-INFO` & `openghg_defs-0.0.3/openghg_defs.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openghg-defs
-Version: 0.0.2
+Name: openghg_defs
+Version: 0.0.3
 Summary: Supplementary definition data for OpenGHG
 License: MIT License
 Project-URL: Homepage, https://github.com/openghg/openghg_defs
 Project-URL: Bug Tracker, https://github.com/openghg/openghg_defs/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,14 @@
 # openghg_defs
 
 This repository contains the supplementary information / metadata around site, species and domain details. This is used within the OpenGHG project.
 
 ## Installation
 
 Note that `openghg_defs` should be installed in the same virtual environment as OpenGHG.
-There are two ways of installing `openghg_defs`, as an editable install of this git repository or via PyPI. 
 
 ### Editable install
 
 If you feel like you'll want to make changes to the metadata stored you should go for an editable install of the git repository. This will help ensure you always have the latest development changes we make to the repository. It also
 means that you can make changes to your local copy of the metadata and see the results straight away in your
 OpenGHG workflow.
 
@@ -28,15 +27,15 @@
 
 ```console
 git clone https://github.com/openghg/openghg_defs.git
 ```
 
 Next, move into the repository and use pip to create an editable install using the `-e` flag.
 
-> **_NOTE:_**  If you're using OpenGHG, please install `openghg_defs` in the [same virtual environment](https://docs.openghg.org/install.html#id1).
+> **_NOTE:_** If you're using OpenGHG, please install `openghg_defs` in the [same virtual environment](https://docs.openghg.org/install.html#id1).
 
 ```console
 cd openghg_defs
 pip install -e .
 ```
 
 This will create a symbolic link between the folder and your Python environment, meaning any changes you make to
@@ -66,14 +65,56 @@
 import openghg_defs
 
 species_info_file = openghg_defs.species_info_file
 site_info_file = openghg_defs.site_info_file
 domain_info_file = openghg_defs.domain_info_file
 ```
 
-## Updating information
+## Development
+
+### Updating information
 
 We invite users to update the information we have stored. If you find a mistake in the data or want to add something, please
 [open an issue](https://github.com/openghg/supplementary_data/issues/new) and fill out the template that matches your
-problem.
+problem. You're also welcome to submit a pull-request with your fix.
+
+For the recommended development process please see the [OpenGHG documentation](https://docs.openghg.org/development/python_devel.html)
+
+### Run the tests
+
+After making changes to the package please ensure you've added a test if adding new functionality and run the tests making sure they all pass.
+
+```console
+pytest -v tests/
+```
+
+### Release
+
+The package is released using GitHub actions and pushed to conda and PyPI.
+
+#### 1. Update the CHANGELOG
+
+- Update the changelog to add the header for the new version and add the date.
+- Update the Unreleased header to match the version you're releasing and `...HEAD`.
+
+#### 2. Update `pyproject.toml`
+
+For a new release the package version must be updated in the `pyproject.toml` file. Try and follow the [Semantic Versioning](https://semver.org/) method.
+
+#### 3. Tag the commit
+
+Now tag the commit. First we create the tag and add a message (remember to insert correct version numbers here).
+
+```console
+git tag -a x.x.x -m "openghg_defs release vx.x.x"
+```
+
+Next push the tag. This will trigger the automated release by GitHub Actions.
+
+```console
+git push origin x.x.x
+```
+
+#### 4. Check GitHub Actions runners
 
-You're also welcome to submit a pull-request with your fix.
+Check the GitHub Actions [runners](https://github.com/openghg/openghg_defs/actions) to ensure the tests have
+all passed and the build for conda and PyPI has run successfully.
```

### Comparing `openghg_defs-0.0.2/openghg_defs.egg-info/SOURCES.txt` & `openghg_defs-0.0.3/openghg_defs.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,27 +3,23 @@
 pyproject.toml
 openghg_defs/__init__.py
 openghg_defs/py.typed
 openghg_defs.egg-info/PKG-INFO
 openghg_defs.egg-info/SOURCES.txt
 openghg_defs.egg-info/dependency_links.txt
 openghg_defs.egg-info/top_level.txt
-openghg_defs/__pycache__/__init__.cpython-310.pyc
-openghg_defs/__pycache__/__init__.cpython-39.pyc
-openghg_defs/__pycache__/_load.cpython-39.pyc
-openghg_defs/__pycache__/_paths.cpython-39.pyc
-openghg_defs/__pycache__/_version.cpython-310.pyc
 openghg_defs/data/domain_info.json
 openghg_defs/data/site_info.json
 openghg_defs/data/species_info.json
 openghg_defs/data/domain/ARCTIC_latitude.dat
 openghg_defs/data/domain/ARCTIC_longitude.dat
 openghg_defs/data/domain/EASTASIA_latitude.dat
 openghg_defs/data/domain/EASTASIA_longitude.dat
 openghg_defs/data/domain/EUROPE_latitude.dat
 openghg_defs/data/domain/EUROPE_longitude.dat
 openghg_defs/data/domain/PACIFIC_latitude.dat
 openghg_defs/data/domain/PACIFIC_longitude.dat
 openghg_defs/data/domain/SOUTHAFRICA_latitude.dat
 openghg_defs/data/domain/SOUTHAFRICA_longitude.dat
 openghg_defs/data/domain/USA_latitude.dat
-openghg_defs/data/domain/USA_longitude.dat
+openghg_defs/data/domain/USA_longitude.dat
+tests/test_valid.py
```

### Comparing `openghg_defs-0.0.2/pyproject.toml` & `openghg_defs-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openghg_defs"
-version = "0.0.2"
+version = "0.0.3"
 description = "Supplementary definition data for OpenGHG"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
 
 [project.urls]
 "Homepage" = "https://github.com/openghg/openghg_defs"
```

