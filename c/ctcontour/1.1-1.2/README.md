# Comparing `tmp/ctcontour-1.1.tar.gz` & `tmp/ctcontour-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ericpace/PycharmProjects/ctcontour/dist/.tmp-2dd2xtmc/ctcontour-1.1.tar", last modified: Thu Mar 21 13:46:36 2024, max compression
+gzip compressed data, was "/Users/ericpace/PycharmProjects/ctcontour/dist/.tmp-6o4d3dgu/ctcontour-1.2.tar", last modified: Wed May 15 13:30:49 2024, max compression
```

## Comparing `ctcontour-1.1.tar` & `ctcontour-1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ericpace   (501) staff       (20)        0 2024-03-21 13:46:36.740869 ctcontour-1.1/
--rw-r--r--   0 ericpace   (501) staff       (20)    35148 2022-05-05 18:36:22.000000 ctcontour-1.1/LICENSE.txt
--rw-r--r--   0 ericpace   (501) staff       (20)      735 2024-03-21 13:46:36.740455 ctcontour-1.1/PKG-INFO
--rw-r--r--   0 ericpace   (501) staff       (20)     4658 2024-03-06 16:59:39.000000 ctcontour-1.1/README.md
-drwxr-xr-x   0 ericpace   (501) staff       (20)        0 2024-03-21 13:46:36.737630 ctcontour-1.1/ctcontour/
--rw-r--r--   0 ericpace   (501) staff       (20)        0 2022-05-05 18:10:17.000000 ctcontour-1.1/ctcontour/__init__.py
--rw-r--r--   0 ericpace   (501) staff       (20)     4529 2024-03-21 13:35:13.000000 ctcontour-1.1/ctcontour/__main__.py
--rw-r--r--   0 ericpace   (501) staff       (20)     1748 2024-03-21 13:35:13.000000 ctcontour-1.1/ctcontour/config.py
--rw-r--r--   0 ericpace   (501) staff       (20)     5800 2024-03-21 13:35:13.000000 ctcontour-1.1/ctcontour/contour_proc.py
--rw-r--r--   0 ericpace   (501) staff       (20)     1431 2024-03-21 13:35:13.000000 ctcontour-1.1/ctcontour/contours.py
--rw-r--r--   0 ericpace   (501) staff       (20)     1117 2024-03-21 13:35:13.000000 ctcontour-1.1/ctcontour/decorator_funcs.py
--rw-r--r--   0 ericpace   (501) staff       (20)     5097 2022-11-08 20:20:01.000000 ctcontour-1.1/ctcontour/io_tools.py
--rw-r--r--   0 ericpace   (501) staff       (20)     3507 2022-11-06 08:16:58.000000 ctcontour-1.1/ctcontour/plot_tools.py
--rw-r--r--   0 ericpace   (501) staff       (20)    16893 2024-03-21 13:35:13.000000 ctcontour-1.1/ctcontour/slice.py
-drwxr-xr-x   0 ericpace   (501) staff       (20)        0 2024-03-21 13:46:36.740008 ctcontour-1.1/ctcontour.egg-info/
--rw-r--r--   0 ericpace   (501) staff       (20)      735 2024-03-21 13:46:36.000000 ctcontour-1.1/ctcontour.egg-info/PKG-INFO
--rw-r--r--   0 ericpace   (501) staff       (20)      436 2024-03-21 13:46:36.000000 ctcontour-1.1/ctcontour.egg-info/SOURCES.txt
--rw-r--r--   0 ericpace   (501) staff       (20)        1 2024-03-21 13:46:36.000000 ctcontour-1.1/ctcontour.egg-info/dependency_links.txt
--rw-r--r--   0 ericpace   (501) staff       (20)       51 2024-03-21 13:46:36.000000 ctcontour-1.1/ctcontour.egg-info/entry_points.txt
--rw-r--r--   0 ericpace   (501) staff       (20)      126 2024-03-21 13:46:36.000000 ctcontour-1.1/ctcontour.egg-info/requires.txt
--rw-r--r--   0 ericpace   (501) staff       (20)       10 2024-03-21 13:46:36.000000 ctcontour-1.1/ctcontour.egg-info/top_level.txt
--rw-r--r--   0 ericpace   (501) staff       (20)       38 2024-03-21 13:46:36.740952 ctcontour-1.1/setup.cfg
--rw-r--r--   0 ericpace   (501) staff       (20)     1750 2024-03-21 13:35:13.000000 ctcontour-1.1/setup.py
+drwxr-xr-x   0 ericpace   (501) staff       (20)        0 2024-05-15 13:30:49.612588 ctcontour-1.2/
+-rw-r--r--   0 ericpace   (501) staff       (20)    35148 2022-05-05 18:36:22.000000 ctcontour-1.2/LICENSE.txt
+-rw-r--r--   0 ericpace   (501) staff       (20)      764 2024-05-15 13:30:49.612150 ctcontour-1.2/PKG-INFO
+-rw-r--r--   0 ericpace   (501) staff       (20)     4658 2024-03-06 16:59:39.000000 ctcontour-1.2/README.md
+drwxr-xr-x   0 ericpace   (501) staff       (20)        0 2024-05-15 13:30:49.608965 ctcontour-1.2/ctcontour/
+-rw-r--r--   0 ericpace   (501) staff       (20)        0 2022-05-05 18:10:17.000000 ctcontour-1.2/ctcontour/__init__.py
+-rw-r--r--   0 ericpace   (501) staff       (20)     4529 2024-05-15 13:14:21.000000 ctcontour-1.2/ctcontour/__main__.py
+-rw-r--r--   0 ericpace   (501) staff       (20)     1748 2024-05-15 13:14:21.000000 ctcontour-1.2/ctcontour/config.py
+-rw-r--r--   0 ericpace   (501) staff       (20)     5800 2024-05-15 13:14:21.000000 ctcontour-1.2/ctcontour/contour_proc.py
+-rw-r--r--   0 ericpace   (501) staff       (20)     1431 2024-05-15 13:14:21.000000 ctcontour-1.2/ctcontour/contours.py
+-rw-r--r--   0 ericpace   (501) staff       (20)     1117 2024-05-15 13:14:21.000000 ctcontour-1.2/ctcontour/decorator_funcs.py
+-rw-r--r--   0 ericpace   (501) staff       (20)     5097 2024-05-15 13:13:20.000000 ctcontour-1.2/ctcontour/io_tools.py
+-rw-r--r--   0 ericpace   (501) staff       (20)     3507 2022-11-06 08:16:58.000000 ctcontour-1.2/ctcontour/plot_tools.py
+-rw-r--r--   0 ericpace   (501) staff       (20)    16893 2024-05-15 13:14:21.000000 ctcontour-1.2/ctcontour/slice.py
+drwxr-xr-x   0 ericpace   (501) staff       (20)        0 2024-05-15 13:30:49.611665 ctcontour-1.2/ctcontour.egg-info/
+-rw-r--r--   0 ericpace   (501) staff       (20)      764 2024-05-15 13:30:49.000000 ctcontour-1.2/ctcontour.egg-info/PKG-INFO
+-rw-r--r--   0 ericpace   (501) staff       (20)      436 2024-05-15 13:30:49.000000 ctcontour-1.2/ctcontour.egg-info/SOURCES.txt
+-rw-r--r--   0 ericpace   (501) staff       (20)        1 2024-05-15 13:30:49.000000 ctcontour-1.2/ctcontour.egg-info/dependency_links.txt
+-rw-r--r--   0 ericpace   (501) staff       (20)       51 2024-05-15 13:30:49.000000 ctcontour-1.2/ctcontour.egg-info/entry_points.txt
+-rw-r--r--   0 ericpace   (501) staff       (20)      140 2024-05-15 13:30:49.000000 ctcontour-1.2/ctcontour.egg-info/requires.txt
+-rw-r--r--   0 ericpace   (501) staff       (20)       10 2024-05-15 13:30:49.000000 ctcontour-1.2/ctcontour.egg-info/top_level.txt
+-rw-r--r--   0 ericpace   (501) staff       (20)       38 2024-05-15 13:30:49.612681 ctcontour-1.2/setup.cfg
+-rw-r--r--   0 ericpace   (501) staff       (20)     1775 2024-05-15 13:16:58.000000 ctcontour-1.2/setup.py
```

### Comparing `ctcontour-1.1/LICENSE.txt` & `ctcontour-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/PKG-INFO` & `ctcontour-1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctcontour
-Version: 1.1
+Version: 1.2
 Summary: Fully automated patient abdomino-pelvic contouring for CT images. https://doi.org/10.1016/j.ejmp.2022.10.027.
 Home-page: https://github.com/ericpace/ct_contour
 Author: Eric Pace
 Author-email: ericpace@pm.me
 License: GNU GPLv3
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
@@ -13,9 +13,10 @@
 Requires-Dist: numba==0.52.0
 Requires-Dist: scipy==1.4.1
 Requires-Dist: scikit-image==0.18.2
 Requires-Dist: pandas==1.2.1
 Requires-Dist: matplotlib==3.3.4
 Requires-Dist: seaborn==0.11.1
 Requires-Dist: PyPDF2==1.26.0
