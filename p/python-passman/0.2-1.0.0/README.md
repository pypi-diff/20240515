# Comparing `tmp/python-passman-0.2.tar.gz` & `tmp/python-passman-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-passman-0.2.tar", last modified: Tue May 14 03:52:13 2024, max compression
+gzip compressed data, was "python-passman-1.0.0.tar", last modified: Tue May 14 04:17:26 2024, max compression
```

## Comparing `python-passman-0.2.tar` & `python-passman-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:52:13.910051 python-passman-0.2/
--rw-rw-rw-   0        0        0     1475 2024-05-14 03:52:13.906799 python-passman-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1214 2024-05-14 03:48:13.000000 python-passman-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 03:52:13.875665 python-passman-0.2/passman/
--rw-rw-rw-   0        0        0        0 2024-05-14 01:42:40.000000 python-passman-0.2/passman/__init__.py
--rw-rw-rw-   0        0        0     4231 2024-05-14 03:41:30.000000 python-passman-0.2/passman/cli.py
--rw-rw-rw-   0        0        0     1265 2024-05-14 02:47:28.000000 python-passman-0.2/passman/errors.py
--rw-rw-rw-   0        0        0     1971 2024-05-14 03:07:21.000000 python-passman-0.2/passman/passman.py
-drwxrwxrwx   0        0        0        0 2024-05-14 03:52:13.902151 python-passman-0.2/python_passman.egg-info/
--rw-rw-rw-   0        0        0     1475 2024-05-14 03:52:13.000000 python-passman-0.2/python_passman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-14 03:52:13.000000 python-passman-0.2/python_passman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:52:13.000000 python-passman-0.2/python_passman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-14 03:52:13.000000 python-passman-0.2/python_passman.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-14 03:52:13.000000 python-passman-0.2/python_passman.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 03:52:13.000000 python-passman-0.2/python_passman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 03:52:13.910471 python-passman-0.2/setup.cfg
--rw-rw-rw-   0        0        0      748 2024-05-14 03:52:08.000000 python-passman-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 04:17:26.509857 python-passman-1.0.0/
+-rw-rw-rw-   0        0        0     1477 2024-05-14 04:17:26.508335 python-passman-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1214 2024-05-14 03:48:13.000000 python-passman-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 04:17:26.476337 python-passman-1.0.0/passman/
+-rw-rw-rw-   0        0        0        0 2024-05-14 01:42:40.000000 python-passman-1.0.0/passman/__init__.py
+-rw-rw-rw-   0        0        0     4231 2024-05-14 03:41:30.000000 python-passman-1.0.0/passman/cli.py
+-rw-rw-rw-   0        0        0     1265 2024-05-14 02:47:28.000000 python-passman-1.0.0/passman/errors.py
+-rw-rw-rw-   0        0        0     1971 2024-05-14 03:07:21.000000 python-passman-1.0.0/passman/passman.py
+drwxrwxrwx   0        0        0        0 2024-05-14 04:17:26.506338 python-passman-1.0.0/python_passman.egg-info/
+-rw-rw-rw-   0        0        0     1477 2024-05-14 04:17:26.000000 python-passman-1.0.0/python_passman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-14 04:17:26.000000 python-passman-1.0.0/python_passman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 04:17:26.000000 python-passman-1.0.0/python_passman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-14 04:17:26.000000 python-passman-1.0.0/python_passman.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-14 04:17:26.000000 python-passman-1.0.0/python_passman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 04:17:26.000000 python-passman-1.0.0/python_passman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 04:17:26.509857 python-passman-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-14 04:17:01.000000 python-passman-1.0.0/setup.py
```

### Comparing `python-passman-0.2/PKG-INFO` & `python-passman-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-passman
-Version: 0.2
+Version: 1.0.0
 Summary: Terminal password manager in Python
 Home-page: https://github.com/profility/passman
 Author: profility
 Author-email: contact@profility.slmail.me
 Description-Content-Type: text/markdown
 
 # PassMan
```

### Comparing `python-passman-0.2/README.md` & `python-passman-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `python-passman-0.2/passman/cli.py` & `python-passman-1.0.0/passman/cli.py`

 * *Files identical despite different names*

### Comparing `python-passman-0.2/passman/errors.py` & `python-passman-1.0.0/passman/errors.py`

 * *Files identical despite different names*

### Comparing `python-passman-0.2/passman/passman.py` & `python-passman-1.0.0/passman/passman.py`

 * *Files identical despite different names*

### Comparing `python-passman-0.2/python_passman.egg-info/PKG-INFO` & `python-passman-1.0.0/python_passman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-passman
-Version: 0.2
+Version: 1.0.0
 Summary: Terminal password manager in Python
 Home-page: https://github.com/profility/passman
 Author: profility
 Author-email: contact@profility.slmail.me
 Description-Content-Type: text/markdown
 
 # PassMan
```

### Comparing `python-passman-0.2/setup.py` & `python-passman-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2"
+VERSION = "1.0.0"
 DESCRIPTION = "Terminal password manager in Python"
 LONG_DESCRIPTION = ""
 
 with open("README.md", "r", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

