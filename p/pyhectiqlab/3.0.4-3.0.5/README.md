# Comparing `tmp/pyhectiqlab-3.0.4.tar.gz` & `tmp/pyhectiqlab-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhectiqlab-3.0.4.tar", last modified: Wed May  8 15:35:42 2024, max compression
+gzip compressed data, was "pyhectiqlab-3.0.5.tar", last modified: Wed May 15 14:37:12 2024, max compression
```

## Comparing `pyhectiqlab-3.0.4.tar` & `pyhectiqlab-3.0.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:42.874255 pyhectiqlab-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-08 15:35:42.874255 pyhectiqlab-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:42.870255 pyhectiqlab-3.0.4/pyhectiqlab/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:42.870255 pyhectiqlab-3.0.4/pyhectiqlab/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    15035 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:42.874255 pyhectiqlab-3.0.4/pyhectiqlab/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/functional/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13962 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:42.874255 pyhectiqlab-3.0.4/pyhectiqlab/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyhectiqlab/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:42.874255 pyhectiqlab-3.0.4/pyhectiqlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-08 15:35:42.000000 pyhectiqlab-3.0.4/pyhectiqlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-08 15:35:42.000000 pyhectiqlab-3.0.4/pyhectiqlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:35:42.000000 pyhectiqlab-3.0.4/pyhectiqlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 15:35:42.000000 pyhectiqlab-3.0.4/pyhectiqlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 15:35:42.000000 pyhectiqlab-3.0.4/pyhectiqlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 15:35:42.000000 pyhectiqlab-3.0.4/pyhectiqlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:35:42.874255 pyhectiqlab-3.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:42.874255 pyhectiqlab-3.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-08 15:35:27.000000 pyhectiqlab-3.0.4/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.286318 pyhectiqlab-3.0.5/pyhectiqlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.286318 pyhectiqlab-3.0.5/pyhectiqlab/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15594 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/pyhectiqlab/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14721 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24795 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/pyhectiqlab/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/tests/test_run.py
```

### Comparing `pyhectiqlab-3.0.4/PKG-INFO` & `pyhectiqlab-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.4
+Version: 3.0.5
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/__init__.py` & `pyhectiqlab-3.0.5/pyhectiqlab/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-__version__ = "3.0.4"
+__version__ = "3.0.5"
 
 from pyhectiqlab.settings import getenv
 
-API_URL = getenv("PYHECTIQLAB_API_URL", "https://api.lab.hectiq.ai")
+API_URL = getenv("HECTIQLAB_API_URL", "https://api.lab.hectiq.ai")
 
 from pyhectiqlab.config import Config
 from pyhectiqlab.dataset import Dataset
 from pyhectiqlab.model import Model
 from pyhectiqlab.run import Run
 from pyhectiqlab import functional
 
-
 def debug_mode():
     from pyhectiqlab.client import Client
-
     Client.online(False)
 
