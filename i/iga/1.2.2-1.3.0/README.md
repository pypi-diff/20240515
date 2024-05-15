# Comparing `tmp/iga-1.2.2.tar.gz` & `tmp/iga-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-1.2.2.tar", last modified: Thu Nov  9 03:04:41 2023, max compression
+gzip compressed data, was "iga-1.3.0.tar", last modified: Wed May 15 21:46:27 2024, max compression
```

## Comparing `iga-1.2.2.tar` & `iga-1.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-11-09 03:04:41.811822 iga-1.2.2/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-11-09 03:02:56.000000 iga-1.2.2/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    41457 2023-11-09 03:04:41.811988 iga-1.2.2/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    40419 2023-11-09 03:03:34.000000 iga-1.2.2/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-11-09 03:04:41.808506 iga-1.2.2/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1533 2023-11-09 03:02:56.000000 iga-1.2.2/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-11-09 03:02:56.000000 iga-1.2.2/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    35597 2023-11-09 03:02:56.000000 iga-1.2.2/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3355 2023-11-09 03:02:56.000000 iga-1.2.2/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2855 2023-11-09 03:02:56.000000 iga-1.2.2/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-11-09 03:02:56.000000 iga-1.2.2/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-11-09 03:02:56.000000 iga-1.2.2/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    17863 2023-11-09 03:02:56.000000 iga-1.2.2/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-11-09 03:02:56.000000 iga-1.2.2/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    19446 2023-11-09 03:02:56.000000 iga-1.2.2/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2064 2023-11-09 03:02:56.000000 iga-1.2.2/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   248567 2023-11-09 03:02:56.000000 iga-1.2.2/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    70406 2023-11-09 03:02:56.000000 iga-1.2.2/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14514 2023-11-09 03:02:56.000000 iga-1.2.2/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-11-09 03:02:56.000000 iga-1.2.2/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-11-09 03:02:56.000000 iga-1.2.2/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-11-09 03:02:56.000000 iga-1.2.2/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-11-09 03:02:56.000000 iga-1.2.2/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-11-09 03:04:41.809368 iga-1.2.2/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    41457 2023-11-09 03:04:41.000000 iga-1.2.2/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-11-09 03:04:41.000000 iga-1.2.2/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-11-09 03:04:41.000000 iga-1.2.2/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-11-09 03:04:41.000000 iga-1.2.2/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-11-09 03:04:41.000000 iga-1.2.2/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      659 2023-11-09 03:04:41.000000 iga-1.2.2/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-11-09 03:04:41.000000 iga-1.2.2/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1216 2023-11-09 03:04:41.812319 iga-1.2.2/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1548 2023-11-09 03:02:56.000000 iga-1.2.2/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-11-09 03:04:41.811718 iga-1.2.2/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     6127 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_is_person.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_name_splitting.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6014 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-11-09 03:02:56.000000 iga-1.2.2/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2024-05-15 21:46:27.592610 iga-1.3.0/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2024-05-15 21:29:58.000000 iga-1.3.0/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    46959 2024-05-15 21:46:27.592511 iga-1.3.0/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    44530 2024-05-15 21:29:58.000000 iga-1.3.0/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2024-05-15 21:46:27.583975 iga-1.3.0/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1533 2024-05-15 21:31:28.000000 iga-1.3.0/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2024-05-15 21:29:58.000000 iga-1.3.0/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    35796 2024-05-15 21:29:58.000000 iga-1.3.0/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3477 2024-05-15 21:29:58.000000 iga-1.3.0/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2855 2024-05-15 21:29:58.000000 iga-1.3.0/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1252 2024-05-15 21:29:58.000000 iga-1.3.0/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1514 2024-05-15 21:29:58.000000 iga-1.3.0/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    17863 2024-05-15 21:29:58.000000 iga-1.3.0/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4905 2024-05-15 21:29:58.000000 iga-1.3.0/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    19651 2024-05-15 21:29:58.000000 iga-1.3.0/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2064 2024-05-15 21:29:58.000000 iga-1.3.0/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   248567 2023-11-09 03:02:56.000000 iga-1.3.0/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    70843 2024-05-15 21:29:58.000000 iga-1.3.0/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    18336 2024-05-15 21:29:58.000000 iga-1.3.0/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2024-05-15 21:29:58.000000 iga-1.3.0/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2024-05-15 21:29:58.000000 iga-1.3.0/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2024-05-15 21:29:58.000000 iga-1.3.0/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2024-05-15 21:29:58.000000 iga-1.3.0/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2024-05-15 21:46:27.592061 iga-1.3.0/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    46959 2024-05-15 21:46:27.000000 iga-1.3.0/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2024-05-15 21:46:27.000000 iga-1.3.0/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2024-05-15 21:46:27.000000 iga-1.3.0/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2024-05-15 21:46:27.000000 iga-1.3.0/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2024-05-15 21:46:27.000000 iga-1.3.0/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      776 2024-05-15 21:46:27.000000 iga-1.3.0/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2024-05-15 21:46:27.000000 iga-1.3.0/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1216 2024-05-15 21:46:27.592938 iga-1.3.0/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1579 2024-05-15 21:29:58.000000 iga-1.3.0/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2024-05-15 21:46:27.591868 iga-1.3.0/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     6127 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3672 2024-05-15 21:29:58.000000 iga-1.3.0/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    52072 2024-05-15 21:29:58.000000 iga-1.3.0/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4407 2024-05-15 21:29:58.000000 iga-1.3.0/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2043 2024-05-15 21:29:58.000000 iga-1.3.0/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6014 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-11-09 03:02:56.000000 iga-1.3.0/tests/test_text_utils.py
```

### Comparing `iga-1.2.2/LICENSE` & `iga-1.3.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022-2023, Caltech
+Copyright (c) 2022-2024, Caltech
 All rights not granted herein are expressly reserved by Caltech.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer.
