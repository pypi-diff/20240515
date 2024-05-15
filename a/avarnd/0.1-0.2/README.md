# Comparing `tmp/avarnd-0.1.tar.gz` & `tmp/avarnd-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avarnd-0.1.tar", last modified: Wed May 15 11:17:20 2024, max compression
+gzip compressed data, was "avarnd-0.2.tar", last modified: Wed May 15 10:35:21 2024, max compression
```

## Comparing `avarnd-0.1.tar` & `avarnd-0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxr-xr-x   0 shriyoki   (502) staff       (20)        0 2024-05-15 11:17:20.624945 avarnd-0.1/
--rw-r--r--   0 shriyoki   (502) staff       (20)     1080 2024-05-15 11:14:13.000000 avarnd-0.1/LICENSE
--rw-r--r--   0 shriyoki   (502) staff       (20)     1086 2024-05-15 11:17:20.624889 avarnd-0.1/PKG-INFO
--rw-r--r--   0 shriyoki   (502) staff       (20)        8 2024-05-15 11:14:13.000000 avarnd-0.1/README.md
-drwxr-xr-x   0 shriyoki   (502) staff       (20)        0 2024-05-15 11:17:20.624728 avarnd-0.1/avarnd.egg-info/
--rw-r--r--   0 shriyoki   (502) staff       (20)     1086 2024-05-15 11:17:20.000000 avarnd-0.1/avarnd.egg-info/PKG-INFO
--rw-r--r--   0 shriyoki   (502) staff       (20)      156 2024-05-15 11:17:20.000000 avarnd-0.1/avarnd.egg-info/SOURCES.txt
--rw-r--r--   0 shriyoki   (502) staff       (20)        1 2024-05-15 11:17:20.000000 avarnd-0.1/avarnd.egg-info/dependency_links.txt
--rw-r--r--   0 shriyoki   (502) staff       (20)        1 2024-05-15 11:17:20.000000 avarnd-0.1/avarnd.egg-info/top_level.txt
--rw-r--r--   0 shriyoki   (502) staff       (20)       79 2024-05-15 11:17:20.625169 avarnd-0.1/setup.cfg
--rw-r--r--   0 shriyoki   (502) staff       (20)     2052 2024-05-15 11:14:13.000000 avarnd-0.1/setup.py
+drwxr-xr-x   0 shriyoki   (502) staff       (20)        0 2024-05-15 10:35:21.772265 avarnd-0.2/
+-rw-r--r--   0 shriyoki   (502) staff       (20)     1080 2024-05-15 09:55:48.000000 avarnd-0.2/LICENSE
+-rw-r--r--   0 shriyoki   (502) staff       (20)     1086 2024-05-15 10:35:21.772172 avarnd-0.2/PKG-INFO
+drwxr-xr-x   0 shriyoki   (502) staff       (20)        0 2024-05-15 10:35:21.771983 avarnd-0.2/avarnd.egg-info/
+-rw-r--r--   0 shriyoki   (502) staff       (20)     1086 2024-05-15 10:35:21.000000 avarnd-0.2/avarnd.egg-info/PKG-INFO
+-rw-r--r--   0 shriyoki   (502) staff       (20)      146 2024-05-15 10:35:21.000000 avarnd-0.2/avarnd.egg-info/SOURCES.txt
+-rw-r--r--   0 shriyoki   (502) staff       (20)        1 2024-05-15 10:35:21.000000 avarnd-0.2/avarnd.egg-info/dependency_links.txt
+-rw-r--r--   0 shriyoki   (502) staff       (20)        1 2024-05-15 10:35:21.000000 avarnd-0.2/avarnd.egg-info/top_level.txt
+-rw-r--r--   0 shriyoki   (502) staff       (20)       79 2024-05-15 10:35:21.772569 avarnd-0.2/setup.cfg
+-rw-r--r--   0 shriyoki   (502) staff       (20)     2051 2024-05-15 10:35:10.000000 avarnd-0.2/setup.py
```

### Comparing `avarnd-0.1/LICENSE` & `avarnd-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `avarnd-0.1/PKG-INFO` & `avarnd-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avarnd
-Version: 0.1
+Version: 0.2
 Summary: Sample package that conssists of addition and subtraction methods.
 Home-page: https://github.com/user/reponame
 Download-URL: https://github.com/Shriyokesh-Thangavel/zeb-rnd/archive/refs/tags/v_0.2.tar.gz
 Author: Shriyokesh
 Author-email: shriyokesh.t@avasoft.com
 License: MIT
 Keywords: SOME,MEANINGFUL,KEYWORDS
```

### Comparing `avarnd-0.1/avarnd.egg-info/PKG-INFO` & `avarnd-0.2/avarnd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avarnd
-Version: 0.1
+Version: 0.2
 Summary: Sample package that conssists of addition and subtraction methods.
 Home-page: https://github.com/user/reponame
 Download-URL: https://github.com/Shriyokesh-Thangavel/zeb-rnd/archive/refs/tags/v_0.2.tar.gz
 Author: Shriyokesh
 Author-email: shriyokesh.t@avasoft.com
 License: MIT
 Keywords: SOME,MEANINGFUL,KEYWORDS
```

### Comparing `avarnd-0.1/setup.py` & `avarnd-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
  
 setup(
     name='avarnd',
     packages=find_packages(),       # Automatically find and include all packages
-    version='0.1',                  # Start with a small number and increase it with every change you make
+    version='0.2',                  # Start with a small number and increase it with every change you make
     license='MIT',                  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Sample package that conssists of addition and subtraction methods.',   # Give a short description about your library
     author='Shriyokesh',             # Type in your name
     author_email='shriyokesh.t@avasoft.com',  # Type in your E-Mail
     url='https://github.com/user/reponame',  # Provide either the link to your github or to your website
     download_url='https://github.com/Shriyokesh-Thangavel/zeb-rnd/archive/refs/tags/v_0.2.tar.gz',  # I explain this later on
     keywords=['SOME', 'MEANINGFUL', 'KEYWORDS'],  # Keywords that define your package best
@@ -25,8 +25,8 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',  # Placeholder for future Python 3.12
         # 'Programming Language :: Python :: 3.13',  # Placeholder for future Python 3.13
     ],
-)
+)
```

