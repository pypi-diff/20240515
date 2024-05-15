# Comparing `tmp/flask-p-extends-restful-0.0.2.tar.gz` & `tmp/flask-p-extends-restful-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-p-extends-restful-0.0.2.tar", last modified: Wed May 15 17:15:13 2024, max compression
+gzip compressed data, was "flask-p-extends-restful-0.0.3.tar", last modified: Wed May 15 17:24:13 2024, max compression
```

## Comparing `flask-p-extends-restful-0.0.2.tar` & `flask-p-extends-restful-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 17:15:13.804254 flask-p-extends-restful-0.0.2/
--rw-rw-rw-   0        0        0      497 2024-05-15 17:15:13.801241 flask-p-extends-restful-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 17:15:13.790493 flask-p-extends-restful-0.0.2/flask_p_extends_restful.egg-info/
--rw-rw-rw-   0        0        0      497 2024-05-15 17:15:13.000000 flask-p-extends-restful-0.0.2/flask_p_extends_restful.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2024-05-15 17:15:13.000000 flask-p-extends-restful-0.0.2/flask_p_extends_restful.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 17:15:13.000000 flask-p-extends-restful-0.0.2/flask_p_extends_restful.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-15 17:15:13.000000 flask-p-extends-restful-0.0.2/flask_p_extends_restful.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 17:15:13.000000 flask-p-extends-restful-0.0.2/flask_p_extends_restful.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 17:15:13.798955 flask-p-extends-restful-0.0.2/restful/
--rw-rw-rw-   0        0        0        0 2024-05-06 06:57:00.000000 flask-p-extends-restful-0.0.2/restful/__init__.py
--rw-rw-rw-   0        0        0      143 2024-05-15 16:13:03.000000 flask-p-extends-restful-0.0.2/restful/container.py
--rw-rw-rw-   0        0        0     1678 2024-05-15 16:13:03.000000 flask-p-extends-restful-0.0.2/restful/convertion.py
--rw-rw-rw-   0        0        0      127 2024-05-15 16:13:03.000000 flask-p-extends-restful-0.0.2/restful/logic.py
--rw-rw-rw-   0        0        0     1223 2024-05-15 17:10:39.000000 flask-p-extends-restful-0.0.2/restful/scanner.py
--rw-rw-rw-   0        0        0       42 2024-05-15 17:15:13.804254 flask-p-extends-restful-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      860 2024-05-15 17:13:18.000000 flask-p-extends-restful-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:24:13.817881 flask-p-extends-restful-0.0.3/
+-rw-rw-rw-   0        0        0      497 2024-05-15 17:24:13.816817 flask-p-extends-restful-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 17:24:13.796317 flask-p-extends-restful-0.0.3/flask_extends/
+-rw-rw-rw-   0        0        0        0 2024-05-15 17:20:59.000000 flask-p-extends-restful-0.0.3/flask_extends/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:24:13.804535 flask-p-extends-restful-0.0.3/flask_extends/restful/
+-rw-rw-rw-   0        0        0        0 2024-05-06 06:57:00.000000 flask-p-extends-restful-0.0.3/flask_extends/restful/__init__.py
+-rw-rw-rw-   0        0        0      143 2024-05-15 16:13:03.000000 flask-p-extends-restful-0.0.3/flask_extends/restful/container.py
+-rw-rw-rw-   0        0        0     1678 2024-05-15 16:13:03.000000 flask-p-extends-restful-0.0.3/flask_extends/restful/convertion.py
+-rw-rw-rw-   0        0        0      127 2024-05-15 16:13:03.000000 flask-p-extends-restful-0.0.3/flask_extends/restful/logic.py
+-rw-rw-rw-   0        0        0     1237 2024-05-15 17:21:47.000000 flask-p-extends-restful-0.0.3/flask_extends/restful/scanner.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:24:13.814778 flask-p-extends-restful-0.0.3/flask_p_extends_restful.egg-info/
+-rw-rw-rw-   0        0        0      497 2024-05-15 17:24:13.000000 flask-p-extends-restful-0.0.3/flask_p_extends_restful.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-05-15 17:24:13.000000 flask-p-extends-restful-0.0.3/flask_p_extends_restful.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:24:13.000000 flask-p-extends-restful-0.0.3/flask_p_extends_restful.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-15 17:24:13.000000 flask-p-extends-restful-0.0.3/flask_p_extends_restful.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 17:24:13.000000 flask-p-extends-restful-0.0.3/flask_p_extends_restful.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 17:24:13.819003 flask-p-extends-restful-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      860 2024-05-15 17:21:47.000000 flask-p-extends-restful-0.0.3/setup.py
```

### Comparing `flask-p-extends-restful-0.0.2/restful/convertion.py` & `flask-p-extends-restful-0.0.3/flask_extends/restful/convertion.py`

 * *Files identical despite different names*

### Comparing `flask-p-extends-restful-0.0.2/restful/scanner.py` & `flask-p-extends-restful-0.0.3/flask_extends/restful/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 import os
 import traceback
 
 from flask_projects.default.router.convention import RouterBasic
 from flask_projects.default.router.plan_0.scanner import Plan0RouterScanner
-from restful.convertion import RestfulRouterBasic
+from flask_extends.restful.convertion import RestfulRouterBasic
 
 
 class RestfulScanner(Plan0RouterScanner):
 
     def scan(self, path_dir: str):
         cls_route = []
```

### Comparing `flask-p-extends-restful-0.0.2/setup.py` & `flask-p-extends-restful-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 - author:bichuantao
 - creation time:2024/5/15
 """
 
 from setuptools import setup, find_packages
 
 # you need to change all these
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = "flask projects系列的restful自定义扩展"
 long_description = "flask projects系列的第三方扩展-restful"
 
 setup(
     name="flask-p-extends-restful",
 
     author="bichuantao",
```

