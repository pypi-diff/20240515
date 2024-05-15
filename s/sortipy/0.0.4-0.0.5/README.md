# Comparing `tmp/sortipy-0.0.4.tar.gz` & `tmp/sortipy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortipy-0.0.4.tar", last modified: Tue May 14 21:18:18 2024, max compression
+gzip compressed data, was "sortipy-0.0.5.tar", last modified: Tue May 14 21:24:44 2024, max compression
```

## Comparing `sortipy-0.0.4.tar` & `sortipy-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.535372 sortipy-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-05-14 10:16:33.000000 sortipy-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-14 10:57:17.000000 sortipy-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3198 2024-05-14 21:18:18.535372 sortipy-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2801 2024-05-14 21:17:57.000000 sortipy-0.0.4/README.md
--rw-rw-rw-   0        0        0       86 2024-05-14 10:58:30.000000 sortipy-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 21:18:18.535372 sortipy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      551 2024-05-14 21:17:52.000000 sortipy-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.455435 sortipy-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.475577 sortipy-0.0.4/src/sortipy/
--rw-rw-rw-   0        0        0        0 2024-05-14 10:25:51.000000 sortipy-0.0.4/src/sortipy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.516987 sortipy-0.0.4/src/sortipy/exceptions/
--rw-rw-rw-   0        0        0        0 2024-05-14 12:17:07.000000 sortipy-0.0.4/src/sortipy/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1546 2024-05-14 18:48:33.000000 sortipy-0.0.4/src/sortipy/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.526970 sortipy-0.0.4/src/sortipy/models/
--rw-rw-rw-   0        0        0     1726 2024-05-14 21:16:43.000000 sortipy-0.0.4/src/sortipy/models/Directory.py
--rw-rw-rw-   0        0        0     2058 2024-05-14 21:16:47.000000 sortipy-0.0.4/src/sortipy/models/File.py
--rw-rw-rw-   0        0        0        0 2024-05-14 12:14:42.000000 sortipy-0.0.4/src/sortipy/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.530863 sortipy-0.0.4/src/sortipy/sorters/
--rw-rw-rw-   0        0        0     1466 2024-05-14 21:17:07.000000 sortipy-0.0.4/src/sortipy/sorters/DefaultSorter.py
--rw-rw-rw-   0        0        0        0 2024-05-14 18:53:00.000000 sortipy-0.0.4/src/sortipy/sorters/__init__.py
--rw-rw-rw-   0        0        0     1141 2024-05-14 21:16:36.000000 sortipy-0.0.4/src/sortipy/sortipy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:18:18.533805 sortipy-0.0.4/src/sortipy.egg-info/
--rw-rw-rw-   0        0        0     3198 2024-05-14 21:18:18.000000 sortipy-0.0.4/src/sortipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-05-14 21:18:18.000000 sortipy-0.0.4/src/sortipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 21:18:18.000000 sortipy-0.0.4/src/sortipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 21:18:18.000000 sortipy-0.0.4/src/sortipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 21:24:43.996063 sortipy-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-05-14 10:16:33.000000 sortipy-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-14 10:57:17.000000 sortipy-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3191 2024-05-14 21:24:43.988166 sortipy-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2794 2024-05-14 21:24:24.000000 sortipy-0.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 10:58:30.000000 sortipy-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 21:24:43.996063 sortipy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      551 2024-05-14 21:24:31.000000 sortipy-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:24:43.895311 sortipy-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 21:24:43.924910 sortipy-0.0.5/src/sortipy/
+-rw-rw-rw-   0        0        0        0 2024-05-14 10:25:51.000000 sortipy-0.0.5/src/sortipy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:24:43.971488 sortipy-0.0.5/src/sortipy/exceptions/
+-rw-rw-rw-   0        0        0        0 2024-05-14 12:17:07.000000 sortipy-0.0.5/src/sortipy/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1546 2024-05-14 18:48:33.000000 sortipy-0.0.5/src/sortipy/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:24:43.981759 sortipy-0.0.5/src/sortipy/models/
+-rw-rw-rw-   0        0        0     1726 2024-05-14 21:16:43.000000 sortipy-0.0.5/src/sortipy/models/Directory.py
+-rw-rw-rw-   0        0        0     2058 2024-05-14 21:16:47.000000 sortipy-0.0.5/src/sortipy/models/File.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 12:14:42.000000 sortipy-0.0.5/src/sortipy/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:24:43.985366 sortipy-0.0.5/src/sortipy/sorters/
+-rw-rw-rw-   0        0        0     1466 2024-05-14 21:17:07.000000 sortipy-0.0.5/src/sortipy/sorters/DefaultSorter.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:53:00.000000 sortipy-0.0.5/src/sortipy/sorters/__init__.py
+-rw-rw-rw-   0        0        0     1141 2024-05-14 21:16:36.000000 sortipy-0.0.5/src/sortipy/sortipy.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:24:43.988166 sortipy-0.0.5/src/sortipy.egg-info/
+-rw-rw-rw-   0        0        0     3191 2024-05-14 21:24:43.000000 sortipy-0.0.5/src/sortipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-05-14 21:24:43.000000 sortipy-0.0.5/src/sortipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:24:43.000000 sortipy-0.0.5/src/sortipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 21:24:43.000000 sortipy-0.0.5/src/sortipy.egg-info/top_level.txt
```

### Comparing `sortipy-0.0.4/LICENSE` & `sortipy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.4/LICENSE.txt` & `sortipy-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.4/PKG-INFO` & `sortipy-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sortipy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sortipy is designed to help you organize files in a directory by sorting them based on their file extensions.
 Home-page: https://github.com/pzzzl/sortipy
 Author: Bruno Peselli
 Author-email: brunopeselli@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 <h1 align="center">Sortipy</h1>
 
 <p align="center">
