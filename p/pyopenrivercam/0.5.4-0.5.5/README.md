# Comparing `tmp/pyopenrivercam-0.5.4.tar.gz` & `tmp/pyopenrivercam-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenrivercam-0.5.4.tar", last modified: Tue Mar 26 08:58:23 2024, max compression
+gzip compressed data, was "pyopenrivercam-0.5.5.tar", last modified: Wed May 15 12:25:37 2024, max compression
```

## Comparing `pyopenrivercam-0.5.4.tar` & `pyopenrivercam-0.5.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:58:23.691597 pyopenrivercam-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-03-26 08:58:23.691597 pyopenrivercam-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:58:23.687597 pyopenrivercam-0.5.4/pyopenrivercam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-03-26 08:58:23.000000 pyopenrivercam-0.5.4/pyopenrivercam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-26 08:58:23.000000 pyopenrivercam-0.5.4/pyopenrivercam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:58:23.000000 pyopenrivercam-0.5.4/pyopenrivercam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-26 08:58:23.000000 pyopenrivercam-0.5.4/pyopenrivercam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:58:23.000000 pyopenrivercam-0.5.4/pyopenrivercam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-26 08:58:23.000000 pyopenrivercam-0.5.4/pyopenrivercam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-26 08:58:23.000000 pyopenrivercam-0.5.4/pyopenrivercam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:58:23.683597 pyopenrivercam-0.5.4/pyorc/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:58:23.687597 pyopenrivercam-0.5.4/pyorc/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44392 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/api/cameraconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    21600 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/api/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/api/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/api/orcbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    26705 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/api/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/api/transect.py
--rw-r--r--   0 runner    (1001) docker     (127)    12044 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/api/velocimetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18935 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:58:23.687597 pyopenrivercam-0.5.4/pyorc/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/cli/cli_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/cli/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    32551 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    25208 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/piv_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:58:23.687597 pyopenrivercam-0.5.4/pyorc/service/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/service/camera_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23635 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/pyorc/service/velocimetry.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 08:58:23.691597 pyopenrivercam-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:58:23.687597 pyopenrivercam-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16875 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/tests/test_cameraconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/tests/test_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/tests/test_transect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/tests/test_velocimetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-26 08:58:04.000000 pyopenrivercam-0.5.4/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:25:37.893223 pyopenrivercam-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-05-15 12:25:37.893223 pyopenrivercam-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:25:37.893223 pyopenrivercam-0.5.5/pyopenrivercam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-05-15 12:25:37.000000 pyopenrivercam-0.5.5/pyopenrivercam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-15 12:25:37.000000 pyopenrivercam-0.5.5/pyopenrivercam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:25:37.000000 pyopenrivercam-0.5.5/pyopenrivercam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 12:25:37.000000 pyopenrivercam-0.5.5/pyopenrivercam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:25:37.000000 pyopenrivercam-0.5.5/pyopenrivercam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-15 12:25:37.000000 pyopenrivercam-0.5.5/pyopenrivercam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:25:37.000000 pyopenrivercam-0.5.5/pyopenrivercam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:25:37.885223 pyopenrivercam-0.5.5/pyorc/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:25:37.889223 pyopenrivercam-0.5.5/pyorc/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44392 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/api/cameraconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21687 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/api/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/api/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/api/orcbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26705 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/api/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/api/transect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12044 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/api/velocimetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19327 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:25:37.889223 pyopenrivercam-0.5.5/pyorc/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/cli/cli_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32602 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25208 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/piv_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:25:37.889223 pyopenrivercam-0.5.5/pyorc/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/service/camera_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23906 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/pyorc/service/velocimetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:25:37.893223 pyopenrivercam-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:25:37.893223 pyopenrivercam-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16875 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/tests/test_cameraconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/tests/test_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/tests/test_transect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/tests/test_velocimetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-15 12:25:05.000000 pyopenrivercam-0.5.5/tests/test_video.py
```

### Comparing `pyopenrivercam-0.5.4/LICENSE` & `pyopenrivercam-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/PKG-INFO` & `pyopenrivercam-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenrivercam
-Version: 0.5.4
+Version: 0.5.5
 Summary: pyopenrivercam (pyorc) is a front and backend to control river camera observation locations
 Home-page: https://github.com/localdevices/pyorc
 Author: Hessel Winsemius
 Author-email: winsemius@rainbowsensing.com
 License: AGPLv3
 Keywords: hydrology,hydrometry,river-flow,pyorc
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopenrivercam-0.5.4/README.md` & `pyopenrivercam-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyopenrivercam.egg-info/PKG-INFO` & `pyopenrivercam-0.5.5/pyopenrivercam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenrivercam
-Version: 0.5.4
+Version: 0.5.5
 Summary: pyopenrivercam (pyorc) is a front and backend to control river camera observation locations
 Home-page: https://github.com/localdevices/pyorc
 Author: Hessel Winsemius
 Author-email: winsemius@rainbowsensing.com
 License: AGPLv3
 Keywords: hydrology,hydrometry,river-flow,pyorc
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopenrivercam-0.5.4/pyopenrivercam.egg-info/SOURCES.txt` & `pyopenrivercam-0.5.5/pyopenrivercam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/api/cameraconfig.py` & `pyopenrivercam-0.5.5/pyorc/api/cameraconfig.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/api/frames.py` & `pyopenrivercam-0.5.5/pyorc/api/frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,16 @@
             self._obj,
             cc,
             x,
             y,
             z,
             **kwargs
         )