-
 __all__ = [
     "API_URL",
     "Artifact",
     "Dataset",
     "Model",
     "Run",
     "Config",
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/artifact.py` & `pyhectiqlab-3.0.5/pyhectiqlab/artifact.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class Artifact:
 
     @staticmethod
     @online_method
     @functional_alias("add_artifact")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def create(
         local_path: str,
         run_id: str,
         project: str,
         name: Optional[str] = None,
         step: Optional[int] = None,
         group: Optional[str] = None,
@@ -46,15 +46,15 @@
             return await Client.upload(local_path=local_path, policy=artifact.get("upload_policy"))
 
         return Client.execute(composition, wait_response=wait_response, is_async_method=True)
 
     @staticmethod
     @online_method
     @functional_alias("delete_artifact")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def delete(
         id: str,
         wait_response: bool = False,
     ):
         """
         Delete an artifact.
 
@@ -76,15 +76,15 @@
             id (str): ID of the artifact.
         """
         return Client.get(f"/app/artifacts/{id}", wait_response=True, params={"fields": fields})
 
     @staticmethod
     @online_method
     @functional_alias("download_artifact")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def download(
         id: str,
         savepath: str = "./",
         wait_response: bool = False,
     ):
         """
         Download an artifact from a run.
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/auth.py` & `pyhectiqlab-3.0.5/pyhectiqlab/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/block.py` & `pyhectiqlab-3.0.5/pyhectiqlab/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,20 @@
         if not block or not project:
             return
         return f"{block}::{project.replace('/', '::')}"
 
     @staticmethod
     @online_method
     @functional_alias("create_block")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def create(
-        title: str, status: Optional[str] = None, project: Optional[str] = None, wait_response: Optional[bool] = False
+        title: str, 
+        status: Optional[str] = None, 
+        project: Optional[str] = None,
+        wait_response: Optional[bool] = False
     ):
         """Create a block.
 
         Args:
             title (str): Block title.
             status (str, optional): Block status. Default: None.
             project (str, optional): Project name. If None, the current project is used. Default: None.
@@ -54,17 +57,20 @@
         body = {"title": title, "status": status, "project": project}
         block = Client.post("/app/blocks", json=body, wait_response=wait_response)
         return block
 
     @staticmethod
     @online_method
     @functional_alias("update_block")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def update(
-        block: str, title: Optional[str] = None, status: Optional[str] = None, wait_response: Optional[bool] = False
+        block: str, 
+        title: Optional[str] = None, 
+        status: Optional[str] = None, 
+        wait_response: Optional[bool] = False
     ):
         """Update a block.
 
         Args:
             block (str): Block ID.
             title (str, optional): Block title. Default: None.
             status (str, optional): Block status. Default: None.
@@ -101,10 +107,12 @@
             return None
         params = {
             "project": project,
             "search": search,
             "fields": fields,
             "page": page,
             "limit": limit,
+            "order_by": order_by,
+            "order_direction": order_direction,
         }
         blocks = Client.get("/app/blocks", params=params, wait_response=True)
         return blocks
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/cli/__init__.py` & `pyhectiqlab-3.0.5/pyhectiqlab/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/cli/auth.py` & `pyhectiqlab-3.0.5/pyhectiqlab/cli/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/client.py` & `pyhectiqlab-3.0.5/pyhectiqlab/client.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/dataset.py` & `pyhectiqlab-3.0.5/pyhectiqlab/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import clisync
 from typing import Optional, List, Union
 import asyncio
+import warnings
 
 from pyhectiqlab.tag import Tag
 from pyhectiqlab.project import Project
 from pyhectiqlab.block import Block
 from pyhectiqlab.block import Block
 from pyhectiqlab.client import Client
 from pyhectiqlab.decorators import functional_alias, online_method
@@ -24,118 +25,122 @@
         source: str,
         host: Optional[str] = None,
         description: Optional[str] = None,
         version: Optional[str] = None,
         block: Optional[str] = None,
         run_id: Optional[str] = None,
         project: Optional[str] = None,
-        upload: Optional[bool] = False,
+        upload: Optional[bool] = False
     ):
         """Create a dataset.
 
         Supported cloud storages:
         - Amazon S3
         - Google Cloud Storage
 
         Args:
             name (str): Name of the dataset.
-            source (str): Path to the dataset. If your dataset is located in a local directory, the path should be the directory path (e.g., "/path/to/dataset"). If
-                the dataset is located in a cloud storage, the path should be the URL of the dataset (e.g., "s3://bucket/dataset").
-            host (str, optional): Source of the dataset. Default: None. If the dataset is located in a local directory,
-                the resource could be your hostname or leave it empty. If the dataset is located in a cloud storage, the resource should be the cloud storage name ("s3" or "gs")
-            version (str]): Version of the dataset. Default: None.
+            source (str): Path to the dataset. If your dataset is located in a local directory, the source should be the directory path (e.g., "/path/to/dataset"). If
+                the dataset is located in a cloud storage, the source should be the URL of the dataset (e.g., "s3://bucket/dataset").
+            host (str, optional): Host of the dataset. Default: None. If the dataset is located in a local directory,
+                the host could be your hostname or leave it empty. If the dataset is located in a cloud storage, the host should be the cloud storage name ("s3" or "gs")
             description (str, optional): Description of the dataset. Default: None.
+            version (str]): Version of the dataset. Default: None.
             block (str, optional): Block of the dataset. Default: None.
