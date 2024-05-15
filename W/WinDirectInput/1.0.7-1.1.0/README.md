# Comparing `tmp/WinDirectInput-1.0.7.tar.gz` & `tmp/WinDirectInput-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinDirectInput-1.0.7.tar", last modified: Mon Feb 19 13:30:03 2024, max compression
+gzip compressed data, was "WinDirectInput-1.1.0.tar", last modified: Wed May 15 14:47:10 2024, max compression
```

## Comparing `WinDirectInput-1.0.7.tar` & `WinDirectInput-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-19 13:30:03.660948 WinDirectInput-1.0.7/
--rw-rw-rw-   0        0        0     1093 2024-02-02 06:02:27.000000 WinDirectInput-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     7530 2024-02-19 13:30:03.660948 WinDirectInput-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6871 2024-02-19 13:27:25.000000 WinDirectInput-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-02-19 13:30:03.659960 WinDirectInput-1.0.7/WinDirectInput.egg-info/
--rw-rw-rw-   0        0        0     7530 2024-02-19 13:30:03.000000 WinDirectInput-1.0.7/WinDirectInput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-02-19 13:30:03.000000 WinDirectInput-1.0.7/WinDirectInput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-19 13:30:03.000000 WinDirectInput-1.0.7/WinDirectInput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-02-19 13:30:03.000000 WinDirectInput-1.0.7/WinDirectInput.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-19 13:30:03.000000 WinDirectInput-1.0.7/WinDirectInput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    22902 2024-02-19 12:39:57.000000 WinDirectInput-1.0.7/directinput.py
--rw-rw-rw-   0        0        0       42 2024-02-19 13:30:03.660948 WinDirectInput-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      832 2024-02-19 13:29:59.000000 WinDirectInput-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:47:10.571281 WinDirectInput-1.1.0/
+-rw-rw-rw-   0        0        0     1093 2024-02-02 06:02:27.000000 WinDirectInput-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7553 2024-05-15 14:47:10.570281 WinDirectInput-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6849 2024-05-15 14:46:35.000000 WinDirectInput-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 14:47:10.569278 WinDirectInput-1.1.0/WinDirectInput.egg-info/
+-rw-rw-rw-   0        0        0     7553 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-15 14:47:10.000000 WinDirectInput-1.1.0/WinDirectInput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    43793 2024-05-15 14:38:13.000000 WinDirectInput-1.1.0/directinput.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:47:10.571281 WinDirectInput-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-05-15 12:32:05.000000 WinDirectInput-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:47:10.568273 WinDirectInput-1.1.0/tests/
+-rw-rw-rw-   0        0        0      118 2024-05-15 12:48:24.000000 WinDirectInput-1.1.0/tests/test.py
```

### Comparing `WinDirectInput-1.0.7/LICENSE` & `WinDirectInput-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WinDirectInput-1.0.7/PKG-INFO` & `WinDirectInput-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: WinDirectInput
-Version: 1.0.7
+Version: 1.1.0
 Summary: A Windows-specific package for simulating keyboard and mouse inputs
 Home-page: https://github.com/abdulrahimpds/WinDirectInput
 Author: AbdulRahim Khan
 Author-email: abdulrahimpds@gmail.com
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: numpy
@@ -73,15 +74,15 @@
 
 ### Writing Complex Strings
 
 ```Python
 import directinput
 
 # Writing a string with special characters
-directinput.write("Hello, world! 😃👍 #PythonRocks")
+directinput.write("Hello, world!")
 ```
 
 This demonstrates the enhanced write function, capable of handling a wide range of characters, surpassing limitations you might find in other modules.
 
 ### Detecting Key Presses
 
 ```Python
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `WinDirectInput-1.0.7/README.md` & `WinDirectInput-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ### Writing Complex Strings
 
 ```Python
 import directinput
 
 # Writing a string with special characters
-directinput.write("Hello, world! 😃👍 #PythonRocks")
+directinput.write("Hello, world!")
 ```
 
 This demonstrates the enhanced write function, capable of handling a wide range of characters, surpassing limitations you might find in other modules.
 
 ### Detecting Key Presses
 
 ```Python
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `WinDirectInput-1.0.7/WinDirectInput.egg-info/PKG-INFO` & `WinDirectInput-1.1.0/WinDirectInput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: WinDirectInput
-Version: 1.0.7
+Version: 1.1.0
 Summary: A Windows-specific package for simulating keyboard and mouse inputs
 Home-page: https://github.com/abdulrahimpds/WinDirectInput
 Author: AbdulRahim Khan
 Author-email: abdulrahimpds@gmail.com
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: numpy
@@ -73,15 +74,15 @@
 
 ### Writing Complex Strings
 
 ```Python
 import directinput
 
 # Writing a string with special characters
-directinput.write("Hello, world! 😃👍 #PythonRocks")
+directinput.write("Hello, world!")
 ```
 
 This demonstrates the enhanced write function, capable of handling a wide range of characters, surpassing limitations you might find in other modules.
 
 ### Detecting Key Presses
 
 ```Python
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `WinDirectInput-1.0.7/setup.py` & `WinDirectInput-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='WinDirectInput',
-    version='1.0.7',
+    version='1.1.0',
     author='AbdulRahim Khan',
     author_email='abdulrahimpds@gmail.com',
     description='A Windows-specific package for simulating keyboard and mouse inputs',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/abdulrahimpds/WinDirectInput',
     py_modules=['directinput'],
@@ -16,12 +16,13 @@
         'mss',
         'pyscreeze',
         'pillow',
         'pyperclip'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.8',
+        'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Microsoft :: Windows',
     ],
     python_requires='>=3.8'
 )
```

