# Comparing `tmp/dictoat-0.1.tar.gz` & `tmp/dictoat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictoat-0.1.tar", last modified: Sat Dec  9 22:09:32 2023, max compression
+gzip compressed data, was "dictoat-1.0.1.tar", last modified: Wed May 15 05:49:18 2024, max compression
```

## Comparing `dictoat-0.1.tar` & `dictoat-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0 elnico     (501) staff       (20)        0 2023-12-09 22:09:32.230000 dictoat-0.1/
--rwxrwxrwx   0 elnico     (501) staff       (20)     1066 2023-12-09 21:30:08.000000 dictoat-0.1/LICENSE
--rwxrwxrwx   0 elnico     (501) staff       (20)     3518 2023-12-09 22:09:32.370000 dictoat-0.1/PKG-INFO
--rwxrwxrwx   0 elnico     (501) staff       (20)     3059 2023-12-09 21:43:37.000000 dictoat-0.1/README.md
--rwxrwxrwx   0 elnico     (501) staff       (20)       28 2023-12-09 21:25:43.000000 dictoat-0.1/__init__.py
-drwxrwxrwx   0 elnico     (501) staff       (20)        0 2023-12-09 22:09:32.230000 dictoat-0.1/dictoat.egg-info/
--rwxrwxrwx   0 elnico     (501) staff       (20)     3518 2023-12-09 22:09:31.000000 dictoat-0.1/dictoat.egg-info/PKG-INFO
--rwxrwxrwx   0 elnico     (501) staff       (20)      209 2023-12-09 22:09:32.000000 dictoat-0.1/dictoat.egg-info/SOURCES.txt
--rwxrwxrwx   0 elnico     (501) staff       (20)        1 2023-12-09 22:09:31.000000 dictoat-0.1/dictoat.egg-info/dependency_links.txt
--rwxrwxrwx   0 elnico     (501) staff       (20)        1 2023-12-09 22:09:31.000000 dictoat-0.1/dictoat.egg-info/top_level.txt
--rwxrwxrwx   0 elnico     (501) staff       (20)      331 2023-12-09 21:25:40.000000 dictoat-0.1/dictoat.py
--rwxrwxrwx   0 elnico     (501) staff       (20)       38 2023-12-09 22:09:32.370000 dictoat-0.1/setup.cfg
--rwxrwxrwx   0 elnico     (501) staff       (20)      648 2023-12-09 08:01:26.000000 dictoat-0.1/setup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:49:18.916274 dictoat-1.0.1/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:40:04.000000 dictoat-1.0.1/LICENSE
+-rw-r--r--   0 nicospok   (501) staff       (20)     3639 2024-05-15 05:49:18.915102 dictoat-1.0.1/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)     3178 2024-05-15 05:40:04.000000 dictoat-1.0.1/README.md
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:49:18.910170 dictoat-1.0.1/dictoat/
+-rw-r--r--   0 nicospok   (501) staff       (20)     6148 2024-05-15 05:40:04.000000 dictoat-1.0.1/dictoat/.DS_Store
+-rw-r--r--   0 nicospok   (501) staff       (20)        6 2024-05-15 05:40:04.000000 dictoat-1.0.1/dictoat/__init__.py
+-rw-r--r--   0 nicospok   (501) staff       (20)      529 2024-05-15 05:40:04.000000 dictoat-1.0.1/dictoat/dictoat.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:49:18.914162 dictoat-1.0.1/dictoat.egg-info/
+-rw-r--r--   0 nicospok   (501) staff       (20)     3639 2024-05-15 05:49:17.000000 dictoat-1.0.1/dictoat.egg-info/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)      207 2024-05-15 05:49:18.000000 dictoat-1.0.1/dictoat.egg-info/SOURCES.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-15 05:49:17.000000 dictoat-1.0.1/dictoat.egg-info/dependency_links.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        8 2024-05-15 05:49:17.000000 dictoat-1.0.1/dictoat.egg-info/top_level.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-15 05:49:18.916514 dictoat-1.0.1/setup.cfg
+-rw-r--r--   0 nicospok   (501) staff       (20)      650 2024-05-15 05:40:04.000000 dictoat-1.0.1/setup.py
```

### Comparing `dictoat-0.1/LICENSE` & `dictoat-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dictoat-0.1/PKG-INFO` & `dictoat-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,46 @@
-Metadata-Version: 2.1
-Name: dictoat
-Version: 0.1
-Summary: Convert a dict into an object to access items faster.
-Home-page: https://github.com/niCodeLine/dictoat
-Author: Nico Spok
-Author-email: nicospok@hotmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Dictoat
 
 Dictoat is a Python utility designed to simplify accessing data stored in dictionaries. It converts dictionaries into Python objects, allowing for more intuitive access to data via attributes instead of dictionary keys. This is ideal for projects where readability and ease of access to complex data structures are essential.
 
 ## Installation
 
 You can easily install `Dictoat` using pip:
 
 ```bash
 pip install dictoat
 ```
