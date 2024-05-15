# Comparing `tmp/ymodem-1.5.1b1.tar.gz` & `tmp/ymodem-1.5.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ymodem-1.5.1b1.tar", last modified: Sat Feb  3 00:09:14 2024, max compression
+gzip compressed data, was "ymodem-1.5.1b2.tar", last modified: Sat Feb  3 00:21:26 2024, max compression
```

## Comparing `ymodem-1.5.1b1.tar` & `ymodem-1.5.1b2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 00:09:14.243432 ymodem-1.5.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-02-03 00:09:14.243432 ymodem-1.5.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 00:09:14.243432 ymodem-1.5.1b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 00:09:14.243432 ymodem-1.5.1b1/ymodem/
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/ymodem/CRC.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/ymodem/Platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/ymodem/Protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    48294 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/ymodem/Socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/ymodem/Version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/ymodem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-02-03 00:09:01.000000 ymodem-1.5.1b1/ymodem/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 00:09:14.243432 ymodem-1.5.1b1/ymodem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-02-03 00:09:14.000000 ymodem-1.5.1b1/ymodem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-03 00:09:14.000000 ymodem-1.5.1b1/ymodem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 00:09:14.000000 ymodem-1.5.1b1/ymodem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-03 00:09:14.000000 ymodem-1.5.1b1/ymodem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-03 00:09:14.000000 ymodem-1.5.1b1/ymodem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-03 00:09:14.000000 ymodem-1.5.1b1/ymodem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 00:21:26.096818 ymodem-1.5.1b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-02-03 00:21:26.096818 ymodem-1.5.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 00:21:26.096818 ymodem-1.5.1b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 00:21:26.096818 ymodem-1.5.1b2/ymodem/
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/ymodem/CRC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/ymodem/Platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/ymodem/Protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48294 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/ymodem/Socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/ymodem/Version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/ymodem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-02-03 00:21:07.000000 ymodem-1.5.1b2/ymodem/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 00:21:26.096818 ymodem-1.5.1b2/ymodem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-02-03 00:21:26.000000 ymodem-1.5.1b2/ymodem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-03 00:21:26.000000 ymodem-1.5.1b2/ymodem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 00:21:26.000000 ymodem-1.5.1b2/ymodem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-03 00:21:26.000000 ymodem-1.5.1b2/ymodem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-03 00:21:26.000000 ymodem-1.5.1b2/ymodem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-03 00:21:26.000000 ymodem-1.5.1b2/ymodem.egg-info/top_level.txt
```

### Comparing `ymodem-1.5.1b1/LICENSE` & `ymodem-1.5.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ymodem-1.5.1b1/PKG-INFO` & `ymodem-1.5.1b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: ymodem
-Version: 1.5.1b1
+Version: 1.5.1b2
 Summary: Ymodem Python3 implementation
 Project-URL: Homepage, https://github.com/o-murphy/ymodem
 Project-URL: Bug Reports, https://github.com/o-murphy/ymodem/issues
 Project-URL: Source, https://github.com/o-murphy/ymodem
 Keywords: pyserial,serial,xmodem,ymodem,python,python3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ordered-set>=4.1.0
 Requires-Dist: pyserial
 
 ![ymodem-logo](https://raw.githubusercontent.com/alexwoo1900/ymodem/master/docs/assets/ymodem-logo.png)
```

### Comparing `ymodem-1.5.1b1/README.md` & `ymodem-1.5.1b2/README.md`

 * *Files identical despite different names*

### Comparing `ymodem-1.5.1b1/pyproject.toml` & `ymodem-1.5.1b2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ymodem"
-version = "1.5.1b1"
+version = "1.5.1b2"
 
 description = "Ymodem Python3 implementation"
 
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 keywords = ["pyserial", "serial", "xmodem", "ymodem", "python", "python3"]
 classifiers = [
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
```

### Comparing `ymodem-1.5.1b1/ymodem/CRC.py` & `ymodem-1.5.1b2/ymodem/CRC.py`

 * *Files identical despite different names*

### Comparing `ymodem-1.5.1b1/ymodem/Platform.py` & `ymodem-1.5.1b2/ymodem/Platform.py`

 * *Files identical despite different names*

### Comparing `ymodem-1.5.1b1/ymodem/Protocol.py` & `ymodem-1.5.1b2/ymodem/Protocol.py`

 * *Files identical despite different names*

### Comparing `ymodem-1.5.1b1/ymodem/Socket.py` & `ymodem-1.5.1b2/ymodem/Socket.py`

 * *Files identical despite different names*

### Comparing `ymodem-1.5.1b1/ymodem/Version.py` & `ymodem-1.5.1b2/ymodem/Version.py`

 * *Files identical despite different names*

### Comparing `ymodem-1.5.1b1/ymodem/__main__.py` & `ymodem-1.5.1b2/ymodem/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     cmd = args.pop('cmd')
     sources = args.pop('sources', [])
     dest = args.pop('dest', './')
 
     socket_args = {
         'packet_size': args.pop('chunk_size', 1024),
-        'protocol': ProtocolType.XMODEM if args.pop('xmodem') else ProtocolType.YMODEM,
+        'protocol_type': ProtocolType.XMODEM if args.pop('xmodem') else ProtocolType.YMODEM,
         'protocol_type_options': ['g'] if args.pop('ymodem_g') else []
     }
 
     debug_level = logging.DEBUG if args.pop('debug') else logging.INFO
 
     logging.basicConfig(level=debug_level, format='%(message)s')
     logger = logging.getLogger('YMODEM')
```

### Comparing `ymodem-1.5.1b1/ymodem.egg-info/PKG-INFO` & `ymodem-1.5.1b2/ymodem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: ymodem
-Version: 1.5.1b1
+Version: 1.5.1b2
 Summary: Ymodem Python3 implementation
 Project-URL: Homepage, https://github.com/o-murphy/ymodem
 Project-URL: Bug Reports, https://github.com/o-murphy/ymodem/issues
 Project-URL: Source, https://github.com/o-murphy/ymodem
 Keywords: pyserial,serial,xmodem,ymodem,python,python3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ordered-set>=4.1.0
 Requires-Dist: pyserial
 
 ![ymodem-logo](https://raw.githubusercontent.com/alexwoo1900/ymodem/master/docs/assets/ymodem-logo.png)
```

