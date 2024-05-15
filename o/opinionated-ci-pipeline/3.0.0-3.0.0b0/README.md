# Comparing `tmp/opinionated-ci-pipeline-3.0.0.tar.gz` & `tmp/opinionated-ci-pipeline-3.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opinionated-ci-pipeline-3.0.0.tar", last modified: Wed May 15 12:46:47 2024, max compression
+gzip compressed data, was "opinionated-ci-pipeline-3.0.0b0.tar", last modified: Tue Feb 27 14:25:48 2024, max compression
```

## Comparing `opinionated-ci-pipeline-3.0.0.tar` & `opinionated-ci-pipeline-3.0.0b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:46:47.681206 opinionated-ci-pipeline-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 12:46:36.000000 opinionated-ci-pipeline-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 12:46:36.000000 opinionated-ci-pipeline-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-05-15 12:46:47.681206 opinionated-ci-pipeline-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-05-15 12:46:36.000000 opinionated-ci-pipeline-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 12:46:36.000000 opinionated-ci-pipeline-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:46:47.681206 opinionated-ci-pipeline-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-15 12:46:36.000000 opinionated-ci-pipeline-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:46:47.681206 opinionated-ci-pipeline-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:46:47.681206 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)    90556 2024-05-15 12:46:36.000000 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:46:47.681206 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 12:46:36.000000 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   381648 2024-05-15 12:46:36.000000 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline/_jsii/opinionated-ci-pipeline@3.0.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:46:36.000000 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:46:47.681206 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-05-15 12:46:47.000000 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 12:46:47.000000 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:46:47.000000 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 12:46:47.000000 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 12:46:47.000000 opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:25:48.384372 opinionated-ci-pipeline-3.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-27 14:25:32.000000 opinionated-ci-pipeline-3.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-27 14:25:32.000000 opinionated-ci-pipeline-3.0.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-02-27 14:25:48.384372 opinionated-ci-pipeline-3.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-02-27 14:25:32.000000 opinionated-ci-pipeline-3.0.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-27 14:25:32.000000 opinionated-ci-pipeline-3.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 14:25:48.384372 opinionated-ci-pipeline-3.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-27 14:25:32.000000 opinionated-ci-pipeline-3.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:25:48.380372 opinionated-ci-pipeline-3.0.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:25:48.384372 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)    90556 2024-02-27 14:25:32.000000 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:25:48.384372 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-27 14:25:32.000000 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   381652 2024-02-27 14:25:32.000000 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline/_jsii/opinionated-ci-pipeline@3.0.0-beta.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 14:25:32.000000 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:25:48.384372 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-02-27 14:25:48.000000 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-27 14:25:48.000000 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 14:25:48.000000 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-27 14:25:48.000000 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-27 14:25:48.000000 opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline.egg-info/top_level.txt
```

### Comparing `opinionated-ci-pipeline-3.0.0/LICENSE` & `opinionated-ci-pipeline-3.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opinionated-ci-pipeline-3.0.0/PKG-INFO` & `opinionated-ci-pipeline-3.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opinionated-ci-pipeline
-Version: 3.0.0
+Version: 3.0.0b0
 Summary: CI/CD on AWS with feature-branch builds, developer-environment deployments, and build status notifications.
 Home-page: https://github.com/merapar/opinionated-ci-pipeline.git
 Author: Maciej Radzikowski<maciej.radzikowski@merapar.com>
 License: MIT
 Project-URL: Source, https://github.com/merapar/opinionated-ci-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `opinionated-ci-pipeline-3.0.0/README.md` & `opinionated-ci-pipeline-3.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `opinionated-ci-pipeline-3.0.0/setup.py` & `opinionated-ci-pipeline-3.0.0b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "opinionated-ci-pipeline",
-    "version": "3.0.0",
+    "version": "3.0.0.b0",
     "description": "CI/CD on AWS with feature-branch builds, developer-environment deployments, and build status notifications.",
     "license": "MIT",
     "url": "https://github.com/merapar/opinionated-ci-pipeline.git",
     "long_description_content_type": "text/markdown",
     "author": "Maciej Radzikowski<maciej.radzikowski@merapar.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "opinionated_ci_pipeline",
         "opinionated_ci_pipeline._jsii"
     ],
     "package_data": {
         "opinionated_ci_pipeline._jsii": [
-            "opinionated-ci-pipeline@3.0.0.jsii.tgz"
+            "opinionated-ci-pipeline@3.0.0-beta.0.jsii.tgz"
         ],
         "opinionated_ci_pipeline": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline/__init__.py` & `opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `opinionated-ci-pipeline-3.0.0/src/opinionated_ci_pipeline.egg-info/PKG-INFO` & `opinionated-ci-pipeline-3.0.0b0/src/opinionated_ci_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opinionated-ci-pipeline
-Version: 3.0.0
+Version: 3.0.0b0
 Summary: CI/CD on AWS with feature-branch builds, developer-environment deployments, and build status notifications.
 Home-page: https://github.com/merapar/opinionated-ci-pipeline.git
 Author: Maciej Radzikowski<maciej.radzikowski@merapar.com>
 License: MIT
 Project-URL: Source, https://github.com/merapar/opinionated-ci-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

