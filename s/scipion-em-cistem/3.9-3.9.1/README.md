# Comparing `tmp/scipion-em-cistem-3.9.tar.gz` & `tmp/scipion-em-cistem-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cistem-3.9.tar", last modified: Thu Apr 18 12:36:04 2024, max compression
+gzip compressed data, was "scipion-em-cistem-3.9.1.tar", last modified: Wed May 15 11:22:30 2024, max compression
```

## Comparing `scipion-em-cistem-3.9.tar` & `scipion-em-cistem-3.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.458840 scipion-em-cistem-3.9/cistem/
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)    95934 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/cistem_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/cistem/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/convert/dataimport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/cistem/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/program_ctffind.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_ctffind.py
--rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_picking.py
--rw-r--r--   0 runner    (1001) docker     (127)    38864 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_refine2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_tomo_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_ts_ctffind.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_ts_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)    20788 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols/protocol_unblur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/cistem/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/tests/test_protocols_cistem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/tests/test_protocols_cistem_movies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/tests/tomo_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/cistem/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/viewers/tomo_viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/viewers/viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/cistem/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 12:36:04.000000 scipion-em-cistem-3.9/scipion_em_cistem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:36:04.462840 scipion-em-cistem-3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-18 12:35:38.000000 scipion-em-cistem-3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:22:30.636232 scipion-em-cistem-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-15 11:22:30.636232 scipion-em-cistem-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:22:30.632232 scipion-em-cistem-3.9.1/cistem/
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95934 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/cistem_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:22:30.632232 scipion-em-cistem-3.9.1/cistem/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/convert/dataimport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:22:30.632232 scipion-em-cistem-3.9.1/cistem/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols/program_ctffind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols/protocol_ctffind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols/protocol_picking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38864 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols/protocol_refine2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols/protocol_tomo_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols/protocol_ts_ctffind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols/protocol_ts_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20788 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols/protocol_unblur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:22:30.636232 scipion-em-cistem-3.9.1/cistem/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/tests/test_protocols_cistem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/tests/test_protocols_cistem_movies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/tests/tomo_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:22:30.636232 scipion-em-cistem-3.9.1/cistem/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/viewers/tomo_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/viewers/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/cistem/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:22:30.636232 scipion-em-cistem-3.9.1/scipion_em_cistem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-15 11:22:30.000000 scipion-em-cistem-3.9.1/scipion_em_cistem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 11:22:30.000000 scipion-em-cistem-3.9.1/scipion_em_cistem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:22:30.000000 scipion-em-cistem-3.9.1/scipion_em_cistem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 11:22:30.000000 scipion-em-cistem-3.9.1/scipion_em_cistem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 11:22:30.000000 scipion-em-cistem-3.9.1/scipion_em_cistem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 11:22:30.000000 scipion-em-cistem-3.9.1/scipion_em_cistem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:22:30.636232 scipion-em-cistem-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-15 11:22:05.000000 scipion-em-cistem-3.9.1/setup.py
```

### Comparing `scipion-em-cistem-3.9/CHANGES.txt` & `scipion-em-cistem-3.9.1/CHANGES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+3.9.1
+  Users:
+   - Adding a main help to the protocols and some helps modified.
+   - Phase shift parameter are now in a line
 3.9:
   Users:
    - add ctffind5, rename config vars
   Developers: 
    - update the acquisition order in the CTFTomo objects (field added to that class in scipion-em-tomo v3.7.0).
 3.8: new protocols to resample tomo and TS
 3.7.1: fix an obsolete import in the viewer.
```

### Comparing `scipion-em-cistem-3.9/LICENSE` & `scipion-em-cistem-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/PKG-INFO` & `scipion-em-cistem-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cistem
-Version: 3.9
+Version: 3.9.1
 Summary: Plugin to use cisTEM programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cistem
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cistem/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cistem/
```

### Comparing `scipion-em-cistem-3.9/README.rst` & `scipion-em-cistem-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/__init__.py` & `scipion-em-cistem-3.9.1/cistem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
 
