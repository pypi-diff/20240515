# Comparing `tmp/rtisdevremotepy-2.14.0.tar.gz` & `tmp/rtisdevremotepy-2.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\woute\Projects\rtisdevremotepy\dist\.tmp-hmakbs83\rtisdevremotepy-2.14.0.tar", last modified: Tue May 14 06:52:01 2024, max compression
+gzip compressed data, was "C:\Users\woute\Projects\rtisdevremotepy\dist\.tmp-46qtipp1\rtisdevremotepy-2.14.1.tar", last modified: Wed May 15 14:41:51 2024, max compression
```

## Comparing `rtisdevremotepy-2.14.0.tar` & `rtisdevremotepy-2.14.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/
--rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdevremotepy-2.14.0/LICENSE
--rw-rw-rw-   0        0        0       37 2024-04-05 06:55:48.000000 rtisdevremotepy-2.14.0/MANIFEST.in
--rw-rw-rw-   0        0        0    32556 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/PKG-INFO
--rw-rw-rw-   0        0        0     6641 2024-05-14 06:48:35.000000 rtisdevremotepy-2.14.0/README.md
--rw-rw-rw-   0        0        0     1449 2024-05-14 06:48:35.000000 rtisdevremotepy-2.14.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/
--rw-rw-rw-   0        0        0    63899 2024-05-14 06:48:35.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/RTISDevRemotePy.py
--rw-rw-rw-   0        0        0     5515 2024-05-14 06:48:35.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/
--rw-rw-rw-   0        0        0    19280 2024-03-29 14:16:26.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/RTISDevRemote.py
--rw-rw-rw-   0        0        0     1314 2024-03-29 14:16:26.000000 rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/
--rw-rw-rw-   0        0        0    32556 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 06:52:01.000000 rtisdevremotepy-2.14.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/
+-rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdevremotepy-2.14.1/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-04-05 06:55:48.000000 rtisdevremotepy-2.14.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    32556 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6641 2024-05-15 14:40:08.000000 rtisdevremotepy-2.14.1/README.md
+-rw-rw-rw-   0        0        0     1449 2024-05-15 14:40:08.000000 rtisdevremotepy-2.14.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/rtisdevremotepy/
+-rw-rw-rw-   0        0        0    63899 2024-05-15 14:40:08.000000 rtisdevremotepy-2.14.1/rtisdevremotepy/RTISDevRemotePy.py
+-rw-rw-rw-   0        0        0     5515 2024-05-15 14:40:08.000000 rtisdevremotepy-2.14.1/rtisdevremotepy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/rtisdevremotepy/rtisdevremote/
+-rw-rw-rw-   0        0        0    19280 2024-03-29 14:16:26.000000 rtisdevremotepy-2.14.1/rtisdevremotepy/rtisdevremote/RTISDevRemote.py
+-rw-rw-rw-   0        0        0     1314 2024-03-29 14:16:26.000000 rtisdevremotepy-2.14.1/rtisdevremotepy/rtisdevremote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/rtisdevremotepy.egg-info/
+-rw-rw-rw-   0        0        0    32556 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/rtisdevremotepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/rtisdevremotepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/rtisdevremotepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/rtisdevremotepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/rtisdevremotepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:41:51.000000 rtisdevremotepy-2.14.1/setup.cfg
```

### Comparing `rtisdevremotepy-2.14.0/LICENSE` & `rtisdevremotepy-2.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rtisdevremotepy-2.14.0/PKG-INFO` & `rtisdevremotepy-2.14.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdevremotepy
-Version: 2.14.0
+Version: 2.14.1
 Summary: Python wrapper for using RTIS Dev remotely
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
@@ -471,15 +471,15 @@
 
 ## Installation
 
 ### Dependencies
 * Python 3.6 or higher with modules:
   * Numpy
   * Scipy
