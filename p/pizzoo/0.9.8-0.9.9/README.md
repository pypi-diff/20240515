# Comparing `tmp/pizzoo-0.9.8.tar.gz` & `tmp/pizzoo-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizzoo-0.9.8.tar", last modified: Tue May 14 11:25:17 2024, max compression
+gzip compressed data, was "pizzoo-0.9.9.tar", last modified: Tue May 14 12:10:11 2024, max compression
```

## Comparing `pizzoo-0.9.8.tar` & `pizzoo-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:25:17.548809 pizzoo-0.9.8/
--rw-rw-rw-   0        0        0       13 2024-05-14 10:02:11.000000 pizzoo-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7178 2024-05-14 11:25:17.546801 pizzoo-0.9.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 11:25:17.521170 pizzoo-0.9.8/pizzoo/
--rw-rw-rw-   0        0        0    22956 2024-05-14 11:19:25.000000 pizzoo-0.9.8/pizzoo/__init__.py
--rw-rw-rw-   0        0        0     1444 2024-04-23 11:16:55.000000 pizzoo-0.9.8/pizzoo/_constants.py
--rw-rw-rw-   0        0        0    17046 2024-05-08 13:13:17.000000 pizzoo-0.9.8/pizzoo/_renderers.py
--rw-rw-rw-   0        0        0      705 2024-04-29 07:23:44.000000 pizzoo-0.9.8/pizzoo/_utils.py
--rw-rw-rw-   0        0        0   106312 2024-05-14 11:17:54.000000 pizzoo-0.9.8/pizzoo/default.bdf
--rw-rw-rw-   0        0        0    21871 2024-05-13 09:32:25.000000 pizzoo-0.9.8/pizzoo/game.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:25:17.544133 pizzoo-0.9.8/pizzoo.egg-info/
--rw-rw-rw-   0        0        0     7178 2024-05-14 11:25:17.000000 pizzoo-0.9.8/pizzoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-05-14 11:25:17.000000 pizzoo-0.9.8/pizzoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:25:17.000000 pizzoo-0.9.8/pizzoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-14 11:25:17.000000 pizzoo-0.9.8/pizzoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 11:25:17.000000 pizzoo-0.9.8/pizzoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 11:25:17.549514 pizzoo-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1247 2024-05-14 11:22:50.000000 pizzoo-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:10:11.146134 pizzoo-0.9.9/
+-rw-rw-rw-   0        0        0       13 2024-05-14 10:02:11.000000 pizzoo-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7178 2024-05-14 12:10:11.142292 pizzoo-0.9.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 12:10:11.116461 pizzoo-0.9.9/pizzoo/
+-rw-rw-rw-   0        0        0    22956 2024-05-14 11:19:25.000000 pizzoo-0.9.9/pizzoo/__init__.py
+-rw-rw-rw-   0        0        0     1444 2024-04-23 11:16:55.000000 pizzoo-0.9.9/pizzoo/_constants.py
+-rw-rw-rw-   0        0        0    17046 2024-05-08 13:13:17.000000 pizzoo-0.9.9/pizzoo/_renderers.py
+-rw-rw-rw-   0        0        0      705 2024-04-29 07:23:44.000000 pizzoo-0.9.9/pizzoo/_utils.py
+-rw-rw-rw-   0        0        0   106312 2024-05-14 11:17:54.000000 pizzoo-0.9.9/pizzoo/default.bdf
+-rw-rw-rw-   0        0        0    21871 2024-05-13 09:32:25.000000 pizzoo-0.9.9/pizzoo/game.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:10:11.140211 pizzoo-0.9.9/pizzoo.egg-info/
+-rw-rw-rw-   0        0        0     7178 2024-05-14 12:10:11.000000 pizzoo-0.9.9/pizzoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-14 12:10:11.000000 pizzoo-0.9.9/pizzoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:10:11.000000 pizzoo-0.9.9/pizzoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-14 12:10:11.000000 pizzoo-0.9.9/pizzoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 12:10:11.000000 pizzoo-0.9.9/pizzoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 12:10:11.146134 pizzoo-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1247 2024-05-14 12:09:53.000000 pizzoo-0.9.9/setup.py
```

### Comparing `pizzoo-0.9.8/PKG-INFO` & `pizzoo-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.8
+Version: 0.9.9
 Summary: Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
