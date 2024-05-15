# Comparing `tmp/unipress-1.1.tar.gz` & `tmp/unipress-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipress-1.1.tar", last modified: Fri Oct  6 11:03:30 2023, max compression
+gzip compressed data, was "unipress-1.3.tar", last modified: Wed May 15 12:31:45 2024, max compression
```

## Comparing `unipress-1.1.tar` & `unipress-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 konrad   (17021) konrad   (17021)        0 2023-10-06 11:03:30.713914 unipress-1.1/
--rw-r--r--   0 konrad   (17021) konrad   (17021)    11357 2020-02-04 13:48:50.000000 unipress-1.1/LICENSE
--rw-------   0 konrad   (17021) konrad   (17021)     1060 2023-10-06 11:03:30.713914 unipress-1.1/PKG-INFO
--rw-------   0 konrad   (17021) konrad   (17021)      584 2023-10-03 15:32:26.000000 unipress-1.1/README.md
--rw-------   0 konrad   (17021) konrad   (17021)       38 2023-10-06 11:03:30.713914 unipress-1.1/setup.cfg
--rw-------   0 konrad   (17021) konrad   (17021)      726 2023-10-06 10:55:18.000000 unipress-1.1/setup.py
-drwx------   0 konrad   (17021) konrad   (17021)        0 2023-10-06 11:03:30.713914 unipress-1.1/unipress/
--rw-------   0 konrad   (17021) konrad   (17021)      929 2023-10-03 15:32:26.000000 unipress-1.1/unipress/__init__.py
--rw-------   0 konrad   (17021) konrad   (17021)     2828 2023-10-03 15:32:26.000000 unipress-1.1/unipress/approximations.py
-drwx------   0 konrad   (17021) konrad   (17021)        0 2023-10-06 11:03:30.713914 unipress-1.1/unipress.egg-info/
--rw-------   0 konrad   (17021) konrad   (17021)     1060 2023-10-06 11:03:30.000000 unipress-1.1/unipress.egg-info/PKG-INFO
--rw-------   0 konrad   (17021) konrad   (17021)      233 2023-10-06 11:03:30.000000 unipress-1.1/unipress.egg-info/SOURCES.txt
--rw-------   0 konrad   (17021) konrad   (17021)        1 2023-10-06 11:03:30.000000 unipress-1.1/unipress.egg-info/dependency_links.txt
--rw-------   0 konrad   (17021) konrad   (17021)       12 2023-10-06 11:03:30.000000 unipress-1.1/unipress.egg-info/requires.txt
--rw-------   0 konrad   (17021) konrad   (17021)        9 2023-10-06 11:03:30.000000 unipress-1.1/unipress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:31:45.614528 unipress-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 12:31:42.000000 unipress-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 12:31:45.614528 unipress-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-15 12:31:42.000000 unipress-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:31:45.614528 unipress-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-15 12:31:42.000000 unipress-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:31:45.610528 unipress-1.3/unipress/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-15 12:31:42.000000 unipress-1.3/unipress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-15 12:31:42.000000 unipress-1.3/unipress/approximations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:31:45.614528 unipress-1.3/unipress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 12:31:45.000000 unipress-1.3/unipress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-15 12:31:45.000000 unipress-1.3/unipress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:31:45.000000 unipress-1.3/unipress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:31:45.000000 unipress-1.3/unipress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 12:31:45.000000 unipress-1.3/unipress.egg-info/top_level.txt
```

### Comparing `unipress-1.1/LICENSE` & `unipress-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unipress-1.1/README.md` & `unipress-1.3/README.md`

 * *Files identical despite different names*

### Comparing `unipress-1.1/setup.py` & `unipress-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="unipress",
-	version="1.1",
+	version="1.3",
 	author="Konrad Sakowski",
 	description="This is a library developed by Institute of High Pressure Physics of Polish Academy of Sciences.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	packages=setuptools.find_packages(),
 	classifiers=[
 		"Programming Language :: Python :: 3",
```

### Comparing `unipress-1.1/unipress/approximations.py` & `unipress-1.3/unipress/approximations.py`

 * *Files identical despite different names*

