# Comparing `tmp/zhlyr-4.1.tar.gz` & `tmp/zhlyr-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhlyr-4.1.tar", last modified: Mon May 13 08:55:46 2024, max compression
+gzip compressed data, was "zhlyr-4.2.tar", last modified: Wed May 15 15:06:32 2024, max compression
```

## Comparing `zhlyr-4.1.tar` & `zhlyr-4.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 08:55:46.417374 zhlyr-4.1/
--rw-rw-rw-   0        0        0     4188 2024-05-13 08:55:46.415372 zhlyr-4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3411 2024-05-13 08:54:58.000000 zhlyr-4.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 08:55:46.418372 zhlyr-4.1/setup.cfg
--rw-rw-rw-   0        0        0     1113 2024-05-13 08:55:28.000000 zhlyr-4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:55:46.386690 zhlyr-4.1/zhlyr/
--rw-rw-rw-   0        0        0       92 2024-05-10 14:01:33.000000 zhlyr-4.1/zhlyr/__init__.py
--rw-rw-rw-   0        0        0     1847 2024-05-13 08:30:55.000000 zhlyr-4.1/zhlyr/recosnize.py
--rw-rw-rw-   0        0        0     1933 2024-05-10 13:40:19.000000 zhlyr-4.1/zhlyr/serilize.py
--rw-rw-rw-   0        0        0     2179 2024-05-10 18:26:37.000000 zhlyr-4.1/zhlyr/zhlyr.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:55:46.413305 zhlyr-4.1/zhlyr.egg-info/
--rw-rw-rw-   0        0        0     4188 2024-05-13 08:55:46.000000 zhlyr-4.1/zhlyr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-05-13 08:55:46.000000 zhlyr-4.1/zhlyr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 08:55:46.000000 zhlyr-4.1/zhlyr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-13 08:55:46.000000 zhlyr-4.1/zhlyr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 15:06:32.310210 zhlyr-4.2/
+-rw-rw-rw-   0        0        0     4226 2024-05-15 15:06:32.309210 zhlyr-4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3411 2024-05-13 08:54:58.000000 zhlyr-4.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 15:06:32.311210 zhlyr-4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2024-05-15 15:05:02.000000 zhlyr-4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:06:32.294545 zhlyr-4.2/zhlyr/
+-rw-rw-rw-   0        0        0       92 2024-05-10 14:01:33.000000 zhlyr-4.2/zhlyr/__init__.py
+-rw-rw-rw-   0        0        0     1847 2024-05-13 08:30:55.000000 zhlyr-4.2/zhlyr/recosnize.py
+-rw-rw-rw-   0        0        0   486120 2024-05-15 15:06:31.000000 zhlyr-4.2/zhlyr/serialize.c
+-rw-rw-rw-   0        0        0     2179 2024-05-10 18:26:37.000000 zhlyr-4.2/zhlyr/zhlyr.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:06:32.306700 zhlyr-4.2/zhlyr.egg-info/
+-rw-rw-rw-   0        0        0     4226 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 15:06:32.000000 zhlyr-4.2/zhlyr.egg-info/top_level.txt
```

### Comparing `zhlyr-4.1/PKG-INFO` & `zhlyr-4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 4.1
+Version: 4.2
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires: requests
-Requires: shazamio
-Requires: shazam
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: shazamio
+Requires-Dist: shazam
+Requires-Dist: cython
 
 - ## What is zhlyr?
 - **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
 
 - ## Code Area :
 
   <details>
```

### Comparing `zhlyr-4.1/README.md` & `zhlyr-4.2/README.md`

 * *Files identical despite different names*

### Comparing `zhlyr-4.1/setup.py` & `zhlyr-4.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-from setuptools import setup , find_packages
-with open('README.md','r') as file:
-    setup(
-        name = 'zhlyr',
-        version = '4.1',
-        packages = find_packages(),
-        requires = ['requests','shazamio','shazam'],
-        long_description =file.read(),
-        long_description_content_type='text/markdown',
-        description = 'Python library for music handling',
-        author = 'Mtsky',
-        author_email = 'secon2636@gmail.com',
-        url = 'https://gaoc3.github.io/zhlyr/',
-        license = 'MIT',
-        classifiers=[
-            "Development Status :: 1 - Planning",
-            "Intended Audience :: Developers",
-            "License :: OSI Approved :: MIT License",
-            "Programming Language :: Python :: 3.9",
-            "Programming Language :: Python :: 3",
-            "Operating System :: Unix",
-            "Operating System :: MacOS :: MacOS X",
-            "Operating System :: Microsoft :: Windows",
-        ],
-        keywords= ['lyrics','music','shazam','serialize','serializer','recognize'],
-        python_requires=">=3.9"
-    )
+from setuptools import setup, find_packages
+from Cython.Build import cythonize
+
+with open('README.md', 'r') as file:
+    long_description = file.read()
+
+setup(
+    name='zhlyr',
+    version='4.2',
+    packages=find_packages(),
+    install_requires=['requests', 'shazamio', 'shazam', 'cython'],
+    ext_modules=cythonize('zhlyr/serialize.pyx'),
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    description='Python library for music handling',
+    author='Mtsky',
+    author_email='secon2636@gmail.com',
+    url='https://gaoc3.github.io/zhlyr/',
+    license='MIT',
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ],
+    keywords=['lyrics', 'music', 'shazam', 'serialize', 'serializer', 'recognize'],
+    python_requires=">=3.9",
+)
```

### Comparing `zhlyr-4.1/zhlyr/recosnize.py` & `zhlyr-4.2/zhlyr/recosnize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-4.1/zhlyr/zhlyr.py` & `zhlyr-4.2/zhlyr/zhlyr.py`

 * *Files identical despite different names*

### Comparing `zhlyr-4.1/zhlyr.egg-info/PKG-INFO` & `zhlyr-4.2/zhlyr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 4.1
+Version: 4.2
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires: requests
-Requires: shazamio
-Requires: shazam
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: shazamio
+Requires-Dist: shazam
+Requires-Dist: cython
 
 - ## What is zhlyr?
 - **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
 
 - ## Code Area :
 
   <details>
```

