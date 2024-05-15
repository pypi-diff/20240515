# Comparing `tmp/imio.pyutils-1.0.1.tar.gz` & `tmp/imio_pyutils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.pyutils-1.0.1.tar", last modified: Mon Apr  8 14:20:40 2024, max compression
+gzip compressed data, was "imio_pyutils-1.0.2.tar", last modified: Wed May 15 13:06:55 2024, max compression
```

## Comparing `imio.pyutils-1.0.1.tar` & `imio_pyutils-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/
--rw-rw-r--   0 sge       (1000) sge       (1000)     5396 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       31 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)     1971 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/Makefile
--rw-rw-r--   0 sge       (1000) sge       (1000)     7361 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     1286 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/README.rst
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.474241 imio.pyutils-1.0.1/imio/
--rw-rw-r--   0 sge       (1000) sge       (1000)      244 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/imio/pyutils/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     3508 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/bs.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     4723 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/postgres.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    13626 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/system.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    10790 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/tests.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     9006 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio/pyutils/utils.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/imio.pyutils.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     7361 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)      503 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       37 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        5 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)       30 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        5 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/imio.pyutils.egg-info/top_level.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2024-04-08 14:20:40.478241 imio.pyutils-1.0.1/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     1480 2024-04-08 14:20:40.000000 imio.pyutils-1.0.1/setup.py
+drwxr-xr-x   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.862451 imio_pyutils-1.0.2/
+-rw-r--r--   0 antoineduchene   (501) staff       (20)     5546 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/CHANGES.rst
+-rw-r--r--   0 antoineduchene   (501) staff       (20)       31 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/MANIFEST.in
+-rw-r--r--   0 antoineduchene   (501) staff       (20)     1971 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/Makefile
+-rw-r--r--   0 antoineduchene   (501) staff       (20)     7566 2024-05-15 13:06:55.862290 imio_pyutils-1.0.2/PKG-INFO
+-rw-r--r--   0 antoineduchene   (501) staff       (20)     1286 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/README.rst
+drwxr-xr-x   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.860572 imio_pyutils-1.0.2/imio/
+-rw-r--r--   0 antoineduchene   (501) staff       (20)      244 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/__init__.py
+drwxr-xr-x   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.861783 imio_pyutils-1.0.2/imio/pyutils/
+-rw-r--r--   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/__init__.py
+-rw-r--r--   0 antoineduchene   (501) staff       (20)     3508 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/bs.py
+-rw-r--r--   0 antoineduchene   (501) staff       (20)     4723 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/postgres.py
+-rw-r--r--   0 antoineduchene   (501) staff       (20)    13626 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/system.py
+-rw-r--r--   0 antoineduchene   (501) staff       (20)    12087 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/tests.py
+-rw-r--r--   0 antoineduchene   (501) staff       (20)    11025 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/utils.py
+drwxr-xr-x   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.862077 imio_pyutils-1.0.2/imio.pyutils.egg-info/
+-rw-r--r--   0 antoineduchene   (501) staff       (20)     7566 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 antoineduchene   (501) staff       (20)      464 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 antoineduchene   (501) staff       (20)        1 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 antoineduchene   (501) staff       (20)        5 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/namespace_packages.txt
+-rw-r--r--   0 antoineduchene   (501) staff       (20)        1 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/not-zip-safe
+-rw-r--r--   0 antoineduchene   (501) staff       (20)       30 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/requires.txt
+-rw-r--r--   0 antoineduchene   (501) staff       (20)        5 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/top_level.txt
+-rw-r--r--   0 antoineduchene   (501) staff       (20)       38 2024-05-15 13:06:55.862484 imio_pyutils-1.0.2/setup.cfg
+-rw-r--r--   0 antoineduchene   (501) staff       (20)     1480 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/setup.py
```

### Comparing `imio.pyutils-1.0.1/CHANGES.rst` & `imio_pyutils-1.0.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.0.2 (2024-05-15)
+------------------
+
+- Added a new helper `utils.get_ordinal_clusters` to cluster ordinal numbers based on an offset.
+  [aduchene]
+
 1.0.1 (2024-04-08)
 ------------------
 
 - Added patterns parameter in `system.read_dir_filter`.
   [sgeulette]
 - Returned original filename in `system.hashed_filename` if string to hash is empty.
   [sgeulette]
