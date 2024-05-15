# Comparing `tmp/regex-2024.4.28.tar.gz` & `tmp/regex-2024.5.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-2024.4.28.tar", last modified: Sun Apr 28 19:12:39 2024, max compression
+gzip compressed data, was "regex-2024.5.10.tar", last modified: Fri May 10 00:58:59 2024, max compression
```

## Comparing `regex-2024.4.28.tar` & `regex-2024.5.10.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:12:39.034421 regex-2024.4.28/
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-28 19:12:38.000000 regex-2024.4.28/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-28 19:12:38.000000 regex-2024.4.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    40846 2024-04-28 19:12:39.034421 regex-2024.4.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39805 2024-04-28 19:12:38.000000 regex-2024.4.28/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:12:39.026421 regex-2024.4.28/docs/
--rw-r--r--   0 runner    (1001) docker     (127)   143294 2024-04-28 19:12:38.000000 regex-2024.4.28/docs/Features.html
--rw-r--r--   0 runner    (1001) docker     (127)    29426 2024-04-28 19:12:38.000000 regex-2024.4.28/docs/UnicodeProperties.rst
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-28 19:12:38.000000 regex-2024.4.28/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:12:39.026421 regex-2024.4.28/regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40846 2024-04-28 19:12:38.000000 regex-2024.4.28/regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-28 19:12:39.000000 regex-2024.4.28/regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:12:38.000000 regex-2024.4.28/regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 19:12:38.000000 regex-2024.4.28/regex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:12:39.034421 regex-2024.4.28/regex_3/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-28 19:12:38.000000 regex-2024.4.28/regex_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   826026 2024-04-28 19:12:38.000000 regex-2024.4.28/regex_3/_regex.c
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-28 19:12:38.000000 regex-2024.4.28/regex_3/_regex.h
--rw-r--r--   0 runner    (1001) docker     (127)   141028 2024-04-28 19:12:38.000000 regex-2024.4.28/regex_3/_regex_core.py
--rw-r--r--   0 runner    (1001) docker     (127)  1878313 2024-04-28 19:12:38.000000 regex-2024.4.28/regex_3/_regex_unicode.c
--rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-28 19:12:38.000000 regex-2024.4.28/regex_3/_regex_unicode.h
--rw-r--r--   0 runner    (1001) docker     (127)    32683 2024-04-28 19:12:38.000000 regex-2024.4.28/regex_3/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)   220091 2024-04-28 19:12:38.000000 regex-2024.4.28/regex_3/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 19:12:39.034421 regex-2024.4.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-28 19:12:38.000000 regex-2024.4.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:12:39.034421 regex-2024.4.28/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    56426 2024-04-28 19:12:38.000000 regex-2024.4.28/tools/build_regex_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:58:59.663351 regex-2024.5.10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-10 00:58:58.000000 regex-2024.5.10/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 00:58:58.000000 regex-2024.5.10/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    40897 2024-05-10 00:58:59.663351 regex-2024.5.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39805 2024-05-10 00:58:58.000000 regex-2024.5.10/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:58:59.659350 regex-2024.5.10/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)   143294 2024-05-10 00:58:58.000000 regex-2024.5.10/docs/Features.html
+-rw-r--r--   0 runner    (1001) docker     (127)    29426 2024-05-10 00:58:58.000000 regex-2024.5.10/docs/UnicodeProperties.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-10 00:58:58.000000 regex-2024.5.10/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:58:59.659350 regex-2024.5.10/regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40897 2024-05-10 00:58:59.000000 regex-2024.5.10/regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-10 00:58:59.000000 regex-2024.5.10/regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 00:58:59.000000 regex-2024.5.10/regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 00:58:59.000000 regex-2024.5.10/regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:58:59.663351 regex-2024.5.10/regex_3/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-10 00:58:58.000000 regex-2024.5.10/regex_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   826044 2024-05-10 00:58:58.000000 regex-2024.5.10/regex_3/_regex.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-10 00:58:58.000000 regex-2024.5.10/regex_3/_regex.h
+-rw-r--r--   0 runner    (1001) docker     (127)   141028 2024-05-10 00:58:58.000000 regex-2024.5.10/regex_3/_regex_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1878313 2024-05-10 00:58:58.000000 regex-2024.5.10/regex_3/_regex_unicode.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-05-10 00:58:58.000000 regex-2024.5.10/regex_3/_regex_unicode.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32683 2024-05-10 00:58:58.000000 regex-2024.5.10/regex_3/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   220091 2024-05-10 00:58:58.000000 regex-2024.5.10/regex_3/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 00:58:59.663351 regex-2024.5.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-10 00:58:58.000000 regex-2024.5.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:58:59.663351 regex-2024.5.10/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    56435 2024-05-10 00:58:58.000000 regex-2024.5.10/tools/build_regex_unicode.py
```

### Comparing `regex-2024.4.28/LICENSE.txt` & `regex-2024.5.10/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `regex-2024.4.28/PKG-INFO` & `regex-2024.5.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: regex
-Version: 2024.4.28
+Version: 2024.5.10
 Summary: Alternative regular expression module, to replace re.
 Home-page: https://github.com/mrabarnett/mrab-regex
 Author: Matthew Barnett
 Author-email: regex@mrabarnett.plus.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

### Comparing `regex-2024.4.28/README.rst` & `regex-2024.5.10/README.rst`

 * *Files identical despite different names*

### Comparing `regex-2024.4.28/docs/Features.html` & `regex-2024.5.10/docs/Features.html`

 * *Files identical despite different names*

### Comparing `regex-2024.4.28/docs/UnicodeProperties.rst` & `regex-2024.5.10/docs/UnicodeProperties.rst`

 * *Files identical despite different names*

### Comparing `regex-2024.4.28/regex.egg-info/PKG-INFO` & `regex-2024.5.10/regex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: regex
-Version: 2024.4.28
+Version: 2024.5.10
 Summary: Alternative regular expression module, to replace re.
 Home-page: https://github.com/mrabarnett/mrab-regex
 Author: Matthew Barnett
 Author-email: regex@mrabarnett.plus.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

