# Comparing `tmp/smartpasslib-0.3.0.tar.gz` & `tmp/smartpasslib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartpasslib-0.3.0.tar", last modified: Wed May  8 08:01:12 2024, max compression
+gzip compressed data, was "smartpasslib-0.4.0.tar", last modified: Wed May 15 05:36:18 2024, max compression
```

## Comparing `smartpasslib-0.3.0.tar` & `smartpasslib-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 08:01:12.803636 smartpasslib-0.3.0/
--rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 07:36:51.000000 smartpasslib-0.3.0/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)      109 2024-05-08 07:50:33.000000 smartpasslib-0.3.0/MANIFEST.in
--rw-r--r--   0 smart     (1000) smart     (1000)     3151 2024-05-08 08:01:12.803636 smartpasslib-0.3.0/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     1952 2024-05-08 08:01:02.000000 smartpasslib-0.3.0/README.md
--rw-r--r--   0 smart     (1000) smart     (1000)        0 2024-05-08 07:49:52.000000 smartpasslib-0.3.0/requirements.txt
--rw-r--r--   0 smart     (1000) smart     (1000)     1251 2024-05-08 08:01:12.803636 smartpasslib-0.3.0/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)      387 2024-05-08 07:55:29.000000 smartpasslib-0.3.0/setup.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 08:01:12.800303 smartpasslib-0.3.0/smartpasslib/
--rw-r--r--   0 smart     (1000) smart     (1000)      371 2024-05-08 08:01:02.000000 smartpasslib-0.3.0/smartpasslib/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)     4545 2024-05-08 07:41:10.000000 smartpasslib-0.3.0/smartpasslib/generators.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 08:01:12.800303 smartpasslib-0.3.0/smartpasslib.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     3151 2024-05-08 08:01:12.000000 smartpasslib-0.3.0/smartpasslib.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      304 2024-05-08 08:01:12.000000 smartpasslib-0.3.0/smartpasslib.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-08 08:01:12.000000 smartpasslib-0.3.0/smartpasslib.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-08 08:01:12.000000 smartpasslib-0.3.0/smartpasslib.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       13 2024-05-08 08:01:12.000000 smartpasslib-0.3.0/smartpasslib.egg-info/top_level.txt
--rw-r--r--   0 smart     (1000) smart     (1000)      103 2024-05-08 07:56:03.000000 smartpasslib-0.3.0/tox.ini
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:36:18.067734 smartpasslib-0.4.0/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 07:36:51.000000 smartpasslib-0.4.0/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)      109 2024-05-08 07:50:33.000000 smartpasslib-0.4.0/MANIFEST.in
+-rw-r--r--   0 smart     (1000) smart     (1000)     3868 2024-05-15 05:36:18.067734 smartpasslib-0.4.0/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     2635 2024-05-15 05:35:24.000000 smartpasslib-0.4.0/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)       18 2024-05-15 05:13:20.000000 smartpasslib-0.4.0/requirements.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)     1271 2024-05-15 05:36:18.071068 smartpasslib-0.4.0/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)      387 2024-05-08 07:55:29.000000 smartpasslib-0.4.0/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:36:18.067734 smartpasslib-0.4.0/smartpasslib/
+-rw-r--r--   0 smart     (1000) smart     (1000)      371 2024-05-15 05:35:24.000000 smartpasslib-0.4.0/smartpasslib/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     2839 2024-05-15 05:33:08.000000 smartpasslib-0.4.0/smartpasslib/generators.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:36:18.067734 smartpasslib-0.4.0/smartpasslib.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     3868 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      339 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       19 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/requires.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)       13 2024-05-15 05:36:18.000000 smartpasslib-0.4.0/smartpasslib.egg-info/top_level.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)      103 2024-05-08 07:56:03.000000 smartpasslib-0.4.0/tox.ini
```

### Comparing `smartpasslib-0.3.0/LICENSE` & `smartpasslib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartpasslib-0.3.0/PKG-INFO` & `smartpasslib-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpasslib
-Version: 0.3.0
+Version: 0.4.0
 Summary: 'Cross-platform library for generating smart passwords.'
 Home-page: https://github.com/smartlegionlab
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartpasslib/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartpasslib/releases
@@ -20,14 +20,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: smartrandom~=0.1.0
 
 # Smart Passwords Library
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartpasslib)](https://github.com/smartlegionlab/smartpasslib/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartpasslib?label=pypi%20downloads)](https://pypi.org/project/smartpasslib/)
@@ -39,25 +40,60 @@
 ***
 
 ## Short Description:
 ___smartpasslib___ - Cross-platform library for generating smart passwords.
 
 ***
 
+Author and developer: ___A.A Suvorov.___
+
+***
+
 ## Supported:
 
 - Linux: All.
 - Windows: 7/8/10.
 - Termux (Android).
   
 ***
 
 ## What's new?
 
-### ___smartpasslib v0.3.0___
+### ___smartpasslib v0.4.0___
+
+***
+
+## Requirements:
+
+[smartrandom](https://github.com/smartlegionlab/smartrandom/) - Random Data Generators.
+
+***
+
+## Help:
+
+`pip install smartpasslib`
+
+```python
+from smartpasslib.generators import SmartPasswordMaster
+
+login = 'login'
+secret = 'secret'
+length = 15
+
+master = SmartPasswordMaster()
+
+smart_password = master.get_smart_password(login=login, secret=secret, length=length)
+smart_password2 = master.get_smart_password(login=login, secret=secret, length=length)
+check_passwords = smart_password == smart_password2  # True
+
+key = master.get_public_key(login, secret)
+
+check_data = master.check_data(login, secret, key)
+
+```
 
 ***
 
     THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
     AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
     IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
     DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
```

### Comparing `smartpasslib-0.3.0/setup.cfg` & `smartpasslib-0.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -32,12 +32,13 @@
 
 [options]
 python_requires = >=3.6
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
+	smartrandom~=0.1.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `smartpasslib-0.3.0/smartpasslib.egg-info/PKG-INFO` & `smartpasslib-0.4.0/smartpasslib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpasslib
-Version: 0.3.0
+Version: 0.4.0
 Summary: 'Cross-platform library for generating smart passwords.'
 Home-page: https://github.com/smartlegionlab
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartpasslib/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartpasslib/releases
@@ -20,14 +20,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: smartrandom~=0.1.0
 
 # Smart Passwords Library
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartpasslib)](https://github.com/smartlegionlab/smartpasslib/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartpasslib?label=pypi%20downloads)](https://pypi.org/project/smartpasslib/)
@@ -39,25 +40,60 @@
 ***
 
 ## Short Description:
 ___smartpasslib___ - Cross-platform library for generating smart passwords.
 
 ***
 
+Author and developer: ___A.A Suvorov.___
+
+***
+
 ## Supported:
 
 - Linux: All.
 - Windows: 7/8/10.
 - Termux (Android).
   
 ***
 
 ## What's new?
 
-### ___smartpasslib v0.3.0___
+### ___smartpasslib v0.4.0___
+
+***
+
+## Requirements:
+
+[smartrandom](https://github.com/smartlegionlab/smartrandom/) - Random Data Generators.
+
+***
+
+## Help:
+
+`pip install smartpasslib`
+
+```python
+from smartpasslib.generators import SmartPasswordMaster
+
+login = 'login'
+secret = 'secret'
+length = 15
+
+master = SmartPasswordMaster()
+
+smart_password = master.get_smart_password(login=login, secret=secret, length=length)
+smart_password2 = master.get_smart_password(login=login, secret=secret, length=length)
+check_passwords = smart_password == smart_password2  # True
+
+key = master.get_public_key(login, secret)
+
+check_data = master.check_data(login, secret, key)
+
+```
 
 ***
 
     THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
     AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
     IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
     DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
```

