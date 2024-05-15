# Comparing `tmp/adafruit_circuitpython_ntp-3.1.0.tar.gz` & `tmp/adafruit_circuitpython_ntp-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_ntp-3.1.0.tar", last modified: Mon May 13 13:20:07 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_ntp-3.1.1.tar", last modified: Wed May 15 18:29:35 2024, max compression
```

## Comparing `adafruit_circuitpython_ntp-3.1.0.tar` & `adafruit_circuitpython_ntp-3.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.436174 adafruit_circuitpython_ntp-3.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.440174 adafruit_circuitpython_ntp-3.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.440174 adafruit_circuitpython_ntp-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.440174 adafruit_circuitpython_ntp-3.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_ntp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.440174 adafruit_circuitpython_ntp-3.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/examples/ntp_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/examples/ntp_cpython.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/examples/ntp_set_rtc.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/examples/ntp_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.354581 adafruit_circuitpython_ntp-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.346581 adafruit_circuitpython_ntp-3.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.350581 adafruit_circuitpython_ntp-3.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.350581 adafruit_circuitpython_ntp-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.350581 adafruit_circuitpython_ntp-3.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-15 18:29:35.354581 adafruit_circuitpython_ntp-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.354581 adafruit_circuitpython_ntp-3.1.1/adafruit_circuitpython_ntp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-15 18:29:35.000000 adafruit_circuitpython_ntp-3.1.1/adafruit_circuitpython_ntp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-15 18:29:35.000000 adafruit_circuitpython_ntp-3.1.1/adafruit_circuitpython_ntp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:29:35.000000 adafruit_circuitpython_ntp-3.1.1/adafruit_circuitpython_ntp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 18:29:35.000000 adafruit_circuitpython_ntp-3.1.1/adafruit_circuitpython_ntp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 18:29:35.000000 adafruit_circuitpython_ntp-3.1.1/adafruit_circuitpython_ntp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-15 18:29:30.000000 adafruit_circuitpython_ntp-3.1.1/adafruit_ntp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.354581 adafruit_circuitpython_ntp-3.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.354581 adafruit_circuitpython_ntp-3.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:29:35.354581 adafruit_circuitpython_ntp-3.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-15 18:29:30.000000 adafruit_circuitpython_ntp-3.1.1/examples/ntp_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-15 18:29:30.000000 adafruit_circuitpython_ntp-3.1.1/examples/ntp_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-15 18:29:30.000000 adafruit_circuitpython_ntp-3.1.1/examples/ntp_set_rtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-15 18:29:30.000000 adafruit_circuitpython_ntp-3.1.1/examples/ntp_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 18:29:30.000000 adafruit_circuitpython_ntp-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 18:29:07.000000 adafruit_circuitpython_ntp-3.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:29:35.354581 adafruit_circuitpython_ntp-3.1.1/setup.cfg
```

### Comparing `adafruit_circuitpython_ntp-3.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_ntp-3.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/.gitignore` & `adafruit_circuitpython_ntp-3.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/.pre-commit-config.yaml` & `adafruit_circuitpython_ntp-3.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/.pylintrc` & `adafruit_circuitpython_ntp-3.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_ntp-3.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/LICENSE` & `adafruit_circuitpython_ntp-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_ntp-3.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/LICENSES/MIT.txt` & `adafruit_circuitpython_ntp-3.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_ntp-3.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/PKG-INFO` & `adafruit_circuitpython_ntp-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ntp
-Version: 3.1.0
+Version: 3.1.1
 Summary: Network Time Protocol (NTP) helper for Python
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NTP
 Keywords: adafruit,blinka,circuitpython,micropython,ntp,ntp,,network,,time
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_ntp-3.1.0/README.rst` & `adafruit_circuitpython_ntp-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/PKG-INFO` & `adafruit_circuitpython_ntp-3.1.1/adafruit_circuitpython_ntp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ntp
-Version: 3.1.0
+Version: 3.1.1
 Summary: Network Time Protocol (NTP) helper for Python
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NTP
 Keywords: adafruit,blinka,circuitpython,micropython,ntp,ntp,,network,,time
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/SOURCES.txt` & `adafruit_circuitpython_ntp-3.1.1/adafruit_circuitpython_ntp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/adafruit_ntp.py` & `adafruit_circuitpython_ntp-3.1.1/adafruit_ntp.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """
 import struct
 import time
 
 from micropython import const
 
 
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NTP.git"
 
 NTP_TO_UNIX_EPOCH = 2208988800  # 1970-01-01 00:00:00
 PACKET_SIZE = const(48)
 
 
 class NTP:
@@ -81,19 +81,16 @@
                     0
                 ][4]
 
             self._packet[0] = 0b00100011  # Not leap second, NTP version 4, Client mode
             for i in range(1, PACKET_SIZE):
                 self._packet[i] = 0
             with self._pool.socket(self._pool.AF_INET, self._pool.SOCK_DGRAM) as sock:
-                # Since the ESP32SPI doesn't support sendto, we are using
-                # connect + send to standardize code
                 sock.settimeout(self._socket_timeout)
-                sock.connect(self._socket_address)
-                sock.send(self._packet)
+                sock.sendto(self._packet, self._socket_address)
                 sock.recv_into(self._packet)
                 # Get the time in the context to minimize the difference between it and receiving
                 # the packet.
                 destination = time.monotonic_ns()
             poll = struct.unpack_from("!B", self._packet, offset=2)[0]
             self.next_sync = destination + (2**poll) * 1_000_000_000
             seconds = struct.unpack_from("!I", self._packet, offset=PACKET_SIZE - 8)[0]
```

### Comparing `adafruit_circuitpython_ntp-3.1.0/docs/_static/favicon.ico` & `adafruit_circuitpython_ntp-3.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/docs/conf.py` & `adafruit_circuitpython_ntp-3.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/docs/examples.rst` & `adafruit_circuitpython_ntp-3.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/docs/index.rst` & `adafruit_circuitpython_ntp-3.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/examples/ntp_connection_manager.py` & `adafruit_circuitpython_ntp-3.1.1/examples/ntp_connection_manager.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/examples/ntp_set_rtc.py` & `adafruit_circuitpython_ntp-3.1.1/examples/ntp_set_rtc.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/examples/ntp_simpletest.py` & `adafruit_circuitpython_ntp-3.1.1/examples/ntp_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_ntp-3.1.0/pyproject.toml` & `adafruit_circuitpython_ntp-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ntp"
 description = "Network Time Protocol (NTP) helper for Python"
-version = "3.1.0"
+version = "3.1.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_NTP"}
 keywords = [
     "adafruit",
```

