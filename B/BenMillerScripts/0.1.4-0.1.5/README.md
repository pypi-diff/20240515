# Comparing `tmp/BenMillerScripts-0.1.4.tar.gz` & `tmp/benmillerscripts-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BenMillerScripts-0.1.4.tar", last modified: Tue Jun  7 19:57:39 2022, max compression
+gzip compressed data, was "benmillerscripts-0.1.5.tar", last modified: Wed May 15 20:19:00 2024, max compression
```

## Comparing `BenMillerScripts-0.1.4.tar` & `benmillerscripts-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/
-drwxrwxrwx   0        0        0        0 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/BenMillerScripts.egg-info/
--rw-rw-rw-   0        0        0     1725 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/BenMillerScripts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/BenMillerScripts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/BenMillerScripts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/BenMillerScripts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/BenMillerScripts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1725 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2022-06-07 19:55:05.000000 BenMillerScripts-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/benmillerscripts/
--rw-rw-rw-   0        0        0    40715 2021-08-16 20:38:01.000000 BenMillerScripts-0.1.4/benmillerscripts/FFTArrayAnalysis.py
--rw-rw-rw-   0        0        0     1764 2021-01-04 23:34:33.000000 BenMillerScripts-0.1.4/benmillerscripts/FileDialogs.py
--rw-rw-rw-   0        0        0       42 2022-06-07 19:57:39.000000 BenMillerScripts-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      800 2022-06-07 19:55:37.000000 BenMillerScripts-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:19:00.288806 benmillerscripts-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-15 20:19:00.283808 benmillerscripts-0.1.5/BenMillerScripts.egg-info/
+-rw-rw-rw-   0        0        0     1673 2024-05-15 20:19:00.000000 benmillerscripts-0.1.5/BenMillerScripts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-15 20:19:00.000000 benmillerscripts-0.1.5/BenMillerScripts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:19:00.000000 benmillerscripts-0.1.5/BenMillerScripts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-15 20:19:00.000000 benmillerscripts-0.1.5/BenMillerScripts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 20:19:00.000000 benmillerscripts-0.1.5/BenMillerScripts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2020-10-05 21:28:14.000000 benmillerscripts-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1673 2024-05-15 20:19:00.286807 benmillerscripts-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1138 2022-06-07 19:55:05.000000 benmillerscripts-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 20:19:00.280809 benmillerscripts-0.1.5/benmillerscripts/
+-rw-rw-rw-   0        0        0    40715 2021-08-16 20:38:01.000000 benmillerscripts-0.1.5/benmillerscripts/FFTArrayAnalysis.py
+-rw-rw-rw-   0        0        0     1764 2021-01-04 23:34:33.000000 benmillerscripts-0.1.5/benmillerscripts/FileDialogs.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:19:00.288806 benmillerscripts-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-05-15 20:18:30.000000 benmillerscripts-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `BenMillerScripts-0.1.4/BenMillerScripts.egg-info/PKG-INFO` & `benmillerscripts-0.1.5/BenMillerScripts.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 Metadata-Version: 2.1
 Name: BenMillerScripts
-Version: 0.1.4
+Version: 0.1.5
 Summary: Modules for Running Python scripts by Ben Miller in DigitalMicrograph
 Home-page: https://www.gatan.com/resources/python-scripts
 Author: Ben Miller
 Author-email: benmiller002@aol.com
 License: MIT
-Description: BenMillerScripts
-        ---
-        This is a collection of Python Modules that I've written to support my Python scripts that can be run from the embedded Python in Gatan's [DigitalMicrograph](https://www.gatan.com/resources/software) software 
-        
-        For more information on using Python in DigitalMicrograph, visit this page on [Gatan's Website](https://www.gatan.com/resources/python-scripts).
-        
-        
-        
-        Installing
-        ---
-        If you don't yet have Python in DigitalMicrograph, first install DigitalMicrograph 3.4 or greater, and during installation, choose to install Python. More details can be found at the links above. 
-        
-        Next, open an Anaconda prompt. This should be listed in the Windows start menu program list. You may want to run this as an admin. 
-        In the Anaconda prompt enter the following:
-        
-        `activate GMS_VENV_PYTHON`
-        
-        This will activate the virtual environment that DigitalMicrograph uses. 
-        
-        Next, install the package by entering the following command.
-        
-        `pip install BenMillerScripts`
-        
-        Usage
-        ---
-        
-        This module is used by my [Live FFT Color Map script](https://www.gatan.com/sites/default/files/Scripts/Live%20FFT%20Color%20Map.py).
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scikit-learn
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-image
+Requires-Dist: pandas
+Requires-Dist: tqdm
+
+BenMillerScripts
+---
+This is a collection of Python Modules that I've written to support my Python scripts that can be run from the embedded Python in Gatan's [DigitalMicrograph](https://www.gatan.com/resources/software) software 
+
+For more information on using Python in DigitalMicrograph, visit this page on [Gatan's Website](https://www.gatan.com/resources/python-scripts).
+
+
+
+Installing
+---
+If you don't yet have Python in DigitalMicrograph, first install DigitalMicrograph 3.4 or greater, and during installation, choose to install Python. More details can be found at the links above. 
+
+Next, open an Anaconda prompt. This should be listed in the Windows start menu program list. You may want to run this as an admin. 
+In the Anaconda prompt enter the following:
+
+`activate GMS_VENV_PYTHON`
+
+This will activate the virtual environment that DigitalMicrograph uses. 
+
+Next, install the package by entering the following command.
+
+`pip install BenMillerScripts`
+
+Usage
+---
+
+This module is used by my [Live FFT Color Map script](https://www.gatan.com/sites/default/files/Scripts/Live%20FFT%20Color%20Map.py).
```

