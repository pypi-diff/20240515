# Comparing `tmp/jonazarov-0.1.2.tar.gz` & `tmp/jonazarov-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jonazarov-0.1.2.tar", last modified: Wed Dec 20 07:55:29 2023, max compression
+gzip compressed data, was "jonazarov-0.1.3.tar", last modified: Wed May 15 13:35:55 2024, max compression
```

## Comparing `jonazarov-0.1.2.tar` & `jonazarov-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-12-20 07:55:29.465947 jonazarov-0.1.2/
--rw-rw-rw-   0        0        0     1087 2023-08-16 08:45:41.000000 jonazarov-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      606 2023-12-20 07:55:29.456955 jonazarov-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-20 07:55:29.392176 jonazarov-0.1.2/jonazarov/
--rw-rw-rw-   0        0        0    47237 2023-09-26 11:53:32.000000 jonazarov-0.1.2/jonazarov/AtlassianCloudRest.py
--rw-rw-rw-   0        0        0       77 2023-12-20 07:55:21.000000 jonazarov-0.1.2/jonazarov/__init__.py
--rw-rw-rw-   0        0        0     3564 2023-09-12 14:44:09.000000 jonazarov-0.1.2/jonazarov/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-20 07:55:29.450969 jonazarov-0.1.2/jonazarov.egg-info/
--rw-rw-rw-   0        0        0      606 2023-12-20 07:55:29.000000 jonazarov-0.1.2/jonazarov.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-12-20 07:55:29.000000 jonazarov-0.1.2/jonazarov.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-20 07:55:29.000000 jonazarov-0.1.2/jonazarov.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-12-20 07:55:29.000000 jonazarov-0.1.2/jonazarov.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-20 07:55:29.000000 jonazarov-0.1.2/jonazarov.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-20 07:55:29.468251 jonazarov-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      810 2023-12-20 07:55:14.000000 jonazarov-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:35:55.529454 jonazarov-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-08-16 08:45:41.000000 jonazarov-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      666 2024-05-15 13:35:55.527547 jonazarov-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1277 2024-05-15 12:41:56.000000 jonazarov-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 13:35:55.434836 jonazarov-0.1.3/jonazarov/
+-rw-rw-rw-   0        0        0    55422 2024-05-15 11:33:26.000000 jonazarov-0.1.3/jonazarov/AtlassianCloudRest.py
+-rw-rw-rw-   0        0        0       77 2024-05-15 13:29:58.000000 jonazarov-0.1.3/jonazarov/__init__.py
+-rw-rw-rw-   0        0        0     3564 2023-09-12 14:44:09.000000 jonazarov-0.1.3/jonazarov/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:35:55.524732 jonazarov-0.1.3/jonazarov.egg-info/
+-rw-rw-rw-   0        0        0      666 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 13:35:55.000000 jonazarov-0.1.3/jonazarov.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 13:35:55.530480 jonazarov-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-05-15 13:30:04.000000 jonazarov-0.1.3/setup.py
```

### Comparing `jonazarov-0.1.2/LICENSE` & `jonazarov-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jonazarov-0.1.2/PKG-INFO` & `jonazarov-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: jonazarov
-Version: 0.1.2
+Version: 0.1.3
 Summary: Verschiedene Python-Tools, vor allem für Atlassian Cloud
 Home-page: https://github.com/jonazarov/pytools
 Author: Johannes Nazarov
 Author-email: johannes.nazarov+dev@gmail.com
 License: GNU
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: German
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+Requires-Dist: bs4>=0.0.1
```

### Comparing `jonazarov-0.1.2/jonazarov/utils.py` & `jonazarov-0.1.3/jonazarov/utils.py`

 * *Files identical despite different names*

### Comparing `jonazarov-0.1.2/jonazarov.egg-info/PKG-INFO` & `jonazarov-0.1.3/jonazarov.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: jonazarov
-Version: 0.1.2
+Version: 0.1.3
 Summary: Verschiedene Python-Tools, vor allem für Atlassian Cloud
 Home-page: https://github.com/jonazarov/pytools
 Author: Johannes Nazarov
 Author-email: johannes.nazarov+dev@gmail.com
 License: GNU
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: German
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+Requires-Dist: bs4>=0.0.1
```

### Comparing `jonazarov-0.1.2/setup.py` & `jonazarov-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='jonazarov',
-    version='0.1.2',    
+    version='0.1.3',    
     description='Verschiedene Python-Tools, vor allem für Atlassian Cloud',
     url='https://github.com/jonazarov/pytools',
     author='Johannes Nazarov',
     author_email='johannes.nazarov+dev@gmail.com',
     license='GNU',
     packages=['jonazarov'],
     install_requires=['requests>=2.31.0',
```

