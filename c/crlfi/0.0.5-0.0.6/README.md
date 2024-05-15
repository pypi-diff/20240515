# Comparing `tmp/crlfi-0.0.5.tar.gz` & `tmp/crlfi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crlfi-0.0.5.tar", last modified: Mon Apr 29 16:41:23 2024, max compression
+gzip compressed data, was "crlfi-0.0.6.tar", last modified: Wed May 15 08:17:11 2024, max compression
```

## Comparing `crlfi-0.0.5.tar` & `crlfi-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.191813 crlfi-0.0.5/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1074 2024-04-29 16:39:36.000000 crlfi-0.0.5/LICENSE
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4752 2024-04-29 16:41:23.191637 crlfi-0.0.5/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4299 2024-04-29 16:39:36.000000 crlfi-0.0.5/README.md
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.185231 crlfi-0.0.5/crlfi/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/__init__.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.189848 crlfi-0.0.5/crlfi/includes/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/includes/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      633 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/includes/bot.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      458 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/includes/filereader.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     2256 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/includes/scan.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      267 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/includes/writefile.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1736 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/main.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.191315 crlfi-0.0.5/crlfi/utils/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/utils/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1948 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/utils/configure.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      662 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/utils/const.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1697 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/utils/helpers.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      227 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/utils/status.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.188189 crlfi-0.0.5/crlfi.egg-info/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4752 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)      478 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/SOURCES.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/dependency_links.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       42 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/entry_points.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/requires.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)        6 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/top_level.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-04-29 16:41:23.191873 crlfi-0.0.5/setup.cfg
--rw-r--r--   0 karthikeyan   (501) staff       (20)      980 2024-04-29 16:41:19.000000 crlfi-0.0.5/setup.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-15 08:17:11.090947 crlfi-0.0.6/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1074 2024-04-29 16:39:36.000000 crlfi-0.0.6/LICENSE
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4752 2024-05-15 08:17:11.090743 crlfi-0.0.6/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4299 2024-04-29 16:39:36.000000 crlfi-0.0.6/README.md
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-15 08:17:11.080326 crlfi-0.0.6/crlfi/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:39:36.000000 crlfi-0.0.6/crlfi/__init__.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-15 08:17:11.088023 crlfi-0.0.6/crlfi/includes/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:39:36.000000 crlfi-0.0.6/crlfi/includes/__init__.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      633 2024-04-29 16:40:08.000000 crlfi-0.0.6/crlfi/includes/bot.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      458 2024-04-29 16:40:08.000000 crlfi-0.0.6/crlfi/includes/filereader.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     2256 2024-04-29 16:40:08.000000 crlfi-0.0.6/crlfi/includes/scan.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      267 2024-04-29 16:39:36.000000 crlfi-0.0.6/crlfi/includes/writefile.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1736 2024-04-29 16:40:08.000000 crlfi-0.0.6/crlfi/main.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-15 08:17:11.090055 crlfi-0.0.6/crlfi/utils/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:39:36.000000 crlfi-0.0.6/crlfi/utils/__init__.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1948 2024-04-29 16:40:08.000000 crlfi-0.0.6/crlfi/utils/configure.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      803 2024-05-15 08:16:51.000000 crlfi-0.0.6/crlfi/utils/const.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1697 2024-04-29 16:39:36.000000 crlfi-0.0.6/crlfi/utils/helpers.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      227 2024-04-29 16:39:36.000000 crlfi-0.0.6/crlfi/utils/status.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-15 08:17:11.081484 crlfi-0.0.6/crlfi.egg-info/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4752 2024-05-15 08:17:11.000000 crlfi-0.0.6/crlfi.egg-info/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      478 2024-05-15 08:17:11.000000 crlfi-0.0.6/crlfi.egg-info/SOURCES.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-05-15 08:17:11.000000 crlfi-0.0.6/crlfi.egg-info/dependency_links.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       42 2024-05-15 08:17:11.000000 crlfi-0.0.6/crlfi.egg-info/entry_points.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-05-15 08:17:11.000000 crlfi-0.0.6/crlfi.egg-info/requires.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        6 2024-05-15 08:17:11.000000 crlfi-0.0.6/crlfi.egg-info/top_level.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-05-15 08:17:11.091270 crlfi-0.0.6/setup.cfg
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      980 2024-05-15 08:16:15.000000 crlfi-0.0.6/setup.py
```

### Comparing `crlfi-0.0.5/LICENSE` & `crlfi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.5/PKG-INFO` & `crlfi-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crlfi
-Version: 0.0.5
+Version: 0.0.6
 Author: @cappriciosec
 Author-email: <contact@cappriciosec.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crlfi Version: 0.0.5 Author: @cappriciosec Author-
+Metadata-Version: 2.1 Name: crlfi Version: 0.0.6 Author: @cappriciosec Author-
 email:
 cappriciosec.com> Classifier: Development Status :: 1 - Planning Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
 Content-Type: text/markdown License-File: LICENSE
                                     [logo]
```

### Comparing `crlfi-0.0.5/README.md` & `crlfi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.5/crlfi/includes/bot.py` & `crlfi-0.0.6/crlfi/includes/bot.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.5/crlfi/includes/scan.py` & `crlfi-0.0.6/crlfi/includes/scan.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.5/crlfi/main.py` & `crlfi-0.0.6/crlfi/main.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.5/crlfi/utils/configure.py` & `crlfi-0.0.6/crlfi/utils/configure.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.5/crlfi/utils/helpers.py` & `crlfi-0.0.6/crlfi/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.5/crlfi.egg-info/PKG-INFO` & `crlfi-0.0.6/crlfi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crlfi
-Version: 0.0.5
+Version: 0.0.6
 Author: @cappriciosec
 Author-email: <contact@cappriciosec.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crlfi Version: 0.0.5 Author: @cappriciosec Author-
+Metadata-Version: 2.1 Name: crlfi Version: 0.0.6 Author: @cappriciosec Author-
 email:
 cappriciosec.com> Classifier: Development Status :: 1 - Planning Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
 Content-Type: text/markdown License-File: LICENSE
                                     [logo]
```

### Comparing `crlfi-0.0.5/setup.py` & `crlfi-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A Tool to find an Easy Bounty - crlfi'
 LONG_DESCRIPTION = 'This is a tool used by several security researchers to find Carriage Return Line Feed Injection Bug'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
```