```

### Comparing `imio.pyutils-1.0.1/Makefile` & `imio_pyutils-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `imio.pyutils-1.0.1/PKG-INFO` & `imio_pyutils-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: imio.pyutils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Some python useful methods
 Home-page: https://github.com/imio/imio.pyutils/
 Author: IMIO
 Author-email: support@imio.be
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.pyutils
 Project-URL: Source, https://github.com/imio/imio.pyutils
 Keywords: Python IMIO
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: setuptools
+Requires-Dist: future
+Requires-Dist: six>=1.16.0
 
 .. image:: https://github.com/IMIO/imio.pyutils/actions/workflows/main.yml/badge.svg?branch=master
     :target: https://github.com/IMIO/imio.pyutils/actions/workflows/main.yml
 
 .. image:: https://coveralls.io/repos/github/IMIO/imio.pyutils/badge.svg
     :target: https://coveralls.io/github/IMIO/imio.pyutils
 
@@ -76,14 +78,20 @@
 =====
 
 Can be run with: `bin/python -m unittest discover`
 
 Changelog
 =========
 
+1.0.2 (2024-05-15)
+------------------
+
+- Added a new helper `utils.get_ordinal_clusters` to cluster ordinal numbers based on an offset.
+  [aduchene]
+
 1.0.1 (2024-04-08)
 ------------------
 
 - Added patterns parameter in `system.read_dir_filter`.
   [sgeulette]
 - Returned original filename in `system.hashed_filename` if string to hash is empty.
   [sgeulette]
@@ -333,9 +341,7 @@
   [sgeulette]
 
 0.1 (2015-06-03)
 ----------------
 
 - Initial release.
   [sgeulette]
-
-
```

### Comparing `imio.pyutils-1.0.1/README.rst` & `imio_pyutils-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `imio.pyutils-1.0.1/imio/pyutils/bs.py` & `imio_pyutils-1.0.2/imio/pyutils/bs.py`

 * *Files identical despite different names*

### Comparing `imio.pyutils-1.0.1/imio/pyutils/postgres.py` & `imio_pyutils-1.0.2/imio/pyutils/postgres.py`

 * *Files identical despite different names*

### Comparing `imio.pyutils-1.0.1/imio/pyutils/system.py` & `imio_pyutils-1.0.2/imio/pyutils/system.py`

 * *Files identical despite different names*

### Comparing `imio.pyutils-1.0.1/imio/pyutils/tests.py` & `imio_pyutils-1.0.2/imio/pyutils/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections import OrderedDict
 from imio.pyutils.system import hashed_filename
 from imio.pyutils.system import read_dir_filter
 from imio.pyutils.system import read_recursive_dir
 from imio.pyutils.utils import all_of_dict_values
 from imio.pyutils.utils import append
 from imio.pyutils.utils import get_clusters
+from imio.pyutils.utils import get_ordinal_clusters
 from imio.pyutils.utils import insert_in_ordereddict
 from imio.pyutils.utils import iterable_as_list_of_list
 from imio.pyutils.utils import letters_sequence
 from imio.pyutils.utils import listify
 from imio.pyutils.utils import merge_dicts
 from imio.pyutils.utils import odict_pos_key
 from imio.pyutils.utils import one_of_dict_values
@@ -51,14 +52,34 @@
         self.assertEqual(get_clusters([1, 2, 3, 5, 6, 8, 10, 15]),
                          '1-3, 5-6, 8, 10, 15')
         self.assertEqual(get_clusters([1, 2, 3, 5, 5.1, 5.3, 6, 8, 10, 15]),
                          '1-3, 5, 5.1, 5.3, 6, 8, 10, 15')
         self.assertEqual(get_clusters([1, 2, 4, 5, 15], separator="|"),
                          '1-2|4-5|15')
 
