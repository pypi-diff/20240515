# Comparing `tmp/placafipy-1.0.1.tar.gz` & `tmp/placafipy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "placafipy-1.0.1.tar", last modified: Wed May 15 03:45:48 2024, max compression
+gzip compressed data, was "placafipy-1.0.2.tar", last modified: Wed May 15 04:11:45 2024, max compression
```

## Comparing `placafipy-1.0.1.tar` & `placafipy-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 03:45:48.873877 placafipy-1.0.1/
--rw-rw-rw-   0        0        0     1102 2024-05-14 20:22:41.000000 placafipy-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       67 2024-05-15 03:29:36.000000 placafipy-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      391 2024-05-15 03:45:48.871877 placafipy-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 03:45:48.870877 placafipy-1.0.1/PlacaFipy.egg-info/
--rw-rw-rw-   0        0        0      391 2024-05-15 03:45:48.000000 placafipy-1.0.1/PlacaFipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-05-15 03:45:48.000000 placafipy-1.0.1/PlacaFipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 03:45:48.000000 placafipy-1.0.1/PlacaFipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-15 03:45:48.000000 placafipy-1.0.1/PlacaFipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-15 03:45:48.000000 placafipy-1.0.1/PlacaFipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2792 2024-05-14 21:45:27.000000 placafipy-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 03:45:48.869876 placafipy-1.0.1/placafipy/
--rw-rw-rw-   0        0        0     8441 2024-05-15 03:45:37.000000 placafipy-1.0.1/placafipy/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-15 03:45:48.874877 placafipy-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      481 2024-05-15 03:45:21.000000 placafipy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:11:45.892746 placafipy-1.0.2/
+-rw-rw-rw-   0        0        0     1102 2024-05-14 20:22:41.000000 placafipy-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       67 2024-05-15 03:29:36.000000 placafipy-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3328 2024-05-15 04:11:45.890746 placafipy-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 04:11:45.889746 placafipy-1.0.2/PlacaFipy.egg-info/
+-rw-rw-rw-   0        0        0     3328 2024-05-15 04:11:45.000000 placafipy-1.0.2/PlacaFipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-05-15 04:11:45.000000 placafipy-1.0.2/PlacaFipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 04:11:45.000000 placafipy-1.0.2/PlacaFipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-15 04:11:45.000000 placafipy-1.0.2/PlacaFipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 04:11:45.000000 placafipy-1.0.2/PlacaFipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2792 2024-05-14 21:45:27.000000 placafipy-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 04:11:45.887745 placafipy-1.0.2/placafipy/
+-rw-rw-rw-   0        0        0     8441 2024-05-15 04:10:24.000000 placafipy-1.0.2/placafipy/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 04:11:45.892746 placafipy-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      742 2024-05-15 04:10:44.000000 placafipy-1.0.2/setup.py
```

### Comparing `placafipy-1.0.1/LICENSE` & `placafipy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `placafipy-1.0.1/README.md` & `placafipy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `placafipy-1.0.1/placafipy/__init__.py` & `placafipy-1.0.2/placafipy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # https://github.com/juniorkrz/placafipy
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __author__ = "Antônio Roberto Júnior"
 
 
 from bs4 import BeautifulSoup
 from unidecode import unidecode
 from string import ascii_lowercase
 from requests import get as requests_get
```

