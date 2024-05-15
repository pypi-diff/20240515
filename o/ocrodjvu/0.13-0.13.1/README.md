# Comparing `tmp/ocrodjvu-0.13.tar.gz` & `tmp/ocrodjvu-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocrodjvu-0.13.tar", last modified: Sun Jan 15 16:29:54 2023, max compression
+gzip compressed data, was "ocrodjvu-0.13.1.tar", last modified: Wed May 15 16:50:44 2024, max compression
```

## Comparing `ocrodjvu-0.13.tar` & `ocrodjvu-0.13.1.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-01-15 16:29:54.315838 ocrodjvu-0.13/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    18092 2023-01-15 16:19:19.000000 ocrodjvu-0.13/COPYING
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       58 2023-01-15 16:19:19.000000 ocrodjvu-0.13/MANIFEST.in
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5087 2023-01-15 16:29:54.315838 ocrodjvu-0.13/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4270 2023-01-15 16:19:19.000000 ocrodjvu-0.13/README.rst
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-01-15 16:29:54.307838 ocrodjvu-0.13/doc/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    23612 2023-01-15 16:22:41.000000 ocrodjvu-0.13/doc/changelog
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-01-15 16:29:54.311838 ocrodjvu-0.13/ocrodjvu/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      354 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/__main__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-01-15 16:29:54.311838 ocrodjvu-0.13/ocrodjvu/cli/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      827 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/cli/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    12152 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/cli/djvu2hocr.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3792 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/cli/hocr2djvused.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    23776 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/cli/ocrodjvu.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-01-15 16:29:54.315838 ocrodjvu-0.13/ocrodjvu/engines/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      865 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/engines/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2168 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/engines/common.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6926 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/engines/cuneiform.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1152 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/engines/dummy.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6102 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/engines/gocr.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6564 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/engines/ocrad.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10791 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/engines/tesseract.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2063 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/errors.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    18162 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/hocr.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1001 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/html5_support.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6372 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/image_io.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5748 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/ipc.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1432 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/iso639.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1245 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/logger.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1154 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/temporary.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6477 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/text_zones.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1566 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/unicode_support.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5349 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/utils.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2257 2023-01-15 16:19:19.000000 ocrodjvu-0.13/ocrodjvu/version.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-01-15 16:29:54.311838 ocrodjvu-0.13/ocrodjvu.egg-info/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5087 2023-01-15 16:29:54.000000 ocrodjvu-0.13/ocrodjvu.egg-info/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      835 2023-01-15 16:29:54.000000 ocrodjvu-0.13/ocrodjvu.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-01-15 16:29:54.000000 ocrodjvu-0.13/ocrodjvu.egg-info/dependency_links.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      157 2023-01-15 16:29:54.000000 ocrodjvu-0.13/ocrodjvu.egg-info/entry_points.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      100 2023-01-15 16:29:54.000000 ocrodjvu-0.13/ocrodjvu.egg-info/requires.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        9 2023-01-15 16:29:54.000000 ocrodjvu-0.13/ocrodjvu.egg-info/top_level.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2023-01-15 16:29:54.315838 ocrodjvu-0.13/setup.cfg
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1948 2023-01-15 16:29:39.000000 ocrodjvu-0.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:50:44.563654 ocrodjvu-0.13.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-15 16:50:44.563654 ocrodjvu-0.13.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:50:44.555654 ocrodjvu-0.13.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    23799 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/doc/changelog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:50:44.559654 ocrodjvu-0.13.1/ocrodjvu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:50:44.559654 ocrodjvu-0.13.1/ocrodjvu/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/cli/djvu2hocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/cli/hocr2djvused.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23774 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/cli/ocrodjvu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:50:44.563654 ocrodjvu-0.13.1/ocrodjvu/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/engines/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/engines/cuneiform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/engines/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/engines/gocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/engines/ocrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/engines/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18164 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/hocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/html5_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/image_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/iso639.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/temporary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/text_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/unicode_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/ocrodjvu/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:50:44.563654 ocrodjvu-0.13.1/ocrodjvu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-15 16:50:44.000000 ocrodjvu-0.13.1/ocrodjvu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-15 16:50:44.000000 ocrodjvu-0.13.1/ocrodjvu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:50:44.000000 ocrodjvu-0.13.1/ocrodjvu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-15 16:50:44.000000 ocrodjvu-0.13.1/ocrodjvu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 16:50:44.000000 ocrodjvu-0.13.1/ocrodjvu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 16:50:44.000000 ocrodjvu-0.13.1/ocrodjvu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:50:44.563654 ocrodjvu-0.13.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:50:44.563654 ocrodjvu-0.13.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/tests/test_ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/tests/test_text_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/tests/test_unicode_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-05-15 16:50:40.000000 ocrodjvu-0.13.1/tests/test_utils.py
```

### Comparing `ocrodjvu-0.13/COPYING` & `ocrodjvu-0.13.1/COPYING`

 * *Files identical despite different names*

### Comparing `ocrodjvu-0.13/PKG-INFO` & `ocrodjvu-0.13.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrodjvu
-Version: 0.13
+Version: 0.13.1
 Summary: OCR for DjVu (Python 3 fork)
 Home-page: https://github.com/FriedrichFroebel/ocrodjvu/
 Author: Jakub Wilk, FriedrichFröbel (Python 3)
 License: GNU GPL 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -13,17 +13,25 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/x-rst
