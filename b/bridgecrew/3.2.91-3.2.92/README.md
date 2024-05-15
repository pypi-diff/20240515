# Comparing `tmp/bridgecrew-3.2.91.tar.gz` & `tmp/bridgecrew-3.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bridgecrew-3.2.91.tar", last modified: Sun May 12 10:41:51 2024, max compression
+gzip compressed data, was "dist/bridgecrew-3.2.92.tar", last modified: Wed May 15 08:49:27 2024, max compression
```

## Comparing `bridgecrew-3.2.91.tar` & `bridgecrew-3.2.92.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/
--rw-r--r--   0 root         (0) root         (0)     1462 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      505 2024-01-22 12:14:48.000000 bridgecrew-3.2.91/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/bin/
--rwxr-xr-x   0 root         (0) root         (0)       93 2024-01-22 12:14:48.000000 bridgecrew-3.2.91/bin/bridgecrew
--rw-r--r--   0 root         (0) root         (0)     1368 2024-01-22 12:14:48.000000 bridgecrew-3.2.91/bin/bridgecrew.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/bridgecrew/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-22 12:14:48.000000 bridgecrew-3.2.91/bridgecrew/__init__.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-01-22 12:14:48.000000 bridgecrew-3.2.91/bridgecrew/banner.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-01-22 12:14:48.000000 bridgecrew-3.2.91/bridgecrew/main.py
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-12 10:41:48.000000 bridgecrew-3.2.91/bridgecrew/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/bridgecrew.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1462 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/bridgecrew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/bridgecrew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/bridgecrew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/bridgecrew.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/bridgecrew.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 10:41:51.000000 bridgecrew-3.2.91/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1773 2024-01-22 12:14:48.000000 bridgecrew-3.2.91/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/
+-rw-r--r--   0 root         (0) root         (0)     1375 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      505 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bin/
+-rwxr-xr-x   0 root         (0) root         (0)       93 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bin/bridgecrew
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bin/bridgecrew.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bridgecrew/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      481 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bridgecrew/banner.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bridgecrew/main.py
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-15 08:49:23.000000 bridgecrew-3.2.92/bridgecrew/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1375 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/setup.py
```

### Comparing `bridgecrew-3.2.91/PKG-INFO` & `bridgecrew-3.2.92/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 3.2.91
+Version: 3.2.92
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
-Description: # DEPRECATED: This project is no longer supported and will be archived end of 2023. Please use [checkov](https://github.com/bridgecrewio/checkov) instead.
-        
-        # Bridgecrew Python Package
-        [![build status](https://github.com/bridgecrewio/bridgecrew-py/workflows/release/badge.svg)](https://github.com/bridgecrewio/bridgecrew-py/actions?query=workflow%3Arelease)
-        [![PyPI](https://img.shields.io/pypi/v/bridgecrew)](https://pypi.org/project/checkov/)
-        
-        Wraps checkov with a bridgecrew cli (does exactly the same)
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
+
+# DEPRECATED: This project is no longer supported and will be archived end of 2023. Please use [checkov](https://github.com/bridgecrewio/checkov) instead.
+
+# Bridgecrew Python Package
+[![build status](https://github.com/bridgecrewio/bridgecrew-py/workflows/release/badge.svg)](https://github.com/bridgecrewio/bridgecrew-py/actions?query=workflow%3Arelease)
+[![PyPI](https://img.shields.io/pypi/v/bridgecrew)](https://pypi.org/project/checkov/)
+
+Wraps checkov with a bridgecrew cli (does exactly the same)
```

### Comparing `bridgecrew-3.2.91/bin/bridgecrew.cmd` & `bridgecrew-3.2.92/bin/bridgecrew.cmd`

 * *Files identical despite different names*

### Comparing `bridgecrew-3.2.91/bridgecrew.egg-info/PKG-INFO` & `bridgecrew-3.2.92/bridgecrew.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 3.2.91
+Version: 3.2.92
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
-Description: # DEPRECATED: This project is no longer supported and will be archived end of 2023. Please use [checkov](https://github.com/bridgecrewio/checkov) instead.
-        
-        # Bridgecrew Python Package
-        [![build status](https://github.com/bridgecrewio/bridgecrew-py/workflows/release/badge.svg)](https://github.com/bridgecrewio/bridgecrew-py/actions?query=workflow%3Arelease)
-        [![PyPI](https://img.shields.io/pypi/v/bridgecrew)](https://pypi.org/project/checkov/)
-        
-        Wraps checkov with a bridgecrew cli (does exactly the same)
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
+
+# DEPRECATED: This project is no longer supported and will be archived end of 2023. Please use [checkov](https://github.com/bridgecrewio/checkov) instead.
+
+# Bridgecrew Python Package
+[![build status](https://github.com/bridgecrewio/bridgecrew-py/workflows/release/badge.svg)](https://github.com/bridgecrewio/bridgecrew-py/actions?query=workflow%3Arelease)
+[![PyPI](https://img.shields.io/pypi/v/bridgecrew)](https://pypi.org/project/checkov/)
+
+Wraps checkov with a bridgecrew cli (does exactly the same)
```

### Comparing `bridgecrew-3.2.91/setup.py` & `bridgecrew-3.2.92/setup.py`

 * *Files identical despite different names*