-            project (str, optional): Project of the dataset. Default: None.
             run_id (str, optional): Run of the dataset. Default: None.
+            project (str, optional): Project of the dataset. Default: None.
             upload (bool): If True, upload the dataset to the Lab. Default: False.
         """
         from pyhectiqlab.run import Run
-
         project = Project.get(project)
         run_id = Run.get_id(run_id)
         block = Block.get(block)
         if project is None:
+            warnings.warn("Project not found, skipping dataset creation.")
             return
 
         if name is None:
             raise ValueError("The `name` parameter is required.")
 
         if source is None:
-            raise ValueError("The `path` parameter is required.")
+            raise ValueError("The `source` parameter is required.")
         source = os.path.abspath(source)
         host = extract_host_from_source(source)
 
         if block:
-            if not "::" in block:
+            if "::" not in block:
                 block = Block.format_id(block, project)
 
         data = {
             "name": name,
             "description": description,
             "version": version,
             "host": host,
             "source": source,
             "block": block,
             "project": project,
             "root_run": run_id,
         }
         dataset = Dataset._client.post("/app/datasets", wait_response=True, json=data)
         if upload and host not in ["s3", "gs"]:
-            Dataset.upload(id=dataset["id"], path=source)
+            Dataset.upload(id=dataset["id"], source=source)
 
-        if run_id is not None:
-            Dataset.attach(name=name, version=version, run_id=run_id, project=project)
+        Dataset.attach(name=name, version=version, run_id=run_id, project=project)
         return dataset
 
     @staticmethod
     @online_method
     @functional_alias("upload_dataset")
     @clisync.include()
-    def upload(id: str, path: str):
-        """Upload local files to a dataset hosted in the Lab."""
-        all_files = list_all_files_in_dir(path)
+    def upload(id: str, 
+               source: str):
+        """Upload local files to a dataset hosted in the Lab.
+        
+        Args:
+            id (str): ID of the dataset.
+            path (str): Path to the directory containing the files to upload.
+        """
+        all_files = list_all_files_in_dir(source)
         batch_size = 50
         Dataset._id = dataset_id = id
         for batch in batched(all_files, batch_size):
             # Create many files
-            batch_body = [{"name": os.path.relpath(f, start=path), "num_bytes": os.path.getsize(f)} for f in batch]
+            batch_body = [{"name": os.path.relpath(f, start=source), "num_bytes": os.path.getsize(f)} for f in batch]
             files = Dataset._client.post(
                 f"/app/datasets/{dataset_id}/files", wait_response=True, json={"files": batch_body}
             )["results"]
 
             # For each file in batch, get the policy in files (use name for finding the file)
             sorted_files = []
             for el in batch:
-                file = [f.get("upload_policy") for f in files if f["name"] == os.path.relpath(el, start=path)][0]
+                file = [f.get("upload_policy") for f in files if f["name"] == os.path.relpath(el, start=source)][0]
                 sorted_files.append(file)
             # Upload dataset files
             asyncio.run(Dataset._client.upload_many(paths=batch, policies=sorted_files))
 
     @staticmethod
     @online_method
     @functional_alias("retrieve_dataset")
-    @clisync.include(wait_response=True)
+    @clisync.include()
     def retrieve(
         name: str,
         version: str,
         project: str,
-        fields: Optional[List[str]] = None,
-        wait_response: bool = True,  # This must be True, else no retrieve is possible.
+        fields: Optional[List[str]] = None
     ):
         """Retrieve a dataset
 
         Args:
             name (str): Name of the dataset
             project (str): Project of the dataset
             version (str): Version of the dataset
             fields (list[str], optional): Fields to retrieve. Default: None.
         """
         body = Dataset._client.get(
-            f"/app/datasets/retrieve",
+            "/app/datasets/retrieve",
             params={
                 "name": name,
                 "project": project,
                 "version": version,
                 "fields": fields or [],
             },
             wait_response=True,
@@ -153,16 +158,15 @@
         block: Optional[str] = None,
         blocks: Optional[List[str]] = None,
         keep_latest_version: bool = False,
         fields: Optional[List[str]] = [],
         page: Optional[int] = 1,
         limit: Optional[int] = 100,
         order_by: Optional[str] = "created_at",
-        order_direction: Optional[str] = "desc",
-        wait_response: bool = False,
+        order_direction: Optional[str] = "desc"
     ):
         """List the datasets
 
         Args:
             project (str, optional): Project of the dataset.
             block (str, optional): Block of the dataset.
             search (str, optional): Search string.
