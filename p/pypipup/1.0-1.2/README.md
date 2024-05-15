# Comparing `tmp/pypipup-1.0.tar.gz` & `tmp/pypipup-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipup-1.0.tar", last modified: Wed Dec 13 03:07:45 2023, max compression
+gzip compressed data, was "pypipup-1.2.tar", last modified: Wed May 15 06:00:57 2024, max compression
```

## Comparing `pypipup-1.0.tar` & `pypipup-1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0 elnico     (501) staff       (20)        0 2023-12-13 03:07:45.610000 pypipup-1.0/
--rwxrwxrwx   0 elnico     (501) staff       (20)     1066 2023-12-12 23:22:08.000000 pypipup-1.0/LICENSE
--rwxrwxrwx   0 elnico     (501) staff       (20)     1481 2023-12-13 03:07:45.640000 pypipup-1.0/PKG-INFO
--rwxrwxrwx   0 elnico     (501) staff       (20)     1017 2023-12-13 03:04:12.000000 pypipup-1.0/README.md
--rwxrwxrwx   0 elnico     (501) staff       (20)        0 2023-12-13 03:01:07.000000 pypipup-1.0/__init__.py
-drwxrwxrwx   0 elnico     (501) staff       (20)        0 2023-12-13 03:07:45.610000 pypipup-1.0/pypipup.egg-info/
--rwxrwxrwx   0 elnico     (501) staff       (20)     1481 2023-12-13 03:07:44.000000 pypipup-1.0/pypipup.egg-info/PKG-INFO
--rwxrwxrwx   0 elnico     (501) staff       (20)      173 2023-12-13 03:07:45.000000 pypipup-1.0/pypipup.egg-info/SOURCES.txt
--rwxrwxrwx   0 elnico     (501) staff       (20)        1 2023-12-13 03:07:44.000000 pypipup-1.0/pypipup.egg-info/dependency_links.txt
--rwxrwxrwx   0 elnico     (501) staff       (20)        1 2023-12-13 03:07:44.000000 pypipup-1.0/pypipup.egg-info/top_level.txt
--rwxrwxrwx   0 elnico     (501) staff       (20)     1448 2023-12-13 03:01:59.000000 pypipup-1.0/pypipup.py
--rwxrwxrwx   0 elnico     (501) staff       (20)       38 2023-12-13 03:07:45.640000 pypipup-1.0/setup.cfg
--rwxrwxrwx   0 elnico     (501) staff       (20)      647 2023-12-12 23:34:55.000000 pypipup-1.0/setup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 06:00:57.246984 pypipup-1.2/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:40:07.000000 pypipup-1.2/LICENSE
+-rw-r--r--   0 nicospok   (501) staff       (20)     1596 2024-05-15 06:00:57.246286 pypipup-1.2/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)     1132 2024-05-15 05:40:07.000000 pypipup-1.2/README.md
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 06:00:57.242252 pypipup-1.2/pypipup/
+-rw-r--r--   0 nicospok   (501) staff       (20)        6 2024-05-15 05:40:07.000000 pypipup-1.2/pypipup/__init__.py
+-rw-r--r--   0 nicospok   (501) staff       (20)     1452 2024-05-15 05:40:07.000000 pypipup-1.2/pypipup/pypipup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-15 06:00:57.245483 pypipup-1.2/pypipup.egg-info/
+-rw-r--r--   0 nicospok   (501) staff       (20)     1596 2024-05-15 06:00:56.000000 pypipup-1.2/pypipup.egg-info/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)      189 2024-05-15 06:00:57.000000 pypipup-1.2/pypipup.egg-info/SOURCES.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-15 06:00:56.000000 pypipup-1.2/pypipup.egg-info/dependency_links.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        8 2024-05-15 06:00:56.000000 pypipup-1.2/pypipup.egg-info/top_level.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-15 06:00:57.247186 pypipup-1.2/setup.cfg
+-rw-r--r--   0 nicospok   (501) staff       (20)      647 2024-05-15 05:52:11.000000 pypipup-1.2/setup.py
```

### Comparing `pypipup-1.0/LICENSE` & `pypipup-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypipup-1.0/PKG-INFO` & `pypipup-1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-Metadata-Version: 2.1
-Name: pypipup
-Version: 1.0
-Summary: Package that identifies and updates outdated pip packages.
-Home-page: https://github.com/niCodeLine/pypipup
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
 # pypipup
 
 This Python script automates the process of updating the Pip package manager and checking for outdated Python packages in your environment and attempts to update the outdated ones. 
 
 ## Installation
 
 You can easily install `pypipup` using pip:
 
 ```bash
 pip install pypipup
 ```