+        # ensure no missing values are persisting
+        da_proj = da_proj.fillna(0.)
         # assign coordinates
         da_proj = da_proj.frames._add_xy_coords([xs, ys, lons, lats], coords, const.GEOGRAPHICAL_ATTRS)
         if "rgb" in da_proj.dims and len(da_proj.dims) == 4:
             # ensure that "rgb" is the last dimension
             da_proj = da_proj.transpose("time", "y", "x", "rgb")
         # in case resolution was changed, overrule the camera_config attribute
         da_proj.attrs.update(camera_config=cc.to_json())
```

### Comparing `pyopenrivercam-0.5.4/pyorc/api/mask.py` & `pyopenrivercam-0.5.5/pyorc/api/mask.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/api/orcbase.py` & `pyopenrivercam-0.5.5/pyorc/api/orcbase.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/api/plot.py` & `pyopenrivercam-0.5.5/pyorc/api/plot.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/api/transect.py` & `pyopenrivercam-0.5.5/pyorc/api/transect.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/api/velocimetry.py` & `pyopenrivercam-0.5.5/pyorc/api/velocimetry.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/api/video.py` & `pyopenrivercam-0.5.5/pyorc/api/video.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import os
 import warnings
 import xarray as xr
 
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Literal
 
 from .. import cv, const, helpers
 from .cameraconfig import load_camera_config, get_camera_config, CameraConfig
 
 
 class Video:  # (cv2.VideoCapture)
     def __repr__(self):
@@ -132,15 +132,15 @@
         # extract times, frame numbers and frames as far as available
         time, frame_number, frames = cv.get_time_frames(
             cap,
             start_frame,
             end_frame,
             lazy=lazy,
             rotation=self.rotation,
-            method="grayscale",
+            method="rgb",
             fps=fps
         )
         self.frames = frames
         # check if end_frame changed
         if frame_number[-1] != end_frame:
             warnings.warn(f"End frame {end_frame} cannot be read from file. End frame is adapted to {frame_number[-1]}")
             end_frame = frame_number[-1]
@@ -389,15 +389,15 @@
         """
         self._rotation = helpers.get_rotation_code(rotation_code)
 
 
     def get_frame(
             self,
             n: int,
-            method: Optional[str] = "grayscale",
+            method: Optional[Literal["grayscale", "rgb", "hsv"]] = "grayscale"
     ) -> np.ndarray:
         """
         Retrieve one frame.
 
         Parameters:
         -----------
         n : int