+License-File: COPYING
+Requires-Dist: python-djvulibre>=0.4
+Requires-Dist: lxml>=2.0
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pep8-naming; extra == "dev"
+Requires-Dist: Pillow; extra == "dev"
 Provides-Extra: docs
-License-File: COPYING
+Requires-Dist: docutils; extra == "docs"
+Requires-Dist: pygments; extra == "docs"
 
 Overview
 ========
 
 **ocrodjvu** is a wrapper for OCR systems that allows you to perform OCR on DjVu_ files.
 
 .. _DjVu:
@@ -67,18 +75,22 @@
 * an OCR engine:
 
   + Cuneiform_ ≥ 0.7
   + Ocrad_ ≥ 0.10
   + GOCR_ ≥ 0.40
   + Tesseract_ ≥ 2.00
 
-* DjVuLibre_ ≥ 3.5.21
+* DjVuLibre_ ≥ 3.5.21 (≥ 3.5.26 for latest python-djvulibre)
 
 * python-djvulibre_ ≥ 0.4
 
+  + Please note that installing this package currently is a bit more complicated since Cython 3 has been relased on 2023-07-17.
+  + While `Issue #11`_ is unresolved, PyPI releases require some workarounds (installing the package from the source archive with the deprecated ``python setup.py install`` beforehand).
+  + Alternative: Install the latest package version from `Git <python-djvulibre-git_>`_.
+
 * lxml_ ≥ 2.0
 
 Additionally, some optional features require the following software:
 
 * PyICU_ ≥ 1.0.1 —
   required for the ``--word-segmentation=uax29`` option
 
@@ -102,31 +114,39 @@
    https://www-e.uni-magdeburg.de/jschulen/ocr/
 .. _Tesseract:
    https://github.com/tesseract-ocr/tesseract
 .. _DjVuLibre:
    http://djvu.sourceforge.net/
 .. _python-djvulibre:
    https://jwilk.net/software/python-djvulibre
+.. _Issue #11:
+   https://github.com/FriedrichFroebel/python-djvulibre/issues/11
+.. _python-djvulibre-git:
+   https://github.com/FriedrichFroebel/python-djvulibre
 .. _lxml:
    https://lxml.de/
 .. _PyICU:
    https://pypi.org/project/PyICU/
 .. _html5lib:
    https://github.com/html5lib/html5lib-python
 .. _xsltproc:
    http://xmlsoft.org/XSLT/xsltproc2.html
 .. _DocBook XSL stylesheets:
    https://github.com/docbook/xslt10-stylesheets
 
 Installation
 ============
 
