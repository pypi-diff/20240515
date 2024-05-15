# Comparing `tmp/python-datauri-2.1.0.tar.gz` & `tmp/python_datauri-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-datauri-2.1.0.tar", last modified: Wed Jul 19 15:55:28 2023, max compression
+gzip compressed data, was "python_datauri-2.1.1.tar", last modified: Wed May 15 01:27:58 2024, max compression
```

## Comparing `python-datauri-2.1.0.tar` & `python_datauri-2.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.544588 python-datauri-2.1.0/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1211 2020-07-31 14:49:13.000000 python-datauri-2.1.0/LICENSE
--rw-r--r--   0 flavio.curella   (502) staff       (20)      231 2023-05-26 15:55:57.000000 python-datauri-2.1.0/MANIFEST.in
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3323 2023-07-19 15:55:28.544836 python-datauri-2.1.0/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)     2579 2023-07-19 15:52:28.000000 python-datauri-2.1.0/README.rst
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.536380 python-datauri-2.1.0/datauri/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     5493 2023-07-19 15:51:43.000000 python-datauri-2.1.0/datauri/__init__.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      134 2020-07-31 14:49:13.000000 python-datauri-2.1.0/datauri/exceptions.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)        0 2023-05-26 15:53:10.000000 python-datauri-2.1.0/datauri/py.typed
--rw-r--r--   0 flavio.curella   (502) staff       (20)      296 2023-05-26 15:52:20.000000 python-datauri-2.1.0/mypy.ini
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.539815 python-datauri-2.1.0/python_datauri.egg-info/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3323 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)      462 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/SOURCES.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/dependency_links.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       18 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/requires.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       14 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/top_level.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)      197 2023-07-19 15:55:28.545974 python-datauri-2.1.0/setup.cfg
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1247 2023-07-19 15:55:12.000000 python-datauri-2.1.0/setup.py
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.542029 python-datauri-2.1.0/tests/
--rw-r--r--   0 flavio.curella   (502) staff       (20)        0 2020-07-31 14:49:13.000000 python-datauri-2.1.0/tests/__init__.py
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.544023 python-datauri-2.1.0/tests/assets/
--rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python-datauri-2.1.0/tests/assets/test_file.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python-datauri-2.1.0/tests/assets/test_file_ebcdic.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3324 2020-07-31 14:49:13.000000 python-datauri-2.1.0/tests/assets/test_long_file.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)     5549 2023-05-26 19:56:28.000000 python-datauri-2.1.0/tests/test_parsing.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      596 2023-05-26 20:10:51.000000 python-datauri-2.1.0/tests/test_pydantic.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2024-05-15 01:27:58.456507 python_datauri-2.1.1/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     1211 2020-07-31 14:49:13.000000 python_datauri-2.1.1/LICENSE
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      231 2023-05-26 15:55:57.000000 python_datauri-2.1.1/MANIFEST.in
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     3326 2024-05-15 01:27:58.456279 python_datauri-2.1.1/PKG-INFO
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     2549 2024-05-15 01:25:39.000000 python_datauri-2.1.1/README.rst
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2024-05-15 01:27:58.450286 python_datauri-2.1.1/datauri/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     5493 2023-07-19 15:51:43.000000 python_datauri-2.1.1/datauri/__init__.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      134 2020-07-31 14:49:13.000000 python_datauri-2.1.1/datauri/exceptions.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        0 2023-05-26 15:53:10.000000 python_datauri-2.1.1/datauri/py.typed
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      296 2023-05-26 15:52:20.000000 python_datauri-2.1.1/mypy.ini
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2024-05-15 01:27:58.455536 python_datauri-2.1.1/python_datauri.egg-info/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     3326 2024-05-15 01:27:58.000000 python_datauri-2.1.1/python_datauri.egg-info/PKG-INFO
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      462 2024-05-15 01:27:58.000000 python_datauri-2.1.1/python_datauri.egg-info/SOURCES.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2024-05-15 01:27:58.000000 python_datauri-2.1.1/python_datauri.egg-info/dependency_links.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       18 2024-05-15 01:27:58.000000 python_datauri-2.1.1/python_datauri.egg-info/requires.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        8 2024-05-15 01:27:58.000000 python_datauri-2.1.1/python_datauri.egg-info/top_level.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      197 2024-05-15 01:27:58.457445 python_datauri-2.1.1/setup.cfg
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     1256 2024-05-15 01:26:00.000000 python_datauri-2.1.1/setup.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2024-05-15 01:27:58.453201 python_datauri-2.1.1/tests/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        0 2020-07-31 14:49:13.000000 python_datauri-2.1.1/tests/__init__.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2024-05-15 01:27:58.454802 python_datauri-2.1.1/tests/assets/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python_datauri-2.1.1/tests/assets/test_file.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python_datauri-2.1.1/tests/assets/test_file_ebcdic.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     3324 2020-07-31 14:49:13.000000 python_datauri-2.1.1/tests/assets/test_long_file.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     5549 2023-05-26 19:56:28.000000 python_datauri-2.1.1/tests/test_parsing.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      596 2023-05-26 20:10:51.000000 python_datauri-2.1.1/tests/test_pydantic.py
```

### Comparing `python-datauri-2.1.0/LICENSE` & `python_datauri-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-datauri-2.1.0/PKG-INFO` & `python_datauri-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-datauri
-Version: 2.1.0
+Version: 2.1.1
 Summary: A li'l class for data URI manipulation in Python
 Home-page: https://github.com/fcurella/python-datauri/
 Maintainer: Flavio Curella
 Maintainer-email: flavio.curella@gmail.com
 License: Unlicense
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
+Requires-Dist: typing_extensions
 
 DataURI
 =======
 
 .. image:: https://github.com/fcurella/python-datauri/workflows/Python%20Tests/badge.svg
     :target: https://github.com/fcurella/python-datauri/actions?query=workflow%3A%22Python+Tests%22
     :alt: Build status of the master branch on Mac/Linux