-* Supported RTIS Dev version is v2.14.0.
+* Supported RTIS Dev version is v2.14.1.
 
 ### From PyPi
 You can install this module from the [PyPi repository](https://pypi.org/project/rtisdevremotepy/) like any other:
 ```bash
 pip install rtisdevremotepy
 ```
```

### Comparing `rtisdevremotepy-2.14.0/README.md` & `rtisdevremotepy-2.14.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## Installation
 
 ### Dependencies
 * Python 3.6 or higher with modules:
   * Numpy
   * Scipy
-* Supported RTIS Dev version is v2.14.0.
+* Supported RTIS Dev version is v2.14.1.
 
 ### From PyPi
 You can install this module from the [PyPi repository](https://pypi.org/project/rtisdevremotepy/) like any other:
 ```bash
 pip install rtisdevremotepy
 ```
```

### Comparing `rtisdevremotepy-2.14.0/pyproject.toml` & `rtisdevremotepy-2.14.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rtisdevremotepy"
-version = "2.14.0"
+version = "2.14.1"
 description = "Python wrapper for using RTIS Dev remotely"
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [{ name = "Wouter Jansen", email = "wouter.jansen@uantwerpen.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 6 - Mature",
     "Programming Language :: Python",
```

### Comparing `rtisdevremotepy-2.14.0/rtisdevremotepy/RTISDevRemotePy.py` & `rtisdevremotepy-2.14.1/rtisdevremotepy/RTISDevRemotePy.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     >>> plt.show()
 """
 
 from typing import List
 from rtisdevremotepy.rtisdevremote import RTISDevRemote
 
 # Global settings
-RTISDEV_VERSION = "2.14.0"
+RTISDEV_VERSION = "2.14.1"
 
 
 class RTISDev:
     """This is class describing a wrapper of the RTIS Dev Remote library to
     %   use RTIS Dev remotely over self.ip from Python. Quickly develop with connected RTIS devices.
     %   Almost all RTIS Dev functions are available as well as automatic conversion of RTIS Dev custom class objects.
```

### Comparing `rtisdevremotepy-2.14.0/rtisdevremotepy/__init__.py` & `rtisdevremotepy-2.14.1/rtisdevremotepy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,8 +103,8 @@
     >>> plt.title("RTIS Dev - 2D Energyscape Example")
     >>> ax = plt.gca()
     >>> ax.invert_yaxis()
     >>> ax.set_aspect("auto")
     >>> plt.show()
 """
 from .RTISDevRemotePy import *
-__version__ = "2.14.0"
+__version__ = "2.14.1"
```

### Comparing `rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/RTISDevRemote.py` & `rtisdevremotepy-2.14.1/rtisdevremotepy/rtisdevremote/RTISDevRemote.py`

 * *Files identical despite different names*

### Comparing `rtisdevremotepy-2.14.0/rtisdevremotepy/rtisdevremote/__init__.py` & `rtisdevremotepy-2.14.1/rtisdevremotepy/rtisdevremote/__init__.py`

 * *Files identical despite different names*

### Comparing `rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/PKG-INFO` & `rtisdevremotepy-2.14.1/rtisdevremotepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdevremotepy
-Version: 2.14.0
+Version: 2.14.1
 Summary: Python wrapper for using RTIS Dev remotely
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
@@ -471,15 +471,15 @@
 
 ## Installation
 
 ### Dependencies
 * Python 3.6 or higher with modules:
   * Numpy
   * Scipy
-* Supported RTIS Dev version is v2.14.0.
+* Supported RTIS Dev version is v2.14.1.
 
 ### From PyPi
 You can install this module from the [PyPi repository](https://pypi.org/project/rtisdevremotepy/) like any other:
 ```bash
 pip install rtisdevremotepy
 ```
```

### Comparing `rtisdevremotepy-2.14.0/rtisdevremotepy.egg-info/SOURCES.txt` & `rtisdevremotepy-2.14.1/rtisdevremotepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

