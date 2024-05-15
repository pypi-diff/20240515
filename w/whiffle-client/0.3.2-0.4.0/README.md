# Comparing `tmp/whiffle_client-0.3.2.tar.gz` & `tmp/whiffle_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whiffle_client-0.3.2.tar", last modified: Thu Apr 25 06:57:57 2024, max compression
+gzip compressed data, was "whiffle_client-0.4.0.tar", last modified: Wed May 15 08:56:35 2024, max compression
```

## Comparing `whiffle_client-0.3.2.tar` & `whiffle_client-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.059095 whiffle_client-0.3.2/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)     3390 2024-04-25 06:57:57.059095 whiffle_client-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2413 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/USER_README.md
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 06:57:57.059095 whiffle_client-0.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.049095 whiffle_client-0.3.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4791 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.050095 whiffle_client-0.3.2/whiffle_client/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.054095 whiffle_client-0.3.2/whiffle_client/analysis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7628 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/io.py
--rw-rw-rw-   0 root         (0) root         (0)    16433 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     4854 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/scatter.py
--rw-rw-rw-   0 root         (0) root         (0)     4957 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/skill.py
--rw-rw-rw-   0 root         (0) root         (0)     3231 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/analysis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     8323 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/entrypoints.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.055095 whiffle_client-0.3.2/whiffle_client/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/resources/example_generic_params.json
--rw-rw-rw-   0 root         (0) root         (0)     1015 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/resources/example_yaml_include.yaml
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/resources/example_yaml_include_metmasts.yaml
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.055095 whiffle_client-0.3.2/whiffle_client/wind/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10808 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.057095 whiffle_client-0.3.2/whiffle_client/wind/components/
--rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/geometries.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/metmast.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/components/turbine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.058095 whiffle_client-0.3.2/whiffle_client/wind/loaders/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/loaders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/loaders/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-25 06:57:54.000000 whiffle_client-0.3.2/whiffle_client/wind/wind_simulation_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 06:57:57.058095 whiffle_client-0.3.2/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3390 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      189 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-25 06:57:57.000000 whiffle_client-0.3.2/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.938131 whiffle_client-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)    11095 2024-05-15 08:56:35.937131 whiffle_client-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    10139 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/USER_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 08:56:35.938131 whiffle_client-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.927131 whiffle_client-0.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.929131 whiffle_client-0.4.0/whiffle_client/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.931131 whiffle_client-0.4.0/whiffle_client/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7628 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    16433 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     4854 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/scatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4957 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/skill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3231 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/analysis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3995 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/base_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/entrypoints.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.932131 whiffle_client-0.4.0/whiffle_client/loaders/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/loaders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/loaders/csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.933131 whiffle_client-0.4.0/whiffle_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/resources/example_generic_params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/resources/example_yaml_include.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/resources/example_yaml_include_metmasts.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.933131 whiffle_client-0.4.0/whiffle_client/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/snippets/create_mock_powercurve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.933131 whiffle_client-0.4.0/whiffle_client/wind/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.935131 whiffle_client-0.4.0/whiffle_client/wind/components/
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/geometries.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/metmast.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/turbine.py
+-rw-rw-rw-   0 root         (0) root         (0)      988 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/turbine_model_specs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5011 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/wind_simulation_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/components/windfarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.936131 whiffle_client-0.4.0/whiffle_client/wind/mapping/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/mapping/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/mapping/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4760 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/mapping/turbine_model_specs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5983 2024-05-15 08:56:32.000000 whiffle_client-0.4.0/whiffle_client/wind/mapping/wind_simulation_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:56:35.936131 whiffle_client-0.4.0/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11095 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1652 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-15 08:56:35.000000 whiffle_client-0.4.0/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.3.2/LICENCE.txt` & `whiffle_client-0.4.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/README.md` & `whiffle_client-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/pyproject.toml` & `whiffle_client-0.4.0/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 dependencies = [
     "click~=8.0.4",
     "PyYAML~=6.0",
     "pyyaml-include~=1.3.1",
     "platformdirs~=4.0.0",
     "requests",
+    "pandas>=2",
     "jupyter"
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 analysis = [
     "numpy",
-    "pandas>=2",
     "scipy",
     "scikit-learn",
     "xarray>=2022.12.0",
     "netcdf4",
     "matplotlib",
     "hvplot",
     "jupyter_bokeh",
```

### Comparing `whiffle_client-0.3.2/whiffle_client/analysis/io.py` & `whiffle_client-0.4.0/whiffle_client/analysis/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/whiffle_client/analysis/plot.py` & `whiffle_client-0.4.0/whiffle_client/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/whiffle_client/analysis/scatter.py` & `whiffle_client-0.4.0/whiffle_client/analysis/scatter.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/whiffle_client/analysis/skill.py` & `whiffle_client-0.4.0/whiffle_client/analysis/skill.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/whiffle_client/analysis/utils.py` & `whiffle_client-0.4.0/whiffle_client/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/whiffle_client/client.py` & `whiffle_client-0.4.0/whiffle_client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 
 import json
 import os
 import time
 
 import pkg_resources
 import platformdirs
-import requests
 import yaml
-from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util.retry import Retry
 from yamlinclude import YamlIncludeConstructor
 
+from whiffle_client.base_client import BaseClient
 from whiffle_client.io import download_write_chunks
 
 CHUNK_SIZE = 1024 * 1024
 CONFIG_FILE_NAME = "whiffle_config.yaml"
 CONFIG_FILE_PATH_LOCATIONS = [
     f"{platformdirs.user_config_dir('whiffle')}/{CONFIG_FILE_NAME}",  # app path
     f"{CONFIG_FILE_NAME}",  # workdir path
@@ -31,91 +29,34 @@
     pass
 
 
 class NoTokenError(Exception):
     pass
 
 
-class Client:
-    """TODO: Client to launch task"""
-
-    def __init__(self, access_token=None, url=None, session=None):
-        """
-        Authentication order:
-        1. `access_token` passed when creating class.
-        2. token in CONFIG_FILE_PATH_LOCATIONS (JSON format)
-        """
-        if access_token is None:
-            config = self.get_config()
-            access_token = config["user"]["token"]
-        if url is None:
-            config = self.get_config()
-            url = config["whiffle"]["url"]
-        self.url = url
-        if session is None:
-            retries = 5
-            backoff_factor = 0.3
-            status_forcelist = (500, 502, 503, 504)
-            session = session or requests.Session()
-            retry = Retry(
-                total=retries,
-                read=retries,
-                connect=retries,
-                backoff_factor=backoff_factor,
-                status_forcelist=status_forcelist,
-            )
-            adapter = HTTPAdapter(max_retries=retry)
-            session.mount("http://", adapter)
-            session.mount("https://", adapter)
-
-        self.session = session
-        self.session.headers = {
-            "Content-Type": "application/json",
-            "Authorization": "Bearer {}".format(access_token),
-        }
-
-    @staticmethod
-    def get_config():
-        config = None
-        for file_path in CONFIG_FILE_PATH_LOCATIONS:
-            try:
-                with open(file_path) as file_object:
-                    config = yaml.safe_load(file_object)
-                if config:
-                    break
-            except FileNotFoundError:
-                continue
-
-        if config is None:
-            raise FileNotFoundError(
-                f"No valid config found on either of {CONFIG_FILE_PATH_LOCATIONS} locations"
-            )
-
-        return config
-
-    @staticmethod
-    def set_config(config):
-        config_file_path = CONFIG_FILE_PATH_LOCATIONS[0]
-        os.makedirs(os.path.dirname(config_file_path), exist_ok=True)
-        with open(config_file_path, "w") as file_object:
-            yaml.safe_dump(config, file_object)
+class Client(BaseClient):
+    """
+    Client to connect to the Whiffle AspForge API
+    """
 
     def _create_request(self, session, endpoint, data=None, params=None, stream=False):
-        res = session(self.url + endpoint, data=data, params=params, stream=stream)
+        res = session(
+            self.server_url + endpoint, data=data, params=params, stream=stream
+        )
         if res.status_code == 200:
             return res
         else:
             try:
                 raise ServerError(
                     "message={}, status_code={}".format(
                         res.json()["message"], res.status_code
                     )
                 )
             except json.JSONDecodeError:
-                raise Exception("{} cannot be reached".format(self.url))
+                raise Exception("{} cannot be reached".format(self.server_url))
 
     def new_task(self, input_params_io):
         data = self._get_params_from_io(input_params_io)
         request_url = "/api/aspforge/tasks"
         res = self._create_request(self.session.post, request_url, data=data).json()
         if "warnings" in res:
             for key, value in res["warnings"].items():
```

### Comparing `whiffle_client-0.3.2/whiffle_client/entrypoints.py` & `whiffle_client-0.4.0/whiffle_client/entrypoints.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/whiffle_client/io.py` & `whiffle_client-0.4.0/whiffle_client/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.4.0/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/whiffle_client/resources/example_yaml_include.yaml` & `whiffle_client-0.4.0/whiffle_client/resources/example_yaml_include.yaml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.2/whiffle_client/wind/loaders/csv.py` & `whiffle_client-0.4.0/whiffle_client/loaders/csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 class CSVLoader:
     # Init attributes
     path_to_csv: InitVar[str] = ""
 
     # Postinit attributes
     name: str = field(default=None)
     location: list[list[float]] = field(default=None)
-    turbine_model: str = field(default=None)
+    turbine_model_name: str = field(default=None)
+    include_in_les: bool = field(default=True)
+    thrust: bool = field(default=True)
 
     def __post_init__(self, path_to_csv: str = ""):
         self.data = pd.read_csv(path_to_csv).to_dict(orient="list")
         self.name = self.data["name"]
         self.location = list(zip(self.data["lon"], self.data["lat"]))
-        self.turbine_model = self.data["type"][0]
+        self.turbine_model_name = self.data["type"][0]
+        self.thrust = self.data["type"][0]
 
     def __repr__(self):
         return_data = {
             "name": self.name,
             "location": self.location,
         }
-        if self.turbine_model != "metmast":
-            return_data.update({"turbine_model": self.turbine_model})
+        if self.turbine_model_name != "metmast":
+            return_data.update({"turbine_model_name": self.turbine_model_name})
 
         return json.dumps(return_data)
 
     def __getitem__(self, item):
         return getattr(self, item)
```

### Comparing `whiffle_client-0.3.2/whiffle_client.egg-info/SOURCES.txt` & `whiffle_client-0.4.0/whiffle_client.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 LICENCE.txt
 README.md
 USER_README.md
 pyproject.toml
+tests/test_cli.py
 tests/test_client.py
 whiffle_client/__init__.py
+whiffle_client/base_client.py
 whiffle_client/client.py
+whiffle_client/decorators.py
 whiffle_client/entrypoints.py
 whiffle_client/io.py
 whiffle_client.egg-info/PKG-INFO
 whiffle_client.egg-info/SOURCES.txt
 whiffle_client.egg-info/dependency_links.txt
 whiffle_client.egg-info/entry_points.txt
 whiffle_client.egg-info/requires.txt
 whiffle_client.egg-info/top_level.txt
 whiffle_client/analysis/__init__.py
 whiffle_client/analysis/io.py
 whiffle_client/analysis/plot.py
 whiffle_client/analysis/scatter.py
 whiffle_client/analysis/skill.py
 whiffle_client/analysis/utils.py
+whiffle_client/loaders/__init__.py
+whiffle_client/loaders/csv.py
 whiffle_client/resources/example_generic_params.json
 whiffle_client/resources/example_yaml_include.yaml
 whiffle_client/resources/example_yaml_include_metmasts.yaml
 whiffle_client/resources/whiffle_config.yaml
+whiffle_client/snippets/create_mock_powercurve.py
 whiffle_client/wind/__init__.py
 whiffle_client/wind/client.py
-whiffle_client/wind/wind_simulation_task.py
 whiffle_client/wind/components/__init__.py
+whiffle_client/wind/components/dates.py
 whiffle_client/wind/components/domain.py
 whiffle_client/wind/components/geometries.py
 whiffle_client/wind/components/metmast.py
 whiffle_client/wind/components/turbine.py
-whiffle_client/wind/loaders/__init__.py
-whiffle_client/wind/loaders/csv.py
+whiffle_client/wind/components/turbine_model_specs.py
+whiffle_client/wind/components/wind_simulation_task.py
+whiffle_client/wind/components/windfarm.py
+whiffle_client/wind/mapping/__init__.py
+whiffle_client/wind/mapping/base.py
+whiffle_client/wind/mapping/turbine_model_specs.py
+whiffle_client/wind/mapping/wind_simulation_tasks.py
```