-    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.4_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
+    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.5_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
 </p>
 
 <p align="center"><b><i>Sortipy</i></b> is a Python package designed to help you organize files in a directory by sorting them based on their file extensions.</p>
 
 ## Summary
 
 - [Summary](#summary)
@@ -96,12 +96,12 @@
 ## Default Behavior
 
 By default, Sortipy considers all file extensions in the directory for sorting. If you want to do this, you don't need to pass the extensions list. Only the directory will work just fine.
 
 
 ## Contributing
 
-If you'd like to contribute to Sortipy, please feel free to submit pull requests or open issues on the [GitHub repository](https://github.com/yourusername/sortipy).
+If you'd like to contribute to Sortipy, please feel free to submit pull requests or open issues on the [GitHub repository](https://github.com/pzzzl/sortipy).
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `sortipy-0.0.4/README.md` & `sortipy-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">Sortipy</h1>
 
 <p align="center">
-    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.4_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
+    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.5_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
 </p>
 
 <p align="center"><b><i>Sortipy</i></b> is a Python package designed to help you organize files in a directory by sorting them based on their file extensions.</p>
 
 ## Summary
 
 - [Summary](#summary)
@@ -84,12 +84,12 @@
 ## Default Behavior
 
 By default, Sortipy considers all file extensions in the directory for sorting. If you want to do this, you don't need to pass the extensions list. Only the directory will work just fine.
 
 
 ## Contributing
 
-If you'd like to contribute to Sortipy, please feel free to submit pull requests or open issues on the [GitHub repository](https://github.com/yourusername/sortipy).
+If you'd like to contribute to Sortipy, please feel free to submit pull requests or open issues on the [GitHub repository](https://github.com/pzzzl/sortipy).
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `sortipy-0.0.4/setup.py` & `sortipy-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sortipy',
-    version='0.0.4',
+    version='0.0.5',
     author='Bruno Peselli',
     author_email='brunopeselli@gmail.com',
     description='Sortipy is designed to help you organize files in a directory by sorting them based on their file extensions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/pzzzl/sortipy',
     packages=find_packages(where='src'),
```

### Comparing `sortipy-0.0.4/src/sortipy/exceptions/exceptions.py` & `sortipy-0.0.5/src/sortipy/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.4/src/sortipy/models/Directory.py` & `sortipy-0.0.5/src/sortipy/models/Directory.py`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.4/src/sortipy/models/File.py` & `sortipy-0.0.5/src/sortipy/models/File.py`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.4/src/sortipy/sorters/DefaultSorter.py` & `sortipy-0.0.5/src/sortipy/sorters/DefaultSorter.py`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.4/src/sortipy/sortipy.py` & `sortipy-0.0.5/src/sortipy/sortipy.py`

 * *Files identical despite different names*

### Comparing `sortipy-0.0.4/src/sortipy.egg-info/PKG-INFO` & `sortipy-0.0.5/src/sortipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sortipy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sortipy is designed to help you organize files in a directory by sorting them based on their file extensions.
 Home-page: https://github.com/pzzzl/sortipy
 Author: Bruno Peselli
 Author-email: brunopeselli@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 <h1 align="center">Sortipy</h1>
 
 <p align="center">
-    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.4_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
+    <img src="https://img.shields.io/badge/Python-%3E%3D3.6-yellow"> <img src="https://img.shields.io/badge/version-0.0.5_alpha-red"> <img src="https://img.shields.io/badge/Category-File_management_-orange"> <img src="https://img.shields.io/badge/Tools-Automation-blue">
 </p>
 
 <p align="center"><b><i>Sortipy</i></b> is a Python package designed to help you organize files in a directory by sorting them based on their file extensions.</p>
 
 ## Summary
 
 - [Summary](#summary)
@@ -96,12 +96,12 @@
 ## Default Behavior
 
 By default, Sortipy considers all file extensions in the directory for sorting. If you want to do this, you don't need to pass the extensions list. Only the directory will work just fine.
 
 
 ## Contributing
 
-If you'd like to contribute to Sortipy, please feel free to submit pull requests or open issues on the [GitHub repository](https://github.com/yourusername/sortipy).
+If you'd like to contribute to Sortipy, please feel free to submit pull requests or open issues on the [GitHub repository](https://github.com/pzzzl/sortipy).
 
 ## License
 
 This project is licensed under the MIT License.
```