-__version__ = '3.9'
+__version__ = '3.9.1'
 _logo = "cistem_logo.png"
 _references = ['Grant2018']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = CISTEM_HOME
     _pathVars = [CISTEM_HOME, CTFFIND_HOME]
```

### Comparing `scipion-em-cistem-3.9/cistem/bibtex.py` & `scipion-em-cistem-3.9.1/cistem/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/cistem_logo.png` & `scipion-em-cistem-3.9.1/cistem/cistem_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/constants.py` & `scipion-em-cistem-3.9.1/cistem/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/convert/__init__.py` & `scipion-em-cistem-3.9.1/cistem/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/convert/convert.py` & `scipion-em-cistem-3.9.1/cistem/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/convert/dataimport.py` & `scipion-em-cistem-3.9.1/cistem/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/protocols/__init__.py` & `scipion-em-cistem-3.9.1/cistem/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/protocols/program_ctffind.py` & `scipion-em-cistem-3.9.1/cistem/protocols/program_ctffind.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,16 +107,19 @@
                                   'to this range of resolution.')
         line.addParam('lowRes', params.FloatParam, default=30., label='Min')
         line.addParam('highRes', params.FloatParam, default=5., label='Max')
 
         line = group.addLine('Defocus search range (A)',
                              condition='not recalculate',
                              help='Select _minimum_ and _maximum_ values for '
-                                  'defocus search range (in A). Underfocus'
-                                  ' is represented by a positive number.')
+                                  'defocus search range (in A). Underfocus '
+                                  'is represented by a positive number. This '
+                                  'range is critical for the proper estimation. '
+                                  'Note that these number should be around the '
+                                  'nominal defocus of the acquisition.')
         line.addParam('minDefocus', params.FloatParam, default=5000.,
                       label='Min')
         line.addParam('maxDefocus', params.FloatParam, default=50000.,
                       label='Max')
         group.addParam('stepDefocus', params.FloatParam, default=500.,
                        label='Defocus step (A)',
                        help='Step size for the defocus search.')
@@ -154,32 +157,30 @@
         form.addParam('findPhaseShift', params.BooleanParam,
                       default=False,
                       label="Find additional phase shift?",
                       help='Was the data recorded using a phase plate '
                            'with variable phase shift that must be '
                            'determined together with the defocus '
                            'parameters?')
-        form.addParam('minPhaseShift', params.FloatParam, default=0.,
-                      label="Minimum phase shift (deg)",
-                      condition='findPhaseShift',
-                      help='If finding an additional phase shift, '
-                           'this value sets the lower bound for the '
-                           'search.')
-        form.addParam('maxPhaseShift', params.FloatParam, default=180,
-                      label="Maximum phase shift (deg)",
-                      condition='findPhaseShift',
-                      help='If finding an additional phase shift, '
-                           'this value sets the upper bound for the '
-                           'search.')
-        form.addParam('stepPhaseShift', params.FloatParam, default=10,
-                      label="Phase shift search step (deg)",
-                      condition='findPhaseShift',
-                      help='If finding an additional phase shift, '
-                           'this value sets the step size for the '
-                           'search.')
+        line = form.addLine('Phase shift (deg)',
+                            condition='findPhaseShift',
+                            help="Select _minimum_ and _maximum_ values for "
+                                 " phase shift search range (in deg). Also "
+                                 "the search step should be provided. "
+                                 "The phase shift will be estimated in step from the "
+                                 "minumum to the maximum pprovided values")
+        line.addParam('minPhaseShift', params.FloatParam, default=0.,
+                      label="Min",
+                      condition='findPhaseShift')
+        line.addParam('maxPhaseShift', params.FloatParam, default=180.,
+                      label="Max",
+                      condition='findPhaseShift')
+        line.addParam('stepPhaseShift', params.FloatParam, default=10.,
+                      label="Step",
+                      condition='findPhaseShift')
 
         form.addParallelSection(threads=3)
 
     def getCommand(self, **kwargs):
         """
         :param kwargs: The input keywords argument should contain key-values
         for one micrograph or group of micrographs.
```

### Comparing `scipion-em-cistem-3.9/cistem/protocols/protocol_ctffind.py` & `scipion-em-cistem-3.9.1/cistem/protocols/protocol_ctffind.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,16 +103,16 @@
         """ Parse output log for errors.
         :param mic: input mic object
         :return: the error string
         """
         file = self._getCtfOutPath(mic)
         with open(file, "r") as fh:
             for line in fh.readlines():
-                if line.startswith("Error"):
-                    return line.replace("Error:", "")
+                if "Error:" in line:
+                    return line.split("Error:")[-1]
         return e
 
     def _estimateCTF(self, mic, *args):
         """ Redefined func from the base class. """
         self._doCtfEstimation(mic)
 
     def _reEstimateCTF(self, mic, ctf):
```

### Comparing `scipion-em-cistem-3.9/cistem/protocols/protocol_picking.py` & `scipion-em-cistem-3.9.1/cistem/protocols/protocol_picking.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/protocols/protocol_refine2d.py` & `scipion-em-cistem-3.9.1/cistem/protocols/protocol_refine2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/protocols/protocol_tomo_resample.py` & `scipion-em-cistem-3.9.1/cistem/protocols/protocol_tomo_resample.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 from cistem import Plugin
 
 OUTPUT_TOMO_NAME = 'resampledTomos'
 
 
 class CistemProtTomoResample(EMProtocol, ProtTomoBase):
     """
