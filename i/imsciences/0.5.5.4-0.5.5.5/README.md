# Comparing `tmp/imsciences-0.5.5.4.tar.gz` & `tmp/imsciences-0.5.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.5.4.tar", last modified: Tue May 14 14:52:44 2024, max compression
+gzip compressed data, was "imsciences-0.5.5.5.tar", last modified: Wed May 15 09:16:40 2024, max compression
```

## Comparing `imsciences-0.5.5.4.tar` & `imsciences-0.5.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 14:52:44.251054 imsciences-0.5.5.4/
--rw-rw-rw-   0        0        0     8855 2024-05-14 14:52:44.246164 imsciences-0.5.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     8350 2024-05-14 14:45:39.000000 imsciences-0.5.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 14:52:44.218266 imsciences-0.5.5.4/imsciences/
--rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.4/imsciences/__init__.py
--rw-rw-rw-   0        0        0    54723 2024-05-14 14:47:52.000000 imsciences-0.5.5.4/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 14:52:44.241809 imsciences-0.5.5.4/imsciences.egg-info/
--rw-rw-rw-   0        0        0     8855 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 14:52:44.000000 imsciences-0.5.5.4/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 14:52:44.251054 imsciences-0.5.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-14 14:45:41.000000 imsciences-0.5.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:16:40.189691 imsciences-0.5.5.5/
+-rw-rw-rw-   0        0        0     8855 2024-05-15 09:16:40.182204 imsciences-0.5.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8350 2024-05-14 14:45:39.000000 imsciences-0.5.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 09:16:40.158360 imsciences-0.5.5.5/imsciences/
+-rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.5/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    54723 2024-05-15 09:12:25.000000 imsciences-0.5.5.5/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:16:40.182204 imsciences-0.5.5.5/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     8855 2024-05-15 09:16:39.000000 imsciences-0.5.5.5/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-15 09:16:40.000000 imsciences-0.5.5.5/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:16:39.000000 imsciences-0.5.5.5/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 09:16:39.000000 imsciences-0.5.5.5/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 09:16:39.000000 imsciences-0.5.5.5/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:16:40.189691 imsciences-0.5.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-15 09:15:45.000000 imsciences-0.5.5.5/setup.py
```

### Comparing `imsciences-0.5.5.4/PKG-INFO` & `imsciences-0.5.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.4
+Version: 0.5.5.5
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.5.4/README.md` & `imsciences-0.5.5.5/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.5.4/imsciences/datafunctions.py` & `imsciences-0.5.5.5/imsciences/datafunctions.py`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.5.4/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.5.5/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.4
+Version: 0.5.5.5
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.5.4/setup.py` & `imsciences-0.5.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.5.4'
+VERSION = '0.5.5.5'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

