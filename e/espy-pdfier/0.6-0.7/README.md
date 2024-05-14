# Comparing `tmp/espy_pdfier-0.6.tar.gz` & `tmp/espy_pdfier-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_pdfier-0.6.tar", last modified: Sun May 12 18:07:38 2024, max compression
+gzip compressed data, was "espy_pdfier-0.7.tar", last modified: Tue May 14 20:34:47 2024, max compression
```

## Comparing `espy_pdfier-0.6.tar` & `espy_pdfier-0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 18:07:38.672979 espy_pdfier-0.6/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-05 23:47:48.000000 espy_pdfier-0.6/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-12 18:07:38.672721 espy_pdfier-0.6/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      120 2024-05-06 00:37:08.000000 espy_pdfier-0.6/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 18:07:38.669710 espy_pdfier-0.6/espy_pdfier/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:00:35.000000 espy_pdfier-0.6/espy_pdfier/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 18:07:38.671223 espy_pdfier-0.6/espy_pdfier/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-05 23:40:00.000000 espy_pdfier-0.6/espy_pdfier/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2039 2024-05-12 18:05:21.000000 espy_pdfier-0.6/espy_pdfier/service/img_serv.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2855 2024-05-06 00:31:42.000000 espy_pdfier-0.6/espy_pdfier/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 18:07:38.671914 espy_pdfier-0.6/espy_pdfier/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1083 2024-05-12 17:18:43.000000 espy_pdfier-0.6/espy_pdfier/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-11 23:21:45.000000 espy_pdfier-0.6/espy_pdfier/util/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 18:07:38.672207 espy_pdfier-0.6/espy_pdfier.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-12 18:07:38.000000 espy_pdfier-0.6/espy_pdfier.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      378 2024-05-12 18:07:38.000000 espy_pdfier-0.6/espy_pdfier.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-12 18:07:38.000000 espy_pdfier-0.6/espy_pdfier.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       48 2024-05-12 18:07:38.000000 espy_pdfier-0.6/espy_pdfier.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       12 2024-05-12 18:07:38.000000 espy_pdfier-0.6/espy_pdfier.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-12 18:07:38.673197 espy_pdfier-0.6/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      607 2024-05-12 18:07:31.000000 espy_pdfier-0.6/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.786586 espy_pdfier-0.7/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-05 23:47:48.000000 espy_pdfier-0.7/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-14 20:34:47.786333 espy_pdfier-0.7/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      120 2024-05-06 00:37:08.000000 espy_pdfier-0.7/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.784001 espy_pdfier-0.7/espy_pdfier/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:00:35.000000 espy_pdfier-0.7/espy_pdfier/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.785230 espy_pdfier-0.7/espy_pdfier/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-05 23:40:00.000000 espy_pdfier-0.7/espy_pdfier/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2497 2024-05-14 20:32:38.000000 espy_pdfier-0.7/espy_pdfier/service/img_serv.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2855 2024-05-06 00:31:42.000000 espy_pdfier-0.7/espy_pdfier/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.785909 espy_pdfier-0.7/espy_pdfier/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1083 2024-05-12 17:18:43.000000 espy_pdfier-0.7/espy_pdfier/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-11 23:21:45.000000 espy_pdfier-0.7/espy_pdfier/util/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.786076 espy_pdfier-0.7/espy_pdfier.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      378 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       48 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       12 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-14 20:34:47.786637 espy_pdfier-0.7/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      607 2024-05-14 20:33:02.000000 espy_pdfier-0.7/setup.py
```

### Comparing `espy_pdfier-0.6/LICENSE` & `espy_pdfier-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_pdfier-0.6/espy_pdfier/service/service.py` & `espy_pdfier-0.7/espy_pdfier/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_pdfier-0.6/espy_pdfier/util/CONSTANTS.py` & `espy_pdfier-0.7/espy_pdfier/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_pdfier-0.6/setup.py` & `espy_pdfier-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.3'
 DESCRIPTION = 'ESSL assets management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL assets management'
 setup(
     name='espy_pdfier',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     install_requires=[
         'reportlab==4.2.0',
         'pillow==10.3.0',
         'boto3==1.34.103',
         ],
     author='Femi Adigun',
```