```

### Comparing `iga-1.2.2/PKG-INFO` & `iga-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,73 +1,60 @@
-Metadata-Version: 2.1
-Name: iga
-Version: 1.2.2
-Summary: The InvenioRDM GitHub Archiver (IGA) automatically archives GitHub releases in an InvenioRDM repository.
-Home-page: https://github.com/caltechlibrary/iga
-Author: Michael Hucka
-Author-email: mhucka@caltech.edu
-License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
-Project-URL: Source Code, https://github.com/caltechlibrary/iga
-Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
-Keywords: Python,applications
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: No Input/Output (Daemon)
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
-
-IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
-
-[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
-[![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
-[![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
-[![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20)](https://data.caltech.edu/records/zsmem-2pg20)
+# IGA<img alt="IGA logo" width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
+
+IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/inveniordm-github-archiver) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+
+[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases) [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/blob/develop/LICENSE) [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/) [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/) [![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20/versions/latest)](https://data.caltech.edu/records/zsmem-2pg20/latest)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
+  * [IGA as a standalone program](#iga-as-a-standalone-program)
+  * [IGA as a GitHub Actions workflow](#iga-as-a-github-actions-workflow)
 * [Quick start](#quick-start)
 * [Usage](#usage)
+  * [Identifying the InvenioRDM server](#identifying-the-inveniordm-server)
+  * [Providing an InvenioRDM access token](#providing-an-inveniordm-access-token)
+  * [Providing a GitHub access token](#providing-a-github-access-token)
+  * [Specifying a GitHub release](#specifying-a-github-release)
+  * [Gathering metadata for an InvenioRDM record](#gathering-metadata-for-an-inveniordm-record)
+  * [Specifying GitHub file assets](#specifying-github-file-assets)
+  * [Handling communities](#handling-communities)
+  * [Indicating draft versus published records](#indicating-draft-versus-published-records)
+  * [Versioning records](#versioning-records)
+  * [Other options recognized by IGA](#other-options-recognized-by-iga)
+  * [Summary of command-line options](#summary-of-command-line-options)
+  * [Return values](#return-values)
+  * [Adding a DOI badge to your GitHub repository](#adding-a-doi-badge-to-your-github-repository)
 * [Known issues and limitations](#known-issues-and-limitations)
 * [Getting help](#getting-help)
 * [Contributing](#contributing)
 * [License](#license)
-* [Acknowledgments](#authors-and-acknowledgments)
+* [Acknowledgments](#acknowledgments)
 
 
 ## Introduction
 
 [InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and data sets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the [_InvenioRDM GitHub Archiver_](https://github.com/caltechlibrary/iga) (IGA) comes in.
 
 IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Actions](https://docs.github.com/en/actions) workflow to archive GitHub releases automatically for a repository each time they are made.
 
 <p align=center>
-<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" alt="Screenshot of a software release in GitHub" width="40%">
 <span style="font-size: 150%">➜</span>
-<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" alt="Screenshot of the corresponding entry in InvenioRDM" width="40%">
 </p>
 
 IGA offers many notable features:
+
 * Automatic metadata extraction from GitHub plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
 * Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
 * Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org), [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
-* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google, and other sources
+* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), Google, and other sources
 * Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
 * Automatic lookup of human names in [ORCID.org](https://orcid.org) (assuming ORCID id's are provided)
 * Automatic splitting of human names into family & given names using [ML](https://en.wikipedia.org/wiki/Machine_learning) methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
 * Support for overriding the record that IGA creates, for complete control if you need it
 * Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
 * Extensive use of logging so you can see what's going on under the hood
@@ -79,68 +66,79 @@
 
 ### IGA as a standalone program
 
 Please choose an approach that suits your situation and preferences.
 
 <details><summary><h4><i>Alternative 1: using <code>pipx</code></i></h4></summary>
 
-[Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies from other Python programs on your system, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
+[Pipx](https://github.com/pypa/pipx) lets you install Python programs in a way that isolates Python dependencies from other Python programs on your system, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
+
 ```sh
 pipx install iga
 ```
 
 After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+
 ```shell
 iga --help
 ```
+
 </details>
 
 <details><summary><h4><i>Alternative 2: using <code>pip</code></i></h4></summary>
 
 IGA is available from the [Python package repository PyPI](https://pypi.org) and can be installed using [`pip`](https://pip.pypa.io/en/stable/installing/):
+
 ```sh
 python3 -m pip install iga
 ```
 
 As an alternative to getting it from [PyPI](https://pypi.org), you can install `iga` directly from GitHub:
+
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
 
 After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+
 ```shell
 iga --help
 ```
+
 </details>
 
 <details><summary><h4><i>Alternative 3: from sources</i></h4></summary>
 
 If  you prefer to install IGA directly from the source code, first obtain a copy by either downloading the source archive from the [IGA releases page on GitHub](https://github.com/caltechlibrary/iga/releases), or by using `git` to clone the repository to a location on your computer. For example,
+
 ```sh
 git clone https://github.com/caltechlibrary/iga
 ```
 
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
+
 ```sh
 cd iga
 python3 setup.py install
 ```
+
 </details>
 
 Once you have installed `iga`, the next steps are (1) [get an InvenioRDM token](#getting-an-inveniordm-token) and (2) [configure `iga` for running locally](#configuring-and-running-iga-locally).
 
 
 ### IGA as a GitHub Actions workflow
 
 A [GitHub Actions](https://docs.github.com/en/actions) workflow is an automated process that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
 1. In the main branch of your GitHub repository, create a `.github/workflows` directory
 2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/main/sample-workflow.yml) into it:
+
     ```yaml
     # ╭────────────────────────────────────────────╮
     # │ Configure this section                     │
     # ╰────────────────────────────────────────────╯
 
     env:
       # 👋🏻 Set the next variable to your InvenioRDM server address 👋🏻
@@ -163,124 +161,127 @@
     name: InvenioRDM GitHub Archiver
     on:
       release:
         types: [published]
       workflow_dispatch:
         inputs:
           release_tag:
-            description: "The release tag (empty = latest):"
+            description: The release tag (empty = latest)
           parent_record:
-            description: "ID of parent record (for versioning):"
+            description: ID of parent record (for versioning)
           community:
-            description: "Name of InvenioRDM community (if any):"
+            description: Name of InvenioRDM community (if any)
           draft:
-            description: "Mark the record as a draft"
+            description: Mark the record as a draft
             type: boolean
           all_assets:
-            description: "Attach all GitHub assets"
+            description: Attach all GitHub assets
             type: boolean
           all_metadata:
-            description: "Include additional GitHub metadata"
+            description: Include additional GitHub metadata
             type: boolean
           debug:
-            description: "Print debug info in the GitHub log"
+            description: Print debug info in the GitHub log
             type: boolean
 
     run-name: Archive ${{inputs.release_tag || 'latest release'}} in InvenioRDM
     jobs:
       run_iga:
-        name: "Send to ${{needs.get_repository.outputs.server}}"
+        name: Send to ${{needs.get_repository.outputs.server}}
         runs-on: ubuntu-latest
         needs: get_repository
         steps:
-          - uses: caltechlibrary/iga@main
+          - uses: caltechlibrary/iga@v1
             with:
               INVENIO_SERVER: ${{env.INVENIO_SERVER}}
               INVENIO_TOKEN:  ${{secrets.INVENIO_TOKEN}}
               all_assets:     ${{github.event.inputs.all_assets || env.all_assets}}
               all_metadata:   ${{github.event.inputs.all_metadata || env.all_metadata}}
               debug:          ${{github.event.inputs.debug || env.debug}}
               draft:          ${{github.event.inputs.draft || env.draft}}
               community:      ${{github.event.inputs.community || env.community}}
               parent_record:  ${{github.event.inputs.parent_record || env.parent_record}}
               release_tag:    ${{github.event.inputs.release_tag || 'latest'}}
       get_repository:
-        name: "Get repository name"
+        name: Get repository name
         runs-on: ubuntu-latest
         outputs:
           server: ${{steps.parse.outputs.host}}
         steps:
           - name: Extract name from INVENIO_SERVER
             id: parse
             run: echo "host=$(cut -d'/' -f3 <<< ${{env.INVENIO_SERVER}} | cut -d':' -f1)" >> $GITHUB_OUTPUT
     ```
+
 3. **Edit the value of the `INVENIO_SERVER` variable (line 7 above)** ↑
 4. Optionally, change the values of other options (`parent_record`, `community`, etc.)
 5. Save the file, commit the changes to git, and push your changes to GitHub
 
 Once you have installed the GitHub Action workflow for IGA, the next steps are (1) [get an InvenioRDM token](#getting-an-inveniordm-token) and (2) [configure the GitHub Action workflow](#configuring-and-running-iga-as-a-github-actions-workflow).
 
 
 ## Quick start
 
-No matter whether IGA is run locally on your computer or as a GitHub Actions workflow, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
-is the first step.
+No matter whether IGA is run locally on your computer or as a GitHub Actions workflow, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one is the first step.
 
 ### Getting an InvenioRDM token
 
-<img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" width="60%" align="right">
+<img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" alt="Screenshot of InvenioRDM PAT menu" width="60%" align="right">
 
 1. Log in to your InvenioRDM account
 2. Go to the _Applications_ page in your account profile
 3. Click the <kbd>New token</kbd> button next to "Personal access tokens"
 4. On the page that is shown after you click that button, name your token (the name does not matter) and click the <kbd>Create</kbd> button
 5. After InvenioRDM creates and shows you the token, **copy it to a safe location** because InvenioRDM will not show it again
 
 ### Configuring and running IGA locally
 
 To send a GitHub release to your InvenioRDM server, IGA needs this information:
+
 1. (Required) The identity of the GitHub release to be archived
 2. (Required) The address of the destination InvenioRDM server
 3. (Required) A personal access token for InvenioRDM (from [above](#getting-an-inveniordm-token))
 4. (Optional) A [personal access token for GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
 
 The identity of the GitHub release is always given as an argument to IGA on the command line; the remaining values can be provided either via command-line options or environment variables. One approach is to set environment variables in shell scripts or your interactive shell. Here is an example using Bash shell syntax, with fake token values:
+
 ```shell
 export INVENIO_SERVER=https://data.caltech.edu
 export INVENIO_TOKEN=qKLoOH0KYf4D98PGYQGnC09hiuqw3Y1SZllYnonRVzGJbWz2
 export GITHUB_TOKEN=ghp_wQXp6sy3AsKyyEo4l9esHNxOdo6T34Zsthz
 ```
 
 Once these are set, use of IGA can be as simple as providing a URL for a release in GitHub. For example, the following command creates a draft record (the `-d` option is short for `--draft`) for another project in GitHub and tells IGA to open (the `-o` option is short for `--open`) the newly-created InvenioRDM entry in a web browser:
+
 ```shell
 iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 More options are described in the section on [detailed usage information](#usage) below.
 
 
 ### Configuring and running IGA as a GitHub Actions workflow
 
-After doing the [GitHub Actions installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
+After doing the [GitHub Actions installation](#configuring-and-running-iga-as-a-github-actions-workflow) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
 
-1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" width="85%"></p>
-2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" width="40%"></p>
-3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" width="60%"></p>
+1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" alt="Screenshot of repository tabs in GitHub" width="85%"></p>
+2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" alt="Screenshot of GitHub secrets sidebar item" width="40%"></p>
+3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" alt="Screenshot of GitHub secrets interface" width="60%"></p>
 4. Name the variable `INVENIO_TOKEN` and paste in your InvenioRDM token
 5. Finish by clicking the green <kbd>Add secret</kbd> button
 
 #### Testing the workflow
 
 After setting up the workflow and storing the InvenioRDM token in your repository on GitHub, it's a good idea to run the workflow manually to test that it works as expected.
 
-1. Go to the _Actions_ tab in your repository and click on the name of the workflow in the sidebar on the left<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-run-workflow.png" width="90%"></p>
+1. Go to the _Actions_ tab in your repository and click on the name of the workflow in the sidebar on the left<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-run-workflow.png" alt="Screenshot of GitHub actions workflow list" width="90%"></p>
 2. Click the <kbd>Run workflow</kbd> button in the right-hand side of the blue strip
-3. In the pull-down, change the value of "Mark the record as a draft" to `true`<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-workflow-options-circled.png" width="40%"></p>
+3. In the pull-down, change the value of "Mark the record as a draft" to `true`<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-workflow-options-circled.png" alt="Screenshot of GitHub Actions workflow menu" width="40%"></p>
 4. Click the green <kbd>Run workflow</kbd> button near the bottom
-5. Refresh the web page and a new line will be shown named after your workflow file<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-running-workflow.png" width="90%"></p>
+5. Refresh the web page and a new line will be shown named after your workflow file<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-running-workflow.png" alt="Screenshot of a running workflow in GitHub Actions" width="90%"></p>
 6. Click the title of the workflow to see the IGA workflow progress and results
 
 
 #### Running the workflow when releasing software
 
 Once the personal access token from InvenioRDM is stored as a GitHub secret, the workflow should run automatically every time a new release is made on GitHub &ndash; no further action should be needed. You can check the results (and look for errors if something went wrong) by going to the _Actions_ tab in your GitHub repository.
 
@@ -297,52 +298,58 @@
 
 A personal access token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
-It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some public repositories IGA will not hit the limit. However, if you are archiving a private repository, run IGA multiple times in a row, or the repository has many contributors, then you will need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some public repositories IGA will not hit the limit. However, if you are archiving a private repository, run IGA multiple times in a row, or the repository has many contributors, then you will need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit [https://docs.github.com/en/authentication](https://docs.github.com/en/authentication) and follow the instructions for creating a "classic" personal access token.
 
 Note that when you run IGA as a GitHub Actions workflow, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Actions workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
- 1. The full URL of the web page on GitHub of a tagged release. In this case,
+
+1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
- 2. A combination of _account name_, _repository name_, and _tag_. In this
+2. A combination of _account name_, _repository name_, and _tag_. In this
     case, the final argument on the command line must be the _tag_, and in
     addition, values for the options `--account` and `--repo` must be provided.
 
 Here's an example using approach #1 (assuming environment variables `INVENIO_SERVER`, `INVENIO_TOKEN`, and `GITHUB_TOKEN` have all been set):
+
 ```shell
 iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
+
 and here's the equivalent using approach #2:
+
 ```shell
 iga --github-account mhucka --github-repo taupe v1.2.0
 ```
+
 Note that when using this form of the command, the release tag (`v1.2.0` above) must be the last item given on the command line.
 
 ### Gathering metadata for an InvenioRDM record
 
 The record created in InvenioRDM is constructed using information obtained using GitHub's API as well as several other APIs as needed. The information includes the following:
- * (if one exists) a `codemeta.json` file in the GitHub repository
- * (if one exists) a `CITATION.cff` file in the GitHub repository
- * data available from GitHub for the release
- * data available from GitHub for the repository
- * data available from GitHub for the account of the owner
- * data available from GitHub for the accounts of repository contributors
- * file assets associated with the GitHub release
- * data available from ORCID.org for ORCID identifiers
- * data available from ROR.org for Research Organization Registry identifiers
- * data available from DOI.org, NCBI, Google Books, & others for publications
- * data available from spdx.org for software licenses
+
+* (if one exists) a `codemeta.json` file in the GitHub repository
+* (if one exists) a `CITATION.cff` file in the GitHub repository
+* data available from GitHub for the release
+* data available from GitHub for the repository
+* data available from GitHub for the account of the owner
+* data available from GitHub for the accounts of repository contributors
+* file assets associated with the GitHub release
+* data available from ORCID.org for ORCID identifiers
+* data available from ROR.org for Research Organization Registry identifiers
+* data available from DOI.org, NCBI, Google Books, & others for publications
+* data available from spdx.org for software licenses
 
 IGA tries to use [`CodeMeta.json`](https://codemeta.github.io) first and [`CITATION.cff`](https://citation-file-format.github.io) second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
 
 To override the auto-created metadata, use the option `--read-metadata` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-metadata` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
 
 ### Specifying GitHub file assets
 
@@ -359,15 +366,16 @@
 ### Indicating draft versus published records
 
 If the `--community` option is not used, then by default, IGA will finalize and publish the record. To make it stop short and leave the record as a draft instead, use the option `--draft`. The draft option also takes precedence over the community option: if you use both `--draft` and `--community`, IGA will stop after creating the draft record and will _not_ submit it to the community.  (You can nevertheless submit the record to a community manually once the draft is created, by visiting the record's web page and using the InvenioRDM interface there.)
 
 ### Versioning records
 
 The option `--parent-record` can be used to indicate that the record being constructed is a new version of an existing record. This will make IGA use the InvenioRDM API for [record versioning](https://inveniordm.docs.cern.ch/releases/versions/version-v2.0.0/#versioning-support). The newly-created record will be linked to a parent record identified by the value passed to `--parent-record`. The value must be either an InvenioRDM record identifier (which is a sequence of alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`, generated by the InvenioRDM server), or a URL to the landing page of the record in the InvenioRDM server. (Note that such URLs end in the record identifier.) Here is an example of using this option:
-```
+
+```shell
 iga --parent-record xbcd4-efgh5 https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 ### Other options recognized by IGA
 
 Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
@@ -387,23 +395,23 @@
 
 As explain above, IGA takes one required argument on the command line: either (1) the full URL of a web page on GitHub of a tagged release, or (2) a release tag name which is to be used in combination with options `--github-account` and `--github-repo`. The following table summarizes all the command line options available.
 
 | Long&nbsp;form&nbsp;option&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Short&nbsp;&nbsp; | Meaning | Default |  |
 |------------------------|----------|--------------------------------------|---------|---|
 | `--all-assets`         | `-A`     | Attach all GitHub assets | Attach only the release source ZIP| |
 | `--all-metadata`       | `-M`     | Include additional metadata from GitHub | Favor CodeMeta & CFF | |
-| `--community` _C_      | `-c` _C_ | Submit record to RDM community _C_ | Don't submit record to any community | | 
+| `--community` _C_      | `-c` _C_ | Submit record to RDM community _C_ | Don't submit record to any community | |
 | `--draft`              | `-d`     | Mark the RDM record as a draft | Publish record when done | |
 | `--file` _F_           | `-f` _F_ | Upload local file _F_ instead of GitHub assets | Upload only GitHub assets | ⚑ |
-| `--github-account` _A_ | `-a` _A_ | Look in GitHub account _A_ | Get account name from release URL | ✯ | 
+| `--github-account` _A_ | `-a` _A_ | Look in GitHub account _A_ | Get account name from release URL | ✯ |
 | `--github-repo` _R_    | `-r` _R_ | Look in GitHub repository _R_ of account _A_ | Get repo name from release URL | ✯ |
 | `--github-token` _T_   | `-t` _T_ | Use GitHub access token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
-| `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
-| `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
+| `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | |
+| `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | |
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
 | `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
 | `--print-doi`          | `-i`     | Print both the DOI & record URL when done | Print only the record URL | |
 | `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
@@ -427,18 +435,47 @@
 | 2    | encountered a bad or missing value for an option         |
 | 3    | encountered a problem with a file or directory           |
 | 4    | encountered a problem interacting with GitHub            |
 | 5    | encountered a problem interacting with InvenioRDM        |
 | 6    | the personal access token was rejected                   |
 | 7    | an exception or fatal error occurred                     |
 
+### Adding a DOI badge to your GitHub repository
+
+Once you have set up the IGA workflow in your GitHub repository, you may wish to add a DOI badge to your repository's README file. It would be a chore to keep updating the DOI value in this badge every time a new release is made, and thankfully, it's not necessary: it's possible to make the badge get the current DOI value dynamically. Here is how:
+
+1. _After_ you have at least one release archived in your InvenioRDM server, find out the DOI of that release in InvenioRDM, and extract the tail end of that DOI. The DOI assigned by InvenioRDM will be a string such as `10.22002/zsmem-2pg20`; the tail end is the `zsmem-2pg20` part. (Your DOI and tail portion will be different.)
+2. Let <i><b><code>SERVERURL</code></b></i> stand for the URL for your InvenioRDM server, and let <i><b><code>IDENTIFIER</code></b></i> stand for the identifier portion of the DOI. In your `README.md` file, write the DOI badge as follows (without line breaks):
+
+    <pre><code>[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&query=$.pids.doi.identifier&uri=<i><b><code>SERVERURL</code></b></i>/api/records/<i><b><code>IDENTIFIER</code></b></i>/versions/latest)](<i><b><code>SERVERURL</code></b></i>/records/<i><b><code>IDENTIFIER</code></b></i>/latest)</code></pre>
+
+For example, for CaltechDATA and the archived IGA releases there,
+
+* <i><b><code>SERVERURL</code></b></i> = `http://data.caltech.edu`
+* <i><b><code>IDENTIFIER</code></b></i> = `zsmem-2pg20`
+
+which leads to the following badge string for IGA's `README.md` file:
+
+```txt
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20/versions/latest)](https://data.caltech.edu/records/zsmem-2pg20/latest)
+```
+
+<br>The result looks like this: <div align="center">
+
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20/versions/latest)](https://data.caltech.edu/records/zsmem-2pg20/latest)
+
+</div>
+
+You can change the look of the badge by using style parameters. Please refer to the [Shields.io](https://shields.io/badges/static-badge) documentation for static badges.
+
 
 ## Known issues and limitations
 
 The following are known issues and limitations.
+
 * As of mid-2023, InvenioRDM requires names of record creators and other contributors to be split into given (first) and family (surname). This is problematic for multiple reasons. The first is that mononyms are common in many countries: a person's name may legitimately be only a single word which is not conceptually a "given" or "family" name.  To compound the difficulty for IGA, names are stored as single fields in GitHub account metadata, so unless a repository has a `codemeta.json` or `CITATION.cff` file (which allow authors more control over how they want their names represented), IGA is forced to try to split the single GitHub name string into two parts. _A foolproof algorithm for doing this does not exist_, so IGA will sometimes get it wrong. (That said, IGA goes to extraordinary lengths to try to do a good job.)
 * InvenioRDM requires that identities (creators, contributors, etc.) to be labeled as personal or organizational. The nature of identities is usually made clear in `codemeta.json` and `CITATION.cff` files. GitHub also provides a flag that is meant to be used to label organizational accounts, but sometimes people don't set the GitHub account information correctly. Consequently, if IGA has to use GitHub data to get (e.g.) the list of contributors on a project, it may mislabel identities in the InvenioRDM record it produces.
 * Some accounts on GitHub are software automation or "bot" accounts, but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub, so if they're not labeled as bot or organizational accounts in GitHub, IGA can't recognize that they're humans. If such an account is the creator of a release in GitHub, and IGA tries to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI".
 * Funder and funding information can only be specified in `codemeta.json` files; neither GitHub nor `CITATION.cff` have provisions to store this kind of metadata. The CodeMeta specification defines two fields for this purpose: `funder` and `funding`. Unfortunately, these map imperfectly to the requirements of InvenioRDM's metadata format. In addition, people don't always follow the CodeMeta guidelines, and sometimes they write funding information as text strings (instead of structured objects), the interpretation of which would require software that can recognize grant and funding agency information from free-text descriptions. This combination of factors means IGA often can't fill in the funding metadata in InvenioRDM records even if there is some funding information in the `codemeta.json` file.
 
 
 ## Getting help
@@ -449,48 +486,51 @@
 ## Contributing
 
 Your help and participation in enhancing IGA is welcome!  Please visit the [guidelines for contributing](CONTRIBUTING.md) for some tips on getting started.
 
 
 ## License
 
-Software produced by the Caltech Library is Copyright © 2023 California Institute of Technology.  This software is freely distributed under a BSD-style license.  Please see the [LICENSE](LICENSE) file for more information.
+Software produced by the Caltech Library is Copyright © 2022–2024 California Institute of Technology.  This software is freely distributed under a BSD-style license.  Please see the [LICENSE](LICENSE) file for more information.
 
 ## Acknowledgments
 
 This work was funded by the California Institute of Technology Library.
 
 IGA uses multiple other open-source packages, without which it would have taken much longer to write the software. I want to acknowledge this debt. In alphabetical order, the packages are:
+
 * [Aenum](https://github.com/ethanfurman/aenum) &ndash; package for advanced enumerations
 * [Arrow](https://pypi.org/project/arrow/) &ndash; a library for creating & manipulating dates
 * [Boltons](https://github.com/mahmoud/boltons/) &ndash; package of miscellaneous Python utilities
 * [caltechdata_api](https://github.com/caltechlibrary/caltechdata_api) &ndash; package for using the CaltechDATA API
 * [CommonPy](https://github.com/caltechlibrary/commonpy) &ndash; a collection of commonly-useful Python functions
-* [demoji](https://github.com/bsolomon1124/demoji) &ndash; find or remove emojis from text
 * [dirtyjson](https://github.com/codecobblers/dirtyjson) &ndash; JSON decoder that copes with problematic JSON files and reports useful error messages
 * [flake8](https://github.com/pycqa/flake8) &ndash; Python code linter and style analyzer
+* [Ginza](https://github.com/megagonlabs/ginza) &ndash; Japanese NLP Library
 * [httpx](https://www.python-httpx.org) &ndash; HTTP client library that supports HTTP/2
 * [humanize](https://github.com/jmoiron/humanize) &ndash; make numbers more easily readable by humans
 * [idutils](https://github.com/inveniosoftware/idutils) &ndash; package for validating and normalizing various kinds of persistent identifiers
 * [ipdb](https://github.com/gotcha/ipdb) &ndash; the IPython debugger
 * [iptools](https://github.com/bd808/python-iptools) &ndash; utilities for dealing with IP addresses
 * [isbnlib](https://github.com/xlcnd/isbnlib) &ndash; utilities for dealing with ISBNs
+* [Jamo](https://github.com/JDongian/python-jamo) &ndash; Hangul character analysis
 * [json5](https://github.com/dpranke/pyjson5) &ndash; extended JSON format parser
 * [latexcodec](https://github.com/mcmtroffaes/latexcodec) &ndash; lexer and codec to work with LaTeX code in Python
+* [Lingua](https://github.com/pemistahl/lingua) &ndash; language detection library
 * [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) &ndash; a link recognition library with full unicode support
 * [lxml](https://lxml.de) &ndash; an XML parsing library
 * [Markdown](https://python-markdown.github.io) &ndash; Python package for working with Markdown
 * [markdown-checklist](https://github.com/FND/markdown-checklist) &ndash; GitHub-style checklist extension for Python Markdown package
 * [mdx-breakless-lists](https://github.com/adamb70/mdx-breakless-lists) &ndash; GitHub-style Markdown lists that don't require a line break above them
 * [mdx_linkify](https://github.com/daGrevis/mdx_linkify) &ndash; extension for Python Markdown will convert text that look like links to HTML anchors
 * [MyST-parser](https://github.com/executablebooks/MyST-Parser) &ndash; A Sphinx and Docutils extension to parse an extended version of Markdown
 * [nameparser](https://github.com/derek73/python-nameparser) &ndash; package for parsing human names into their individual components
 * [probablepeople](https://github.com/datamade/probablepeople) &ndash; package for parsing names into components using ML-based techniques
 * [pybtex](https://pybtex.org) &ndash; BibTeX parser and formatter
-* [pybtex-apa7-style]() &ndash; plugin for [pybtex](https://pybtex.org) that provides APA7 style formatting
+* [pybtex-apa7-style](https://pypi.org/project/pybtex-apa7-style/) &ndash; plugin for [pybtex](https://pybtex.org) that provides APA7 style formatting
 * [pymdown-extensions](https://github.com/facelessuser/pymdown-extensions) &ndash; extensions for Python Markdown
 * [pytest](https://docs.pytest.org/en/stable/) &ndash; testing framework
 * [pytest-cov](https://github.com/pytest-dev/pytest-cov) &ndash; coverage reports for use with `pytest`
 * [pytest-mock](https://pypi.org/project/pytest-mock/) &ndash; wrapper around the `mock` package for use with `pytest`
 * [PyYAML](https://pyyaml.org) &ndash; YAML parser
 * [Rich](https://github.com/Textualize/rich) &ndash; library for writing styled text to the terminal
 * [rich-click](https://github.com/ewels/rich-click) &ndash; CLI interface built on top of [Rich](https://github.com/Textualize/rich)
@@ -511,10 +551,10 @@
 * [url-normalize](https://github.com/niksite/url-normalize) &ndash; URI/URL normalization utilities
 * [validators](https://github.com/kvesteri/validators) &ndash; data validation package for Python
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
-    <img width="100" height="100" src="https://github.com/caltechlibrary/iga/raw/main/.graphics/caltech-round.png">
+    <img width="100" height="100" alt="Caltech logo" src="https://github.com/caltechlibrary/iga/raw/main/.graphics/caltech-round.png">
   </a>
 </div>
```

### Comparing `iga-1.2.2/README.md` & `iga-1.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,126 @@
-# IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
+Metadata-Version: 2.1
+Name: iga
+Version: 1.3.0
+Summary: The InvenioRDM GitHub Archiver (IGA) automatically archives GitHub releases in an InvenioRDM repository.
+Home-page: https://github.com/caltechlibrary/iga
+Author: Michael Hucka
+Author-email: mhucka@caltech.edu
+License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
+Project-URL: Source Code, https://github.com/caltechlibrary/iga
+Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
+Keywords: Python,applications
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: No Input/Output (Daemon)
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aenum==3.1.15
+Requires-Dist: arrow==1.3.0
+Requires-Dist: boltons==21.0.0
+Requires-Dist: caltechdata-api==1.6.1
+Requires-Dist: commonpy==1.13.0
+Requires-Dist: dirtyjson==1.0.8
+Requires-Dist: ginza==5.2.0
+Requires-Dist: ja_ginza_electra==5.2.0
+Requires-Dist: httpx==0.23.1
+Requires-Dist: humanize==4.9.0
+Requires-Dist: idutils==1.2.1
+Requires-Dist: iptools==0.7.0
+Requires-Dist: isbnlib==3.10.14
+Requires-Dist: jamo==0.4.1
+Requires-Dist: json5==0.9.25
+Requires-Dist: latexcodec==3.0.0
+Requires-Dist: lingua-language-detector==2.0.2
+Requires-Dist: lxml==5.2.2
+Requires-Dist: Markdown==3.6
+Requires-Dist: markdown-checklist==0.4.4
+Requires-Dist: mdx-breakless-lists==1.0.1
+Requires-Dist: mdx_linkify==2.1
+Requires-Dist: nameparser==1.1.3
+Requires-Dist: probablepeople==0.5.5
+Requires-Dist: pybtex==0.24.0
+Requires-Dist: pybtex-apa7-style==0.1.3
+Requires-Dist: pymdown-extensions==10.8.1
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: regex==2022.3.2
+Requires-Dist: rich-click==1.8.2
+Requires-Dist: sidetrack==2.0.1
+Requires-Dist: spacy==3.7.4
+Requires-Dist: spacy-alignments==0.9.1
+Requires-Dist: spacy-curated-transformers==0.2.2
+Requires-Dist: spacy-legacy==3.0.12
+Requires-Dist: spacy-loggers==1.0.5
+Requires-Dist: spacy-pkuseg==0.0.33
+Requires-Dist: spacy-transformers==1.1.9
+Requires-Dist: StringDist==1.0.9
+Requires-Dist: url-normalize==1.4.3
+Requires-Dist: validators==0.28.1
 
-IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+# IGA<img alt="IGA logo" width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
-[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
-[![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
-[![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
-[![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20)](https://data.caltech.edu/records/zsmem-2pg20)
+IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/inveniordm-github-archiver) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+
+[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases) [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/blob/develop/LICENSE) [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/) [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/) [![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20/versions/latest)](https://data.caltech.edu/records/zsmem-2pg20/latest)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
+  * [IGA as a standalone program](#iga-as-a-standalone-program)
+  * [IGA as a GitHub Actions workflow](#iga-as-a-github-actions-workflow)
 * [Quick start](#quick-start)
 * [Usage](#usage)
+  * [Identifying the InvenioRDM server](#identifying-the-inveniordm-server)
+  * [Providing an InvenioRDM access token](#providing-an-inveniordm-access-token)
+  * [Providing a GitHub access token](#providing-a-github-access-token)
+  * [Specifying a GitHub release](#specifying-a-github-release)
+  * [Gathering metadata for an InvenioRDM record](#gathering-metadata-for-an-inveniordm-record)
+  * [Specifying GitHub file assets](#specifying-github-file-assets)
+  * [Handling communities](#handling-communities)
+  * [Indicating draft versus published records](#indicating-draft-versus-published-records)
+  * [Versioning records](#versioning-records)
+  * [Other options recognized by IGA](#other-options-recognized-by-iga)
+  * [Summary of command-line options](#summary-of-command-line-options)
+  * [Return values](#return-values)
+  * [Adding a DOI badge to your GitHub repository](#adding-a-doi-badge-to-your-github-repository)
 * [Known issues and limitations](#known-issues-and-limitations)
 * [Getting help](#getting-help)
 * [Contributing](#contributing)
 * [License](#license)
-* [Acknowledgments](#authors-and-acknowledgments)
+* [Acknowledgments](#acknowledgments)
 
 
 ## Introduction
 
 [InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and data sets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the [_InvenioRDM GitHub Archiver_](https://github.com/caltechlibrary/iga) (IGA) comes in.
 
 IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Actions](https://docs.github.com/en/actions) workflow to archive GitHub releases automatically for a repository each time they are made.
 
 <p align=center>
-<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" alt="Screenshot of a software release in GitHub" width="40%">
 <span style="font-size: 150%">➜</span>
-<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" alt="Screenshot of the corresponding entry in InvenioRDM" width="40%">
 </p>
 
 IGA offers many notable features:
+
 * Automatic metadata extraction from GitHub plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
 * Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
 * Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org), [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
-* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google, and other sources
+* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), Google, and other sources
 * Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
 * Automatic lookup of human names in [ORCID.org](https://orcid.org) (assuming ORCID id's are provided)
 * Automatic splitting of human names into family & given names using [ML](https://en.wikipedia.org/wiki/Machine_learning) methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
 * Support for overriding the record that IGA creates, for complete control if you need it
 * Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
 * Extensive use of logging so you can see what's going on under the hood
@@ -54,68 +132,79 @@
 
 ### IGA as a standalone program
 
 Please choose an approach that suits your situation and preferences.
 
 <details><summary><h4><i>Alternative 1: using <code>pipx</code></i></h4></summary>
 
-[Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies from other Python programs on your system, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
+[Pipx](https://github.com/pypa/pipx) lets you install Python programs in a way that isolates Python dependencies from other Python programs on your system, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
+
 ```sh
 pipx install iga
 ```
 
 After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+
 ```shell
 iga --help
 ```
+
 </details>
 
 <details><summary><h4><i>Alternative 2: using <code>pip</code></i></h4></summary>
 
 IGA is available from the [Python package repository PyPI](https://pypi.org) and can be installed using [`pip`](https://pip.pypa.io/en/stable/installing/):
+
 ```sh
 python3 -m pip install iga
 ```
 
 As an alternative to getting it from [PyPI](https://pypi.org), you can install `iga` directly from GitHub:
+
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
 
 After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+
 ```shell
 iga --help
 ```
+
 </details>
 
 <details><summary><h4><i>Alternative 3: from sources</i></h4></summary>
 
 If  you prefer to install IGA directly from the source code, first obtain a copy by either downloading the source archive from the [IGA releases page on GitHub](https://github.com/caltechlibrary/iga/releases), or by using `git` to clone the repository to a location on your computer. For example,
+
 ```sh
 git clone https://github.com/caltechlibrary/iga
 ```
 
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
+
 ```sh
 cd iga
 python3 setup.py install
 ```
+
 </details>
 
 Once you have installed `iga`, the next steps are (1) [get an InvenioRDM token](#getting-an-inveniordm-token) and (2) [configure `iga` for running locally](#configuring-and-running-iga-locally).
 
 
 ### IGA as a GitHub Actions workflow
 
 A [GitHub Actions](https://docs.github.com/en/actions) workflow is an automated process that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
 1. In the main branch of your GitHub repository, create a `.github/workflows` directory
 2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/main/sample-workflow.yml) into it:
+
     ```yaml
     # ╭────────────────────────────────────────────╮
     # │ Configure this section                     │
     # ╰────────────────────────────────────────────╯
 
     env:
       # 👋🏻 Set the next variable to your InvenioRDM server address 👋🏻
@@ -138,124 +227,127 @@
     name: InvenioRDM GitHub Archiver
     on:
       release:
         types: [published]
       workflow_dispatch:
         inputs:
           release_tag:
-            description: "The release tag (empty = latest):"
+            description: The release tag (empty = latest)
           parent_record:
-            description: "ID of parent record (for versioning):"
+            description: ID of parent record (for versioning)
           community:
-            description: "Name of InvenioRDM community (if any):"
+            description: Name of InvenioRDM community (if any)
           draft:
-            description: "Mark the record as a draft"
+            description: Mark the record as a draft
             type: boolean
           all_assets:
-            description: "Attach all GitHub assets"
+            description: Attach all GitHub assets
             type: boolean
           all_metadata:
-            description: "Include additional GitHub metadata"
+            description: Include additional GitHub metadata
             type: boolean
           debug:
-            description: "Print debug info in the GitHub log"
+            description: Print debug info in the GitHub log
             type: boolean
 
     run-name: Archive ${{inputs.release_tag || 'latest release'}} in InvenioRDM
     jobs:
       run_iga:
-        name: "Send to ${{needs.get_repository.outputs.server}}"
+        name: Send to ${{needs.get_repository.outputs.server}}
         runs-on: ubuntu-latest
         needs: get_repository
         steps:
-          - uses: caltechlibrary/iga@main
+          - uses: caltechlibrary/iga@v1
             with:
               INVENIO_SERVER: ${{env.INVENIO_SERVER}}
               INVENIO_TOKEN:  ${{secrets.INVENIO_TOKEN}}
               all_assets:     ${{github.event.inputs.all_assets || env.all_assets}}
               all_metadata:   ${{github.event.inputs.all_metadata || env.all_metadata}}
               debug:          ${{github.event.inputs.debug || env.debug}}
               draft:          ${{github.event.inputs.draft || env.draft}}
               community:      ${{github.event.inputs.community || env.community}}
               parent_record:  ${{github.event.inputs.parent_record || env.parent_record}}
               release_tag:    ${{github.event.inputs.release_tag || 'latest'}}
       get_repository:
-        name: "Get repository name"
+        name: Get repository name
         runs-on: ubuntu-latest
         outputs:
           server: ${{steps.parse.outputs.host}}
         steps:
           - name: Extract name from INVENIO_SERVER
             id: parse
             run: echo "host=$(cut -d'/' -f3 <<< ${{env.INVENIO_SERVER}} | cut -d':' -f1)" >> $GITHUB_OUTPUT
     ```
+
 3. **Edit the value of the `INVENIO_SERVER` variable (line 7 above)** ↑
 4. Optionally, change the values of other options (`parent_record`, `community`, etc.)
 5. Save the file, commit the changes to git, and push your changes to GitHub
 
 Once you have installed the GitHub Action workflow for IGA, the next steps are (1) [get an InvenioRDM token](#getting-an-inveniordm-token) and (2) [configure the GitHub Action workflow](#configuring-and-running-iga-as-a-github-actions-workflow).
 
 
 ## Quick start
 
-No matter whether IGA is run locally on your computer or as a GitHub Actions workflow, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
-is the first step.
+No matter whether IGA is run locally on your computer or as a GitHub Actions workflow, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one is the first step.
 
 ### Getting an InvenioRDM token
 
-<img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" width="60%" align="right">
+<img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" alt="Screenshot of InvenioRDM PAT menu" width="60%" align="right">
 
 1. Log in to your InvenioRDM account
 2. Go to the _Applications_ page in your account profile
 3. Click the <kbd>New token</kbd> button next to "Personal access tokens"
 4. On the page that is shown after you click that button, name your token (the name does not matter) and click the <kbd>Create</kbd> button
 5. After InvenioRDM creates and shows you the token, **copy it to a safe location** because InvenioRDM will not show it again
 
 ### Configuring and running IGA locally
 
 To send a GitHub release to your InvenioRDM server, IGA needs this information:
+
 1. (Required) The identity of the GitHub release to be archived
 2. (Required) The address of the destination InvenioRDM server
 3. (Required) A personal access token for InvenioRDM (from [above](#getting-an-inveniordm-token))
 4. (Optional) A [personal access token for GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
 
 The identity of the GitHub release is always given as an argument to IGA on the command line; the remaining values can be provided either via command-line options or environment variables. One approach is to set environment variables in shell scripts or your interactive shell. Here is an example using Bash shell syntax, with fake token values:
+
 ```shell
 export INVENIO_SERVER=https://data.caltech.edu
 export INVENIO_TOKEN=qKLoOH0KYf4D98PGYQGnC09hiuqw3Y1SZllYnonRVzGJbWz2
 export GITHUB_TOKEN=ghp_wQXp6sy3AsKyyEo4l9esHNxOdo6T34Zsthz
 ```
 
 Once these are set, use of IGA can be as simple as providing a URL for a release in GitHub. For example, the following command creates a draft record (the `-d` option is short for `--draft`) for another project in GitHub and tells IGA to open (the `-o` option is short for `--open`) the newly-created InvenioRDM entry in a web browser:
+
 ```shell
 iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 More options are described in the section on [detailed usage information](#usage) below.
 
 
 ### Configuring and running IGA as a GitHub Actions workflow
 
-After doing the [GitHub Actions installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
+After doing the [GitHub Actions installation](#configuring-and-running-iga-as-a-github-actions-workflow) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
 
-1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" width="85%"></p>
-2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" width="40%"></p>
-3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" width="60%"></p>
+1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" alt="Screenshot of repository tabs in GitHub" width="85%"></p>
+2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" alt="Screenshot of GitHub secrets sidebar item" width="40%"></p>
+3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" alt="Screenshot of GitHub secrets interface" width="60%"></p>
 4. Name the variable `INVENIO_TOKEN` and paste in your InvenioRDM token
 5. Finish by clicking the green <kbd>Add secret</kbd> button
 
 #### Testing the workflow
 
 After setting up the workflow and storing the InvenioRDM token in your repository on GitHub, it's a good idea to run the workflow manually to test that it works as expected.
 
-1. Go to the _Actions_ tab in your repository and click on the name of the workflow in the sidebar on the left<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-run-workflow.png" width="90%"></p>
+1. Go to the _Actions_ tab in your repository and click on the name of the workflow in the sidebar on the left<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-run-workflow.png" alt="Screenshot of GitHub actions workflow list" width="90%"></p>
 2. Click the <kbd>Run workflow</kbd> button in the right-hand side of the blue strip
-3. In the pull-down, change the value of "Mark the record as a draft" to `true`<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-workflow-options-circled.png" width="40%"></p>
+3. In the pull-down, change the value of "Mark the record as a draft" to `true`<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-workflow-options-circled.png" alt="Screenshot of GitHub Actions workflow menu" width="40%"></p>
 4. Click the green <kbd>Run workflow</kbd> button near the bottom
-5. Refresh the web page and a new line will be shown named after your workflow file<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-running-workflow.png" width="90%"></p>
+5. Refresh the web page and a new line will be shown named after your workflow file<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-running-workflow.png" alt="Screenshot of a running workflow in GitHub Actions" width="90%"></p>
 6. Click the title of the workflow to see the IGA workflow progress and results
 
 
 #### Running the workflow when releasing software
 
 Once the personal access token from InvenioRDM is stored as a GitHub secret, the workflow should run automatically every time a new release is made on GitHub &ndash; no further action should be needed. You can check the results (and look for errors if something went wrong) by going to the _Actions_ tab in your GitHub repository.
 
@@ -272,52 +364,58 @@
 
 A personal access token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
-It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some public repositories IGA will not hit the limit. However, if you are archiving a private repository, run IGA multiple times in a row, or the repository has many contributors, then you will need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some public repositories IGA will not hit the limit. However, if you are archiving a private repository, run IGA multiple times in a row, or the repository has many contributors, then you will need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit [https://docs.github.com/en/authentication](https://docs.github.com/en/authentication) and follow the instructions for creating a "classic" personal access token.
 
 Note that when you run IGA as a GitHub Actions workflow, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Actions workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
- 1. The full URL of the web page on GitHub of a tagged release. In this case,
+
+1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
- 2. A combination of _account name_, _repository name_, and _tag_. In this
+2. A combination of _account name_, _repository name_, and _tag_. In this
     case, the final argument on the command line must be the _tag_, and in
     addition, values for the options `--account` and `--repo` must be provided.
 
 Here's an example using approach #1 (assuming environment variables `INVENIO_SERVER`, `INVENIO_TOKEN`, and `GITHUB_TOKEN` have all been set):
+
 ```shell
 iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
+
 and here's the equivalent using approach #2:
+
 ```shell
 iga --github-account mhucka --github-repo taupe v1.2.0
 ```
+
 Note that when using this form of the command, the release tag (`v1.2.0` above) must be the last item given on the command line.
 
 ### Gathering metadata for an InvenioRDM record
 
 The record created in InvenioRDM is constructed using information obtained using GitHub's API as well as several other APIs as needed. The information includes the following:
- * (if one exists) a `codemeta.json` file in the GitHub repository
- * (if one exists) a `CITATION.cff` file in the GitHub repository
- * data available from GitHub for the release
- * data available from GitHub for the repository
- * data available from GitHub for the account of the owner
- * data available from GitHub for the accounts of repository contributors
- * file assets associated with the GitHub release
- * data available from ORCID.org for ORCID identifiers
- * data available from ROR.org for Research Organization Registry identifiers
- * data available from DOI.org, NCBI, Google Books, & others for publications
- * data available from spdx.org for software licenses
+
+* (if one exists) a `codemeta.json` file in the GitHub repository
+* (if one exists) a `CITATION.cff` file in the GitHub repository
+* data available from GitHub for the release
+* data available from GitHub for the repository
+* data available from GitHub for the account of the owner
+* data available from GitHub for the accounts of repository contributors
+* file assets associated with the GitHub release
+* data available from ORCID.org for ORCID identifiers
+* data available from ROR.org for Research Organization Registry identifiers
+* data available from DOI.org, NCBI, Google Books, & others for publications
+* data available from spdx.org for software licenses
 
 IGA tries to use [`CodeMeta.json`](https://codemeta.github.io) first and [`CITATION.cff`](https://citation-file-format.github.io) second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
 
 To override the auto-created metadata, use the option `--read-metadata` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-metadata` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
 
 ### Specifying GitHub file assets
 
@@ -334,15 +432,16 @@
 ### Indicating draft versus published records
 
 If the `--community` option is not used, then by default, IGA will finalize and publish the record. To make it stop short and leave the record as a draft instead, use the option `--draft`. The draft option also takes precedence over the community option: if you use both `--draft` and `--community`, IGA will stop after creating the draft record and will _not_ submit it to the community.  (You can nevertheless submit the record to a community manually once the draft is created, by visiting the record's web page and using the InvenioRDM interface there.)
 
 ### Versioning records
 
 The option `--parent-record` can be used to indicate that the record being constructed is a new version of an existing record. This will make IGA use the InvenioRDM API for [record versioning](https://inveniordm.docs.cern.ch/releases/versions/version-v2.0.0/#versioning-support). The newly-created record will be linked to a parent record identified by the value passed to `--parent-record`. The value must be either an InvenioRDM record identifier (which is a sequence of alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`, generated by the InvenioRDM server), or a URL to the landing page of the record in the InvenioRDM server. (Note that such URLs end in the record identifier.) Here is an example of using this option:
-```
+
+```shell
 iga --parent-record xbcd4-efgh5 https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 ### Other options recognized by IGA
 
 Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
@@ -362,23 +461,23 @@
 
 As explain above, IGA takes one required argument on the command line: either (1) the full URL of a web page on GitHub of a tagged release, or (2) a release tag name which is to be used in combination with options `--github-account` and `--github-repo`. The following table summarizes all the command line options available.
 
 | Long&nbsp;form&nbsp;option&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Short&nbsp;&nbsp; | Meaning | Default |  |
 |------------------------|----------|--------------------------------------|---------|---|
 | `--all-assets`         | `-A`     | Attach all GitHub assets | Attach only the release source ZIP| |
 | `--all-metadata`       | `-M`     | Include additional metadata from GitHub | Favor CodeMeta & CFF | |
-| `--community` _C_      | `-c` _C_ | Submit record to RDM community _C_ | Don't submit record to any community | | 
+| `--community` _C_      | `-c` _C_ | Submit record to RDM community _C_ | Don't submit record to any community | |
 | `--draft`              | `-d`     | Mark the RDM record as a draft | Publish record when done | |
 | `--file` _F_           | `-f` _F_ | Upload local file _F_ instead of GitHub assets | Upload only GitHub assets | ⚑ |
-| `--github-account` _A_ | `-a` _A_ | Look in GitHub account _A_ | Get account name from release URL | ✯ | 
+| `--github-account` _A_ | `-a` _A_ | Look in GitHub account _A_ | Get account name from release URL | ✯ |
 | `--github-repo` _R_    | `-r` _R_ | Look in GitHub repository _R_ of account _A_ | Get repo name from release URL | ✯ |
 | `--github-token` _T_   | `-t` _T_ | Use GitHub access token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
-| `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
-| `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
+| `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | |
+| `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | |
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
 | `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
 | `--print-doi`          | `-i`     | Print both the DOI & record URL when done | Print only the record URL | |
 | `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
@@ -402,18 +501,47 @@
 | 2    | encountered a bad or missing value for an option         |
 | 3    | encountered a problem with a file or directory           |
 | 4    | encountered a problem interacting with GitHub            |
 | 5    | encountered a problem interacting with InvenioRDM        |
 | 6    | the personal access token was rejected                   |
 | 7    | an exception or fatal error occurred                     |
 
+### Adding a DOI badge to your GitHub repository
+
+Once you have set up the IGA workflow in your GitHub repository, you may wish to add a DOI badge to your repository's README file. It would be a chore to keep updating the DOI value in this badge every time a new release is made, and thankfully, it's not necessary: it's possible to make the badge get the current DOI value dynamically. Here is how:
+
+1. _After_ you have at least one release archived in your InvenioRDM server, find out the DOI of that release in InvenioRDM, and extract the tail end of that DOI. The DOI assigned by InvenioRDM will be a string such as `10.22002/zsmem-2pg20`; the tail end is the `zsmem-2pg20` part. (Your DOI and tail portion will be different.)
+2. Let <i><b><code>SERVERURL</code></b></i> stand for the URL for your InvenioRDM server, and let <i><b><code>IDENTIFIER</code></b></i> stand for the identifier portion of the DOI. In your `README.md` file, write the DOI badge as follows (without line breaks):
+
+    <pre><code>[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&query=$.pids.doi.identifier&uri=<i><b><code>SERVERURL</code></b></i>/api/records/<i><b><code>IDENTIFIER</code></b></i>/versions/latest)](<i><b><code>SERVERURL</code></b></i>/records/<i><b><code>IDENTIFIER</code></b></i>/latest)</code></pre>
+
+For example, for CaltechDATA and the archived IGA releases there,
+
+* <i><b><code>SERVERURL</code></b></i> = `http://data.caltech.edu`
+* <i><b><code>IDENTIFIER</code></b></i> = `zsmem-2pg20`
+
+which leads to the following badge string for IGA's `README.md` file:
+
+```txt
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20/versions/latest)](https://data.caltech.edu/records/zsmem-2pg20/latest)
+```
+
+<br>The result looks like this: <div align="center">
+
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20/versions/latest)](https://data.caltech.edu/records/zsmem-2pg20/latest)
+
+</div>
+
+You can change the look of the badge by using style parameters. Please refer to the [Shields.io](https://shields.io/badges/static-badge) documentation for static badges.
+
 
 ## Known issues and limitations
 
 The following are known issues and limitations.
+
 * As of mid-2023, InvenioRDM requires names of record creators and other contributors to be split into given (first) and family (surname). This is problematic for multiple reasons. The first is that mononyms are common in many countries: a person's name may legitimately be only a single word which is not conceptually a "given" or "family" name.  To compound the difficulty for IGA, names are stored as single fields in GitHub account metadata, so unless a repository has a `codemeta.json` or `CITATION.cff` file (which allow authors more control over how they want their names represented), IGA is forced to try to split the single GitHub name string into two parts. _A foolproof algorithm for doing this does not exist_, so IGA will sometimes get it wrong. (That said, IGA goes to extraordinary lengths to try to do a good job.)
 * InvenioRDM requires that identities (creators, contributors, etc.) to be labeled as personal or organizational. The nature of identities is usually made clear in `codemeta.json` and `CITATION.cff` files. GitHub also provides a flag that is meant to be used to label organizational accounts, but sometimes people don't set the GitHub account information correctly. Consequently, if IGA has to use GitHub data to get (e.g.) the list of contributors on a project, it may mislabel identities in the InvenioRDM record it produces.
 * Some accounts on GitHub are software automation or "bot" accounts, but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub, so if they're not labeled as bot or organizational accounts in GitHub, IGA can't recognize that they're humans. If such an account is the creator of a release in GitHub, and IGA tries to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI".
 * Funder and funding information can only be specified in `codemeta.json` files; neither GitHub nor `CITATION.cff` have provisions to store this kind of metadata. The CodeMeta specification defines two fields for this purpose: `funder` and `funding`. Unfortunately, these map imperfectly to the requirements of InvenioRDM's metadata format. In addition, people don't always follow the CodeMeta guidelines, and sometimes they write funding information as text strings (instead of structured objects), the interpretation of which would require software that can recognize grant and funding agency information from free-text descriptions. This combination of factors means IGA often can't fill in the funding metadata in InvenioRDM records even if there is some funding information in the `codemeta.json` file.
 
 
 ## Getting help
@@ -424,48 +552,51 @@
 ## Contributing
 
 Your help and participation in enhancing IGA is welcome!  Please visit the [guidelines for contributing](CONTRIBUTING.md) for some tips on getting started.
 
 
 ## License
 
-Software produced by the Caltech Library is Copyright © 2023 California Institute of Technology.  This software is freely distributed under a BSD-style license.  Please see the [LICENSE](LICENSE) file for more information.
+Software produced by the Caltech Library is Copyright © 2022–2024 California Institute of Technology.  This software is freely distributed under a BSD-style license.  Please see the [LICENSE](LICENSE) file for more information.
 
 ## Acknowledgments
 
 This work was funded by the California Institute of Technology Library.
 
 IGA uses multiple other open-source packages, without which it would have taken much longer to write the software. I want to acknowledge this debt. In alphabetical order, the packages are:
+
 * [Aenum](https://github.com/ethanfurman/aenum) &ndash; package for advanced enumerations
 * [Arrow](https://pypi.org/project/arrow/) &ndash; a library for creating & manipulating dates
 * [Boltons](https://github.com/mahmoud/boltons/) &ndash; package of miscellaneous Python utilities
 * [caltechdata_api](https://github.com/caltechlibrary/caltechdata_api) &ndash; package for using the CaltechDATA API
 * [CommonPy](https://github.com/caltechlibrary/commonpy) &ndash; a collection of commonly-useful Python functions
-* [demoji](https://github.com/bsolomon1124/demoji) &ndash; find or remove emojis from text
 * [dirtyjson](https://github.com/codecobblers/dirtyjson) &ndash; JSON decoder that copes with problematic JSON files and reports useful error messages
 * [flake8](https://github.com/pycqa/flake8) &ndash; Python code linter and style analyzer
+* [Ginza](https://github.com/megagonlabs/ginza) &ndash; Japanese NLP Library
 * [httpx](https://www.python-httpx.org) &ndash; HTTP client library that supports HTTP/2
 * [humanize](https://github.com/jmoiron/humanize) &ndash; make numbers more easily readable by humans
 * [idutils](https://github.com/inveniosoftware/idutils) &ndash; package for validating and normalizing various kinds of persistent identifiers
 * [ipdb](https://github.com/gotcha/ipdb) &ndash; the IPython debugger
 * [iptools](https://github.com/bd808/python-iptools) &ndash; utilities for dealing with IP addresses
 * [isbnlib](https://github.com/xlcnd/isbnlib) &ndash; utilities for dealing with ISBNs
+* [Jamo](https://github.com/JDongian/python-jamo) &ndash; Hangul character analysis
 * [json5](https://github.com/dpranke/pyjson5) &ndash; extended JSON format parser
 * [latexcodec](https://github.com/mcmtroffaes/latexcodec) &ndash; lexer and codec to work with LaTeX code in Python
+* [Lingua](https://github.com/pemistahl/lingua) &ndash; language detection library
 * [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) &ndash; a link recognition library with full unicode support
 * [lxml](https://lxml.de) &ndash; an XML parsing library
 * [Markdown](https://python-markdown.github.io) &ndash; Python package for working with Markdown
 * [markdown-checklist](https://github.com/FND/markdown-checklist) &ndash; GitHub-style checklist extension for Python Markdown package
 * [mdx-breakless-lists](https://github.com/adamb70/mdx-breakless-lists) &ndash; GitHub-style Markdown lists that don't require a line break above them
 * [mdx_linkify](https://github.com/daGrevis/mdx_linkify) &ndash; extension for Python Markdown will convert text that look like links to HTML anchors
 * [MyST-parser](https://github.com/executablebooks/MyST-Parser) &ndash; A Sphinx and Docutils extension to parse an extended version of Markdown
 * [nameparser](https://github.com/derek73/python-nameparser) &ndash; package for parsing human names into their individual components
 * [probablepeople](https://github.com/datamade/probablepeople) &ndash; package for parsing names into components using ML-based techniques
 * [pybtex](https://pybtex.org) &ndash; BibTeX parser and formatter
-* [pybtex-apa7-style]() &ndash; plugin for [pybtex](https://pybtex.org) that provides APA7 style formatting
+* [pybtex-apa7-style](https://pypi.org/project/pybtex-apa7-style/) &ndash; plugin for [pybtex](https://pybtex.org) that provides APA7 style formatting
 * [pymdown-extensions](https://github.com/facelessuser/pymdown-extensions) &ndash; extensions for Python Markdown
 * [pytest](https://docs.pytest.org/en/stable/) &ndash; testing framework
 * [pytest-cov](https://github.com/pytest-dev/pytest-cov) &ndash; coverage reports for use with `pytest`
 * [pytest-mock](https://pypi.org/project/pytest-mock/) &ndash; wrapper around the `mock` package for use with `pytest`
 * [PyYAML](https://pyyaml.org) &ndash; YAML parser
 * [Rich](https://github.com/Textualize/rich) &ndash; library for writing styled text to the terminal
 * [rich-click](https://github.com/ewels/rich-click) &ndash; CLI interface built on top of [Rich](https://github.com/Textualize/rich)
@@ -486,10 +617,10 @@
 * [url-normalize](https://github.com/niksite/url-normalize) &ndash; URI/URL normalization utilities
 * [validators](https://github.com/kvesteri/validators) &ndash; data validation package for Python
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
-    <img width="100" height="100" src="https://github.com/caltechlibrary/iga/raw/main/.graphics/caltech-round.png">
+    <img width="100" height="100" alt="Caltech logo" src="https://github.com/caltechlibrary/iga/raw/main/.graphics/caltech-round.png">
   </a>
 </div>
```

### Comparing `iga-1.2.2/iga/__init__.py` & `iga-1.3.0/iga/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 '''
 __init__.py for iga
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2022-2023 by the California Institute of Technology.  This code
+Copyright (c) 2022-2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 # Package metadata
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  │    The following values are automatically updated at every release    │
 #  │    by the Makefile. Manual changes to these values will be lost.      │
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '1.2.2'
+__version__     = '1.3.0'
 __description__ = 'The InvenioRDM GitHub Archiver (IGA) automatically archives GitHub releases in an InvenioRDM repository.'
 __url__         = 'https://caltechlibrary.github.io/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'mhucka@caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-1.2.2/iga/__main__.py` & `iga-1.3.0/iga/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 __main__.py: main entry point for IGA.
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2022-2023 by the California Institute of Technology.  This code
+Copyright (c) 2022-2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 import sys
 if sys.version_info <= (3, 9):
     print('IGA requires Python version 3.9 or higher,')
```

### Comparing `iga-1.2.2/iga/cli.py` & `iga-1.3.0/iga/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 '''
 cli.py: command-line interface for IGA
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2022-2023 by the California Institute of Technology.  This code
+Copyright (c) 2022-2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 import bdb
 import os
 import rich
 from   rich.console import Console
 from   rich.style import Style
 import rich_click as click
 from   rich_click import File, Path, INT, Choice
 import sys
 from   sidetrack import set_debug, log
 
+from iga import __version__
 from iga.exit_codes import ExitCode
 from iga.exceptions import GitHubError, InvenioRDMError, RecordNotFound
 from iga.github import (
     github_account_repo_tag,
     github_release,
     github_release_assets,
     valid_github_release_url,
 )
-from iga.id_utils import is_invenio_rdm
+from iga.id_utils import is_inveniordm_id
 from iga.invenio import (
     invenio_api_available,
     invenio_communities,
     invenio_community_send,
     invenio_create,
     invenio_publish,
     invenio_server_name,
@@ -103,14 +104,15 @@
     If CLI argument value is None, the environment variable env_var is checked
     and if it has a value, it's returned; otherwise, this function prints an
     error message and exits with a status code signifying "bad argument".
 
     If the value is "help", this function prints help text and causes the
     program to exit.
     '''
+    log(f'>>> This is IGA version {__version__} <<<')
     if ctx.params.get('url_or_tag') == 'help':
         _print_help_and_exit(ctx)
     elif value:
         log(f'using CLI option "--{param.name} {value}" for the {thing}')
         os.environ[env_var] = str(value).strip()
     elif env_var in os.environ:
         log(f"using value of environment variable {env_var} as the {thing}")
@@ -662,15 +664,15 @@
 
     if community and community not in invenio_communities():
         _alert(ctx, f'"{community}" is not the name of a known community in'
                ' the InvenioRDM server. The known communities can be obtained'
                ' by using the option `--list-communities`.')
         sys.exit(int(ExitCode.file_error))
 
-    if parent_id and not is_invenio_rdm(parent_id):
+    if parent_id and not is_inveniordm_id(parent_id):
         _alert(ctx, f'"{parent_id}" does not appear to be an InvenioRDM'
                ' record identifier.')
         sys.exit(int(ExitCode.file_error))
 
 
     # Do the main work ........................................................
 
@@ -711,15 +713,16 @@
 
             _inform('Attaching assets:')
             for item in files_to_upload or github_assets:
                 invenio_upload(record, item, _print_text)
 
             if draft:
                 _inform(f'The draft record is available at {record.draft_url}')
-            elif community:
+            elif community and not parent_id:
+                # Record versions (when we have a parent_id) do not go through review workflow
                 invenio_community_send(record, community)
                 _inform(f'The record has been submitted to community "{community}"'
                         f' and the draft is available at {record.draft_url}')
             else:
                 invenio_publish(record)
                 _inform(f'The published record is available at {record.record_url}')
                 if print_doi and record.doi:
```

### Comparing `iga-1.2.2/iga/data_utils.py` & `iga-1.3.0/iga/data_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 data_utils.py: miscellaneous data-handling utilities.
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2023 by the California Institute of Technology.  This code
+Copyright (c) 2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 from typing import Generator, Iterator
 from url_normalize import url_normalize
 
@@ -78,7 +78,12 @@
         or url1.replace('http://', 'https://') == url2
         or url1.replace('https://', 'http://') == url2
         or url1.replace('http://', 'https://').removesuffix('/') == url2
         or url1.replace('http://', 'https://') == url2.removesuffix('/')
         or url1.replace('https://', 'http://').removesuffix('/') == url2
         or url1.replace('https://', 'http://') == url2.removesuffix('/')
     )
+
+
+def constant_factory(value):
+    '''Helper for use with defaultdict to set a default value.'''
+    return lambda: value
```

### Comparing `iga-1.2.2/iga/doi.py` & `iga-1.3.0/iga/doi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 doi.py: module for fetching information using DOIs
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2023 by the California Institute of Technology.  This code
+Copyright (c) 2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 import commonpy.exceptions
 from   commonpy.network_utils import network
 from   contextlib import suppress
```

### Comparing `iga-1.2.2/iga/exceptions.py` & `iga-1.3.0/iga/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 exceptions.py: exceptions for IGA
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2022-2023 by the California Institute of Technology.  This code
+Copyright (c) 2022-2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 
 # Base class.
 # .............................................................................
```

### Comparing `iga-1.2.2/iga/exit_codes.py` & `iga-1.3.0/iga/exit_codes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 exit_codes.py: define exit codes for program return values
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2022-2023 by the California Institute of Technology.  This code
+Copyright (c) 2022-2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 from aenum import Enum, MultiValue
```

### Comparing `iga-1.2.2/iga/github.py` & `iga-1.3.0/iga/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 github.py: IGA module for interacting with GitHub
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2022-2023 by the California Institute of Technology.  This code
+Copyright (c) 2022-2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 import commonpy.exceptions
 from   commonpy.network_utils import net
 import contextlib
```

### Comparing `iga-1.2.2/iga/id_utils.py` & `iga-1.3.0/iga/id_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 id_utils.py: utilities for dealing with identifiers
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2023 by the California Institute of Technology.  This code
+Copyright (c) 2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 from idutils import (
     detect_identifier_schemes,
     is_pmid,
@@ -30,15 +30,15 @@
 # Douglas Crockford base 32 (https://github.com/inveniosoftware/base32-lib),
 # which means 0-9 and letters except for i, l, o, and u.
 
 rdm_regex = re.compile(r'([abcdefghjkmnpqrstvwxyz0-9]{5}-[abcdefghjkmnpqrstvwxyz0-9]{5})')
 '''Matches an InvenioRDM record id.'''
 
 
-def is_invenio_rdm(val):
+def is_inveniordm_id(val):
     '''Return True if the given string is an InvenioRDM record identifier.'''
     return bool(normalize_invenio_rdm(val))
 
 
 def normalize_invenio_rdm(val):
     '''Normalize an InvenioRDM record identifier.
 
@@ -156,15 +156,15 @@
         return RECOGNIZED_SCHEMES[scheme](text)
     return ''
 
 
 def recognized_scheme(text):
     # We allow URLs that contain InvenioRDM identifiers. They're URLs & would
     # be reported as 'url' by detect_identifier_schemes, so test this case 1st.
-    if is_invenio_rdm(text):
+    if is_inveniordm_id(text):
         return 'rdm'
     for scheme in detect_identifier_schemes(text):
         if scheme in RECOGNIZED_SCHEMES:
             return scheme
     else:
         # Special case not handled well by idutils. PMID's are a particular
         # PITA b/c they're integers & cause false-positives for other things.
```

### Comparing `iga-1.2.2/iga/invenio.py` & `iga-1.3.0/iga/invenio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 invenio.py: Code for interacting with InvenioRDM
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2022-2023 by the California Institute of Technology.  This code
+Copyright (c) 2022-2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 from   commonpy.network_utils import net, network, netloc
 from   commonpy.data_utils import pluralized
 import commonpy.exceptions
@@ -126,14 +126,19 @@
         # If the next one can't reach the host, it'll throw an exception.
         socket.socket(socket.AF_INET, socket.SOCK_STREAM).connect((server_host, 443))
         # If we can reach the host, check that it responds to the API endpoint.
         if response := network('get', server_url + endpoint):
             log(f'we can reach {server_url} and it responds to {endpoint}')
             data = response.json()
             record = data.get('hits', {}).get('hits', {})[0]
+            if publisher := record.get('metadata', {}).get('publisher'):
+                return publisher
+            else:
+                # Fall back to the host name.
+                return server_host
             return record['metadata']['publisher']
     except KeyboardInterrupt:
         raise
     except socket.error:
         log(f'{server_url} did not respond')
         return None
     except json.decoder.JSONDecodeError:
```

### Comparing `iga-1.2.2/iga/json_utils.py` & `iga-1.3.0/iga/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 json_utils.py: utilities for working with JSON
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2023 by the California Institute of Technology.  This code
+Copyright (c) 2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 import dirtyjson
 from   sidetrack import log
```

### Comparing `iga-1.2.2/iga/licenses.py` & `iga-1.3.0/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/iga/metadata.py` & `iga-1.3.0/iga/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   cover the whole key set of CodeMeta at some point), and more "detailed" in
   terms of citation metadata."
 
 Since the use of InvenioRDM is more about archiving repository code than about
 citing software, the code below looks for and uses codemeta.json first,
 followed by CITATION.cff if a CodeMeta file can't be found.
 
-Copyright (c) 2022-2023 by the California Institute of Technology.  This code
+Copyright (c) 2022-2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 import arrow
 from   commonpy.data_structures import CaseFoldSet, CaseFoldDict
 from   commonpy.data_utils import pluralized
@@ -1220,14 +1220,19 @@
 #   3. affiliations (optional, dict, only if type is "personal")
 #       a. id OR name
 #
 # Note that for people, we MUST produce names split into given + family names
 # or InvenioRDM will reject the record.
 
 def _entity(data, role=None):
+    '''Try to extract person or org from the given data object.
+    The "data" can be either a dict or a string. (When data comes from a
+    CodeMeta field or CITATION.cff file, it will be a dict; it comes from
+    elsewhere, it is more likely to be a string.)
+    '''
     if isinstance(data, dict):          # Correct data type.
         return _entity_from_dict(data, role)
     elif isinstance(data, str):         # Wrong data type, but we try anyway.
         return _entity_from_string(data, role)
     else:                               # If we get here, it's beyond us.
         log('entity value is neither a string nor a dict -- giving up')
         return {}
@@ -1263,15 +1268,17 @@
         if name:
             result = {'person_or_org': {'name': name,
                                         'type': 'organizational'}}
     elif account := _parsed_github_account(data):
         # It's the name of an account in GitHub.
         result = _identity_from_github(account)
     else:
-        # We're getting into expensive heuristic guesswork now.
+        # We have to parse a single string to guess whether it's the name of
+        # a person or org, and if a person, to split the string into family
+        # and give name. We're getting into expensive heuristic guesswork now.
         from iga.name_utils import is_person
         if is_person(data):
             (given, family) = split_name(data)
             if family or given:
                 result = {'person_or_org': {'family_name': flattened_name(family),
                                             'given_name': flattened_name(given),
                                             'type': 'personal'}}
```

### Comparing `iga-1.2.2/iga/orcid.py` & `iga-1.3.0/iga/orcid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 orcid.py: simple functions for interfacing to ORCID
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2023 by the California Institute of Technology.  This code
+Copyright (c) 2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 import commonpy.exceptions
 from   commonpy.network_utils import network
 from   functools import cache
```

### Comparing `iga-1.2.2/iga/reference.py` & `iga-1.3.0/iga/reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 reference.py: create a formatted reference for a given publication.
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2023 by the California Institute of Technology.  This code
+Copyright (c) 2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 from   commonpy.network_utils import network
 import commonpy.exceptions
 import json
```

### Comparing `iga-1.2.2/iga/ror.py` & `iga-1.3.0/iga/ror.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 ror.py: utilities for getting information from ROR
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2023 by the California Institute of Technology.  This code
+Copyright (c) 2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 import commonpy.exceptions
 from   commonpy.network_utils import network
 from   functools import cache
```

### Comparing `iga-1.2.2/iga/text_utils.py` & `iga-1.3.0/iga/text_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 text_utils.py: misc. utilities for doing stuff with text
 
 This file is part of https://github.com/caltechlibrary/iga/.
 
-Copyright (c) 2023 by the California Institute of Technology.  This code
+Copyright (c) 2024 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
 
 def cleaned_text(text):
     '''Return text that has been mildly cleaned up.
```

### Comparing `iga-1.2.2/iga.egg-info/PKG-INFO` & `iga-1.3.0/iga.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 1.2.2
+Version: 1.3.0
 Summary: The InvenioRDM GitHub Archiver (IGA) automatically archives GitHub releases in an InvenioRDM repository.
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -18,56 +18,109 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aenum==3.1.15
+Requires-Dist: arrow==1.3.0
+Requires-Dist: boltons==21.0.0
+Requires-Dist: caltechdata-api==1.6.1
+Requires-Dist: commonpy==1.13.0
+Requires-Dist: dirtyjson==1.0.8
+Requires-Dist: ginza==5.2.0
+Requires-Dist: ja_ginza_electra==5.2.0
+Requires-Dist: httpx==0.23.1
+Requires-Dist: humanize==4.9.0
+Requires-Dist: idutils==1.2.1
+Requires-Dist: iptools==0.7.0
+Requires-Dist: isbnlib==3.10.14
+Requires-Dist: jamo==0.4.1
+Requires-Dist: json5==0.9.25
+Requires-Dist: latexcodec==3.0.0
+Requires-Dist: lingua-language-detector==2.0.2
+Requires-Dist: lxml==5.2.2
+Requires-Dist: Markdown==3.6
+Requires-Dist: markdown-checklist==0.4.4
+Requires-Dist: mdx-breakless-lists==1.0.1
+Requires-Dist: mdx_linkify==2.1
+Requires-Dist: nameparser==1.1.3
+Requires-Dist: probablepeople==0.5.5
+Requires-Dist: pybtex==0.24.0
+Requires-Dist: pybtex-apa7-style==0.1.3
+Requires-Dist: pymdown-extensions==10.8.1
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: regex==2022.3.2
+Requires-Dist: rich-click==1.8.2
+Requires-Dist: sidetrack==2.0.1
+Requires-Dist: spacy==3.7.4
+Requires-Dist: spacy-alignments==0.9.1
+Requires-Dist: spacy-curated-transformers==0.2.2
+Requires-Dist: spacy-legacy==3.0.12
+Requires-Dist: spacy-loggers==1.0.5
+Requires-Dist: spacy-pkuseg==0.0.33
+Requires-Dist: spacy-transformers==1.1.9
+Requires-Dist: StringDist==1.0.9
+Requires-Dist: url-normalize==1.4.3
+Requires-Dist: validators==0.28.1
 
-# IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
+# IGA<img alt="IGA logo" width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
-IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/inveniordm-github-archiver) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
-[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
-[![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
-[![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
-[![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20)](https://data.caltech.edu/records/zsmem-2pg20)
+[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases) [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/blob/develop/LICENSE) [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/) [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/) [![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20/versions/latest)](https://data.caltech.edu/records/zsmem-2pg20/latest)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
+  * [IGA as a standalone program](#iga-as-a-standalone-program)
+  * [IGA as a GitHub Actions workflow](#iga-as-a-github-actions-workflow)
 * [Quick start](#quick-start)
 * [Usage](#usage)
+  * [Identifying the InvenioRDM server](#identifying-the-inveniordm-server)
+  * [Providing an InvenioRDM access token](#providing-an-inveniordm-access-token)
+  * [Providing a GitHub access token](#providing-a-github-access-token)
+  * [Specifying a GitHub release](#specifying-a-github-release)
+  * [Gathering metadata for an InvenioRDM record](#gathering-metadata-for-an-inveniordm-record)
+  * [Specifying GitHub file assets](#specifying-github-file-assets)
+  * [Handling communities](#handling-communities)
+  * [Indicating draft versus published records](#indicating-draft-versus-published-records)
+  * [Versioning records](#versioning-records)
+  * [Other options recognized by IGA](#other-options-recognized-by-iga)
+  * [Summary of command-line options](#summary-of-command-line-options)
+  * [Return values](#return-values)
+  * [Adding a DOI badge to your GitHub repository](#adding-a-doi-badge-to-your-github-repository)
 * [Known issues and limitations](#known-issues-and-limitations)
 * [Getting help](#getting-help)
 * [Contributing](#contributing)
 * [License](#license)
-* [Acknowledgments](#authors-and-acknowledgments)
+* [Acknowledgments](#acknowledgments)
 
 
 ## Introduction
 
 [InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and data sets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the [_InvenioRDM GitHub Archiver_](https://github.com/caltechlibrary/iga) (IGA) comes in.
 
 IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Actions](https://docs.github.com/en/actions) workflow to archive GitHub releases automatically for a repository each time they are made.
 
 <p align=center>
-<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" alt="Screenshot of a software release in GitHub" width="40%">
 <span style="font-size: 150%">➜</span>
-<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" alt="Screenshot of the corresponding entry in InvenioRDM" width="40%">
 </p>
 
 IGA offers many notable features:
+
 * Automatic metadata extraction from GitHub plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
 * Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
 * Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org), [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
-* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google, and other sources
+* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), Google, and other sources
 * Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
 * Automatic lookup of human names in [ORCID.org](https://orcid.org) (assuming ORCID id's are provided)
 * Automatic splitting of human names into family & given names using [ML](https://en.wikipedia.org/wiki/Machine_learning) methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
 * Support for overriding the record that IGA creates, for complete control if you need it
 * Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
 * Extensive use of logging so you can see what's going on under the hood
@@ -79,68 +132,79 @@
 
 ### IGA as a standalone program
 
 Please choose an approach that suits your situation and preferences.
 
 <details><summary><h4><i>Alternative 1: using <code>pipx</code></i></h4></summary>
 
-[Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies from other Python programs on your system, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
+[Pipx](https://github.com/pypa/pipx) lets you install Python programs in a way that isolates Python dependencies from other Python programs on your system, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
+
 ```sh
 pipx install iga
 ```
 
 After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+
 ```shell
 iga --help
 ```
+
 </details>
 
 <details><summary><h4><i>Alternative 2: using <code>pip</code></i></h4></summary>
 
 IGA is available from the [Python package repository PyPI](https://pypi.org) and can be installed using [`pip`](https://pip.pypa.io/en/stable/installing/):
+
 ```sh
 python3 -m pip install iga
 ```
 
 As an alternative to getting it from [PyPI](https://pypi.org), you can install `iga` directly from GitHub:
+
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
 
 After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+
 ```shell
 iga --help
 ```
+
 </details>
 
 <details><summary><h4><i>Alternative 3: from sources</i></h4></summary>
 
 If  you prefer to install IGA directly from the source code, first obtain a copy by either downloading the source archive from the [IGA releases page on GitHub](https://github.com/caltechlibrary/iga/releases), or by using `git` to clone the repository to a location on your computer. For example,
+
 ```sh
 git clone https://github.com/caltechlibrary/iga
 ```
 
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
+
 ```sh
 cd iga
 python3 setup.py install
 ```
+
 </details>
 
 Once you have installed `iga`, the next steps are (1) [get an InvenioRDM token](#getting-an-inveniordm-token) and (2) [configure `iga` for running locally](#configuring-and-running-iga-locally).
 
 
 ### IGA as a GitHub Actions workflow
 
 A [GitHub Actions](https://docs.github.com/en/actions) workflow is an automated process that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
 1. In the main branch of your GitHub repository, create a `.github/workflows` directory
 2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/main/sample-workflow.yml) into it:
+
     ```yaml
     # ╭────────────────────────────────────────────╮
     # │ Configure this section                     │
     # ╰────────────────────────────────────────────╯
 
     env:
       # 👋🏻 Set the next variable to your InvenioRDM server address 👋🏻
@@ -163,124 +227,127 @@
     name: InvenioRDM GitHub Archiver
     on:
       release:
         types: [published]
       workflow_dispatch:
         inputs:
           release_tag:
-            description: "The release tag (empty = latest):"
+            description: The release tag (empty = latest)
           parent_record:
-            description: "ID of parent record (for versioning):"
+            description: ID of parent record (for versioning)
           community:
-            description: "Name of InvenioRDM community (if any):"
+            description: Name of InvenioRDM community (if any)
           draft:
-            description: "Mark the record as a draft"
+            description: Mark the record as a draft
             type: boolean
           all_assets:
-            description: "Attach all GitHub assets"
+            description: Attach all GitHub assets
             type: boolean
           all_metadata:
-            description: "Include additional GitHub metadata"
+            description: Include additional GitHub metadata
             type: boolean
           debug:
-            description: "Print debug info in the GitHub log"
+            description: Print debug info in the GitHub log
             type: boolean
 
     run-name: Archive ${{inputs.release_tag || 'latest release'}} in InvenioRDM
     jobs:
       run_iga:
-        name: "Send to ${{needs.get_repository.outputs.server}}"
+        name: Send to ${{needs.get_repository.outputs.server}}
         runs-on: ubuntu-latest
         needs: get_repository
         steps:
-          - uses: caltechlibrary/iga@main
+          - uses: caltechlibrary/iga@v1
             with:
               INVENIO_SERVER: ${{env.INVENIO_SERVER}}
               INVENIO_TOKEN:  ${{secrets.INVENIO_TOKEN}}
               all_assets:     ${{github.event.inputs.all_assets || env.all_assets}}
               all_metadata:   ${{github.event.inputs.all_metadata || env.all_metadata}}
               debug:          ${{github.event.inputs.debug || env.debug}}
               draft:          ${{github.event.inputs.draft || env.draft}}
               community:      ${{github.event.inputs.community || env.community}}
               parent_record:  ${{github.event.inputs.parent_record || env.parent_record}}
               release_tag:    ${{github.event.inputs.release_tag || 'latest'}}
       get_repository:
-        name: "Get repository name"
+        name: Get repository name
         runs-on: ubuntu-latest
         outputs:
           server: ${{steps.parse.outputs.host}}
         steps:
           - name: Extract name from INVENIO_SERVER
             id: parse
             run: echo "host=$(cut -d'/' -f3 <<< ${{env.INVENIO_SERVER}} | cut -d':' -f1)" >> $GITHUB_OUTPUT
     ```
+
 3. **Edit the value of the `INVENIO_SERVER` variable (line 7 above)** ↑
 4. Optionally, change the values of other options (`parent_record`, `community`, etc.)
 5. Save the file, commit the changes to git, and push your changes to GitHub
 
 Once you have installed the GitHub Action workflow for IGA, the next steps are (1) [get an InvenioRDM token](#getting-an-inveniordm-token) and (2) [configure the GitHub Action workflow](#configuring-and-running-iga-as-a-github-actions-workflow).
 
 
 ## Quick start
 
-No matter whether IGA is run locally on your computer or as a GitHub Actions workflow, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
-is the first step.
+No matter whether IGA is run locally on your computer or as a GitHub Actions workflow, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one is the first step.
 
 ### Getting an InvenioRDM token
 
-<img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" width="60%" align="right">
+<img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" alt="Screenshot of InvenioRDM PAT menu" width="60%" align="right">
 
 1. Log in to your InvenioRDM account
 2. Go to the _Applications_ page in your account profile
 3. Click the <kbd>New token</kbd> button next to "Personal access tokens"
 4. On the page that is shown after you click that button, name your token (the name does not matter) and click the <kbd>Create</kbd> button
 5. After InvenioRDM creates and shows you the token, **copy it to a safe location** because InvenioRDM will not show it again
 
 ### Configuring and running IGA locally
 
 To send a GitHub release to your InvenioRDM server, IGA needs this information:
+
 1. (Required) The identity of the GitHub release to be archived
 2. (Required) The address of the destination InvenioRDM server
 3. (Required) A personal access token for InvenioRDM (from [above](#getting-an-inveniordm-token))
 4. (Optional) A [personal access token for GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
 
 The identity of the GitHub release is always given as an argument to IGA on the command line; the remaining values can be provided either via command-line options or environment variables. One approach is to set environment variables in shell scripts or your interactive shell. Here is an example using Bash shell syntax, with fake token values:
+
 ```shell
 export INVENIO_SERVER=https://data.caltech.edu
 export INVENIO_TOKEN=qKLoOH0KYf4D98PGYQGnC09hiuqw3Y1SZllYnonRVzGJbWz2
 export GITHUB_TOKEN=ghp_wQXp6sy3AsKyyEo4l9esHNxOdo6T34Zsthz
 ```
 
 Once these are set, use of IGA can be as simple as providing a URL for a release in GitHub. For example, the following command creates a draft record (the `-d` option is short for `--draft`) for another project in GitHub and tells IGA to open (the `-o` option is short for `--open`) the newly-created InvenioRDM entry in a web browser:
+
 ```shell
 iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 More options are described in the section on [detailed usage information](#usage) below.
 
 
 ### Configuring and running IGA as a GitHub Actions workflow
 
-After doing the [GitHub Actions installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
+After doing the [GitHub Actions installation](#configuring-and-running-iga-as-a-github-actions-workflow) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
 
-1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" width="85%"></p>
-2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" width="40%"></p>
-3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" width="60%"></p>
+1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" alt="Screenshot of repository tabs in GitHub" width="85%"></p>
+2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" alt="Screenshot of GitHub secrets sidebar item" width="40%"></p>
+3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" alt="Screenshot of GitHub secrets interface" width="60%"></p>
 4. Name the variable `INVENIO_TOKEN` and paste in your InvenioRDM token
 5. Finish by clicking the green <kbd>Add secret</kbd> button
 
 #### Testing the workflow
 
 After setting up the workflow and storing the InvenioRDM token in your repository on GitHub, it's a good idea to run the workflow manually to test that it works as expected.
 
-1. Go to the _Actions_ tab in your repository and click on the name of the workflow in the sidebar on the left<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-run-workflow.png" width="90%"></p>
+1. Go to the _Actions_ tab in your repository and click on the name of the workflow in the sidebar on the left<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-run-workflow.png" alt="Screenshot of GitHub actions workflow list" width="90%"></p>
 2. Click the <kbd>Run workflow</kbd> button in the right-hand side of the blue strip
-3. In the pull-down, change the value of "Mark the record as a draft" to `true`<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-workflow-options-circled.png" width="40%"></p>
+3. In the pull-down, change the value of "Mark the record as a draft" to `true`<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-workflow-options-circled.png" alt="Screenshot of GitHub Actions workflow menu" width="40%"></p>
 4. Click the green <kbd>Run workflow</kbd> button near the bottom
-5. Refresh the web page and a new line will be shown named after your workflow file<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-running-workflow.png" width="90%"></p>
+5. Refresh the web page and a new line will be shown named after your workflow file<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-running-workflow.png" alt="Screenshot of a running workflow in GitHub Actions" width="90%"></p>
 6. Click the title of the workflow to see the IGA workflow progress and results
 
 
 #### Running the workflow when releasing software
 
 Once the personal access token from InvenioRDM is stored as a GitHub secret, the workflow should run automatically every time a new release is made on GitHub &ndash; no further action should be needed. You can check the results (and look for errors if something went wrong) by going to the _Actions_ tab in your GitHub repository.
 
@@ -297,52 +364,58 @@
 
 A personal access token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
-It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some public repositories IGA will not hit the limit. However, if you are archiving a private repository, run IGA multiple times in a row, or the repository has many contributors, then you will need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some public repositories IGA will not hit the limit. However, if you are archiving a private repository, run IGA multiple times in a row, or the repository has many contributors, then you will need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit [https://docs.github.com/en/authentication](https://docs.github.com/en/authentication) and follow the instructions for creating a "classic" personal access token.
 
 Note that when you run IGA as a GitHub Actions workflow, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Actions workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
- 1. The full URL of the web page on GitHub of a tagged release. In this case,
+
+1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
- 2. A combination of _account name_, _repository name_, and _tag_. In this
+2. A combination of _account name_, _repository name_, and _tag_. In this
     case, the final argument on the command line must be the _tag_, and in
     addition, values for the options `--account` and `--repo` must be provided.
 
 Here's an example using approach #1 (assuming environment variables `INVENIO_SERVER`, `INVENIO_TOKEN`, and `GITHUB_TOKEN` have all been set):
+
 ```shell
 iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
+
 and here's the equivalent using approach #2:
+
 ```shell
 iga --github-account mhucka --github-repo taupe v1.2.0
 ```
+
 Note that when using this form of the command, the release tag (`v1.2.0` above) must be the last item given on the command line.
 
 ### Gathering metadata for an InvenioRDM record
 
 The record created in InvenioRDM is constructed using information obtained using GitHub's API as well as several other APIs as needed. The information includes the following:
- * (if one exists) a `codemeta.json` file in the GitHub repository
- * (if one exists) a `CITATION.cff` file in the GitHub repository
- * data available from GitHub for the release
- * data available from GitHub for the repository
- * data available from GitHub for the account of the owner
- * data available from GitHub for the accounts of repository contributors
- * file assets associated with the GitHub release
- * data available from ORCID.org for ORCID identifiers
- * data available from ROR.org for Research Organization Registry identifiers
- * data available from DOI.org, NCBI, Google Books, & others for publications
- * data available from spdx.org for software licenses
+
+* (if one exists) a `codemeta.json` file in the GitHub repository
+* (if one exists) a `CITATION.cff` file in the GitHub repository
+* data available from GitHub for the release
+* data available from GitHub for the repository
+* data available from GitHub for the account of the owner
+* data available from GitHub for the accounts of repository contributors
+* file assets associated with the GitHub release
+* data available from ORCID.org for ORCID identifiers
+* data available from ROR.org for Research Organization Registry identifiers
+* data available from DOI.org, NCBI, Google Books, & others for publications
+* data available from spdx.org for software licenses
 
 IGA tries to use [`CodeMeta.json`](https://codemeta.github.io) first and [`CITATION.cff`](https://citation-file-format.github.io) second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
 
 To override the auto-created metadata, use the option `--read-metadata` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-metadata` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
 
 ### Specifying GitHub file assets
 
@@ -359,15 +432,16 @@
 ### Indicating draft versus published records
 
 If the `--community` option is not used, then by default, IGA will finalize and publish the record. To make it stop short and leave the record as a draft instead, use the option `--draft`. The draft option also takes precedence over the community option: if you use both `--draft` and `--community`, IGA will stop after creating the draft record and will _not_ submit it to the community.  (You can nevertheless submit the record to a community manually once the draft is created, by visiting the record's web page and using the InvenioRDM interface there.)
 
 ### Versioning records
 
 The option `--parent-record` can be used to indicate that the record being constructed is a new version of an existing record. This will make IGA use the InvenioRDM API for [record versioning](https://inveniordm.docs.cern.ch/releases/versions/version-v2.0.0/#versioning-support). The newly-created record will be linked to a parent record identified by the value passed to `--parent-record`. The value must be either an InvenioRDM record identifier (which is a sequence of alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`, generated by the InvenioRDM server), or a URL to the landing page of the record in the InvenioRDM server. (Note that such URLs end in the record identifier.) Here is an example of using this option:
-```
+
+```shell
 iga --parent-record xbcd4-efgh5 https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 ### Other options recognized by IGA
 
 Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
@@ -387,23 +461,23 @@
 
 As explain above, IGA takes one required argument on the command line: either (1) the full URL of a web page on GitHub of a tagged release, or (2) a release tag name which is to be used in combination with options `--github-account` and `--github-repo`. The following table summarizes all the command line options available.
 
 | Long&nbsp;form&nbsp;option&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Short&nbsp;&nbsp; | Meaning | Default |  |
 |------------------------|----------|--------------------------------------|---------|---|
 | `--all-assets`         | `-A`     | Attach all GitHub assets | Attach only the release source ZIP| |
 | `--all-metadata`       | `-M`     | Include additional metadata from GitHub | Favor CodeMeta & CFF | |
-| `--community` _C_      | `-c` _C_ | Submit record to RDM community _C_ | Don't submit record to any community | | 
+| `--community` _C_      | `-c` _C_ | Submit record to RDM community _C_ | Don't submit record to any community | |
 | `--draft`              | `-d`     | Mark the RDM record as a draft | Publish record when done | |
 | `--file` _F_           | `-f` _F_ | Upload local file _F_ instead of GitHub assets | Upload only GitHub assets | ⚑ |
-| `--github-account` _A_ | `-a` _A_ | Look in GitHub account _A_ | Get account name from release URL | ✯ | 
+| `--github-account` _A_ | `-a` _A_ | Look in GitHub account _A_ | Get account name from release URL | ✯ |
 | `--github-repo` _R_    | `-r` _R_ | Look in GitHub repository _R_ of account _A_ | Get repo name from release URL | ✯ |
 | `--github-token` _T_   | `-t` _T_ | Use GitHub access token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
-| `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
-| `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
+| `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | |
+| `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | |
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
 | `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
 | `--print-doi`          | `-i`     | Print both the DOI & record URL when done | Print only the record URL | |
 | `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
@@ -427,18 +501,47 @@
 | 2    | encountered a bad or missing value for an option         |
 | 3    | encountered a problem with a file or directory           |
 | 4    | encountered a problem interacting with GitHub            |
 | 5    | encountered a problem interacting with InvenioRDM        |
 | 6    | the personal access token was rejected                   |
 | 7    | an exception or fatal error occurred                     |
 
+### Adding a DOI badge to your GitHub repository
+
+Once you have set up the IGA workflow in your GitHub repository, you may wish to add a DOI badge to your repository's README file. It would be a chore to keep updating the DOI value in this badge every time a new release is made, and thankfully, it's not necessary: it's possible to make the badge get the current DOI value dynamically. Here is how:
+
+1. _After_ you have at least one release archived in your InvenioRDM server, find out the DOI of that release in InvenioRDM, and extract the tail end of that DOI. The DOI assigned by InvenioRDM will be a string such as `10.22002/zsmem-2pg20`; the tail end is the `zsmem-2pg20` part. (Your DOI and tail portion will be different.)
+2. Let <i><b><code>SERVERURL</code></b></i> stand for the URL for your InvenioRDM server, and let <i><b><code>IDENTIFIER</code></b></i> stand for the identifier portion of the DOI. In your `README.md` file, write the DOI badge as follows (without line breaks):
+
+    <pre><code>[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&query=$.pids.doi.identifier&uri=<i><b><code>SERVERURL</code></b></i>/api/records/<i><b><code>IDENTIFIER</code></b></i>/versions/latest)](<i><b><code>SERVERURL</code></b></i>/records/<i><b><code>IDENTIFIER</code></b></i>/latest)</code></pre>
+
+For example, for CaltechDATA and the archived IGA releases there,
+
+* <i><b><code>SERVERURL</code></b></i> = `http://data.caltech.edu`
+* <i><b><code>IDENTIFIER</code></b></i> = `zsmem-2pg20`
+
+which leads to the following badge string for IGA's `README.md` file:
+
+```txt
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20/versions/latest)](https://data.caltech.edu/records/zsmem-2pg20/latest)
+```
+
+<br>The result looks like this: <div align="center">
+
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/zsmem-2pg20/versions/latest)](https://data.caltech.edu/records/zsmem-2pg20/latest)
+
+</div>
+
+You can change the look of the badge by using style parameters. Please refer to the [Shields.io](https://shields.io/badges/static-badge) documentation for static badges.
+
 
 ## Known issues and limitations
 
 The following are known issues and limitations.
+
 * As of mid-2023, InvenioRDM requires names of record creators and other contributors to be split into given (first) and family (surname). This is problematic for multiple reasons. The first is that mononyms are common in many countries: a person's name may legitimately be only a single word which is not conceptually a "given" or "family" name.  To compound the difficulty for IGA, names are stored as single fields in GitHub account metadata, so unless a repository has a `codemeta.json` or `CITATION.cff` file (which allow authors more control over how they want their names represented), IGA is forced to try to split the single GitHub name string into two parts. _A foolproof algorithm for doing this does not exist_, so IGA will sometimes get it wrong. (That said, IGA goes to extraordinary lengths to try to do a good job.)
 * InvenioRDM requires that identities (creators, contributors, etc.) to be labeled as personal or organizational. The nature of identities is usually made clear in `codemeta.json` and `CITATION.cff` files. GitHub also provides a flag that is meant to be used to label organizational accounts, but sometimes people don't set the GitHub account information correctly. Consequently, if IGA has to use GitHub data to get (e.g.) the list of contributors on a project, it may mislabel identities in the InvenioRDM record it produces.
 * Some accounts on GitHub are software automation or "bot" accounts, but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub, so if they're not labeled as bot or organizational accounts in GitHub, IGA can't recognize that they're humans. If such an account is the creator of a release in GitHub, and IGA tries to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI".
 * Funder and funding information can only be specified in `codemeta.json` files; neither GitHub nor `CITATION.cff` have provisions to store this kind of metadata. The CodeMeta specification defines two fields for this purpose: `funder` and `funding`. Unfortunately, these map imperfectly to the requirements of InvenioRDM's metadata format. In addition, people don't always follow the CodeMeta guidelines, and sometimes they write funding information as text strings (instead of structured objects), the interpretation of which would require software that can recognize grant and funding agency information from free-text descriptions. This combination of factors means IGA often can't fill in the funding metadata in InvenioRDM records even if there is some funding information in the `codemeta.json` file.
 
 
 ## Getting help
@@ -449,48 +552,51 @@
 ## Contributing
 
 Your help and participation in enhancing IGA is welcome!  Please visit the [guidelines for contributing](CONTRIBUTING.md) for some tips on getting started.
 
 
 ## License
 
-Software produced by the Caltech Library is Copyright © 2023 California Institute of Technology.  This software is freely distributed under a BSD-style license.  Please see the [LICENSE](LICENSE) file for more information.
+Software produced by the Caltech Library is Copyright © 2022–2024 California Institute of Technology.  This software is freely distributed under a BSD-style license.  Please see the [LICENSE](LICENSE) file for more information.
 
 ## Acknowledgments
 
 This work was funded by the California Institute of Technology Library.
 
 IGA uses multiple other open-source packages, without which it would have taken much longer to write the software. I want to acknowledge this debt. In alphabetical order, the packages are:
+
 * [Aenum](https://github.com/ethanfurman/aenum) &ndash; package for advanced enumerations
 * [Arrow](https://pypi.org/project/arrow/) &ndash; a library for creating & manipulating dates
 * [Boltons](https://github.com/mahmoud/boltons/) &ndash; package of miscellaneous Python utilities
 * [caltechdata_api](https://github.com/caltechlibrary/caltechdata_api) &ndash; package for using the CaltechDATA API
 * [CommonPy](https://github.com/caltechlibrary/commonpy) &ndash; a collection of commonly-useful Python functions
-* [demoji](https://github.com/bsolomon1124/demoji) &ndash; find or remove emojis from text
 * [dirtyjson](https://github.com/codecobblers/dirtyjson) &ndash; JSON decoder that copes with problematic JSON files and reports useful error messages
 * [flake8](https://github.com/pycqa/flake8) &ndash; Python code linter and style analyzer
+* [Ginza](https://github.com/megagonlabs/ginza) &ndash; Japanese NLP Library
 * [httpx](https://www.python-httpx.org) &ndash; HTTP client library that supports HTTP/2
 * [humanize](https://github.com/jmoiron/humanize) &ndash; make numbers more easily readable by humans
 * [idutils](https://github.com/inveniosoftware/idutils) &ndash; package for validating and normalizing various kinds of persistent identifiers
 * [ipdb](https://github.com/gotcha/ipdb) &ndash; the IPython debugger
 * [iptools](https://github.com/bd808/python-iptools) &ndash; utilities for dealing with IP addresses
 * [isbnlib](https://github.com/xlcnd/isbnlib) &ndash; utilities for dealing with ISBNs
+* [Jamo](https://github.com/JDongian/python-jamo) &ndash; Hangul character analysis
 * [json5](https://github.com/dpranke/pyjson5) &ndash; extended JSON format parser
 * [latexcodec](https://github.com/mcmtroffaes/latexcodec) &ndash; lexer and codec to work with LaTeX code in Python
+* [Lingua](https://github.com/pemistahl/lingua) &ndash; language detection library
 * [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) &ndash; a link recognition library with full unicode support
 * [lxml](https://lxml.de) &ndash; an XML parsing library
 * [Markdown](https://python-markdown.github.io) &ndash; Python package for working with Markdown
 * [markdown-checklist](https://github.com/FND/markdown-checklist) &ndash; GitHub-style checklist extension for Python Markdown package
 * [mdx-breakless-lists](https://github.com/adamb70/mdx-breakless-lists) &ndash; GitHub-style Markdown lists that don't require a line break above them
 * [mdx_linkify](https://github.com/daGrevis/mdx_linkify) &ndash; extension for Python Markdown will convert text that look like links to HTML anchors
 * [MyST-parser](https://github.com/executablebooks/MyST-Parser) &ndash; A Sphinx and Docutils extension to parse an extended version of Markdown
 * [nameparser](https://github.com/derek73/python-nameparser) &ndash; package for parsing human names into their individual components
 * [probablepeople](https://github.com/datamade/probablepeople) &ndash; package for parsing names into components using ML-based techniques
 * [pybtex](https://pybtex.org) &ndash; BibTeX parser and formatter
-* [pybtex-apa7-style]() &ndash; plugin for [pybtex](https://pybtex.org) that provides APA7 style formatting
+* [pybtex-apa7-style](https://pypi.org/project/pybtex-apa7-style/) &ndash; plugin for [pybtex](https://pybtex.org) that provides APA7 style formatting
 * [pymdown-extensions](https://github.com/facelessuser/pymdown-extensions) &ndash; extensions for Python Markdown
 * [pytest](https://docs.pytest.org/en/stable/) &ndash; testing framework
 * [pytest-cov](https://github.com/pytest-dev/pytest-cov) &ndash; coverage reports for use with `pytest`
 * [pytest-mock](https://pypi.org/project/pytest-mock/) &ndash; wrapper around the `mock` package for use with `pytest`
 * [PyYAML](https://pyyaml.org) &ndash; YAML parser
 * [Rich](https://github.com/Textualize/rich) &ndash; library for writing styled text to the terminal
 * [rich-click](https://github.com/ewels/rich-click) &ndash; CLI interface built on top of [Rich](https://github.com/Textualize/rich)
@@ -511,10 +617,10 @@
 * [url-normalize](https://github.com/niksite/url-normalize) &ndash; URI/URL normalization utilities
 * [validators](https://github.com/kvesteri/validators) &ndash; data validation package for Python
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
-    <img width="100" height="100" src="https://github.com/caltechlibrary/iga/raw/main/.graphics/caltech-round.png">
+    <img width="100" height="100" alt="Caltech logo" src="https://github.com/caltechlibrary/iga/raw/main/.graphics/caltech-round.png">
   </a>
 </div>
```

### Comparing `iga-1.2.2/iga.egg-info/SOURCES.txt` & `iga-1.3.0/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/setup.cfg` & `iga-1.3.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 1.2.2
+version = 1.3.0
 description = The InvenioRDM GitHub Archiver (IGA) automatically archives GitHub releases in an InvenioRDM repository.
 author = Michael Hucka
 author_email = mhucka@caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-1.2.2/setup.py` & `iga-1.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
-# @file    setup.py
-# @brief   Installation setup file
-# @created 2022-12-08
-# @license Please see the file named LICENSE in the project directory
-# @website https://github.com/caltechlibrary/iga
+# Summary: IGA installation setup.py file.
 #
 # Note: the full configuration metadata is maintained in setup.cfg, not here.
 # This file exists to hook in setup.cfg and requirements.txt, so that the
 # requirements don't have to be repeated and so that "python3 setup.py" works.
+#
+# Copyright 2024 California Institute of Technology.
+# License: Modified BSD 3-clause – see file "LICENSE" in the project website.
+# Website: https://github.com/caltechlibrary/iga
 
 from setuptools import setup
 
 
 def requirements(file):
     from os import path
     required = []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iga-1.2.2/tests/test_cli.py` & `iga-1.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_data_utils.py` & `iga-1.3.0/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_doi.py` & `iga-1.3.0/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_exceptions.py` & `iga-1.3.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_github.py` & `iga-1.3.0/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_github_mocks.py` & `iga-1.3.0/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_id_utils.py` & `iga-1.3.0/tests/test_id_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # =============================================================================
 
 from iga.id_utils import (
     contains_pmcid,
     detected_id,
     normalize_pmcid,
     recognized_scheme,
-    is_invenio_rdm,
+    is_inveniordm_id,
 )
 
 sample_ids = [
     ('arXiv:2012.13117v1'                                 , 'arxiv'),
     ('10.48550/arXiv.2012.13117'                          , 'doi'),
     ('PMC4908318'                                         , 'pmcid'),
     ('26861819'                                           , 'pmid'),
@@ -75,9 +75,9 @@
 
 def test_detected_id():
     for text, id_ in sample_unnormalized_ids:
         assert detected_id(text) == id_
 
 
 def test_is_invenio_rdm():
-    assert is_invenio_rdm('https://a.b/records/ry4vm-wny44')
-    assert not is_invenio_rdm('https://a.b/something/ry4vm-wny44')
+    assert is_inveniordm_id('https://a.b/records/ry4vm-wny44')
+    assert not is_inveniordm_id('https://a.b/something/ry4vm-wny44')
```

### Comparing `iga-1.2.2/tests/test_init.py` & `iga-1.3.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_is_person.py` & `iga-1.3.0/tests/test_is_person.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     "Gregory Brown",
     "John-David Dalton",
     "Paul Betts",
     "Paul Reioux",
     "Tony Arcieri",
     "Kana Natsuno",
     "Ben Alman",
-    "Astro",
+#    "Astro",
     "Jeff Forcier",
     "Sindre Sorhus",
     "Marijn Haverbeke",
     "Richard Huang",
     "Tim Caswell",
     "Joshua Peek",
     "Mitchell Hashimoto",
@@ -176,15 +176,14 @@
     "Rebecca Murphey",
     "Christian Amor Kvalheim",
     "Evan Coury",
     "Jakub Vrána",
     "Mark McGranaghan",
     "Steve Klabnik",
     "Ricardo Quesada",
-#    "Ingy döt Net",
     "lestrrat",
     "Aaron Patterson",
     "Aaron Straup Cope",
     "Thomas Davis",
     "Charles Oliver Nutter",
     "Kris Kowal",
     "Douglas Campos",
@@ -232,15 +231,15 @@
     "Naitik Shah",
     "Marcus Westin",
     "Coda Hale",
     "James Ward",
     "Mislav Marohnić",
     "Álvaro Justen",
     "Brian Noguchi",
-#    "Wynn Netherland",
+    "Wynn Netherland",
     "Koushik Dutta",
     "Oliver Drobnik",
     "Richard Schneeman",
     "Salvatore Sanfilippo",
     "fat-kun",
     "Christopher Jeffrey",
     "SHIBATA Hiroshi",
@@ -282,15 +281,15 @@
     "Charles Leifer",
     "Mike Perham",
     "David Walsh",
     "Dave Reisner",
     "Thomas Reynolds",
     "Phus Lu",
     "Javier Jiménez",
-    "Fuji, Goro",
+#    "Fuji, Goro",
     "Justin Hileman",
     "Vincent Driessen",
     "Jason Davies",
     "Caolan McMahon",
     "Igor Minar",
     "Jonathan &quot;Duke&quot; Leto",
     "Zach Holman",
@@ -305,15 +304,15 @@
     "Nathan Hamblen",
     "Jed Schmidt",
     "Stevan Little",
     "Chris Done",
     "Bozhidar Batsov",
     "Stefan Kanev",
     "Craig Campbell",
-#    "antimatter15",
+    "antimatter15",
     "Ian Bicking",
     "Dennis Reimann",
     "Miguel de Icaza",
     "Mathias Bynens",
     "Ward Cunningham",
     "Tim Pope",
     "Nicolas Gramlich",
@@ -435,15 +434,15 @@
     "Davies Lliu",
     "Ethan Schoonover",
     "cho45",
     "Feross Aboukhadijeh",
     "Adán Miguel Sánchez Albert",
     "TAKANO Mitsuhiro",
     "Qiang Xue",
-#    "Weibin Yao(姚伟斌)",
+    "Weibin Yao(姚伟斌)",
     "Max Goodman",
     "Idan Gazit",
     "Endy Muhardin",
     "Shaun McCormick",
     "Mikito Takada",
     "ara.t.howard",
     "Gareth Rushgrove",
@@ -465,19 +464,19 @@
     "Caleb Troughton",
     "Theodore Watson",
     "Jerome Gravel-Niquet",
     "James Turnbull",
     "Yuichiro MASUI",
     "Guillaume Bort",
     "Jeremy Bush",
-#    "hitode909",
+    "hitode909",
     "Magnus Holm",
     "Arun Agrawal",
     "Miško Hevery",
-#    "云风",
+#    "云风",   # it's a user account on github, called "cloudwu"
     "James Dennis",
     "Guilherme Blanco",
     "Luciano Ramalho",
     "Jeremy Kemper",
     "Yoshihiro Sugi",
     "Dan Croak",
     "Alex Ott",
@@ -888,28 +887,186 @@
     "Ching-Lan 'digdog' HUANG 黃 青嵐",
     "Bret Taylor",
     "Paul Pajo",
     "Krystal Mok",
     "Yuval Kogman",
     "Peter Boctor",
     "Aaron Newton",
-    "The Octocat",
+#    "The Octocat",
+    "布客飞龙",
+    "小弟调调",
+    "芋道源码",
+    "三咲智子",
+    "题叶",
+    "王下邀月熊",
+    "张炎泼",
+    "徐明",
+    "灵茶山艾府",
+    "王诗翔",
+    "云游君",
+    "吴晟",
+    "卡色",
+    "罗泽轩",
+    "贤心",
+    "前端开发博客",
+    "李鼎",
+    "响马",
+    "管宜尧",
+#    "辉鸭蛋",
+    "伊撒尔",
+    "依云",
+    "程序员",
+    "大帅老猿",
+    "阿崔",
+    "吴多益",
+    "荣顶",
+    "李宗英",
+    "安正超",
+    "彭于斌",
+    "大漠穷秋",
+    "文翼",
+    "曾哥",
+    "崔庆才丨静觅",
+    "一蓑烟雨",
+    "유용민",
+    "정승훈",
+    "도경",
+    "이정호",
+    "박현우",
+    "김성길",
+#    "깃짱",
+    "전민재",
+    "안예성",
+    "구영표",
+    "박준현",
+    "변찬우",
+    "이은비",
+    "권강빈",
+    "洪民憙",
+    "정현수",
+    "최미래",
+    "백승하",
+#    "스타샤",
+    "신수형",
+    "임우찬",
+    "신종화",
+    "이강욱",
+    "윤정민",
+    "이석호",
+    "김지현",
+    "전해성",
+    "이정호",
+    "심미진",
+    "웹스토리보이",
+    "이수진",
+    "김서진",
+    "최민재",
+    "황준승",
+    "백여우",
+    "전해림",
+    "니콜라스",
+    "박준현",
+    "김노트",
+    "강대현",
+    "김재호",
+    "김세현",
+    "임세현",
+    "시니어코딩",
+    "이정은",
+    "김준환",
+    "한규진",
+    "신준서",
+    "강지석",
+    "김승우",
+    "테디",
+    "고석진",
+    "이정민",
+    "임동현",
+    "권용빈",
+    "차승호",
+    "나상우",
+    "이규진빌규진",
+    "박찬인",
+    "김한수",
+    "차경민",
+    "김도형",
+    "홍정현",
+    "소연",
+    "우준성",
+    "이선우",
+    "이원중",
+    "강수진",
+    "정우일",
+    "박우빈",
+    "황성현",
+    "조성동",
+    "정찬효",
+    "박우림",
+    "페르난도",
+    "레이크한영수",
+    "주엽",
+    "정석호",
+    "강성진",
+    "정시원",
+    "승민",
+    "김나영",
+    "이재하",
+    "정성민",
+    "전지환",
+    "재이다",
+    "김민혁",
+    "이정연",
+    "조용주",
+    "사이먼",
+    "프로그래머스교육팀",
+    "토르",
+    "태민",
+    "이안",
+    "아구몬",
+    "안성현",
+    "이승우",
+    "양윤재",
+    "박창주",
+    "이승규",
+    "이준혁",
+    "강종연",
+    "박연오",
+    "서울정보소통광장",
+    "조은",
+    "정건우",
+    "류성두",
+    "노종원",
+    "小河",
+    "서현석",
+    "홍영준",
+    "신백균",
+    "령이",
+    "이동영",
+    "신중빈",
+    "黒音キト",
+    "仲田将之",
+    "川村亮太",
+    "桂素伟",
+    "雪月秋水",
+    "しまぶー",
+    "卜部昌平",
 ]
 
 NONPEOPLE = [
-    "开源中国",
+#    "开源中国",   # contains a known surname => confusing case.
+    "さくらインターネット",
     "California Institute Of Technology",
     "UCSB",
     "MIT",
     "Google",
     "Google Brain",
     "Sony",
 #    "Ovid",
     "Account for Github research",
-    "cocos2d",
+#    "cocos2d",
     "20th Century Fox",
     "3Com",
     "3M",
     "7-Up",
     "A Mild",
 #    "A.G. Edwards",
     "ABC",
```

### Comparing `iga-1.2.2/tests/test_licenses.py` & `iga-1.3.0/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_name_splitting.py` & `iga-1.3.0/tests/test_name_splitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,29 +48,29 @@
     ('Jean-Jacques Rousseau', Name(first='Jean-Jacques', last='Rousseau')),
     ('Jose Diaz-Gonzalez', Name(first='Jose', last='Diaz-Gonzalez')),
     ('José Lorenzo Rodríguez', Name(first='José Lorenzo', last='Rodríguez')),
     ('Lukas Kahwe Smith', Name(first='Lukas Kahwe', last='Smith')),
     ('Martin Luther King, Jr.', Name(first='Martin Luther', last='King')),
     ('Miguel de Val-Borro', Name(first='Miguel', last='de Val-Borro')),
     ('Mike Hucka', Name(first='Mike', last='Hucka')),
-    ('Mr.doob', Name(first='', last='Doob')),
+    ('Mr. Hamm', Name(first='', last='Hamm')),
     ('Mu-An ✌️ Chiou', Name(first='Mu-An', last='Chiou')),
     ('PatrickJS [tipe.io]', Name(first='', last='PatrickJS')),
     ('Philip (flip) Kromer', Name(first='Philip', last='Kromer')),
     ('R. Tyler Croy', Name(first='R. Tyler', last='Croy')),
     ('R.I.Pienaar', Name(first='R. I.', last='Pienaar')),
     ('Rafael França', Name(first='Rafael', last='França')),
     ('TJ Holowaychuk', Name(first='TJ', last='Holowaychuk')),
     ('TZ | 天猪', Name(first='', last='Tz')),
     ('Tokuhiro Matsuno', Name(first='Tokuhiro', last='Matsuno')),
     ('Weibin Yao(姚伟斌)', Name(first='Weibin', last='Yao')),
     ('Wladimir J. van der Laan', Name(first='Wladimir J.', last='van der Laan')),
     ('Yukihiro &quot;Matz&quot; Matsumoto', Name(first='Yukihiro', last='Matsumoto')),
     ('ara.t.howard', Name(first='Ara T.', last='Howard')),
-    ('cho45', Name(first='', last='cho45')),
+    ('cho45', Name(first='', last='Cho')),
     ('王爵nice', Name(first='', last='Nice')),
     # ('', Name(first='', last='')),
 
     # Known failures:
     # ("SHIBATA Hiroshi", Name(first='Hiroshi', last='SHIBATA')),
 ]
```

### Comparing `iga-1.2.2/tests/test_name_utils.py` & `iga-1.3.0/tests/test_name_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,27 +3,32 @@
 # @brief   Py.test cases for parts of name_utils.py
 # @created 2023-03-02
 # @license Please see the file named LICENSE in the project directory
 # @website https://github.com/caltechlibrary/iga
 # =============================================================================
 
 from iga.name_utils import (
-    _cleaned_name,
+    _plain_name,
     _plain_word,
     _first_letters_upcased,
     contains_cjk,
     flattened_name,
 )
 
 RAW_NAMES = [
     ('偏右', ''),
     ('王爵nice', 'nice'),
     ('勾三股四', ''),
     ('TZ | 天猪', 'TZ'),
+    ("Maciej Małecki", "Maciej Małecki"),
+    ("Gabriel Falcão", "Gabriel Falcão"),
     ('Mu-An ✌️ Chiou', 'Mu-An Chiou'),
+    ('Zip J. Zippy', 'Zip J. Zippy'),
+    ('Zip J. Zippy [the Zip]', 'Zip J. Zippy'),
+    ('Zip J. Zippy-Zip', 'Zip J. Zippy-Zip'),
 ]
 
 
 def test_contains_cjk():
     assert contains_cjk('偏右')
     assert contains_cjk('王爵nice')
     assert not contains_cjk('test')
@@ -33,17 +38,17 @@
 def test_flattened_name():
     assert flattened_name('foo bar') == 'foo bar'
     assert flattened_name(['foo', 'bar']) == 'foo bar'
     assert flattened_name(['Foo J.', 'Bar']) == 'Foo J. Bar'
     assert flattened_name(['Foo', 'J.', 'Bar']) == 'Foo J. Bar'
 
 
-def test_cleaned_name():
+def test_plain_name():
     for original, cleaned in RAW_NAMES:
-        assert _cleaned_name(original) == cleaned
+        assert _plain_name(original) == cleaned
 
 
 def test_plain_word():
     assert _plain_word('foo')
     assert _plain_word('FOO')
     assert _plain_word('Foo')
     assert not _plain_word('foo bar')
```

### Comparing `iga-1.2.2/tests/test_orcid.py` & `iga-1.3.0/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_record_from_codemeta.py` & `iga-1.3.0/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_reference.py` & `iga-1.3.0/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_ror.py` & `iga-1.3.0/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.2/tests/test_text_utils.py` & `iga-1.3.0/tests/test_text_utils.py`

 * *Files identical despite different names*