-You can use ocrodjvu without installing it, straight out of unpacked source tarball or a VCS checkout.
+The easiest way to install ocrodjvu is from PyPI::
+
+    pip install ocrodjvu
+
+Alternatively, you can use ocrodjvu without installing it, straight out of an unpacked source tarball or a VCS checkout.
 
-It's also possible to install it system-wide with::
+It's also possible to install it from source for the current interpreter with::
 
    pip install .
 
 The man pages can be deployed using::
 
    make install_manpage
```

### Comparing `ocrodjvu-0.13/README.rst` & `ocrodjvu-0.13.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -44,18 +44,22 @@
 * an OCR engine:
 
   + Cuneiform_ ≥ 0.7
   + Ocrad_ ≥ 0.10
   + GOCR_ ≥ 0.40
   + Tesseract_ ≥ 2.00
 
-* DjVuLibre_ ≥ 3.5.21
+* DjVuLibre_ ≥ 3.5.21 (≥ 3.5.26 for latest python-djvulibre)
 
 * python-djvulibre_ ≥ 0.4
 
+  + Please note that installing this package currently is a bit more complicated since Cython 3 has been relased on 2023-07-17.
+  + While `Issue #11`_ is unresolved, PyPI releases require some workarounds (installing the package from the source archive with the deprecated ``python setup.py install`` beforehand).
+  + Alternative: Install the latest package version from `Git <python-djvulibre-git_>`_.
+
 * lxml_ ≥ 2.0
 
 Additionally, some optional features require the following software:
 
 * PyICU_ ≥ 1.0.1 —
   required for the ``--word-segmentation=uax29`` option
 
@@ -79,31 +83,39 @@
    https://www-e.uni-magdeburg.de/jschulen/ocr/
 .. _Tesseract:
    https://github.com/tesseract-ocr/tesseract
 .. _DjVuLibre:
    http://djvu.sourceforge.net/
 .. _python-djvulibre:
    https://jwilk.net/software/python-djvulibre
+.. _Issue #11:
+   https://github.com/FriedrichFroebel/python-djvulibre/issues/11
+.. _python-djvulibre-git:
+   https://github.com/FriedrichFroebel/python-djvulibre
 .. _lxml:
    https://lxml.de/
 .. _PyICU:
    https://pypi.org/project/PyICU/
 .. _html5lib:
    https://github.com/html5lib/html5lib-python
 .. _xsltproc:
    http://xmlsoft.org/XSLT/xsltproc2.html
 .. _DocBook XSL stylesheets:
    https://github.com/docbook/xslt10-stylesheets
 
 Installation
 ============
 
-You can use ocrodjvu without installing it, straight out of unpacked source tarball or a VCS checkout.
+The easiest way to install ocrodjvu is from PyPI::
+
+    pip install ocrodjvu
+
+Alternatively, you can use ocrodjvu without installing it, straight out of an unpacked source tarball or a VCS checkout.
 
-It's also possible to install it system-wide with::
+It's also possible to install it from source for the current interpreter with::
 
    pip install .
 
 The man pages can be deployed using::
 
    make install_manpage
```

### Comparing `ocrodjvu-0.13/doc/changelog` & `ocrodjvu-0.13.1/doc/changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+ocrodjvu (0.13.1) unstable; urgency=low
+
+  [ FriedrichFroebel ]
+  * Avoid deprecation warnings with the latest `lxml` versions.
+
+ -- FriedrichFroebel <>  Wed, 15 May 2024 16:42:10 +0200
+
 ocrodjvu (0.13) unstable; urgency=low
 
   [ FriedrichFroebel ]
   * Port to Python 3. At least Python 3.6 is required now.
   * Migrate tests from `nose` to plain `unittest` stdlib module.
   * Conform to PEP8 coding style.
   * Use standardized `setup.py`-based approach.