+    def test_get_ordinal_clusters(self):
+        self.assertEqual(get_ordinal_clusters([100, 200, 300, 500, 600, 800, 1000, 1500]),
+                         '1-3, 5-6, 8, 10, 15')
+        self.assertEqual(get_ordinal_clusters([100, 200, 300, 500, 501, 503, 600, 700, 1000, 1500]),
+                         '1-3, 5-5.1, 5.3, 6-7, 10, 15')
+        self.assertEqual(
+            get_ordinal_clusters(
+                [100, 200, 300, 400, 500, 501, 502, 521, 522, 540, 550, 1200, 1300], separator="|"),
+            '1-5.2|5.21-5.22|5.40|5.50|12-13')
+        self.assertEqual(
+            get_ordinal_clusters(
+                [100, 200, 300, 301, 302, 321, 322, 340, 1199, 1200, 1300], cluster_format="from {} to {}"),
+            'from 1 to 3.2, from 3.21 to 3.22, 3.40, 11.99, from 12 to 13')
+        self.assertEqual(get_ordinal_clusters([100, 200, 250, 400, 700], single_cluster_format="({})"),
+                         '1-2, (2.50), (4), (7)')
+        self.assertEqual(get_ordinal_clusters([10, 20, 30, 31, 32, 110, 112, 130], offset=10),
+                         '1-3.2, 11, 11.2, 13')
+        self.assertListEqual(get_ordinal_clusters([100, 200, 250, 400, 700], as_str=False),
+                             [[100, 200], [250], [400], [700]])
+
     def test_insert_in_ordered_dict(self):
         dic = OrderedDict([('a', 1), ('b', 2)])
         self.assertEqual(insert_in_ordereddict(dic, ('bad', 3)), None)
         self.assertEqual(list(insert_in_ordereddict(dic, ('c', 3), after_key='a').items()),
                          [('a', 1), ('c', 3), ('b', 2)])
         self.assertEqual(list(insert_in_ordereddict(dic, ('c', 3), after_key='b').items()),
                          [('a', 1), ('b', 2), ('c', 3)])
```

### Comparing `imio.pyutils-1.0.1/imio.pyutils.egg-info/PKG-INFO` & `imio_pyutils-1.0.2/imio.pyutils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: imio.pyutils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Some python useful methods
 Home-page: https://github.com/imio/imio.pyutils/
 Author: IMIO
 Author-email: support@imio.be
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.pyutils
 Project-URL: Source, https://github.com/imio/imio.pyutils
 Keywords: Python IMIO
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: setuptools
+Requires-Dist: future
+Requires-Dist: six>=1.16.0
 
 .. image:: https://github.com/IMIO/imio.pyutils/actions/workflows/main.yml/badge.svg?branch=master
     :target: https://github.com/IMIO/imio.pyutils/actions/workflows/main.yml
 
 .. image:: https://coveralls.io/repos/github/IMIO/imio.pyutils/badge.svg
     :target: https://coveralls.io/github/IMIO/imio.pyutils
 
@@ -76,14 +78,20 @@
 =====
 
 Can be run with: `bin/python -m unittest discover`
 
 Changelog
 =========
 
+1.0.2 (2024-05-15)
+------------------
+
+- Added a new helper `utils.get_ordinal_clusters` to cluster ordinal numbers based on an offset.
+  [aduchene]
+
 1.0.1 (2024-04-08)
 ------------------
 
 - Added patterns parameter in `system.read_dir_filter`.
   [sgeulette]
 - Returned original filename in `system.hashed_filename` if string to hash is empty.
   [sgeulette]
@@ -333,9 +341,7 @@
   [sgeulette]
 
 0.1 (2015-06-03)
 ----------------
 
 - Initial release.
   [sgeulette]
-
-
```

### Comparing `imio.pyutils-1.0.1/setup.py` & `imio_pyutils-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '1.0.1'
+version = '1.0.2'
 
 setup(name='imio.pyutils',
       version=version,
       description="Some python useful methods",
       long_description=open("README.rst").read() + "\n" + open('CHANGES.rst').read(),
       # Get more strings from
       # http://pypi.python.org/pypi?:action=list_classifiers
```