@@ -409,16 +409,16 @@
         -------
         frame : np.ndarray
             2d array (grayscale) or 3d (rgb/hsv) with frame
         """
         assert (n >= 0), "frame number cannot be negative"
         assert (
                 n - self.start_frame <= self.end_frame - self.start_frame), "frame number is larger than the different between the start and end frame"
-        assert (method in ["grayscale", "rgb",
-                           "hsv"]), f'method must be "grayscale", "rgb" or "hsv", method is "{method}"'
+        # assert (method in ["grayscale", "rgb",
+        #                    "hsv"]), f'method must be "grayscale", "rgb" or "hsv", method is "{method}"'
         cap = cv2.VideoCapture(self.fn)
         cap.set(cv2.CAP_PROP_POS_FRAMES, n + self.start_frame)
         ret, img = cv.get_frame(
             cap,
             rotation=self.rotation,
             ms=self.ms[n] if self.ms else None,
             method=method
@@ -426,51 +426,57 @@
         self.frame_count = n + 1
         cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
         cap.release()
         return img
 
     def get_frames(
             self,
-            **kwargs
+            method: Optional[Literal["grayscale", "rgb", "hsv"]] = "grayscale"
     ) -> xr.DataArray:
         """
         Get a xr.DataArray, containing a dask array of frames, from `start_frame` until `end_frame`, expected to be read
         lazily. The xr.DataArray will contain all coordinate variables and attributes, needed for further processing
         steps.
 
         Parameters
         ----------
-        **kwargs: dict, optional
-            keyword arguments to pass to `get_frame`. Currently only `grayscale` is supported.
+        method: str, optional
+            method for color scaling, can be "
 
         Returns
         -------
         frames : xr.DataArray
             containing all requested frames
         """
         assert (hasattr(self,
                         "_camera_config")), "No camera configuration is set, add it to the video using the .camera_config method"
         # camera_config may be altered for the frames object, so copy below
         camera_config = copy.deepcopy(self.camera_config)
 
-        if self.frames is None or len(kwargs) > 0:
+        if self.frames is None:
             # a specific method for collecting frames is requested or lazy access is requested.
             get_frame = dask.delayed(self.get_frame, pure=True)  # Lazy version of get_frame
             # get all listed frames
-            frames = [get_frame(n=n, **kwargs) for n, f_number in enumerate(self.frame_number)]
+            frames = [get_frame(n=n, method=method) for n, f_number in enumerate(self.frame_number)]
             sample = frames[0].compute()
             data_array = [da.from_delayed(
                 frame,
                 dtype=sample.dtype,
                 shape=sample.shape
             ) for frame in frames]
             da_stack = da.stack(data_array, axis=0)
         else:
-            sample = self.frames[0]
             da_stack = self.frames
+            # ensure stabilisation and color scaling is applied
+            if self.ms is not None:
+                da_stack = np.array([cv.transform(cv.color_scale(img, method), m) for img, m in zip(da_stack, self.ms)])
+            else:
+                # only color transform
+                da_stack = np.array([cv.color_scale(img, method) for img in da_stack])
+            sample = da_stack[0]
 
         # undistort source control points
         # if hasattr(camera_config, "gcps"):
         #     camera_config.gcps["src"] = cv.undistort_points(
         #         camera_config.gcps["src"],
         #         camera_config.camera_matrix,
         #         camera_config.dist_coeffs,
```

### Comparing `pyopenrivercam-0.5.4/pyorc/cli/cli_elements.py` & `pyopenrivercam-0.5.5/pyorc/cli/cli_elements.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/cli/cli_utils.py` & `pyopenrivercam-0.5.5/pyorc/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/cli/log.py` & `pyopenrivercam-0.5.5/pyorc/cli/log.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/cli/main.py` & `pyopenrivercam-0.5.5/pyorc/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/const.py` & `pyopenrivercam-0.5.5/pyorc/const.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/cv.py` & `pyopenrivercam-0.5.5/pyorc/cv.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,14 +635,27 @@
     # dist_coeffs[4][0] = opt.x[3]
     # dist_coeffs[3][0] = opt.x[4]
     print(f"CAMERA MATRIX: {camera_matrix}")
     print(f"DIST COEFFS: {dist_coeffs}")
     return camera_matrix, dist_coeffs, opt.fun
 
 
+def color_scale(img, method):
+    if method == "grayscale":
+        # apply gray scaling, contrast- and gamma correction
+        # img = _corr_color(img, alpha=None, beta=None, gamma=0.4)
+        img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)  # mean(axis=2)
+    elif method == "rgb":
+        # turn bgr to rgb for plotting purposes
+        img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+    elif method == "hsv":
+        img = cv2.cvtColor(img, cv2.COLOR_BGR2HSV)
+    return img
+
+
 def get_frame(
         cap,
         rotation=None,
         ms=None,
         method="grayscale"
 ):
     try:
@@ -651,25 +664,18 @@
            img = cv2.rotate(img, rotation)
     except:
         raise IOError(f"Cannot read")
     if ret:
         if ms is not None:
             img = transform(img, ms)
         # apply lens distortion correction
-        if method == "grayscale":
-            # apply gray scaling, contrast- and gamma correction
-            # img = _corr_color(img, alpha=None, beta=None, gamma=0.4)
-            img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)  # mean(axis=2)
-        elif method == "rgb":
-            # turn bgr to rgb for plotting purposes
-            img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-        elif method == "hsv":
-            img = cv2.cvtColor(img, cv2.COLOR_BGR2HSV)
+        img = color_scale(img, method)
     return ret, img
 
+
 def get_frames(cap, start_frame, end_frame):
     """
     Get a set of frames from start_frame to end frame from a cap object
 
     Parameters
     ----------
     cap : cv.VideoCapture
