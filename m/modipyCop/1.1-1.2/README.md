# Comparing `tmp/modipyCop-1.1.tar.gz` & `tmp/modipyCop-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modipyCop-1.1.tar", last modified: Sun Dec 10 04:00:31 2023, max compression
+gzip compressed data, was "modipyCop-1.2.tar", last modified: Wed May 15 05:00:47 2024, max compression
```

## Comparing `modipyCop-1.1.tar` & `modipyCop-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 elnico     (501) staff       (20)        0 2023-12-10 04:00:31.370000 modipyCop-1.1/
--rwxrwxrwx   0 elnico     (501) staff       (20)     1066 2023-12-10 03:46:04.000000 modipyCop-1.1/LICENSE
--rwxrwxrwx   0 elnico     (501) staff       (20)     2456 2023-12-10 04:00:31.400000 modipyCop-1.1/PKG-INFO
--rwxrwxrwx   0 elnico     (501) staff       (20)     2015 2023-12-10 03:55:46.000000 modipyCop-1.1/README.md
--rwxrwxrwx   0 elnico     (501) staff       (20)       20 2023-12-10 03:46:04.000000 modipyCop-1.1/__init__.py
--rwxrwxrwx   0 elnico     (501) staff       (20)     2249 2023-12-10 03:46:04.000000 modipyCop-1.1/cop.py
-drwxrwxrwx   0 elnico     (501) staff       (20)        0 2023-12-10 04:00:31.380000 modipyCop-1.1/modipyCop.egg-info/
--rwxrwxrwx   0 elnico     (501) staff       (20)     2456 2023-12-10 04:00:30.000000 modipyCop-1.1/modipyCop.egg-info/PKG-INFO
--rwxrwxrwx   0 elnico     (501) staff       (20)      189 2023-12-10 04:00:31.000000 modipyCop-1.1/modipyCop.egg-info/SOURCES.txt
--rwxrwxrwx   0 elnico     (501) staff       (20)        1 2023-12-10 04:00:30.000000 modipyCop-1.1/modipyCop.egg-info/dependency_links.txt
--rwxrwxrwx   0 elnico     (501) staff       (20)        1 2023-12-10 04:00:30.000000 modipyCop-1.1/modipyCop.egg-info/top_level.txt
--rwxrwxrwx   0 elnico     (501) staff       (20)       38 2023-12-10 04:00:31.400000 modipyCop-1.1/setup.cfg
--rwxrwxrwx   0 elnico     (501) staff       (20)      624 2023-12-10 03:59:51.000000 modipyCop-1.1/setup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:00:47.630288 modipyCop-1.2/
+-rw-r--r--   0 nicospok   (501) staff       (20)     2782 2024-05-15 05:00:47.629588 modipyCop-1.2/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)     2363 2024-05-12 18:43:38.000000 modipyCop-1.2/README.md
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:00:47.624457 modipyCop-1.2/cop/
+-rw-r--r--   0 nicospok   (501) staff       (20)       20 2024-05-12 17:24:55.000000 modipyCop-1.2/cop/__init__.py
+-rw-r--r--   0 nicospok   (501) staff       (20)     2824 2024-05-12 19:46:43.000000 modipyCop-1.2/cop/cop.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 05:00:47.628792 modipyCop-1.2/modipyCop.egg-info/
+-rw-r--r--   0 nicospok   (501) staff       (20)     2782 2024-05-15 05:00:46.000000 modipyCop-1.2/modipyCop.egg-info/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)      177 2024-05-15 05:00:47.000000 modipyCop-1.2/modipyCop.egg-info/SOURCES.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-15 05:00:46.000000 modipyCop-1.2/modipyCop.egg-info/dependency_links.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        4 2024-05-15 05:00:46.000000 modipyCop-1.2/modipyCop.egg-info/top_level.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-15 05:00:47.630714 modipyCop-1.2/setup.cfg
+-rw-r--r--   0 nicospok   (501) staff       (20)      624 2024-05-12 19:11:57.000000 modipyCop-1.2/setup.py
```

### Comparing `modipyCop-1.1/PKG-INFO` & `modipyCop-1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: modipyCop
-Version: 1.1
+Version: 1.2
 Summary: Track modification made to file/s.
 Home-page: https://github.com/niCodeLine/modipy
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # ModipyCop
 
 ModipyCop is a Python tool that allows you to track modifications made to files or directories. Ideal for projects where monitoring changes in files is crucial, ModipyCop offers a simple and efficient way to get information on when files were last modified.
 
 ## Installation
 