### Comparing `regex-2024.4.28/regex_3/_regex.c` & `regex-2024.5.10/regex_3/_regex.c`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 #endif
 
 #define PY_SSIZE_T_CLEAN
 
 #include "Python.h"
 #include "structmember.h" /* offsetof */
 #include <ctype.h>
+#include <time.h>
 #include "_regex.h"
 #include "pyport.h"
 #include "pythread.h"
 
 #if PY_VERSION_HEX < 0x03070000
 /* Issue 29943: PySlice_GetIndicesEx change broke ABI in 3.5 and 3.6 branches
  */
```

### Comparing `regex-2024.4.28/regex_3/_regex.h` & `regex-2024.5.10/regex_3/_regex.h`

 * *Files identical despite different names*

### Comparing `regex-2024.4.28/regex_3/_regex_core.py` & `regex-2024.5.10/regex_3/_regex_core.py`

 * *Files identical despite different names*

### Comparing `regex-2024.4.28/regex_3/_regex_unicode.c` & `regex-2024.5.10/regex_3/_regex_unicode.c`

 * *Files identical despite different names*

### Comparing `regex-2024.4.28/regex_3/_regex_unicode.h` & `regex-2024.5.10/regex_3/_regex_unicode.h`

 * *Files identical despite different names*

### Comparing `regex-2024.4.28/regex_3/regex.py` & `regex-2024.5.10/regex_3/regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
   "sub", "subf", "subfn", "subn", "template", "Scanner", "A", "ASCII", "B",
   "BESTMATCH", "D", "DEBUG", "E", "ENHANCEMATCH", "S", "DOTALL", "F",
   "FULLCASE", "I", "IGNORECASE", "L", "LOCALE", "M", "MULTILINE", "P", "POSIX",
   "R", "REVERSE", "T", "TEMPLATE", "U", "UNICODE", "V0", "VERSION0", "V1",
   "VERSION1", "X", "VERBOSE", "W", "WORD", "error", "Regex", "__version__",
   "__doc__", "RegexFlag"]
 
-__version__ = "2.5.142"
+__version__ = "2.5.144"
 
 # --------------------------------------------------------------------
 # Public interface.
 
 def match(pattern, string, flags=0, pos=None, endpos=None, partial=False,
   concurrent=None, timeout=None, ignore_unused=False, **kwargs):
     """Try to apply the pattern at the start of the string, returning a match
```

### Comparing `regex-2024.4.28/regex_3/test_regex.py` & `regex-2024.5.10/regex_3/test_regex.py`

 * *Files identical despite different names*

### Comparing `regex-2024.4.28/setup.py` & `regex-2024.5.10/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 from setuptools import setup, Extension
 from os.path import join
 
 with open('README.rst', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='regex',
-    version='2024.4.28',
+    version='2024.5.10',
     description='Alternative regular expression module, to replace re.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Matthew Barnett',
     author_email='regex@mrabarnett.plus.com',
     url='https://github.com/mrabarnett/mrab-regex',
     license='Apache Software License',
@@ -22,14 +23,15 @@
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Text Processing',
         'Topic :: Text Processing :: General',
     ],
     python_requires='>=3.8',
```

### Comparing `regex-2024.4.28/tools/build_regex_unicode.py` & `regex-2024.5.10/tools/build_regex_unicode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! python3.11
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # This Python script parses the Unicode data files in the UCD.zip file and
 # generates the C files for the regex module.
 #
 # Written by MRAB.
 #
```