+Requires-Dist: numpy==1.23.4
 
 Fully automated patient abdomino-pelvic contouring for CT images. https://doi.org/10.1016/j.ejmp.2022.10.027.
```

### Comparing `ctcontour-1.1/README.md` & `ctcontour-1.2/README.md`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/ctcontour/__main__.py` & `ctcontour-1.2/ctcontour/__main__.py`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/ctcontour/config.py` & `ctcontour-1.2/ctcontour/config.py`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/ctcontour/contour_proc.py` & `ctcontour-1.2/ctcontour/contour_proc.py`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/ctcontour/contours.py` & `ctcontour-1.2/ctcontour/contours.py`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/ctcontour/decorator_funcs.py` & `ctcontour-1.2/ctcontour/decorator_funcs.py`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/ctcontour/io_tools.py` & `ctcontour-1.2/ctcontour/io_tools.py`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/ctcontour/plot_tools.py` & `ctcontour-1.2/ctcontour/plot_tools.py`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/ctcontour/slice.py` & `ctcontour-1.2/ctcontour/slice.py`

 * *Files identical despite different names*

### Comparing `ctcontour-1.1/ctcontour.egg-info/PKG-INFO` & `ctcontour-1.2/ctcontour.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctcontour
-Version: 1.1
+Version: 1.2
 Summary: Fully automated patient abdomino-pelvic contouring for CT images. https://doi.org/10.1016/j.ejmp.2022.10.027.
 Home-page: https://github.com/ericpace/ct_contour
 Author: Eric Pace
 Author-email: ericpace@pm.me
 License: GNU GPLv3
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
@@ -13,9 +13,10 @@
 Requires-Dist: numba==0.52.0
 Requires-Dist: scipy==1.4.1
 Requires-Dist: scikit-image==0.18.2
 Requires-Dist: pandas==1.2.1
 Requires-Dist: matplotlib==3.3.4
 Requires-Dist: seaborn==0.11.1
 Requires-Dist: PyPDF2==1.26.0