@@ -174,15 +178,15 @@
             limit (int, optional): Limit of the datasets.
             order_by (str, optional): Order by.
             order_direction (str, optional): Order direction.
             wait_response (bool): Wait for the response from the server. Default: False.
         """
         block = Block.get(block)
         if block is not None:
-            if not "::" in block:
+            if "::" not in block:
                 block = Block.format_id(block, project)
 
         params = {
             "project": project,
             "block": block,
             "search": search,
             "author": author,
@@ -191,20 +195,20 @@
             "fields": fields,
             "page": page,
             "limit": limit,
             "order_by": order_by,
             "order_direction": order_direction,
         }
 
-        return Dataset._client.get("/app/datasets", params=params, wait_response=wait_response)
+        return Dataset._client.get("/app/datasets", params=params, wait_response=True)
 
     @staticmethod
     @online_method
     @functional_alias("update_dataset")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def update(
         id: str,
         name: Optional[str] = None,
         description: Optional[str] = None,
         version: Optional[str] = None,
         block: Optional[str] = None,
         wait_response: bool = False,
@@ -226,15 +230,15 @@
             json={"name": name, "description": description, "version": version, "block": block},
             wait_response=wait_response,
         )
 
     @staticmethod
     @online_method
     @functional_alias("delete_dataset")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def delete(
         id: Optional[str] = None,
         name: Optional[str] = None,
         version: Optional[str] = None,
         project: Optional[str] = None,
         wait_response: bool = False,
     ):
@@ -254,15 +258,15 @@
                 return
             id = dataset["id"]
         return Dataset._client.delete(f"/app/datasets/{id}", wait_response=wait_response)
 
     @staticmethod
     @online_method
     @functional_alias("download_dataset")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def download(
         name: str,
         version: str,
         project: Optional[str] = None,
         path: Optional[str] = "./",
         wait_response: bool = False,
     ):
@@ -274,16 +278,15 @@
             project (str, optional): Project of the dataset.
             path (str): Path to download the dataset. Default: "./".
             wait_response (bool): Wait for the response from the server. Default: False.
         """
         path = path or "./"
         path = os.path.join(path, f"{name}-{version.replace('.', '-')}")
         os.makedirs(path, exist_ok=True)
-        Dataset.attach(name=name, version=version, project=project)
-
+        Dataset.attach(name=name, version=version, project=project, wait_response=True)
         async def composition():
             dataset = Dataset.retrieve(name=name, project=project, version=version, fields=["id"])
             if not dataset:
                 return
             dataset_id = dataset["id"]
 
             num_results = 0
@@ -310,29 +313,33 @@
         return Dataset._client.execute(composition, wait_response=wait_response, is_async_method=True)
 
     @staticmethod
     @online_method
     def attach(
         name: str,
         version: str,
-        run_id: str,
+        run_id: Optional[str] = None,
         project: Optional[str] = None,
         wait_response: bool = False,
     ):
         """Attach a dataset to a run
 
         Args:
             name (str): Name of the dataset.
             version (str): Version of the dataset.
             run_id (str): ID of the run.
             project (str, optional): Project of the dataset.
             wait_response (bool): Wait for the response from the server. Default: False.
         """
