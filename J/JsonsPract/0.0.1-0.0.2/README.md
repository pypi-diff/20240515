# Comparing `tmp/JsonsPract-0.0.1.tar.gz` & `tmp/JsonsPract-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonsPract-0.0.1.tar", last modified: Tue May 14 22:15:12 2024, max compression
+gzip compressed data, was "JsonsPract-0.0.2.tar", last modified: Wed May 15 06:55:47 2024, max compression
```

## Comparing `JsonsPract-0.0.1.tar` & `JsonsPract-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 22:15:12.812632 JsonsPract-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-14 22:15:12.810330 JsonsPract-0.0.1/JsonsPract.egg-info/
--rw-rw-rw-   0        0        0     1553 2024-05-14 22:15:12.000000 JsonsPract-0.0.1/JsonsPract.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-05-14 22:15:12.000000 JsonsPract-0.0.1/JsonsPract.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 22:15:12.000000 JsonsPract-0.0.1/JsonsPract.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-14 22:15:12.000000 JsonsPract-0.0.1/JsonsPract.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 22:15:12.000000 JsonsPract-0.0.1/JsonsPract.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1553 2024-05-14 22:15:12.811327 JsonsPract-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1123 2024-05-13 22:12:59.000000 JsonsPract-0.0.1/README.md
--rw-rw-rw-   0        0        0       43 2024-05-14 22:15:12.813634 JsonsPract-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      651 2024-05-14 22:14:14.000000 JsonsPract-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:55:47.643416 JsonsPract-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-15 06:55:47.642099 JsonsPract-0.0.2/JsonsPract.egg-info/
+-rw-rw-rw-   0        0        0     1553 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1553 2024-05-15 06:55:47.643416 JsonsPract-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1123 2024-05-13 22:12:59.000000 JsonsPract-0.0.2/README.md
+-rw-rw-rw-   0        0        0       43 2024-05-15 06:55:47.645477 JsonsPract-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      651 2024-05-15 06:55:24.000000 JsonsPract-0.0.2/setup.py
```

### Comparing `JsonsPract-0.0.1/JsonsPract.egg-info/PKG-INFO` & `JsonsPract-0.0.2/JsonsPract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonsPract
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is the simplest module for quick work with json files.
 Author: sonin
 Author-email: fediasonin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `JsonsPract-0.0.1/PKG-INFO` & `JsonsPract-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonsPract
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is the simplest module for quick work with json files.
 Author: sonin
 Author-email: fediasonin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `JsonsPract-0.0.1/README.md` & `JsonsPract-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `JsonsPract-0.0.1/setup.py` & `JsonsPract-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='JsonsPract',
-  version='0.0.1',
+  version='0.0.2',
   author='sonin',
   author_email='fediasonin@gmail.com',
   description='This is the simplest module for quick work with json files.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['requests>=2.25.1'],
```

