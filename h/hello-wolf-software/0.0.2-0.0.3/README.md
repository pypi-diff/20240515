# Comparing `tmp/hello_wolf_software-0.0.2.tar.gz` & `tmp/hello_wolf_software-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_wolf_software-0.0.2.tar", last modified: Wed May 15 12:42:09 2024, max compression
+gzip compressed data, was "hello_wolf_software-0.0.3.tar", last modified: Wed May 15 14:10:17 2024, max compression
```

## Comparing `hello_wolf_software-0.0.2.tar` & `hello_wolf_software-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wolf       (501) staff       (20)        0 2024-05-15 12:42:09.760337 hello_wolf_software-0.0.2/
--rw-r--r--   0 wolf       (501) staff       (20)     1118 2024-05-15 12:09:29.000000 hello_wolf_software-0.0.2/LICENSE.md
--rw-r--r--   0 wolf       (501) staff       (20)       51 2024-05-15 12:21:50.000000 hello_wolf_software-0.0.2/MANIFEST.in
--rw-r--r--   0 wolf       (501) staff       (20)     3397 2024-05-15 12:42:09.760105 hello_wolf_software-0.0.2/PKG-INFO
--rw-r--r--   0 wolf       (501) staff       (20)     2938 2024-05-15 12:09:29.000000 hello_wolf_software-0.0.2/README.md
-drwxr-xr-x   0 wolf       (501) staff       (20)        0 2024-05-15 12:42:09.756502 hello_wolf_software-0.0.2/hello_wolf_software/
--rw-r--r--   0 wolf       (501) staff       (20)       14 2024-05-15 12:36:58.000000 hello_wolf_software-0.0.2/hello_wolf_software/__init__.py
--rw-r--r--   0 wolf       (501) staff       (20)      159 2024-05-15 12:27:13.000000 hello_wolf_software-0.0.2/hello_wolf_software/hello.py
-drwxr-xr-x   0 wolf       (501) staff       (20)        0 2024-05-15 12:42:09.759270 hello_wolf_software-0.0.2/hello_wolf_software.egg-info/
--rw-r--r--   0 wolf       (501) staff       (20)     3397 2024-05-15 12:42:09.000000 hello_wolf_software-0.0.2/hello_wolf_software.egg-info/PKG-INFO
--rw-r--r--   0 wolf       (501) staff       (20)      330 2024-05-15 12:42:09.000000 hello_wolf_software-0.0.2/hello_wolf_software.egg-info/SOURCES.txt
--rw-r--r--   0 wolf       (501) staff       (20)        1 2024-05-15 12:42:09.000000 hello_wolf_software-0.0.2/hello_wolf_software.egg-info/dependency_links.txt
--rw-r--r--   0 wolf       (501) staff       (20)       57 2024-05-15 12:42:09.000000 hello_wolf_software-0.0.2/hello_wolf_software.egg-info/entry_points.txt
--rw-r--r--   0 wolf       (501) staff       (20)       20 2024-05-15 12:42:09.000000 hello_wolf_software-0.0.2/hello_wolf_software.egg-info/top_level.txt
--rw-r--r--   0 wolf       (501) staff       (20)      295 2024-05-15 12:42:09.761147 hello_wolf_software-0.0.2/setup.cfg
--rw-r--r--   0 wolf       (501) staff       (20)      848 2024-05-15 12:41:36.000000 hello_wolf_software-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:10:17.956288 hello_wolf_software-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-15 14:10:09.000000 hello_wolf_software-0.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 14:10:09.000000 hello_wolf_software-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-15 14:10:17.956288 hello_wolf_software-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-15 14:10:09.000000 hello_wolf_software-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:10:17.956288 hello_wolf_software-0.0.3/hello_wolf_software/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 14:10:09.000000 hello_wolf_software-0.0.3/hello_wolf_software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 14:10:09.000000 hello_wolf_software-0.0.3/hello_wolf_software/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:10:17.956288 hello_wolf_software-0.0.3/hello_wolf_software.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-15 14:10:17.000000 hello_wolf_software-0.0.3/hello_wolf_software.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-15 14:10:17.000000 hello_wolf_software-0.0.3/hello_wolf_software.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:10:17.000000 hello_wolf_software-0.0.3/hello_wolf_software.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 14:10:17.000000 hello_wolf_software-0.0.3/hello_wolf_software.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 14:10:17.000000 hello_wolf_software-0.0.3/hello_wolf_software.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-15 14:10:17.956288 hello_wolf_software-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-15 14:10:09.000000 hello_wolf_software-0.0.3/setup.py
```

### Comparing `hello_wolf_software-0.0.2/LICENSE.md` & `hello_wolf_software-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_wolf_software-0.0.2/PKG-INFO` & `hello_wolf_software-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello-wolf-software
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple hello world test
 Home-page: https://github.com/DevelopersToolbox/hello-wolf-software
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hello-wolf-software Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: hello-wolf-software Version: 0.0.3 Summary: A
 simple hello world test Home-page: https://github.com/DevelopersToolbox/hello-
 wolf-software Author: Wolf Software Author-email: pypi@wolfsoftware.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE.md
                            _[_D_e_v_e_l_o_p_e_r_s_T_o_o_l_b_o_x_ _l_o_g_o_]
```

### Comparing `hello_wolf_software-0.0.2/README.md` & `hello_wolf_software-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hello_wolf_software-0.0.2/hello_wolf_software.egg-info/PKG-INFO` & `hello_wolf_software-0.0.3/hello_wolf_software.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello-wolf-software
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple hello world test
 Home-page: https://github.com/DevelopersToolbox/hello-wolf-software
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hello-wolf-software Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: hello-wolf-software Version: 0.0.3 Summary: A
 simple hello world test Home-page: https://github.com/DevelopersToolbox/hello-
 wolf-software Author: Wolf Software Author-email: pypi@wolfsoftware.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE.md
                            _[_D_e_v_e_l_o_p_e_r_s_T_o_o_l_b_o_x_ _l_o_g_o_]
```

### Comparing `hello_wolf_software-0.0.2/setup.py` & `hello_wolf_software-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # setup.py
 
 """Setup script."""
 
 from setuptools import setup, find_packages
 
-with open("README.MD", 'r', encoding='UTF-8') as f:
+with open("README.md", 'r', encoding='UTF-8') as f:
     long_description: str = f.read()
 
 setup(
     name='hello-wolf-software',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'hello=hello_wolf_software.hello:main',
         ],
     },
     author='Wolf Software',
```

