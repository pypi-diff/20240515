# Comparing `tmp/qfieldcloud-sdk-0.8.2.tar.gz` & `tmp/qfieldcloud_sdk-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfieldcloud-sdk-0.8.2.tar", last modified: Wed Oct 25 02:01:41 2023, max compression
+gzip compressed data, was "qfieldcloud_sdk-0.8.3.tar", last modified: Wed May 15 13:26:47 2024, max compression
```

## Comparing `qfieldcloud-sdk-0.8.2.tar` & `qfieldcloud_sdk-0.8.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 02:01:41.635419 qfieldcloud-sdk-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/.env.example
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 02:01:41.631419 qfieldcloud-sdk-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 02:01:41.631419 qfieldcloud-sdk-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/.github/workflows/continuous_integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2023-10-25 02:01:41.635419 qfieldcloud-sdk-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 02:01:41.631419 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15193 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    25805 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 02:01:41.635419 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2023-10-25 02:01:41.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-10-25 02:01:41.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 02:01:41.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-25 02:01:41.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-10-25 02:01:41.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-25 02:01:41.000000 qfieldcloud-sdk-0.8.2/qfieldcloud_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 02:01:41.635419 qfieldcloud-sdk-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 02:01:41.635419 qfieldcloud-sdk-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-10-25 02:01:28.000000 qfieldcloud-sdk-0.8.2/tests/test_cli_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:47.722681 qfieldcloud_sdk-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/.env.example
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:47.718681 qfieldcloud_sdk-0.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:47.722681 qfieldcloud_sdk-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/.github/workflows/continuous_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-15 13:26:47.722681 qfieldcloud_sdk-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:47.722681 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15193 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25805 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:47.722681 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-15 13:26:47.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 13:26:47.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:26:47.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 13:26:47.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 13:26:47.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 13:26:47.000000 qfieldcloud_sdk-0.8.3/qfieldcloud_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:26:47.722681 qfieldcloud_sdk-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:47.722681 qfieldcloud_sdk-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-15 13:26:39.000000 qfieldcloud_sdk-0.8.3/tests/test_cli_client.py
```

### Comparing `qfieldcloud-sdk-0.8.2/.github/workflows/continuous_integration.yml` & `qfieldcloud_sdk-0.8.3/.github/workflows/continuous_integration.yml`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/.github/workflows/deploy_to_pypi.yml` & `qfieldcloud_sdk-0.8.3/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/.pre-commit-config.yaml` & `qfieldcloud_sdk-0.8.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/LICENCE` & `qfieldcloud_sdk-0.8.3/LICENCE`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/PKG-INFO` & `qfieldcloud_sdk-0.8.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfieldcloud-sdk
-Version: 0.8.2
+Version: 0.8.3
 Summary: The official QFieldCloud SDK and CLI.
 Author-email: Ivan Ivanov <ivan@opengis.ch>
 Project-URL: homepage, https://github.com/opengisch/qfieldcloud-sdk-python
 Project-URL: documentation, https://github.com/opengisch/qfieldcloud-sdk-python
 Project-URL: repository, https://github.com/opengisch/qfieldcloud-sdk-python
 Project-URL: tracker, https://github.com/opengisch/qfieldcloud-sdk-python/issues
 Keywords: QFieldCloud,QField,QGIS,CI,SDK
@@ -19,21 +19,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: certifi==2023.7.22; python_version >= "3.6"
-Requires-Dist: charset-normalizer==3.2.0; python_full_version >= "3.7.0"
-Requires-Dist: click==8.1.5
-Requires-Dist: idna==3.4; python_version >= "3.5"
-Requires-Dist: requests==2.31.0
-Requires-Dist: tqdm==4.65.0
-Requires-Dist: urllib3==2.0.7
+Requires-Dist: certifi>=2023.7.22
+Requires-Dist: charset-normalizer>=3.2.0
+Requires-Dist: click>=8.1.5
+Requires-Dist: idna>=3.4
+Requires-Dist: requests>=2.31.0
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: urllib3>=2.0.7
 
 # The official QFieldCloud SDK and CLI
 
 `qfieldcloud-sdk` is the official client to connect to QFieldCloud API either as a python module, or directly from the command line.
 
 ## Contents
```

### Comparing `qfieldcloud-sdk-0.8.2/README.md` & `qfieldcloud_sdk-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/pyproject.toml` & `qfieldcloud_sdk-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/cli.py` & `qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/interfaces.py` & `qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/sdk.py` & `qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/qfieldcloud_sdk/utils.py` & `qfieldcloud_sdk-0.8.3/qfieldcloud_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/qfieldcloud_sdk.egg-info/PKG-INFO` & `qfieldcloud_sdk-0.8.3/qfieldcloud_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfieldcloud-sdk
-Version: 0.8.2
+Version: 0.8.3
 Summary: The official QFieldCloud SDK and CLI.
 Author-email: Ivan Ivanov <ivan@opengis.ch>
 Project-URL: homepage, https://github.com/opengisch/qfieldcloud-sdk-python
 Project-URL: documentation, https://github.com/opengisch/qfieldcloud-sdk-python
 Project-URL: repository, https://github.com/opengisch/qfieldcloud-sdk-python
 Project-URL: tracker, https://github.com/opengisch/qfieldcloud-sdk-python/issues
 Keywords: QFieldCloud,QField,QGIS,CI,SDK
@@ -19,21 +19,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: certifi==2023.7.22; python_version >= "3.6"
-Requires-Dist: charset-normalizer==3.2.0; python_full_version >= "3.7.0"
-Requires-Dist: click==8.1.5
-Requires-Dist: idna==3.4; python_version >= "3.5"
-Requires-Dist: requests==2.31.0
-Requires-Dist: tqdm==4.65.0
-Requires-Dist: urllib3==2.0.7
+Requires-Dist: certifi>=2023.7.22
+Requires-Dist: charset-normalizer>=3.2.0
+Requires-Dist: click>=8.1.5
+Requires-Dist: idna>=3.4
+Requires-Dist: requests>=2.31.0
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: urllib3>=2.0.7
 
 # The official QFieldCloud SDK and CLI
 
 `qfieldcloud-sdk` is the official client to connect to QFieldCloud API either as a python module, or directly from the command line.
 
 ## Contents
```

### Comparing `qfieldcloud-sdk-0.8.2/qfieldcloud_sdk.egg-info/SOURCES.txt` & `qfieldcloud_sdk-0.8.3/qfieldcloud_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qfieldcloud-sdk-0.8.2/tests/test_cli_client.py` & `qfieldcloud_sdk-0.8.3/tests/test_cli_client.py`

 * *Files identical despite different names*