```

### Comparing `ocrodjvu-0.13/ocrodjvu/cli/__init__.py` & `ocrodjvu-0.13.1/ocrodjvu/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2011-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -20,9 +19,7 @@
 
 class ArgumentParser(argparse.ArgumentParser):
 
     def exit(self, status=0, message=None):
         if status:
             status = errors.EXIT_FATAL
         argparse.ArgumentParser.exit(self, status=status, message=message)
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/cli/djvu2hocr.py` & `ocrodjvu-0.13.1/ocrodjvu/cli/djvu2hocr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2009-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -344,9 +343,7 @@
                 page_text = sexpr.Expression.from_stream(djvused.stdout)
             except sexpr.ExpressionSyntaxError:
                 break
             LOGGER.info(f'- Page #{n}')
             page_zone = Zone(page_text, page_size[1])
             process_page(page_zone, options)
         sys.stdout.write(HOCR_FOOTER)
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/cli/hocr2djvused.py` & `ocrodjvu-0.13.1/ocrodjvu/cli/hocr2djvused.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2008-2017 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -90,9 +89,7 @@
 def main(argv=None):
     argv = argv if argv is not None else sys.argv
     options = ArgumentParser().parse_args(argv[1:])
     for i, text in enumerate(get_texts(options)):
         sys.stdout.write(f'select {i + 1}\nremove-txt\nset-txt\n')
         text_zones.print_sexpr(text, sys.stdout, width=80)
         sys.stdout.write('\n.\n\n')
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/cli/ocrodjvu.py` & `ocrodjvu-0.13.1/ocrodjvu/cli/ocrodjvu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2008-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -639,9 +638,7 @@
     except KeyboardInterrupt:
         LOGGER.info('Interrupted by user.')
         sys.exit(errors.EXIT_FATAL)
     finally:
         temp_dir = context.close()
         if temp_dir is not None:
             LOGGER.info(f'Intermediate files were left in the {temp_dir!r} directory.')
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/engines/__init__.py` & `ocrodjvu-0.13.1/ocrodjvu/engines/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2010-2015 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -19,9 +18,7 @@
 def get_engines():
     for importer, name, is_pkg in pkgutil.iter_modules(__path__):
         this_module = __import__('', globals=globals(), fromlist=(name,), level=1)
         engine = getattr(this_module, name).Engine
         if engine.name is None:
             continue
         yield engine
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/engines/common.py` & `ocrodjvu-0.13.1/ocrodjvu/engines/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2010-2019 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -61,9 +60,7 @@
         return self._contents
 
     def as_stringio(self):
         return io.StringIO(str(self))
 
     def as_bytesio(self):
         return io.BytesIO(bytes(self))
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/engines/cuneiform.py` & `ocrodjvu-0.13.1/ocrodjvu/engines/cuneiform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2010-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -165,9 +164,7 @@
                 return common.Output(
                     hocr_file.read(),
                     format_='html',
                 )
 
     def extract_text(self, *args, **kwargs):
         return self._hocr.extract_text(*args, **kwargs)
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/engines/dummy.py` & `ocrodjvu-0.13.1/ocrodjvu/engines/dummy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2018-2019 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -31,9 +30,7 @@
     def recognize(self, image, language, details=None, uax29=None):
         return common.Output('', format_='dummy')
 
     def extract_text(self, stream, **kwargs):
         bbox = text_zones.BBox(0, 0, 0, 0)
         page = text_zones.Zone(text_zones.const.TEXT_ZONE_PAGE, bbox, [])
         return [page.sexpr]
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/engines/gocr.py` & `ocrodjvu-0.13.1/ocrodjvu/engines/gocr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2010-2021 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -160,9 +159,7 @@
             )
 
     def extract_text(self, stream, **kwargs):
         settings = ExtractSettings(**kwargs)
         stream = etree.iterparse(stream)
         scan_result = scan(stream, settings)
         return [scan_result.sexpr]
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/engines/ocrad.py` & `ocrodjvu-0.13.1/ocrodjvu/engines/ocrad.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2010-2019 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -172,9 +171,7 @@
             )
 
     def extract_text(self, stream, **kwargs):
         settings = ExtractSettings(**kwargs)
         settings.replacement_character = self.replacement_character
         scan_result = scan(stream, settings)
         return [scan_result.sexpr]
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/engines/tesseract.py` & `ocrodjvu-0.13.1/ocrodjvu/engines/tesseract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2009-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -295,9 +294,7 @@
             return self._hocr.extract_text(stream, **kwargs)
         settings = ExtractSettings(**kwargs)
         bbox = text_zones.BBox(*((0, 0) + settings.page_size))
         text = stream.read()
         zone = text_zones.Zone(const.TEXT_ZONE_PAGE, bbox, [text])
         zone.rotate(settings.rotation)
         return [zone.sexpr]
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/errors.py` & `ocrodjvu-0.13.1/ocrodjvu/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2009-2019 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -74,9 +73,7 @@
     'EngineNotFoundError',
     'MalformedOcrOutputError',
     'MalformedHocrError',
     'EXIT_FATAL',
     'EXIT_NONFATAL',
     'fatal',
 ]
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/hocr.py` & `ocrodjvu-0.13.1/ocrodjvu/hocr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2008-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -449,33 +448,31 @@
     Extract DjVu text from an hOCR stream.
 
     details: TEXT_DETAILS_LINES or TEXT_DETAILS_WORD or TEXT_DETAILS_CHAR
     uax29: None or a PyICU locale
     """
     settings = ExtractSettings(**kwargs)
     doc = read_document(stream, settings)
-    ocr_system = doc.find('/head/meta[@name="ocr-system"]')
+    ocr_system = doc.find('./head/meta[@name="ocr-system"]')
     if ocr_system is None:
-        if doc.find('/head/meta[@name="ocr-capabilities"]') is None:
+        if doc.find('./head/meta[@name="ocr-capabilities"]') is None:
             # This is wild guess. However, since ocr-system is a required meta
             # tag, the hOCR we are processing is broken anyway.
             settings.cuneiform = (0, 8)
     elif ocr_system.get('content') == 'openocr':
         settings.cuneiform = (0, 9)
     elif ocr_system.get('content').split()[0] == 'tesseract':
         settings.tesseract = True
     if settings.details < TEXT_DETAILS_WORD or (settings.uax29 and settings.details <= text_zones.TEXT_DETAILS_WORD):
-        tesseract_bbox_data = doc.find('//script[@type="application/x-ocrodjvu-tesseract"]')
+        tesseract_bbox_data = doc.find('.//script[@type="application/x-ocrodjvu-tesseract"]')
         if tesseract_bbox_data is not None:
             settings.tesseract = True
             tesseract_bbox_data = extract_tesseract_bbox_data(tesseract_bbox_data)
             settings.bbox_data = tesseract_bbox_data
-    scan_result = scan(doc.find('/body'), settings)
+    scan_result = scan(doc.find('./body'), settings)
     return [zone.sexpr for zone in scan_result]
 
 
 __all__ = [
     'extract_text',
     'TEXT_DETAILS_LINE', 'TEXT_DETAILS_WORD', 'TEXT_DETAILS_CHARACTER'
 ]
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/html5_support.py` & `ocrodjvu-0.13.1/ocrodjvu/html5_support.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2011-2015 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -25,9 +24,7 @@
         utils.enhance_import_error(ex, 'html5lib', 'python-html5lib', 'https://github.com/html5lib/html5lib-python')
         raise
     return html5lib.parse(
         stream,
         treebuilder='lxml',
         namespaceHTMLElements=False
     )
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/image_io.py` & `ocrodjvu-0.13.1/ocrodjvu/image_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2008-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -183,9 +182,7 @@
         header += struct.pack('<HHII', 0x11B, 5, 1, 14),  # YResolution
         header += struct.pack('<I', 0),  # offset to next IFD
         assert len(header) == n_tags + 5
         header = b''.join(header)
         assert len(header) == data_offset
         file.write(header)
         file.write(data)
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/ipc.py` & `ocrodjvu-0.13.1/ocrodjvu/ipc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2008-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -187,9 +186,7 @@
 # =======
 
 __all__ = [
     'CalledProcessError', 'CalledProcessInterrupted',
     'Subprocess', 'PIPE', 'DEVNULL',
     'require',
 ]
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/iso639.py` & `ocrodjvu-0.13.1/ocrodjvu/iso639.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2013-2016 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -55,9 +54,7 @@
         raise TypeError
     if len(lang) != 3:
         if not permissive:
             raise ValueError(lang)
         else:
             return lang
     return _B_TO_T.get(lang, lang)
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/logger.py` & `ocrodjvu-0.13.1/ocrodjvu/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2011-2018 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -33,9 +32,7 @@
         handler.setFormatter(formatter)
         ipc_logger.addHandler(handler)
         ipc_logger.setLevel(logging.INFO)
     return logger
 
 
 __all__ = ['setup']
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/temporary.py` & `ocrodjvu-0.13.1/ocrodjvu/temporary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2009-2010 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -33,9 +32,7 @@
     try:
         yield tmpdir
     finally:
         shutil.rmtree(tmpdir)
 
 
 __all__ = ['raw', 'file', 'directory', 'name', 'wrapper']
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/text_zones.py` & `ocrodjvu-0.13.1/ocrodjvu/text_zones.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2008-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -221,9 +220,7 @@
             ]
         i = j
     return words
 
 
 def print_sexpr(expr, file, width=None):
     return expr.print_into(file, width=width, escape_unicode=False)
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/unicode_support.py` & `ocrodjvu-0.13.1/ocrodjvu/unicode_support.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2008-2018 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -50,9 +49,7 @@
     """
     if locale is None:
         return simple_word_break_iterator(text)
     icu = get_icu()
     break_iterator = icu.BreakIterator.createWordInstance(locale)
     break_iterator.setText(text)
     return break_iterator
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/utils.py` & `ocrodjvu-0.13.1/ocrodjvu/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2008-2022 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -188,9 +187,7 @@
         return 1
 
 
 def get_thread_limit(nitems, njobs):
     if nitems == 0:
         return 1
     return max(1, njobs // nitems)
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu/version.py` & `ocrodjvu-0.13.1/ocrodjvu/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# encoding=UTF-8
-
 # Copyright © 2016-2019 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
 #
 # This file is part of ocrodjvu.
 #
 # ocrodjvu is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 #
@@ -12,15 +11,15 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
 # FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License
 # for more details.
 
 import argparse
 import sys
 
-__version__ = '0.13'
+__version__ = '0.13.1'
 
 
 class VersionAction(argparse.Action):
     """
     argparse --version action
     """
 
@@ -67,9 +66,7 @@
         parser.exit()
 
 
 __all__ = [
     'VersionAction',
     '__version__',
 ]
-
-# vim:ts=4 sts=4 sw=4 et
```

### Comparing `ocrodjvu-0.13/ocrodjvu.egg-info/PKG-INFO` & `ocrodjvu-0.13.1/ocrodjvu.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrodjvu
-Version: 0.13
+Version: 0.13.1
 Summary: OCR for DjVu (Python 3 fork)
 Home-page: https://github.com/FriedrichFroebel/ocrodjvu/
 Author: Jakub Wilk, FriedrichFröbel (Python 3)
 License: GNU GPL 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -13,17 +13,25 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/x-rst
+License-File: COPYING
+Requires-Dist: python-djvulibre>=0.4
+Requires-Dist: lxml>=2.0
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pep8-naming; extra == "dev"
+Requires-Dist: Pillow; extra == "dev"
 Provides-Extra: docs
-License-File: COPYING
+Requires-Dist: docutils; extra == "docs"
+Requires-Dist: pygments; extra == "docs"
 
 Overview
 ========
 
 **ocrodjvu** is a wrapper for OCR systems that allows you to perform OCR on DjVu_ files.
 
 .. _DjVu:
@@ -67,18 +75,22 @@
 * an OCR engine:
 
   + Cuneiform_ ≥ 0.7
   + Ocrad_ ≥ 0.10
   + GOCR_ ≥ 0.40
   + Tesseract_ ≥ 2.00
 
-* DjVuLibre_ ≥ 3.5.21
+* DjVuLibre_ ≥ 3.5.21 (≥ 3.5.26 for latest python-djvulibre)
 
 * python-djvulibre_ ≥ 0.4
 
+  + Please note that installing this package currently is a bit more complicated since Cython 3 has been relased on 2023-07-17.
+  + While `Issue #11`_ is unresolved, PyPI releases require some workarounds (installing the package from the source archive with the deprecated ``python setup.py install`` beforehand).
+  + Alternative: Install the latest package version from `Git <python-djvulibre-git_>`_.
+
 * lxml_ ≥ 2.0
 
 Additionally, some optional features require the following software:
 
 * PyICU_ ≥ 1.0.1 —
   required for the ``--word-segmentation=uax29`` option
 
@@ -102,31 +114,39 @@
    https://www-e.uni-magdeburg.de/jschulen/ocr/
 .. _Tesseract:
    https://github.com/tesseract-ocr/tesseract
 .. _DjVuLibre:
    http://djvu.sourceforge.net/
 .. _python-djvulibre:
    https://jwilk.net/software/python-djvulibre
+.. _Issue #11:
+   https://github.com/FriedrichFroebel/python-djvulibre/issues/11
+.. _python-djvulibre-git:
+   https://github.com/FriedrichFroebel/python-djvulibre
 .. _lxml:
    https://lxml.de/
 .. _PyICU:
    https://pypi.org/project/PyICU/
 .. _html5lib:
    https://github.com/html5lib/html5lib-python
 .. _xsltproc:
    http://xmlsoft.org/XSLT/xsltproc2.html
 .. _DocBook XSL stylesheets:
    https://github.com/docbook/xslt10-stylesheets
 
 Installation
 ============
 
-You can use ocrodjvu without installing it, straight out of unpacked source tarball or a VCS checkout.
+The easiest way to install ocrodjvu is from PyPI::
+
+    pip install ocrodjvu
+
+Alternatively, you can use ocrodjvu without installing it, straight out of an unpacked source tarball or a VCS checkout.
 
-It's also possible to install it system-wide with::
+It's also possible to install it from source for the current interpreter with::
 
    pip install .
 
 The man pages can be deployed using::
 
    make install_manpage
```

### Comparing `ocrodjvu-0.13/ocrodjvu.egg-info/SOURCES.txt` & `ocrodjvu-0.13.1/ocrodjvu.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 COPYING
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 doc/changelog
 ocrodjvu/__init__.py
 ocrodjvu/__main__.py
 ocrodjvu/errors.py
 ocrodjvu/hocr.py
 ocrodjvu/html5_support.py
@@ -29,8 +30,12 @@
 ocrodjvu/cli/ocrodjvu.py
 ocrodjvu/engines/__init__.py
 ocrodjvu/engines/common.py
 ocrodjvu/engines/cuneiform.py
 ocrodjvu/engines/dummy.py
 ocrodjvu/engines/gocr.py
 ocrodjvu/engines/ocrad.py
-ocrodjvu/engines/tesseract.py
+ocrodjvu/engines/tesseract.py
+tests/test_ipc.py
+tests/test_text_zones.py
+tests/test_unicode_support.py
+tests/test_utils.py
```

### Comparing `ocrodjvu-0.13/setup.py` & `ocrodjvu-0.13.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,21 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
+# Copyright © 2009-2019 Jakub Wilk <jwilk@jwilk.net>
+# Copyright © 2022-2024 FriedrichFroebel
+#
+# This file is part of ocrodjvu.
+#
+# ocrodjvu is free software; you can redistribute it and/or modify it
+# under the terms of the GNU General Public License version 2 as
+# published by the Free Software Foundation.
+#
+# ocrodjvu is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
+# FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License
+# for more details.
+
 from setuptools import setup, find_packages
 from pathlib import Path
 
 
 ROOT_DIRECTORY = Path(__file__).parent.resolve()
```