```

### Comparing `pyopenrivercam-0.5.4/pyorc/helpers.py` & `pyopenrivercam-0.5.5/pyorc/helpers.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/piv_process.py` & `pyopenrivercam-0.5.5/pyorc/piv_process.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/project.py` & `pyopenrivercam-0.5.5/pyorc/project.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/service/camera_config.py` & `pyopenrivercam-0.5.5/pyorc/service/camera_config.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/pyorc/service/velocimetry.py` & `pyopenrivercam-0.5.5/pyorc/service/velocimetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,20 @@
             if set, only update components with changed inputs and configurations
         concurrency : bool, optional
             if set to False, then dask will only run synchronous preventing overuse of memory. This will be slower
 
         """
         if h_a is not None:
             recipe["video"]["h_a"] = h_a
+        # check what projection method is used, use throughout
+        self.proj_method = "cv"
+        proj = recipe["frames"].get("project")
+        if proj:
+            if proj.get("method") == "numpy":
+                self.proj_method = "numpy"
         self.update = update  # set to True when checks are needed if data already exists or not
         self.recipe = recipe
         self.output = output
         self.concurrency = concurrency
         self.prefix = prefix
         self.fn_piv = os.path.join(self.output, prefix + fn_piv)
         self.fn_piv_mask = os.path.join(self.output, prefix + fn_piv_mask) if "mask" in recipe else self.fn_piv
@@ -459,15 +465,15 @@
                 if "frame_number" in plot_params:
                     n = plot_params["frame_number"]
                 else:
                     n = 0
                 opts = plot_params["frames"] if plot_params["frames"] is not None else {}
                 f = self.video_obj.get_frames(method="rgb")
                 if mode != "camera":
-                    f = f.frames.project()[n]
+                    f = f.frames.project(method=self.proj_method)[n]
                 else:
                     f = f[n]
                 p = f.frames.plot(ax=ax, mode=mode, **opts)
                 # continue with axes of p
                 ax = p.axes
             if "velocimetry" in plot_params:
                 opts = plot_params["velocimetry"]
```

### Comparing `pyopenrivercam-0.5.4/setup.py` & `pyopenrivercam-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="pyopenrivercam",
     description="pyopenrivercam (pyorc) is a front and backend to control river camera observation locations",
-    version="0.5.4",
+    version="0.5.5",
     long_description=readme + "\n\n",
     long_description_content_type="text/markdown",
     url="https://github.com/localdevices/pyorc",
     author="Hessel Winsemius",
     author_email="winsemius@rainbowsensing.com",
     packages=find_packages(),
     package_dir={"pyorc": "pyorc"},
```

### Comparing `pyopenrivercam-0.5.4/tests/conftest.py` & `pyopenrivercam-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/tests/test_cameraconfig.py` & `pyopenrivercam-0.5.5/tests/test_cameraconfig.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/tests/test_cli.py` & `pyopenrivercam-0.5.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/tests/test_frames.py` & `pyopenrivercam-0.5.5/tests/test_frames.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/tests/test_mask.py` & `pyopenrivercam-0.5.5/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/tests/test_transect.py` & `pyopenrivercam-0.5.5/tests/test_transect.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/tests/test_velocimetry.py` & `pyopenrivercam-0.5.5/tests/test_velocimetry.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.4/tests/test_video.py` & `pyopenrivercam-0.5.5/tests/test_video.py`

 * *Files identical despite different names*