@@ -28,34 +27,48 @@
 ## Usage
 
 To use ModipyCop, first import the Cop class into your Python project and then follow these steps:
 
 ```python
 from modipyCop import Cop
 
-# Create an instance of the Cop class for a specific directory or file and save the current state of files
+# Create an instance of the Cop class for a specific 
+# directory or file and save the current state of files
 directory = Cop("your/directory/path")
 directory.prev_revision()
 
 # Making changes in the directory files...
 
 # Check and get a list of the modified files
 directory.post_revision()
 ```
+
+Or be used as a decorator:
+
+```python
+from modipyCop import decoprator
+
+@decoprator('your/directory/path')
+def some_function(var,var_1):
+    # some_function code...
+
+```
+
 ## Outputs
 Depending on whether a path to a folder or a specific file is given, you can get different outputs:
 
 ### Folder
 For a folder path:
 ```markdown
 No file was modified in your/directory/path
 ```
 and
 ```markdown
 Modified files in your/directory/path:
+
 file_1.py, 1.23 seconds ago.
 text_1.txt, 4.56 seconds ago.
 ```
 
 ### File
 For an individual file path:
 
@@ -67,18 +80,21 @@
 file_1.py modified 7.89 seconds ago.
 ```
 
 ## Features
 
 - **Modification Tracking**: Allows tracking of the latest modifications of files or directories.
 - **Easy to Use**: A simple and straightforward interface for reviewing file changes.
+- **Usable as Decorator**: Avoid unneceserly writing and use the decorator module.
 
 ## Reminder
 Before using `post_revision()`, it's important to call `prev_revision()` to save the current state of the files. This ensures that `post_revision()` can accurately detect and report any changes made.
 
+*You can forget about this concern by just using the decoprator module as a decorator.*
+
 ## Contributions
 
 Contributions are welcome! If you have improvements or fixes, please feel free to send a pull request or open an issue in the GitHub repository.
 
 ## License
 
 This project is licensed under the MIT License. See the `LICENSE` file for more details.
```

### Comparing `modipyCop-1.1/README.md` & `modipyCop-1.2/modipyCop.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: modipyCop
+Version: 1.2
+Summary: Track modification made to file/s.
+Home-page: https://github.com/niCodeLine/modipy
+Author: Nico Spok
+Author-email: nicospok@hotmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # ModipyCop
 
 ModipyCop is a Python tool that allows you to track modifications made to files or directories. Ideal for projects where monitoring changes in files is crucial, ModipyCop offers a simple and efficient way to get information on when files were last modified.
 
 ## Installation
 
 You can easily install `modipyCop` using pip:
@@ -13,34 +27,48 @@
 ## Usage
 
 To use ModipyCop, first import the Cop class into your Python project and then follow these steps:
 
 ```python
 from modipyCop import Cop
 
-# Create an instance of the Cop class for a specific directory or file and save the current state of files
+# Create an instance of the Cop class for a specific 
+# directory or file and save the current state of files
 directory = Cop("your/directory/path")
 directory.prev_revision()
 
 # Making changes in the directory files...
 
 # Check and get a list of the modified files
 directory.post_revision()
 ```
+
+Or be used as a decorator:
+
+```python
+from modipyCop import decoprator
+
+@decoprator('your/directory/path')
+def some_function(var,var_1):
+    # some_function code...
+
+```
+
 ## Outputs
 Depending on whether a path to a folder or a specific file is given, you can get different outputs:
 
 ### Folder
 For a folder path:
 ```markdown
 No file was modified in your/directory/path
 ```
 and
 ```markdown
 Modified files in your/directory/path:
+
 file_1.py, 1.23 seconds ago.
 text_1.txt, 4.56 seconds ago.
 ```
 
 ### File
 For an individual file path:
 
@@ -52,18 +80,21 @@
 file_1.py modified 7.89 seconds ago.
 ```
 
 ## Features
 
 - **Modification Tracking**: Allows tracking of the latest modifications of files or directories.
 - **Easy to Use**: A simple and straightforward interface for reviewing file changes.
+- **Usable as Decorator**: Avoid unneceserly writing and use the decorator module.
 
 ## Reminder
 Before using `post_revision()`, it's important to call `prev_revision()` to save the current state of the files. This ensures that `post_revision()` can accurately detect and report any changes made.
 
+*You can forget about this concern by just using the decoprator module as a decorator.*
+
 ## Contributions
 
 Contributions are welcome! If you have improvements or fixes, please feel free to send a pull request or open an issue in the GitHub repository.
 
 ## License
 
 This project is licensed under the MIT License. See the `LICENSE` file for more details.
```

### Comparing `modipyCop-1.1/setup.py` & `modipyCop-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modipyCop',
-    version='1.1',
+    version='1.2',
     packages=find_packages(),
     description='Track modification made to file/s.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/niCodeLine/modipy',
     author='Nico Spok',
     author_email='nicospok@hotmail.com',
```

