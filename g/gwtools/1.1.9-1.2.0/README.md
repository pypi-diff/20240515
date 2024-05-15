# Comparing `tmp/gwtools-1.1.9.tar.gz` & `tmp/gwtools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwtools-1.1.9.tar", last modified: Sat Apr  6 14:33:28 2024, max compression
+gzip compressed data, was "gwtools-1.2.0.tar", last modified: Wed May 15 20:44:00 2024, max compression
```

## Comparing `gwtools-1.1.9.tar` & `gwtools-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-04-06 14:33:28.230347 gwtools-1.1.9/
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1155 2018-08-24 21:42:03.000000 gwtools-1.1.9/LICENSE
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)      166 2018-08-24 21:42:03.000000 gwtools-1.1.9/MANIFEST.in
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)     1052 2024-04-06 14:33:28.230347 gwtools-1.1.9/PKG-INFO
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)      441 2023-11-17 16:39:55.000000 gwtools-1.1.9/README.md
-drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-04-06 14:33:28.226347 gwtools-1.1.9/docs/
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     6666 2017-07-03 01:39:34.000000 gwtools-1.1.9/docs/mismatch.tex
-drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-04-06 14:33:28.230347 gwtools-1.1.9/gwtools/
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)       85 2022-09-30 22:46:55.000000 gwtools-1.1.9/gwtools/__init__.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     2143 2020-02-11 05:01:09.000000 gwtools-1.1.9/gwtools/const.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)    58642 2024-04-06 13:44:54.000000 gwtools-1.1.9/gwtools/gwtools.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)    12924 2024-02-27 21:45:52.000000 gwtools-1.1.9/gwtools/gwutils.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1636 2017-07-31 19:01:07.000000 gwtools-1.1.9/gwtools/harmonics.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)    12538 2019-10-21 16:14:54.000000 gwtools-1.1.9/gwtools/mismatch.py
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)    19691 2017-07-31 19:01:07.000000 gwtools-1.1.9/gwtools/rotations.py
-drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-04-06 14:33:28.230347 gwtools-1.1.9/gwtools.egg-info/
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1052 2024-04-06 14:33:28.000000 gwtools-1.1.9/gwtools.egg-info/PKG-INFO
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)      317 2024-04-06 14:33:28.000000 gwtools-1.1.9/gwtools.egg-info/SOURCES.txt
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)        1 2024-04-06 14:33:28.000000 gwtools-1.1.9/gwtools.egg-info/dependency_links.txt
--rw-r--r--   0 balzani57  (1000) balzani57  (1000)        8 2024-04-06 14:33:28.000000 gwtools-1.1.9/gwtools.egg-info/top_level.txt
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)       38 2024-04-06 14:33:28.230347 gwtools-1.1.9/setup.cfg
--rw-rw-r--   0 balzani57  (1000) balzani57  (1000)     1466 2024-04-06 14:31:52.000000 gwtools-1.1.9/setup.py
+drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-05-15 20:44:00.194129 gwtools-1.2.0/
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1155 2018-08-24 21:42:03.000000 gwtools-1.2.0/LICENSE
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)      166 2018-08-24 21:42:03.000000 gwtools-1.2.0/MANIFEST.in
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1052 2024-05-15 20:44:00.194129 gwtools-1.2.0/PKG-INFO
+-rw-rw-r--   0 balzani57  (1000) balzani57  (1000)      441 2023-11-17 16:39:55.000000 gwtools-1.2.0/README.md
+drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-05-15 20:44:00.193129 gwtools-1.2.0/docs/
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     6666 2017-07-03 01:39:34.000000 gwtools-1.2.0/docs/mismatch.tex
+drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-05-15 20:44:00.193129 gwtools-1.2.0/gwtools/
+-rw-rw-r--   0 balzani57  (1000) balzani57  (1000)       85 2022-09-30 22:46:55.000000 gwtools-1.2.0/gwtools/__init__.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     2143 2020-02-11 05:01:09.000000 gwtools-1.2.0/gwtools/const.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)    58639 2024-05-15 20:39:38.000000 gwtools-1.2.0/gwtools/gwtools.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)    12924 2024-02-27 21:45:52.000000 gwtools-1.2.0/gwtools/gwutils.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1636 2017-07-31 19:01:07.000000 gwtools-1.2.0/gwtools/harmonics.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)    12538 2019-10-21 16:14:54.000000 gwtools-1.2.0/gwtools/mismatch.py
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)    19691 2017-07-31 19:01:07.000000 gwtools-1.2.0/gwtools/rotations.py
+drwxrwxr-x   0 balzani57  (1000) balzani57  (1000)        0 2024-05-15 20:44:00.194129 gwtools-1.2.0/gwtools.egg-info/
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)     1052 2024-05-15 20:44:00.000000 gwtools-1.2.0/gwtools.egg-info/PKG-INFO
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)      317 2024-05-15 20:44:00.000000 gwtools-1.2.0/gwtools.egg-info/SOURCES.txt
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)        1 2024-05-15 20:44:00.000000 gwtools-1.2.0/gwtools.egg-info/dependency_links.txt
+-rw-r--r--   0 balzani57  (1000) balzani57  (1000)        8 2024-05-15 20:44:00.000000 gwtools-1.2.0/gwtools.egg-info/top_level.txt
+-rw-rw-r--   0 balzani57  (1000) balzani57  (1000)       38 2024-05-15 20:44:00.194129 gwtools-1.2.0/setup.cfg
+-rw-rw-r--   0 balzani57  (1000) balzani57  (1000)     1466 2024-05-15 20:39:56.000000 gwtools-1.2.0/setup.py
```

### Comparing `gwtools-1.1.9/LICENSE` & `gwtools-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.9/PKG-INFO` & `gwtools-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwtools
-Version: 1.1.9
+Version: 1.2.0
 Summary: A collection of gravitational wave tools
 Author: Jonathan Blackman, Scott Field, Chad Galley
 Author-email: sfield@umassd.edu
 License: MIT
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `gwtools-1.1.9/docs/mismatch.tex` & `gwtools-1.2.0/docs/mismatch.tex`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.9/gwtools/const.py` & `gwtools-1.2.0/gwtools/const.py`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.9/gwtools/gwtools.py` & `gwtools-1.2.0/gwtools/gwtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1690,15 +1690,15 @@
     for k,v in mode_dict.items():
       mode_list.append(k)
       i = i + 1
   else:
     for mode in mode_list:
       assert(mode in list(mode_dict.keys())) 
 
-  mode_array = np.zeros((len(list(mode_dict.values())[0]),len(mode_list)),dtype=np.complex)
+  mode_array = np.zeros((len(list(mode_dict.values())[0]),len(mode_list)),dtype=complex)
   i=0
   for mode in mode_list:
     mode_array[:,i] = mode_dict[mode]
     i = i + 1
 
   return mode_list, mode_array
```

