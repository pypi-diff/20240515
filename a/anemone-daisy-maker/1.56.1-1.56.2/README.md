# Comparing `tmp/anemone_daisy_maker-1.56.1.tar.gz` & `tmp/anemone_daisy_maker-1.56.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.56.1.tar", last modified: Tue May 14 07:14:18 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.56.2.tar", last modified: Tue May 14 07:22:51 2024, max compression
```

## Comparing `anemone_daisy_maker-1.56.1.tar` & `anemone_daisy_maker-1.56.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:14:18.441958 anemone_daisy_maker-1.56.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-14 07:13:31.000000 anemone_daisy_maker-1.56.1/LICENSE
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6892 2024-05-14 07:14:18.441958 anemone_daisy_maker-1.56.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:14:18.437958 anemone_daisy_maker-1.56.1/anemone/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    75174 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone/__main__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:14:18.437958 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6892 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      316 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-14 07:14:18.441958 anemone_daisy_maker-1.56.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7094 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:22:51.620202 anemone_daisy_maker-1.56.2/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-14 07:13:31.000000 anemone_daisy_maker-1.56.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6928 2024-05-14 07:22:51.616202 anemone_daisy_maker-1.56.2/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:22:51.616202 anemone_daisy_maker-1.56.2/anemone/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    75174 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:22:51.616202 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6928 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      316 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-14 07:22:51.620202 anemone_daisy_maker-1.56.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7078 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/setup.py
```

### Comparing `anemone_daisy_maker-1.56.1/LICENSE` & `anemone_daisy_maker-1.56.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anemone_daisy_maker-1.56.1/PKG-INFO` & `anemone_daisy_maker-1.56.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: anemone_daisy_maker
-Version: 1.56.1
+Version: 1.56.2
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
-Home-page: UNKNOWN
+Home-page: http://ssb22.user.srcf.net/indexer/anemone.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: UNKNOWN
+Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `anemone_daisy_maker-1.56.1/anemone/__init__.py` & `anemone_daisy_maker-1.56.2/anemone/__init__.py`

 * *Files identical despite different names*

### Comparing `anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/PKG-INFO` & `anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: anemone-daisy-maker
-Version: 1.56.1
+Version: 1.56.2
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
-Home-page: UNKNOWN
+Home-page: http://ssb22.user.srcf.net/indexer/anemone.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: UNKNOWN
+Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `anemone_daisy_maker-1.56.1/setup.py` & `anemone_daisy_maker-1.56.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.56.1',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},license='Apache 2',platform='cross-platform',home_page='http://ssb22.user.srcf.net/indexer/anemone.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
+from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.56.2',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/indexer/anemone.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
 `anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
```