@@ -145,8 +145,8 @@
 
 ## Contribute and/or donate
 This library was created and is maintained by a single developer, consider contributing with pull requests, new integrations, proposals or [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W).
 
 ## Special thanks
 This library exists thanks to other libraries that were an inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
 
-Also I want to give a special thanks [to my lovely fiancee](https://github.com/srtashadowfax) for all his support while developing this library, both technical and emotional 💖
+Also I want to give a special thanks [to my lovely fiancee](https://github.com/srtashadowfax) for all her support while developing this library, both technical and emotional 💖
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.8 Summary: Pizzoo is a easy-to-
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.9 Summary: Pizzoo is a easy-to-
 use library for rendering on pixel matrix screens like the Pixoo64, featuring
 easy new device integration, animation tools, and XML template rendering
 support. Home-page: https://github.com/pabletos/pizzoo#readme Author: Pablo
 Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics Classifier: License :: OSI Approved
@@ -69,9 +69,9 @@
 consider contributing with pull requests, new integrations, proposals or
 [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W). ##
 Special thanks This library exists thanks to other libraries that were an
 inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/
 pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://
 github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
 Also I want to give a special thanks [to my lovely fiancee](https://github.com/
-srtashadowfax) for all his support while developing this library, both
+srtashadowfax) for all her support while developing this library, both
 technical and emotional ð
```

### Comparing `pizzoo-0.9.8/pizzoo/__init__.py` & `pizzoo-0.9.9/pizzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.8/pizzoo/_constants.py` & `pizzoo-0.9.9/pizzoo/_constants.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.8/pizzoo/_renderers.py` & `pizzoo-0.9.9/pizzoo/_renderers.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.8/pizzoo/_utils.py` & `pizzoo-0.9.9/pizzoo/_utils.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.8/pizzoo/default.bdf` & `pizzoo-0.9.9/pizzoo/default.bdf`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.8/pizzoo/game.py` & `pizzoo-0.9.9/pizzoo/game.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.8/pizzoo.egg-info/PKG-INFO` & `pizzoo-0.9.9/pizzoo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.8
+Version: 0.9.9
 Summary: Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
@@ -145,8 +145,8 @@
 
 ## Contribute and/or donate
 This library was created and is maintained by a single developer, consider contributing with pull requests, new integrations, proposals or [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W).
 
 ## Special thanks
 This library exists thanks to other libraries that were an inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
 
-Also I want to give a special thanks [to my lovely fiancee](https://github.com/srtashadowfax) for all his support while developing this library, both technical and emotional 💖
+Also I want to give a special thanks [to my lovely fiancee](https://github.com/srtashadowfax) for all her support while developing this library, both technical and emotional 💖
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.8 Summary: Pizzoo is a easy-to-
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.9 Summary: Pizzoo is a easy-to-
 use library for rendering on pixel matrix screens like the Pixoo64, featuring
 easy new device integration, animation tools, and XML template rendering
 support. Home-page: https://github.com/pabletos/pizzoo#readme Author: Pablo
 Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics Classifier: License :: OSI Approved
@@ -69,9 +69,9 @@
 consider contributing with pull requests, new integrations, proposals or
 [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W). ##
 Special thanks This library exists thanks to other libraries that were an
 inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/
 pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://
 github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
 Also I want to give a special thanks [to my lovely fiancee](https://github.com/
-srtashadowfax) for all his support while developing this library, both
+srtashadowfax) for all her support while developing this library, both
 technical and emotional ð
```

### Comparing `pizzoo-0.9.8/setup.py` & `pizzoo-0.9.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 current_folder = path.abspath(path.dirname(__file__))
 long_description = open('%s\\README.md' % current_folder, encoding='utf-8').read()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name="pizzoo",
-    version="0.9.8",
+    version="0.9.9",
     author="Pablo Huet",
     description="Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.",
     long_description=long_description,
 	long_description_content_type='text/markdown',
 	license="MIT",
     keywords="pixoo, pixoo64, divoom, screen, pixel, matrix, render, buffer, LED matrix, LED, raspberry, raspberry pi",
     url="https://github.com/pabletos/pizzoo#readme",
```