@@ -103,15 +104,14 @@
 ----------------
 
 You can use `DataURI` as a type for `Pydantic` v1:
 
 .. code-block:: python
 
   from datauri import DataURI
-  from datauri import DataURI
   from pydantic import BaseModel
 
 
   class ProfilePicture(BaseModel):
     image_data: DataURI
 
 License
```

### Comparing `python-datauri-2.1.0/README.rst` & `python_datauri-2.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 ----------------
 
 You can use `DataURI` as a type for `Pydantic` v1:
 
 .. code-block:: python
 
   from datauri import DataURI
-  from datauri import DataURI
   from pydantic import BaseModel
 
 
   class ProfilePicture(BaseModel):
     image_data: DataURI
 
 License
```

### Comparing `python-datauri-2.1.0/datauri/__init__.py` & `python_datauri-2.1.1/datauri/__init__.py`

 * *Files identical despite different names*

### Comparing `python-datauri-2.1.0/python_datauri.egg-info/PKG-INFO` & `python_datauri-2.1.1/python_datauri.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-datauri
-Version: 2.1.0
+Version: 2.1.1
 Summary: A li'l class for data URI manipulation in Python
 Home-page: https://github.com/fcurella/python-datauri/
 Maintainer: Flavio Curella
 Maintainer-email: flavio.curella@gmail.com
 License: Unlicense
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
+Requires-Dist: typing_extensions
 
 DataURI
 =======
 
 .. image:: https://github.com/fcurella/python-datauri/workflows/Python%20Tests/badge.svg
     :target: https://github.com/fcurella/python-datauri/actions?query=workflow%3A%22Python+Tests%22
     :alt: Build status of the master branch on Mac/Linux
@@ -103,15 +104,14 @@
 ----------------
 
 You can use `DataURI` as a type for `Pydantic` v1:
 
 .. code-block:: python
 
   from datauri import DataURI
-  from datauri import DataURI
   from pydantic import BaseModel
 
 
   class ProfilePicture(BaseModel):
     image_data: DataURI
 
 License
```

### Comparing `python-datauri-2.1.0/setup.py` & `python_datauri-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import find_packages, setup
 
-VERSION = "2.1.0"
+VERSION = "2.1.1"
 
 
 def read(fname):
     try:
         with open(os.path.join(os.path.dirname(__file__), fname)) as fh:
             return fh.read()
     except IOError:
@@ -18,15 +18,15 @@
     version=VERSION,
     url="https://github.com/fcurella/python-datauri/",
     maintainer="Flavio Curella",
     maintainer_email="flavio.curella@gmail.com",
     description="A li'l class for data URI manipulation in Python",
     long_description=read("README.rst"),
     license="Unlicense",
-    packages=find_packages(exclude=["*.tests"]),
+    packages=find_packages(exclude=["tests", "*.tests"]),
     package_data={
         "faker": ["py.typed"],
     },
     platforms=["any"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: The Unlicense (Unlicense)",
```

### Comparing `python-datauri-2.1.0/tests/assets/test_long_file.txt` & `python_datauri-2.1.1/tests/assets/test_long_file.txt`

 * *Files identical despite different names*

### Comparing `python-datauri-2.1.0/tests/test_parsing.py` & `python_datauri-2.1.1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `python-datauri-2.1.0/tests/test_pydantic.py` & `python_datauri-2.1.1/tests/test_pydantic.py`

 * *Files identical despite different names*