+or via git:
 
+```bash
+git clone https://github.com/niCodeLine/pypipup.git
+```
+or just copy-paste it into your code.
 ## Usage
 
 To use pypipup open a terminal or command prompt and run the script:
 
 ```bash
 python -m pypipup
 ```
 or for Python 3:
 ```bash
-python -m pypipup
+python3 -m pypipup
 ```
 
 ## Features
 
 - **Update Pip**: Guarantees the latest version of Pip is installed
 - **Check and Update Packages**: Scans for outdated packages and updates them.
 - **Verification**: Verifies the success of the update by rechecking for outdated packages.
```

### Comparing `pypipup-1.0/pypipup.egg-info/PKG-INFO` & `pypipup-1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipup
-Version: 1.0
+Version: 1.2
 Summary: Package that identifies and updates outdated pip packages.
 Home-page: https://github.com/niCodeLine/pypipup
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,25 +20,30 @@
 ## Installation
 
 You can easily install `pypipup` using pip:
 
 ```bash
 pip install pypipup
 ```
+or via git:
 
+```bash
+git clone https://github.com/niCodeLine/pypipup.git
+```
+or just copy-paste it into your code.
 ## Usage
 
 To use pypipup open a terminal or command prompt and run the script:
 
 ```bash
 python -m pypipup
 ```
 or for Python 3:
 ```bash
-python -m pypipup
+python3 -m pypipup
 ```
 
 ## Features
 
 - **Update Pip**: Guarantees the latest version of Pip is installed
 - **Check and Update Packages**: Scans for outdated packages and updates them.
 - **Verification**: Verifies the success of the update by rechecking for outdated packages.
```

### Comparing `pypipup-1.0/pypipup.py` & `pypipup-1.2/pypipup/pypipup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import subprocess
 
 def update_pips():
     try:
         print('> Updating pip...')
-        subprocess.call('pip install --upgrade pip', shell=True)
+        subprocess.call('pip3 install --upgrade pip', shell=True)
         print('Pip updated!')
 
         print('> Checking for outdated packages...')
-        subprocess.call('pip list -o > outdated_pips.txt', shell=True)
+        subprocess.call('pip3 list -o > outdated_pips.txt', shell=True)
 
         out_pips_file = 'outdated_pips.txt'
         print('- Updating packages...')
         with open(out_pips_file, 'r') as f:
             lines = f.readlines()
             for index, line in enumerate(lines):
                 package_name = line.strip().split(' ')[0]
                 if index > 1:
                     print(f'> Updating {package_name}...')
-                    subprocess.call(f'pip install {package_name} --upgrade', shell=True)
+                    subprocess.call(f'pip3 install {package_name} --upgrade', shell=True)
 
         print('Packages updated')
 
         print('> Checking un-updated pips...')
-        subprocess.call('pip list -o > outdated_pips.txt', shell=True)
+        subprocess.call('pip3 list -o > outdated_pips.txt', shell=True)
         with open(out_pips_file, 'r') as f:
             content = f.read()
             if not content:
                 print('All packages updated successfully!')
             else:
                 print(f'The following packages could not be updated:\n\n{content}')
         print('> Cleaning caché...')
```

### Comparing `pypipup-1.0/setup.py` & `pypipup-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pypipup',
-    version='1.0',
+    version='1.2',
     packages=find_packages(),
     description='Package that identifies and updates outdated pip packages.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/niCodeLine/pypipup',
     author='Nico Spok',
     author_email='nicospok@hotmail.com',
```

