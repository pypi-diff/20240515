# Comparing `tmp/python_esios-0.1.1.tar.gz` & `tmp/python_esios-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_esios-0.1.1.tar", last modified: Wed May 15 06:24:08 2024, max compression
+gzip compressed data, was "python_esios-0.1.2.tar", last modified: Wed May 15 06:30:20 2024, max compression
```

## Comparing `python_esios-0.1.1.tar` & `python_esios-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:24:08.048573 python_esios-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:23:55.000000 python_esios-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:24:08.048573 python_esios-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 06:23:55.000000 python_esios-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:24:08.044573 python_esios-0.1.1/esios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:23:55.000000 python_esios-0.1.1/esios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 06:23:55.000000 python_esios-0.1.1/esios/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:24:08.044573 python_esios-0.1.1/esios/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 06:23:55.000000 python_esios-0.1.1/esios/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:24:08.044573 python_esios-0.1.1/esios/endpoints/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-15 06:23:55.000000 python_esios-0.1.1/esios/endpoints/indicators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:24:08.044573 python_esios-0.1.1/python_esios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:24:08.000000 python_esios-0.1.1/python_esios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 06:24:08.000000 python_esios-0.1.1/python_esios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:24:08.000000 python_esios-0.1.1/python_esios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 06:24:08.000000 python_esios-0.1.1/python_esios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 06:24:08.000000 python_esios-0.1.1/python_esios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:24:08.048573 python_esios-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 06:23:55.000000 python_esios-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.144859 python_esios-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:07.000000 python_esios-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:30:20.144859 python_esios-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 06:30:07.000000 python_esios-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.140859 python_esios-0.1.2/esios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:07.000000 python_esios-0.1.2/esios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-15 06:30:07.000000 python_esios-0.1.2/esios/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.140859 python_esios-0.1.2/esios/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 06:30:07.000000 python_esios-0.1.2/esios/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.140859 python_esios-0.1.2/esios/endpoints/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-15 06:30:07.000000 python_esios-0.1.2/esios/endpoints/indicators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.144859 python_esios-0.1.2/python_esios.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:30:20.144859 python_esios-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 06:30:07.000000 python_esios-0.1.2/setup.py
```

### Comparing `python_esios-0.1.1/PKG-INFO` & `python_esios-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.1/esios/endpoints/indicators/__init__.py` & `python_esios-0.1.2/esios/endpoints/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `python_esios-0.1.1/python_esios.egg-info/PKG-INFO` & `python_esios-0.1.2/python_esios.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.1/setup.py` & `python_esios-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 setup(
     name='python-esios',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pandas',
     ],
     author="Jesús López",
     author_email="jesus.lopez@datons.ai",
```

