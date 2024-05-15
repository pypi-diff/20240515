# Comparing `tmp/pyaxml-0.0.7.tar.gz` & `tmp/pyaxml-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaxml-0.0.7.tar", last modified: Tue Apr  2 21:34:10 2024, max compression
+gzip compressed data, was "pyaxml-0.0.8.tar", last modified: Wed May 15 10:32:37 2024, max compression
```

## Comparing `pyaxml-0.0.7.tar` & `pyaxml-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.871738 pyaxml-0.0.7/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2024-04-02 21:33:29.000000 pyaxml-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22742 2024-04-02 21:34:10.871738 pyaxml-0.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1267 2024-04-02 21:33:29.000000 pyaxml-0.0.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1174 2024-04-02 21:33:29.000000 pyaxml-0.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 21:34:10.871738 pyaxml-0.0.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.866738 pyaxml-0.0.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.868738 pyaxml-0.0.7/src/pyaxml/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30159 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/axml.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.870738 pyaxml-0.0.7/src/pyaxml/proto/
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/proto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3345 2024-04-02 21:33:29.000000 pyaxml-0.0.7/src/pyaxml/proto/axml.proto
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:34:10.870738 pyaxml-0.0.7/src/pyaxml.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22742 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-02 21:34:10.000000 pyaxml-0.0.7/src/pyaxml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.617050 pyaxml-0.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2024-05-15 10:31:58.000000 pyaxml-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22709 2024-05-15 10:32:37.616049 pyaxml-0.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2024-05-15 10:31:58.000000 pyaxml-0.0.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2024-05-15 10:31:58.000000 pyaxml-0.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 10:32:37.617050 pyaxml-0.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.611050 pyaxml-0.0.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.614050 pyaxml-0.0.8/src/pyaxml/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    65663 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/axml.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.616049 pyaxml-0.0.8/src/pyaxml/proto/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/proto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5694 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/proto/axml.proto
+-rw-rw-rw-   0 root         (0) root         (0)   106820 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/public.json
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/public.py
+-rw-rw-rw-   0 root         (0) root         (0)   191207 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/public.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.616049 pyaxml-0.0.8/src/pyaxml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22709 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      399 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.616049 pyaxml-0.0.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-05-15 10:31:58.000000 pyaxml-0.0.8/tests/test.py
```

### Comparing `pyaxml-0.0.7/LICENSE` & `pyaxml-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.7/PKG-INFO` & `pyaxml-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaxml
-Version: 0.0.7
+Version: 0.0.8
 Summary: Manipulate AXML file and create one from scratch
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
@@ -348,15 +348,14 @@
 Project-URL: Documentation, https://madsquirrels.gitlab.io/mobile/pyaxml/pyaxml.html
 Project-URL: Repository, https://gitlab.com/MadSquirrels/mobile/pyaxml
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: androguard==4.1.1
 Requires-Dist: click
 Requires-Dist: protobuf
 
 # README
 
 
 ## GENERAL INFO
```

### Comparing `pyaxml-0.0.7/README.md` & `pyaxml-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.7/pyproject.toml` & `pyaxml-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pyaxml"
 dynamic = ["version", "readme"]
 dependencies = [
-  'androguard==4.1.1',
   'click',
   'protobuf',
 ]
 requires-python = ">=3.5"
 authors = [
   {name = "Benoit Forgette (MadSquirrel)", email = "benoit.forgette@ci-yow.com"},
 ]
@@ -37,15 +36,15 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-pyaxml = ["proto/*.proto"]
+pyaxml = ["proto/*.proto", "public.xml", "public.json"]
 
 
 [project.urls]
 Homepage = "https://ci-yow.com"
 Documentation = "https://madsquirrels.gitlab.io/mobile/pyaxml/pyaxml.html"
 Repository = "https://gitlab.com/MadSquirrels/mobile/pyaxml"
```

### Comparing `pyaxml-0.0.7/src/pyaxml.egg-info/PKG-INFO` & `pyaxml-0.0.8/src/pyaxml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaxml
-Version: 0.0.7
+Version: 0.0.8
 Summary: Manipulate AXML file and create one from scratch
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
@@ -348,15 +348,14 @@
 Project-URL: Documentation, https://madsquirrels.gitlab.io/mobile/pyaxml/pyaxml.html
 Project-URL: Repository, https://gitlab.com/MadSquirrels/mobile/pyaxml
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: androguard==4.1.1
 Requires-Dist: click
 Requires-Dist: protobuf
 
 # README
 
 
 ## GENERAL INFO
```