+        from pyhectiqlab.run import Run
+        run_id = Run.get_id(run_id)
+        if run_id is None:
+            return
         dataset = Dataset.retrieve(name=name, project=project, version=version, fields=["id"])
-        if dataset is None or run_id is None:
+        if dataset is None:
             return
         return Dataset._client.post(
             f"/app/datasets/{dataset['id']}/attach-to-run/{run_id}", wait_response=wait_response
         )
 
     @staticmethod
     @online_method
@@ -348,14 +355,16 @@
         Args:
             name (str): Name of the dataset.
             version (str): Version of the dataset.
             run_id (str): ID of the run.
             project (str, optional): Project of the dataset.
             wait_response (bool, optional): Wait for the response from the server. Default: False.
         """
+        if not run_id:
+            return
         dataset = Dataset.retrieve(name=name, project=project, version=version, fields=["id"])
         if not dataset:
             return
         dataset_id = dataset["id"]
         return Dataset._client.post(
             f"/app/datasets/{dataset_id}/detach-from-run/{run_id}", wait_response=wait_response
         )
@@ -363,37 +372,40 @@
     @staticmethod
     @online_method
     def add_tags(
         tags: Union[str, List[str]],
         name: str,
         version: str,
         project: Optional[str] = None,
+        wait_response: Optional[bool] = False,
     ):
         """Add tags to a dataset
 
         Args:
             tags (Union[str, List[str]]): Tags to add.
             name (str): Name of the dataset.
             version (str): Version of the dataset.
             project (str, optional): Project name. Default: None.
+            wait_response (bool, optional): Wait for the response from the server. Default: False.
         """
         project = Project.get(project)
         dataset = Dataset.retrieve(name=name, project=project, version=version, fields=["id"])
         if not dataset:
             return
         dataset_id = dataset["id"]
-        return Tag.attach_to_dataset(tags=tags, dataset_id=dataset_id, project=project)
+        return Tag.attach_to_dataset(tags=tags, dataset_id=dataset_id, project=project, wait_response=wait_response)
 
     @staticmethod
     @online_method
     def detach_tag(
         tag: str,
         name: str,
         version: str,
         project: Optional[str] = None,
+        wait_response: Optional[bool] = False,
     ):
         """Remove a tag from the run.
         For functional alias, use `detach_tag_from_run`.
 
         Args:
             title (str): The new title of the run.
             name (str): Name of the dataset.
@@ -401,8 +413,8 @@
             project (str, optional): Project name. Default: None.
         """
         project = Project.get(project)
         dataset = Dataset.retrieve(name=name, version=version, project=project, fields=["id"])
         if not dataset:
             return
         dataset_id = dataset["id"]
-        Tag.detach_from_dataset(tag=tag, dataset_id=dataset_id, project=project)
+        Tag.detach_from_dataset(tag=tag, dataset_id=dataset_id, project=project, wait_response=wait_response)
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/decorators.py` & `pyhectiqlab-3.0.5/pyhectiqlab/decorators.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/logging.py` & `pyhectiqlab-3.0.5/pyhectiqlab/logging.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/metrics.py` & `pyhectiqlab-3.0.5/pyhectiqlab/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/model.py` & `pyhectiqlab-3.0.5/pyhectiqlab/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,75 +18,99 @@
 
     @staticmethod
     @online_method
     @functional_alias("create_model")
     @clisync.include()
     def create(
         name: str,
+        path: Optional[str] = None,
+        version: Optional[str] = None,
         run_id: Optional[str] = None,
         project: Optional[str] = None,
         block: Optional[str] = None,
-        path: Optional[str] = None,
         description: Optional[str] = None,
-        version: Optional[str] = None,
-        wait_response: bool = False,
+        upload: Optional[bool] = True
     ):
         """Create a model
 
         Args:
             name (str): Name of the model
             run_id (str, optional):  ID of the run
             project (str, optional): Project of the model
             path (str, optional): Path to the model directory
             description (str, optional): Description of the model
             version (str, optional): Version of the model
             block (str, optional): Block of the model