-    Resample tomograms by Fourier cropping/padding using cisTEM. This is equivalent to binning/unbinning operations but free of aliasing artifacts.
+    Resample tomograms by Fourier cropping/padding using cisTEM.
+    This is equivalent to binning/unbinning operations but free of aliasing artifacts.
 
     More info:
         https://cistem.org
     """
 
     _label = 'resample tomogram'
     _possibleOutputs = {OUTPUT_TOMO_NAME: SetOfTomograms}
```

### Comparing `scipion-em-cistem-3.9/cistem/protocols/protocol_ts_ctffind.py` & `scipion-em-cistem-3.9.1/cistem/protocols/protocol_ts_ctffind.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,23 +42,47 @@
 from tomo.protocols.protocol_ts_estimate_ctf import createCtfParams
 from .program_ctffind import ProgramCtffind
 from ..convert import readCtfModelStack, parseCtffindOutput
 from tomo.objects import CTFTomo, SetOfCTFTomoSeries, CTFTomoSeries
 
 MRCS_EXT = ".mrcs"
 # create simple, lightweight data structures similar to a class, but without the overhead of defining a full class
-CistemTsCtfMd = namedtuple('CistemTsCtfMd', ['ts', 'tsFn', 'outputLog', 'outputPsd'])
+CistemTsCtfMd = namedtuple('CistemTsCtfMd',
+                           ['ts', 'tsFn', 'outputLog', 'outputPsd'])
 
 
 class TsCtffindOutputs(Enum):
     CTFs = SetOfCTFTomoSeries
 
 
 class CistemProtTsCtffind(EMProtocol):
-    """ CTF estimation on a set of tilt series using CTFFIND. """
+    """ The contrast transfer function (CTF) affects the relative signal-to-noise
+    ratio (SNR) of Fourier components of each image. Those Fourier components
+    where the CTF is near 0.0 have very low SNR compared to others. It is therefore
+    essential to obtain accurate estimates of the CTF for each image so that
+    data from multiple imges may be combined in an optimal manner during later
+    processing.\n
+
+    You can use CTFfind (Rohou & Grigorieff, 2015) to estimate CTF parameter values
+    for each image. The main parameter to be determined for each image is the
+    objective lens defocus (in Angstroms). Because in general lenses are astigmatic,
+    one actually needs to determine two defocus values (describing defocus along
+    the lens' major and minor axes) and the angle of astigmatism.\n
+
+    To estimate the values of these three defocus parameters for an image,
+    CTFfind computes a filtered version of the amplitude spectrum of the micrograph
+    and then fits a model of the CTF (Equation 6 of Rohou & Grigorieff) to this
+    filtered amplitude spectrum. It then returns the values of the defocus parameters
+    which maximize the quality of the fit, as well as an image of the filtered
+    amplitude spectrum, with the CTF model.\n
+
+    Another diagnostic output is a 1D plot of the experimental amplitude spectrum,
+    the CTF fit and the quality of fitting.
+    """
+
     _label = 'tilt-series ctffind'
     _devStatus = PROD
     _possibleOutputs = TsCtffindOutputs
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.stepsExecutionMode = STEPS_PARALLEL
@@ -68,15 +92,15 @@
         self.inTsSet = None
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form, stream=False):
         form.addSection(label='Input')
         form.addParam('inputTiltSeries', params.PointerParam, important=True,
                       pointerClass='SetOfTiltSeries, SetOfCTFTomoSeries',
-                      label='Input tilt series')
+                      label='Tilt series')
         form.addHidden('recalculate', params.BooleanParam,
                        default=False,
                        condition='recalculate',
                        label="Do recalculate ctf?")
         form.addHidden('continueRun', params.PointerParam,
                        allowsNull=True,
                        condition='recalculate',
@@ -90,23 +114,27 @@
         ProgramCtffind.defineProcessParams(form)
 
     # --------------------------- STEPS functions -----------------------------
     def _insertAllSteps(self):
         self._initialize()
         pIdList = []
         for mdObj in self.tsCtfMdList:
-            pidConvert = self._insertFunctionStep(self.convertInputStep, mdObj, prerequisites=[])
-            pidProcess = self._insertFunctionStep(self.processTiltSeriesStep, mdObj, prerequisites=pidConvert)
-            pidCreateOutput = self._insertFunctionStep(self.createOutputStep, mdObj, prerequisites=pidProcess)
+            pidConvert = self._insertFunctionStep(self.convertInputStep,
+                                                  mdObj, prerequisites=[])
+            pidProcess = self._insertFunctionStep(self.processTiltSeriesStep,
+                                                  mdObj, prerequisites=pidConvert)
+            pidCreateOutput = self._insertFunctionStep(self.createOutputStep,
+                                                       mdObj, prerequisites=pidProcess)
             pIdList.append(pidCreateOutput)
         self._insertFunctionStep(self.closeStep, prerequisites=pIdList)
 
     def _initialize(self):
         self.inTsSet = self._getInputTs()
-        self._params = createCtfParams(self.inTsSet, self.windowSize.get(), self.lowRes.get(), self.highRes.get(),
+        self._params = createCtfParams(self.inTsSet, self.windowSize.get(),
+                                       self.lowRes.get(), self.highRes.get(),
                                        self.minDefocus.get(), self.maxDefocus.get())
         self._ctfProgram = ProgramCtffind(self)
         for ts in self.inTsSet.iterItems():
             outputLog = self._getExtraPath(ts.getTsId() + "_ctf.txt")
             md = CistemTsCtfMd(
                 ts=ts.clone(ignoreAttrs=[]),
                 tsFn=self._getTmpPath(ts.getTsId() + MRCS_EXT),
@@ -139,15 +167,16 @@
 
     def createOutputStep(self, mdObj):
         outCtfSet = self.getOutputCtfTomoSet()
 
         if outCtfSet:
             outCtfSet.enableAppend()
         else:
-            outCtfSet = SetOfCTFTomoSeries.create(self._getPath(), template='ctfTomoSeriess%s.sqlite')
+            outCtfSet = SetOfCTFTomoSeries.create(self._getPath(),
+                                                  template='ctfTomoSeriess%s.sqlite')
             outCtfSet.setSetOfTiltSeries(self.inTsSet)
             outCtfSet.setStreamState(Set.STREAM_OPEN)
             self._defineOutputs(**{self._possibleOutputs.CTFs.name: outCtfSet})
             self._defineSourceRelation(self.inTsSet, outCtfSet)
 
         ts = mdObj.ts
         outputLog = mdObj.outputLog
@@ -217,9 +246,7 @@
     def getOutputCtfTomoSet(self):
         return getattr(self, TsCtffindOutputs.CTFs.name, None)
 
     def getCtfParamsDict(self):
         """ Return a copy of the global params dict,
         to avoid overwriting values. """
         return self._params
-
-
```

### Comparing `scipion-em-cistem-3.9/cistem/protocols/protocol_ts_resample.py` & `scipion-em-cistem-3.9.1/cistem/protocols/protocol_ts_resample.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 from cistem import Plugin
 
 OUTPUT_TS_NAME = 'resampledTiltSeries'
 
 
 class CistemProtTsResample(EMProtocol, ProtTomoBase):
     """
-    Resample tilt series by Fourier cropping/padding using cisTEM. This is equivalent to binning/unbinning operations but free of aliasing artifacts.
+    Resample tilt series by Fourier cropping/padding using cisTEM.
+    This is equivalent to binning/unbinning operations but free of aliasing artifacts.
 
     More info:
         https://cistem.org
     """
 
     _label = 'resample tilt series'
     _possibleOutputs = {OUTPUT_TS_NAME: SetOfTiltSeries}
@@ -78,25 +79,25 @@
         # New X-Size [464]                                   : 928
         # New Y-Size [464]                                   : 928
 
         # You need a params to belong to a section:
         form.addSection(label=pwutils.Message.LABEL_INPUT)
         form.addParam('inputSetOfTiltSeries', PointerParam,
                       pointerClass='SetOfTiltSeries',
-                      allowsNull=False,
-                      label='Input tilt series')
+                      important=True,
+                      label='Tilt series')
 
         form.addParam('newXsize', IntParam,
                       default=512, validators=[Positive],
-                      label='New X-Size',
-                      help='Volume will be rescaled to this size in X dimension (voxels)')
+                      label='New X-Size (px)',
+                      help='Images will be rescaled to this size in X dimension (pixels)')
         form.addParam('newYsize', IntParam,
                       default=512, validators=[Positive],
-                      label='New Y-Size',
-                      help='Volume will be rescaled to this size in Y dimension (voxels)')
+                      label='New Y-Size (px)',
+                      help='Images will be rescaled to this size in Y dimension (pixels)')
 
     # -------------------------- INSERT steps functions -----------------------
     def _insertAllSteps(self):
         for ts in self.inputSetOfTiltSeries.get():
 
             self._insertFunctionStep(self.runTsResample,
                                      ts.getFirstItem().getFileName())
```

### Comparing `scipion-em-cistem-3.9/cistem/protocols/protocol_unblur.py` & `scipion-em-cistem-3.9.1/cistem/protocols/protocol_unblur.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/protocols.conf` & `scipion-em-cistem-3.9.1/cistem/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/tests/__init__.py` & `scipion-em-cistem-3.9.1/cistem/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/tests/test_protocols_cistem.py` & `scipion-em-cistem-3.9.1/cistem/tests/test_protocols_cistem.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/tests/test_protocols_cistem_movies.py` & `scipion-em-cistem-3.9.1/cistem/tests/test_protocols_cistem_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/tests/tomo_tests.py` & `scipion-em-cistem-3.9.1/cistem/tests/tomo_tests.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/viewers/tomo_viewers.py` & `scipion-em-cistem-3.9.1/cistem/viewers/tomo_viewers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/viewers/viewers.py` & `scipion-em-cistem-3.9.1/cistem/viewers/viewers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/cistem/wizards.py` & `scipion-em-cistem-3.9.1/cistem/wizards.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         protParams['sampling'] = protocol.inputMicrographs.get().getSamplingRate()
         return protParams
     
     def _getProvider(self, protocol):
         _objs = self._getParameters(protocol)['input']
         return CtfWizard._getListProvider(self, _objs)
         
-    def show(self, form):
+    def show(self, form, *args):
         protocol = form.protocol
         params = self._getParameters(protocol)
         _value = params['value']
         _label = params['label']
         _sampling = params['sampling']
         
         provider = self._getProvider(protocol)
```

### Comparing `scipion-em-cistem-3.9/scipion_em_cistem.egg-info/PKG-INFO` & `scipion-em-cistem-3.9.1/scipion_em_cistem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cistem
-Version: 3.9
+Version: 3.9.1
 Summary: Plugin to use cisTEM programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cistem
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cistem/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cistem/
```

### Comparing `scipion-em-cistem-3.9/scipion_em_cistem.egg-info/SOURCES.txt` & `scipion-em-cistem-3.9.1/scipion_em_cistem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cistem-3.9/setup.py` & `scipion-em-cistem-3.9.1/setup.py`

 * *Files identical despite different names*

