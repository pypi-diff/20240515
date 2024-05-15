# Comparing `tmp/pywebframework_uz-0.1.2.tar.gz` & `tmp/pywebframework_uz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebframework_uz-0.1.2.tar", last modified: Wed May 15 09:16:33 2024, max compression
+gzip compressed data, was "pywebframework_uz-0.1.3.tar", last modified: Wed May 15 09:20:36 2024, max compression
```

## Comparing `pywebframework_uz-0.1.2.tar` & `pywebframework_uz-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 09:16:33.166936 pywebframework_uz-0.1.2/
--rw-rw-rw-   0        0        0     4736 2024-05-15 09:16:33.165935 pywebframework_uz-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3864 2024-05-15 09:16:20.000000 pywebframework_uz-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 09:16:33.162946 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/
--rw-rw-rw-   0        0        0     4736 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 09:16:33.166936 pywebframework_uz-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     4069 2024-05-15 09:16:20.000000 pywebframework_uz-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:20:36.859597 pywebframework_uz-0.1.3/
+-rw-rw-rw-   0        0        0     4732 2024-05-15 09:20:36.857599 pywebframework_uz-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3860 2024-05-15 09:19:06.000000 pywebframework_uz-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 09:20:36.855598 pywebframework_uz-0.1.3/pywebframework_uz.egg-info/
+-rw-rw-rw-   0        0        0     4732 2024-05-15 09:20:36.000000 pywebframework_uz-0.1.3/pywebframework_uz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-05-15 09:20:36.000000 pywebframework_uz-0.1.3/pywebframework_uz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:20:36.000000 pywebframework_uz-0.1.3/pywebframework_uz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-15 09:20:36.000000 pywebframework_uz-0.1.3/pywebframework_uz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:20:36.000000 pywebframework_uz-0.1.3/pywebframework_uz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:20:36.859597 pywebframework_uz-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     4069 2024-05-15 09:20:21.000000 pywebframework_uz-0.1.3/setup.py
```

### Comparing `pywebframework_uz-0.1.2/PKG-INFO` & `pywebframework_uz-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebframework_uz
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python web-framework building for learning purpose
 Home-page: https://github.com/me/myproject
 Author: Madaminov Khojiakbar
 Author-email: hojiakbarmadaminov45@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -20,16 +20,16 @@
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==6.6.0
 
 
 PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
-![purpose](https://image.shields.io/badge/purpose-learning-green)
-![PyPy - Version](https://image.shields.io/pypi/v/pywebframework)
+![purpose](https://img.shields.io/badge/purpose-learning-green)
+![PyPy - Version](https://img.shields.io/pypi/v/pywebframework)
 
 
 PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
 Installation
 ```shell
 pip install pywebframework-uz
```

### Comparing `pywebframework_uz-0.1.2/README.md` & `pywebframework_uz-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
-![purpose](https://image.shields.io/badge/purpose-learning-green)
-![PyPy - Version](https://image.shields.io/pypi/v/pywebframework)
+![purpose](https://img.shields.io/badge/purpose-learning-green)
+![PyPy - Version](https://img.shields.io/pypi/v/pywebframework)
 
 
 PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
 Installation
 ```shell
 pip install pywebframework-uz
```

### Comparing `pywebframework_uz-0.1.2/pywebframework_uz.egg-info/PKG-INFO` & `pywebframework_uz-0.1.3/pywebframework_uz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebframework_uz
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python web-framework building for learning purpose
 Home-page: https://github.com/me/myproject
 Author: Madaminov Khojiakbar
 Author-email: hojiakbarmadaminov45@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -20,16 +20,16 @@
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==6.6.0
 
 
 PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
-![purpose](https://image.shields.io/badge/purpose-learning-green)
-![PyPy - Version](https://image.shields.io/pypi/v/pywebframework)
+![purpose](https://img.shields.io/badge/purpose-learning-green)
+![PyPy - Version](https://img.shields.io/pypi/v/pywebframework)
 
 
 PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
 Installation
 ```shell
 pip install pywebframework-uz
```

### Comparing `pywebframework_uz-0.1.2/setup.py` & `pywebframework_uz-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pywebframework_uz'
 DESCRIPTION = 'Python web-framework building for learning purpose'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'hojiakbarmadaminov45@gmail.com'
 AUTHOR = 'Madaminov Khojiakbar'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     'requests-wsgi-adapter==0.4.1',
```