### Comparing `BenMillerScripts-0.1.4/PKG-INFO` & `benmillerscripts-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 Metadata-Version: 2.1
 Name: BenMillerScripts
-Version: 0.1.4
+Version: 0.1.5
 Summary: Modules for Running Python scripts by Ben Miller in DigitalMicrograph
 Home-page: https://www.gatan.com/resources/python-scripts
 Author: Ben Miller
 Author-email: benmiller002@aol.com
 License: MIT
-Description: BenMillerScripts
-        ---
-        This is a collection of Python Modules that I've written to support my Python scripts that can be run from the embedded Python in Gatan's [DigitalMicrograph](https://www.gatan.com/resources/software) software 
-        
-        For more information on using Python in DigitalMicrograph, visit this page on [Gatan's Website](https://www.gatan.com/resources/python-scripts).
-        
-        
-        
-        Installing
-        ---
-        If you don't yet have Python in DigitalMicrograph, first install DigitalMicrograph 3.4 or greater, and during installation, choose to install Python. More details can be found at the links above. 
-        
-        Next, open an Anaconda prompt. This should be listed in the Windows start menu program list. You may want to run this as an admin. 
-        In the Anaconda prompt enter the following:
-        
-        `activate GMS_VENV_PYTHON`
-        
-        This will activate the virtual environment that DigitalMicrograph uses. 
-        
-        Next, install the package by entering the following command.
-        
-        `pip install BenMillerScripts`
-        
-        Usage
-        ---
-        
-        This module is used by my [Live FFT Color Map script](https://www.gatan.com/sites/default/files/Scripts/Live%20FFT%20Color%20Map.py).
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scikit-learn
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-image
+Requires-Dist: pandas
+Requires-Dist: tqdm
+
+BenMillerScripts
+---
+This is a collection of Python Modules that I've written to support my Python scripts that can be run from the embedded Python in Gatan's [DigitalMicrograph](https://www.gatan.com/resources/software) software 
+
+For more information on using Python in DigitalMicrograph, visit this page on [Gatan's Website](https://www.gatan.com/resources/python-scripts).
+
+
+
+Installing
+---
+If you don't yet have Python in DigitalMicrograph, first install DigitalMicrograph 3.4 or greater, and during installation, choose to install Python. More details can be found at the links above. 
+
+Next, open an Anaconda prompt. This should be listed in the Windows start menu program list. You may want to run this as an admin. 
+In the Anaconda prompt enter the following:
+
+`activate GMS_VENV_PYTHON`
+
+This will activate the virtual environment that DigitalMicrograph uses. 
+
+Next, install the package by entering the following command.
+
+`pip install BenMillerScripts`
+
+Usage
+---
+
+This module is used by my [Live FFT Color Map script](https://www.gatan.com/sites/default/files/Scripts/Live%20FFT%20Color%20Map.py).
```

### Comparing `BenMillerScripts-0.1.4/README.md` & `benmillerscripts-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `BenMillerScripts-0.1.4/benmillerscripts/FFTArrayAnalysis.py` & `benmillerscripts-0.1.5/benmillerscripts/FFTArrayAnalysis.py`

 * *Files identical despite different names*

### Comparing `BenMillerScripts-0.1.4/benmillerscripts/FileDialogs.py` & `benmillerscripts-0.1.5/benmillerscripts/FileDialogs.py`

 * *Files identical despite different names*

### Comparing `BenMillerScripts-0.1.4/setup.py` & `benmillerscripts-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     url='https://www.gatan.com/resources/python-scripts',
     author='Ben Miller',
     author_email='benmiller002@aol.com',
     packages=['benmillerscripts'],
     # Needed for dependencies
     install_requires=['scikit-learn', 'matplotlib', 'numpy', 'scipy', 'scikit-image', 'pandas', 'tqdm'],
     # *strongly* suggested for sharing
-    version='0.1.4',
+    version='0.1.5',
     # The license can be anything you like
     license='MIT',
     description='Modules for Running Python scripts by Ben Miller in DigitalMicrograph',
     long_description=long_description,
     long_description_content_type="text/markdown",
 	python_requires = '>=3.7',
 	)
```