-            wait_response (bool, optional): Wait for the response from the server
+            upload (bool, optional): Upload the model files. Default: True
         """
+        from pyhectiqlab.run import Run
         project = Project.get(project)
+        run_id = Run.get_id(run_id)
+        block = Block.get(block)
+
         if project is None:
             warnings.warn("Project not found, skipping model creation.")
             return
+        
+        if name is None:
+            raise ValueError("The `name` parameter is required.")
+        
         if block:
-            if not "::" in block:
+            if "::" not in block:
                 block = Block.format_id(block, project)
 
-        def composition():
-            json = {
-                "name": name,
-                "description": description,
-                "version": version,
-                "block": block,
-                "project": project,
-                "root_run": run_id,
-            }
+        json = {
+            "name": name,
+            "description": description,
+            "version": version,
+            "block": block,
+            "project": project,
+            "root_run": run_id,
+        }
 
-            model = Model._client.post("/app/models", wait_response=True, json=json)
-            if not model or "id" not in model:
-                return
+        model = Model._client.post("/app/models", wait_response=True, json=json)
+        if not model or "id" not in model:
+            return
+        
+        if upload and path:
+            Model.upload(id=model["id"], path=path)
 
-            all_files = list_all_files_in_dir(path)
-            batch_size = 50
-            model_id = model["id"]
-            for batch in batched(all_files, batch_size):
-                # Create many files
-                batch_body = [{"name": os.path.relpath(f, start=path), "num_bytes": os.path.getsize(f)} for f in batch]
-                files = Model._client.post(
-                    f"/app/models/{model_id}/files", wait_response=True, json={"files": batch_body}
-                )["results"]
-
-                # For each file in batch, get the policy in files (use name for finding the file)
-                sorted_files = []
-                for el in batch:
-                    file = [f.get("upload_policy") for f in files if f["name"] == os.path.relpath(el, start=path)][0]
-                    sorted_files.append(file)
-                # Upload model files
-                asyncio.run(Model._client.upload_many(paths=batch, policies=sorted_files))
+        Model.attach(name=name, version=version, run_id=run_id, project=project, wait_response=True)
+        return model
 
-        Model._client.execute(composition, wait_response=wait_response)
+    @staticmethod
+    @online_method
+    @functional_alias("upload_model")
+    @clisync.include()
+    def upload(id: str, 
+               path: str):
+        """Upload local files to a model hosted in the Lab.
+
+        Args:
+            id (str): ID of the model.
+            path (str): Path to the model directory.
+        """
+        all_files = list_all_files_in_dir(path)
+        batch_size = 50
+        Model._id = model_id = id
+        for batch in batched(all_files, batch_size):
+            # Create many files
+            batch_body = [{"name": os.path.relpath(f, start=path), "num_bytes": os.path.getsize(f)} for f in batch]
+            files = Model._client.post(
+                f"/app/models/{model_id}/files", wait_response=True, json={"files": batch_body}
+            )["results"]
+
+            # For each file in batch, get the policy in files (use name for finding the file)
+            sorted_files = []
+            for el in batch:
+                file = [f.get("upload_policy") for f in files if f["name"] == os.path.relpath(el, start=path)][0]
+                sorted_files.append(file)
+
+            # Upload model files
+            asyncio.run(Model._client.upload_many(paths=batch, policies=sorted_files))
 
     @staticmethod
     @online_method
     @functional_alias("retrieve_model")
     @clisync.include()
     def retrieve(
         name: str,
@@ -104,28 +128,28 @@
             wait_response (bool, optional): Wait for the response from the server
         """
         project = Project.get(project)
         if project is None:
             return
 
         return Model._client.get(
-            f"/app/models/retrieve",
+            "/app/models/retrieve",
             params={
                 "name": name,
                 "project": project,
                 "version": version,
                 "fields": fields,
             },
             wait_response=True,
         )
 
     @staticmethod
     @online_method
     @functional_alias("list_models")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def list(
         project: Optional[str] = None,
         search: Optional[str] = None,
         author: Optional[str] = None,
         block: Optional[str] = None,
         blocks: Optional[List[str]] = None,
         keep_latest_version: bool = False,
@@ -150,15 +174,15 @@
             limit (int, optional): Limit of the models
             order_by (str, optional): Order by
             order_direction (str, optional): Order direction
             wait_response (bool, optional): Wait for the response from the server
         """
 
         if block is not None:
-            if not "::" in block:
+            if "::" not in block:
                 from pyhectiqlab.block import Block
 
                 block = Block.format_id(block, project)
 
         params = {
             "project": Project.get(project),
             "block": block,
@@ -174,15 +198,15 @@
         }
 
         return Model._client.get("/app/models", params=params, wait_response=wait_response)
 
     @staticmethod
     @online_method
     @functional_alias("update_model")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def update(
         id: str,
         name: Optional[str] = None,
         description: Optional[str] = None,
         version: Optional[str] = None,
         block: Optional[str] = None,
         wait_response: bool = False,
@@ -204,15 +228,15 @@
             json={"name": name, "description": description, "version": version, "block": block},
             wait_response=wait_response,
         )
 
     @staticmethod
     @online_method
     @functional_alias("delete_model")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def delete(
         id: Optional[str] = None,
         name: Optional[str] = None,
         version: Optional[str] = None,
         project: Optional[str] = None,
         wait_response: bool = False,
     ):
@@ -233,15 +257,15 @@
                 return
             id = model["id"]
         return Model._client.delete(f"/app/models/{id}", wait_response=wait_response)
 
     @staticmethod
     @online_method
     @functional_alias("download_model")
-    @clisync.include()
+    @clisync.include(wait_response=True)
     def download(
         name: str,
         version: str,
         project: Optional[str] = None,
         path: Optional[str] = "./",
         wait_response: bool = False,
     ):
@@ -294,27 +318,31 @@
         return Model._client.execute(composition, wait_response=wait_response, is_async_method=True)
 
     @staticmethod
     @online_method
     def attach(
         name: str,
         version: str,
-        run_id: str,
+        run_id: Optional[str] = None,
         project: Optional[str] = None,
-        wait_response: bool = False,
+        wait_response: bool = True,
     ):
         """Attach a model to a run
 
         Args:
             run_id (str): ID of the run.
             name (str): Name of the model.
             version (str): Version of the model.
             project (str, optional): Project of the model. If None, the project of the current run is used. Default: None.
             wait_response (bool, optional): Wait for the response from the server. Default: False.
         """
+        from pyhectiqlab.run import Run
+        run_id = Run.get_id(run_id)
+        if run_id is None:
+            return
         project = Project.get(project)
         model = Model.retrieve(name=name, project=project, version=version, fields=["id"])
         if not model:
             return
         model_id = model["id"]
         return Model._client.post(f"/app/models/{model_id}/attach-to-run/{run_id}", wait_response=wait_response)
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/project.py` & `pyhectiqlab-3.0.5/pyhectiqlab/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     def slug(cls) -> str:
         return cls._slug
 
     @classproperty
     def repo(cls) -> str:
         if not cls._slug:
             return None
+        if not os.path.exists(cls._configs):
+            return None
         with open(cls._configs, "r") as file:
             config = toml.load(file)
             return config.get(cls._slug, {}).get("repo")
 
     @classmethod
     def allow_dirty(cls) -> bool:
         if not Client.online():
@@ -79,15 +81,15 @@
             "slug": slug,
             "name": name,
             "repo": repo,
             "force_no_git_diff": force_no_git_diff,
         }
         project = Project._client.post("/app/projects", json=body, wait_response=True)
         if project is None:
-            warnings.warn(f"Failed to create project.")
+            warnings.warn("Failed to create project.")
             return
         if write_config:
             Project.write_config(slug)
         logger.info(f"Project `{slug}` created.")
         return slug
 
     @staticmethod
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/run.py` & `pyhectiqlab-3.0.5/pyhectiqlab/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import tempfile
 import slugify
 import logging
 import warnings
 import clisync
 
 from typing import Any, List, Optional, Union, Literal, Tuple
-from matplotlib.pyplot import Figure
 
 from pyhectiqlab import API_URL
 from pyhectiqlab import Config
 from pyhectiqlab.project import Project
 from pyhectiqlab.artifact import Artifact
 from pyhectiqlab.block import Block
 from pyhectiqlab.tag import Tag
@@ -382,15 +381,15 @@
             wait_response=wait_response,
         )
 
     @staticmethod
     @online_method
     @functional_alias(alias="add_figure")
     def add_figure(
-        figure: Figure,
+        figure,
         name: str,
         step: Optional[int] = None,
         dpi: int = 200,
         extension: str = "png",
         wait_response: bool = False,
         run_id: Optional[str] = None,
         project: Optional[str] = None,
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/settings/__init__.py` & `pyhectiqlab-3.0.5/pyhectiqlab/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/step.py` & `pyhectiqlab-3.0.5/pyhectiqlab/step.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/tag.py` & `pyhectiqlab-3.0.5/pyhectiqlab/tag.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/utils.py` & `pyhectiqlab-3.0.5/pyhectiqlab/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,34 @@
     for i in range(0, len(iterable), n):
         i1 = min(i + n, len(iterable))
         yield iterable[i:i1]
 
 
 def list_all_files_in_dir(local_folder: str) -> List[str]:
     """List all files in a directory.
+    If the path is a file, the file is returned.
 
     Args:
         local_folder (str): The folder to list files from.
     """
     if not os.path.exists(local_folder):
         raise FileNotFoundError(f"Directory {local_folder} does not exist.")
     filenames = []
-    if os.path.isdir(local_folder) == False:
-        return filenames
+    if not os.path.isdir(local_folder):
+        # If the path is a file, return the file
+        return [local_folder]
 
     for el in os.walk(local_folder):
         for f in os.listdir(el[0]):
             complete_path = os.path.join(el[0], f)
-            if os.path.isdir(complete_path) == False:
+            if not os.path.isdir(complete_path):
                 if os.path.isfile(complete_path):
                     filenames.append(complete_path)
     return filenames
 
-
 def extract_host_from_source(source: str) -> str:
     """Extract the resource from a path.
 
     If the path is a cloud path (e.g., s3://bucket/dataset), the resource is inferred from the path.
     If the path is a local path, the resource is set to "local" if not provided.
 
     Args:
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab/versions.py` & `pyhectiqlab-3.0.5/pyhectiqlab/versions.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab.egg-info/PKG-INFO` & `pyhectiqlab-3.0.5/pyhectiqlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.4
+Version: 3.0.5
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.4/pyhectiqlab.egg-info/SOURCES.txt` & `pyhectiqlab-3.0.5/pyhectiqlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.4/pyproject.toml` & `pyhectiqlab-3.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 maintainers = [
   {name = "Edward Laurence", email = "edwardl@hectiq.ai"},
   {name = "Charles Murphy", email = "cmurphy@hectiq.ai"},
 ]
 name = "pyhectiqlab"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "3.0.4"
+version = "3.0.5"
 
 [project.urls]
 Repository = "https://github.com/HectiqAI/hectiq-lab-revision.git"
 
 [project.entry-points.console_scripts]
 hectiq-lab = "pyhectiqlab.cli:main"
```

### Comparing `pyhectiqlab-3.0.4/tests/test_project.py` & `pyhectiqlab-3.0.5/tests/test_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
-from util import mock_client
+from utils import random_uuid
+from mock_client import mock_client
 
 
 @pytest.fixture
 def slug():
     return "hectiq-ai/test2"
```

### Comparing `pyhectiqlab-3.0.4/tests/test_run.py` & `pyhectiqlab-3.0.5/tests/test_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from pyhectiqlab import Run
-from util import mock_client
+from mock_client import mock_client
 
 
 @pytest.fixture
 def config():
     return {"param": "test", "x": 1}
```

