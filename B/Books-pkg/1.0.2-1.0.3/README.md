# Comparing `tmp/books_pkg-1.0.2.tar.gz` & `tmp/books_pkg-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "books_pkg-1.0.2.tar", last modified: Tue May 14 02:50:19 2024, max compression
+gzip compressed data, was "books_pkg-1.0.3.tar", last modified: Wed May 15 03:01:57 2024, max compression
```

## Comparing `books_pkg-1.0.2.tar` & `books_pkg-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 02:50:19.089003 books_pkg-1.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-14 02:50:19.027495 books_pkg-1.0.2/Books_pkg/
--rw-rw-rw-   0        0        0       37 2024-05-14 02:18:23.000000 books_pkg-1.0.2/Books_pkg/__init__.py
--rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_pkg-1.0.2/Books_pkg/books.csv
--rw-rw-rw-   0        0        0     1284 2024-05-14 02:50:13.000000 books_pkg-1.0.2/Books_pkg/random_books.py
-drwxrwxrwx   0        0        0        0 2024-05-14 02:50:19.058734 books_pkg-1.0.2/Books_pkg.egg-info/
--rw-rw-rw-   0        0        0      334 2024-05-14 02:50:18.000000 books_pkg-1.0.2/Books_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-14 02:50:18.000000 books_pkg-1.0.2/Books_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 02:50:18.000000 books_pkg-1.0.2/Books_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-14 02:50:18.000000 books_pkg-1.0.2/Books_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-14 02:50:18.000000 books_pkg-1.0.2/Books_pkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      334 2024-05-14 02:50:19.060687 books_pkg-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      860 2024-05-14 02:27:18.000000 books_pkg-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 02:50:19.089975 books_pkg-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      535 2024-05-14 02:50:13.000000 books_pkg-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 03:01:57.744938 books_pkg-1.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-15 03:01:57.362940 books_pkg-1.0.3/Books_pkg/
+-rw-rw-rw-   0        0        0       37 2024-05-15 01:57:37.000000 books_pkg-1.0.3/Books_pkg/__init__.py
+-rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_pkg-1.0.3/Books_pkg/books.csv
+-rw-rw-rw-   0        0        0     1235 2024-05-15 03:01:09.000000 books_pkg-1.0.3/Books_pkg/buscar_books.py
+drwxrwxrwx   0        0        0        0 2024-05-15 03:01:57.684408 books_pkg-1.0.3/Books_pkg.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-05-15 03:01:54.000000 books_pkg-1.0.3/Books_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-15 03:01:54.000000 books_pkg-1.0.3/Books_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 03:01:54.000000 books_pkg-1.0.3/Books_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-15 03:01:54.000000 books_pkg-1.0.3/Books_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 03:01:54.000000 books_pkg-1.0.3/Books_pkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      334 2024-05-15 03:01:57.742009 books_pkg-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2024-05-14 02:27:18.000000 books_pkg-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 03:01:57.745913 books_pkg-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      541 2024-05-15 02:44:34.000000 books_pkg-1.0.3/setup.py
```

### Comparing `books_pkg-1.0.2/Books_pkg/books.csv` & `books_pkg-1.0.3/Books_pkg/books.csv`

 * *Files identical despite different names*

### Comparing `books_pkg-1.0.2/Books_pkg/random_books.py` & `books_pkg-1.0.3/Books_pkg/buscar_books.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-import pkg_resources
 import pandas as pd
+import pkg_resources
+
 
-class RandomBooks:
-    FILE_PATH = pkg_resources.resource_filename(__name__,'books.csv')
+class SelectBooks:
+    FILE_PATH = pkg_resources.resource_filename(__name__, 'books.csv')
 
     def __init__(self):
-        self._file = pd.read_csv(RandomBooks.FILE_PATH)
+        self._file = pd.read_csv(SelectBooks.FILE_PATH)
         self._books = None
         self._title = None
         self._author = None
         self._genre = None
         self._height = None
         self._publisher = None
 
-    def generate_random(self):
+    def generate_libro(self):
         self._books = self._file.sample()
         self._title = self._books["Title"].values[0]
         self._author = self._books["Author"].values[0]
         self._genre = self._books["Genre"].values[0]
-        self._height = self._books["#"].values[0]
+        self._height = self._books["Height"].values[0]
         self._publisher = self._books["Publisher"].values[0]
 
-    def buscar_title(title):
-        file = "books.csv"
-        datos = pd.read_csv(file)
+    def buscar_title(self,title):
+        datos = self._file
         buscar = datos[datos["Title"] == title]
         if buscar.size == 0:
-            return "No se encontro el Titulo: "
+            return "No se encontro el titulo. "
         else:
             return buscar
 
-    def buscar_author(author):
-        file = "books.csv"
-        datos = pd.read_csv(file)
+    def buscar_author(self,author):
+        datos = self._file
         buscar = datos[datos["Author"] == author]
         if buscar.size == 0:
-            return "No se encontro el Titulo: "
+            return "No se encontro el titulo. "
         else:
             return buscar
 
+
+
```

### Comparing `books_pkg-1.0.2/README.md` & `books_pkg-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `books_pkg-1.0.2/setup.py` & `books_pkg-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
 
    name='Books_pkg',
-   version='1.0.2',
+   version='1.0.3',
    author='Milton Alejandro Angel Cardenas ',
    author_email='milton_ac@tesch.edu.mx',
    description='Es una libreria en la cual podremos encontrar el autor y el libro, de pende el que se escriba',
    packages= ['Books_pkg'],
    package_data={'Books_pkg': ['books.csv']},
    install_requires=['pandas',
                      'twine',
                      'wheel' ,
                      'setuptools'
                      ],
-)
+)
+
+
```

