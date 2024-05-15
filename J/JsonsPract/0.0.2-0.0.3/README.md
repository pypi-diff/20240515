# Comparing `tmp/JsonsPract-0.0.2.tar.gz` & `tmp/JsonsPract-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonsPract-0.0.2.tar", last modified: Wed May 15 06:55:47 2024, max compression
+gzip compressed data, was "JsonsPract-0.0.3.tar", last modified: Wed May 15 07:07:09 2024, max compression
```

## Comparing `JsonsPract-0.0.2.tar` & `JsonsPract-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 06:55:47.643416 JsonsPract-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:55:47.642099 JsonsPract-0.0.2/JsonsPract.egg-info/
--rw-rw-rw-   0        0        0     1553 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 06:55:47.000000 JsonsPract-0.0.2/JsonsPract.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1553 2024-05-15 06:55:47.643416 JsonsPract-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1123 2024-05-13 22:12:59.000000 JsonsPract-0.0.2/README.md
--rw-rw-rw-   0        0        0       43 2024-05-15 06:55:47.645477 JsonsPract-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      651 2024-05-15 06:55:24.000000 JsonsPract-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:07:09.024129 JsonsPract-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-15 07:07:09.019126 JsonsPract-0.0.3/JsonsPract/
+-rw-rw-rw-   0        0        0     2523 2024-05-15 06:55:03.000000 JsonsPract-0.0.3/JsonsPract/Jsons.py
+-rw-rw-rw-   0        0        0       20 2024-05-13 21:17:40.000000 JsonsPract-0.0.3/JsonsPract/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:07:09.023131 JsonsPract-0.0.3/JsonsPract.egg-info/
+-rw-rw-rw-   0        0        0     1553 2024-05-15 07:07:08.000000 JsonsPract-0.0.3/JsonsPract.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-15 07:07:08.000000 JsonsPract-0.0.3/JsonsPract.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 07:07:08.000000 JsonsPract-0.0.3/JsonsPract.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 07:07:08.000000 JsonsPract-0.0.3/JsonsPract.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 07:07:08.000000 JsonsPract-0.0.3/JsonsPract.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1553 2024-05-15 07:07:09.024129 JsonsPract-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1123 2024-05-13 22:12:59.000000 JsonsPract-0.0.3/README.md
+-rw-rw-rw-   0        0        0       43 2024-05-15 07:07:09.025129 JsonsPract-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      651 2024-05-15 07:07:06.000000 JsonsPract-0.0.3/setup.py
```

### Comparing `JsonsPract-0.0.2/JsonsPract.egg-info/PKG-INFO` & `JsonsPract-0.0.3/JsonsPract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonsPract
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the simplest module for quick work with json files.
 Author: sonin
 Author-email: fediasonin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `JsonsPract-0.0.2/PKG-INFO` & `JsonsPract-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonsPract
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the simplest module for quick work with json files.
 Author: sonin
 Author-email: fediasonin@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `JsonsPract-0.0.2/README.md` & `JsonsPract-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `JsonsPract-0.0.2/setup.py` & `JsonsPract-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='JsonsPract',
-  version='0.0.2',
+  version='0.0.3',
   author='sonin',
   author_email='fediasonin@gmail.com',
   description='This is the simplest module for quick work with json files.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['requests>=2.25.1'],
```