+Requires-Dist: numpy==1.23.4
 
 Fully automated patient abdomino-pelvic contouring for CT images. https://doi.org/10.1016/j.ejmp.2022.10.027.
```

### Comparing `ctcontour-1.1/setup.py` & `ctcontour-1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 setuptools.setup(
     author="Eric Pace",
     author_email="ericpace@pm.me",
     name='ctcontour',
     license="GNU GPLv3",
     description='Fully automated patient abdomino-pelvic contouring for CT images. https://doi.org/10.1016/j.ejmp.2022.10.027.',
-    version='v1.1',
+    version='v1.2',
     long_description='Fully automated patient abdomino-pelvic contouring for CT images. https://doi.org/10.1016/j.ejmp.2022.10.027.',
     url='https://github.com/ericpace/ct_contour',
     packages=setuptools.find_packages(),
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'ctc=ctcontour.__main__:contour',
@@ -42,13 +42,14 @@
         'pydicom==2.1.2',
         'numba==0.52.0',
         'scipy==1.4.1',
         'scikit-image==0.18.2',
         'pandas==1.2.1',
         'matplotlib==3.3.4',
         'seaborn==0.11.1',
-        'PyPDF2==1.26.0'
+        'PyPDF2==1.26.0',
+        'numpy==1.23.4'
     ],
     classifiers=[
         'Programming Language :: Python'
     ],
 )
```