+or via git:
 
+```bash
+git clone https://github.com/niCodeLine/dictoat.git
+```
+or just copy-paste it into your code.
 ## Usage
 
 To use Dictoat, simply import the `Dictoat` class in your Python project and pass a dictionary as an argument. For example:
 
 ```python
 from dictoat import Dictoat
 
 # Example of using Dictoat
-apple_dict = {"color": "red", "dimentions": {"weigh": 185, "radius": 5, "units": ["g", "cm"]}}
+apple_dict = {"flavor": "sweet", "colors": ["red", "green"],"dimentions": {"weigh": 185, "radius": 5}}
 apple = Dictoat(apple_dict)
 
 # Accessing the data
-print(apple.color_)
+print(apple.flavor_)
 print(apple.dimentions_.radius_)
-print(apple.dimentions_.units_)
+print(apple.colors_)
 ```
 
 The output would show:
 ```markdown
-red
+sweet
 5
-['g', 'cm']
+["red", "green"]
 ```
 
 Or a more complete example:
 
 ```python
 from dictoat import Dictoat
```

### Comparing `dictoat-0.1/README.md` & `dictoat-1.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,61 @@
+Metadata-Version: 2.1
+Name: dictoat
+Version: 1.0.1
+Summary: Convert a dict into an object to access items faster.
+Home-page: https://github.com/niCodeLine/dictoat
+Author: Nico Spok
+Author-email: nicospok@hotmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Dictoat
 
 Dictoat is a Python utility designed to simplify accessing data stored in dictionaries. It converts dictionaries into Python objects, allowing for more intuitive access to data via attributes instead of dictionary keys. This is ideal for projects where readability and ease of access to complex data structures are essential.
 
 ## Installation
 
 You can easily install `Dictoat` using pip:
 
 ```bash
 pip install dictoat
 ```
+or via git:
 
+```bash
+git clone https://github.com/niCodeLine/dictoat.git
+```
+or just copy-paste it into your code.
 ## Usage
 
 To use Dictoat, simply import the `Dictoat` class in your Python project and pass a dictionary as an argument. For example:
 
 ```python
 from dictoat import Dictoat
 
 # Example of using Dictoat
-apple_dict = {"color": "red", "dimentions": {"weigh": 185, "radius": 5, "units": ["g", "cm"]}}
+apple_dict = {"flavor": "sweet", "colors": ["red", "green"],"dimentions": {"weigh": 185, "radius": 5}}
 apple = Dictoat(apple_dict)
 
 # Accessing the data
-print(apple.color_)
+print(apple.flavor_)
 print(apple.dimentions_.radius_)
-print(apple.dimentions_.units_)
+print(apple.colors_)
 ```
 
 The output would show:
 ```markdown
-red
+sweet
 5
-['g', 'cm']
+["red", "green"]
 ```
 
 Or a more complete example:
 
 ```python
 from dictoat import Dictoat
```

### Comparing `dictoat-0.1/dictoat.egg-info/PKG-INFO` & `dictoat-1.0.1/dictoat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictoat
-Version: 0.1
+Version: 1.0.1
 Summary: Convert a dict into an object to access items faster.
 Home-page: https://github.com/niCodeLine/dictoat
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,37 +20,42 @@
 ## Installation
 
 You can easily install `Dictoat` using pip:
 
 ```bash
 pip install dictoat
 ```
+or via git:
 
+```bash
+git clone https://github.com/niCodeLine/dictoat.git
+```
+or just copy-paste it into your code.
 ## Usage
 
 To use Dictoat, simply import the `Dictoat` class in your Python project and pass a dictionary as an argument. For example:
 
 ```python
 from dictoat import Dictoat
 
 # Example of using Dictoat
-apple_dict = {"color": "red", "dimentions": {"weigh": 185, "radius": 5, "units": ["g", "cm"]}}
+apple_dict = {"flavor": "sweet", "colors": ["red", "green"],"dimentions": {"weigh": 185, "radius": 5}}
 apple = Dictoat(apple_dict)
 
 # Accessing the data
-print(apple.color_)
+print(apple.flavor_)
 print(apple.dimentions_.radius_)
-print(apple.dimentions_.units_)
+print(apple.colors_)
 ```
 
 The output would show:
 ```markdown
-red
+sweet
 5
-['g', 'cm']
+["red", "green"]
 ```
 
 Or a more complete example:
 
 ```python
 from dictoat import Dictoat
```

### Comparing `dictoat-0.1/setup.py` & `dictoat-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dictoat',
-    version='0.1',
+    version='1.0.1',
     packages=find_packages(),
     description='Convert a dict into an object to access items faster.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/niCodeLine/dictoat',
     author='Nico Spok',
     author_email='nicospok@hotmail.com',
```