### Comparing `gwtools-1.1.9/gwtools/gwutils.py` & `gwtools-1.2.0/gwtools/gwutils.py`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.9/gwtools/harmonics.py` & `gwtools-1.2.0/gwtools/harmonics.py`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.9/gwtools/mismatch.py` & `gwtools-1.2.0/gwtools/mismatch.py`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.9/gwtools/rotations.py` & `gwtools-1.2.0/gwtools/rotations.py`

 * *Files identical despite different names*

### Comparing `gwtools-1.1.9/gwtools.egg-info/PKG-INFO` & `gwtools-1.2.0/gwtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwtools
-Version: 1.1.9
+Version: 1.2.0
 Summary: A collection of gravitational wave tools
 Author: Jonathan Blackman, Scott Field, Chad Galley
 Author-email: sfield@umassd.edu
 License: MIT
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `gwtools-1.1.9/setup.py` & `gwtools-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     import pypandoc
     long_description = pypandoc.convert('README.md', 'rst')
 except ImportError:
     long_description = open('README.md').read()
 
 
 setup(name='gwtools',
-      version='1.1.9',
+      version='1.2.0',
       author='Jonathan Blackman, Scott Field, Chad Galley',
       author_email='sfield@umassd.edu',
       packages=['gwtools'],
       license='MIT',
       include_package_data=True,
       contributors=[
       # Alphabetical by last name.
```

