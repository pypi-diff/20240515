# Comparing `tmp/iguana-0.1.0.tar.gz` & `tmp/iguana-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iguana-0.1.0.tar", last modified: Wed May 15 14:44:44 2024, max compression
+gzip compressed data, was "iguana-0.1.1.tar", last modified: Wed May 15 20:43:47 2024, max compression
```

## Comparing `iguana-0.1.0.tar` & `iguana-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 14:44:44.057209 iguana-0.1.0/
--rw-r--r--   0 keksi     (1000) keksi     (1000)     1066 2024-05-15 13:59:07.000000 iguana-0.1.0/LICENSE
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 14:44:44.057209 iguana-0.1.0/PKG-INFO
--rw-r--r--   0 keksi     (1000) keksi     (1000)     6745 2024-05-15 13:59:07.000000 iguana-0.1.0/README.md
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 14:44:44.057209 iguana-0.1.0/iguana/
--rw-r--r--   0 keksi     (1000) keksi     (1000)        0 2024-05-15 13:59:07.000000 iguana-0.1.0/iguana/__init__.py
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7668 2024-05-15 13:59:07.000000 iguana-0.1.0/iguana/iguana.py
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 14:44:44.057209 iguana-0.1.0/iguana.egg-info/
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 14:44:43.000000 iguana-0.1.0/iguana.egg-info/PKG-INFO
--rw-r--r--   0 keksi     (1000) keksi     (1000)      244 2024-05-15 14:44:44.000000 iguana-0.1.0/iguana.egg-info/SOURCES.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)        1 2024-05-15 14:44:43.000000 iguana-0.1.0/iguana.egg-info/dependency_links.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       46 2024-05-15 14:44:43.000000 iguana-0.1.0/iguana.egg-info/entry_points.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       16 2024-05-15 14:44:43.000000 iguana-0.1.0/iguana.egg-info/requires.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)        7 2024-05-15 14:44:43.000000 iguana-0.1.0/iguana.egg-info/top_level.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       38 2024-05-15 14:44:44.057209 iguana-0.1.0/setup.cfg
--rw-r--r--   0 keksi     (1000) keksi     (1000)      768 2024-05-15 14:44:04.000000 iguana-0.1.0/setup.py
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 20:43:47.971476 iguana-0.1.1/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     1066 2024-05-15 13:59:07.000000 iguana-0.1.1/LICENSE
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 20:43:47.971476 iguana-0.1.1/PKG-INFO
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     6745 2024-05-15 13:59:07.000000 iguana-0.1.1/README.md
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 20:43:47.971476 iguana-0.1.1/iguana/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        0 2024-05-15 13:59:07.000000 iguana-0.1.1/iguana/__init__.py
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7668 2024-05-15 13:59:07.000000 iguana-0.1.1/iguana/iguana.py
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 20:43:47.971476 iguana-0.1.1/iguana.egg-info/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/PKG-INFO
+-rw-r--r--   0 keksi     (1000) keksi     (1000)      244 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/SOURCES.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        1 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/dependency_links.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       39 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/entry_points.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       16 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/requires.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        7 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/top_level.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       38 2024-05-15 20:43:47.971476 iguana-0.1.1/setup.cfg
+-rw-r--r--   0 keksi     (1000) keksi     (1000)      761 2024-05-15 20:42:05.000000 iguana-0.1.1/setup.py
```

### Comparing `iguana-0.1.0/LICENSE` & `iguana-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iguana-0.1.0/PKG-INFO` & `iguana-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguana
-Version: 0.1.0
+Version: 0.1.1
 Summary: A network scanning tool for Kali Linux
 Home-page: https://github.com/uveissmjl/iguana
 Author: Uveis Smajli
 Author-email: smajliuveis@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iguana-0.1.0/README.md` & `iguana-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `iguana-0.1.0/iguana/iguana.py` & `iguana-0.1.1/iguana/iguana.py`

 * *Files identical despite different names*

### Comparing `iguana-0.1.0/iguana.egg-info/PKG-INFO` & `iguana-0.1.1/iguana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguana
-Version: 0.1.0
+Version: 0.1.1
 Summary: A network scanning tool for Kali Linux
 Home-page: https://github.com/uveissmjl/iguana
 Author: Uveis Smajli
 Author-email: smajliuveis@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iguana-0.1.0/setup.py` & `iguana-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='iguana',
-    version='0.1.0',
+    version='0.1.1',
     description='A network scanning tool for Kali Linux',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Uveis Smajli',
     author_email='smajliuveis@yahoo.com',
     url='https://github.com/uveissmjl/iguana',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'iguana=iguana.iguana:main',
+            'iguana=iguana:main',
         ],
     },
     install_requires=[
         'scapy',
         'dnspython',
     ],
     classifiers=[
```

