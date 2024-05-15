# Comparing `tmp/MDRefine-0.0.1.tar.gz` & `tmp/MDRefine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDRefine-0.0.1.tar", last modified: Wed May 15 15:23:06 2024, max compression
+gzip compressed data, was "MDRefine-0.0.2.tar", last modified: Wed May 15 18:54:28 2024, max compression
```

## Comparing `MDRefine-0.0.1.tar` & `MDRefine-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bussi      (503) staff       (20)        0 2024-05-15 15:23:06.629533 MDRefine-0.0.1/
-drwxr-xr-x   0 bussi      (503) staff       (20)        0 2024-05-15 15:23:06.627898 MDRefine-0.0.1/MDRefine/
--rw-r--r--   0 bussi      (503) staff       (20)      179 2024-05-15 15:19:57.000000 MDRefine-0.0.1/MDRefine/__init__.py
--rw-r--r--   0 bussi      (503) staff       (20)       40 2024-05-15 15:17:30.000000 MDRefine-0.0.1/MDRefine/_version.py
-drwxr-xr-x   0 bussi      (503) staff       (20)        0 2024-05-15 15:23:06.629031 MDRefine-0.0.1/MDRefine.egg-info/
--rw-r--r--   0 bussi      (503) staff       (20)      705 2024-05-15 15:23:06.000000 MDRefine-0.0.1/MDRefine.egg-info/PKG-INFO
--rw-r--r--   0 bussi      (503) staff       (20)      219 2024-05-15 15:23:06.000000 MDRefine-0.0.1/MDRefine.egg-info/SOURCES.txt
--rw-r--r--   0 bussi      (503) staff       (20)        1 2024-05-15 15:23:06.000000 MDRefine-0.0.1/MDRefine.egg-info/dependency_links.txt
--rw-r--r--   0 bussi      (503) staff       (20)       13 2024-05-15 15:23:06.000000 MDRefine-0.0.1/MDRefine.egg-info/requires.txt
--rw-r--r--   0 bussi      (503) staff       (20)        9 2024-05-15 15:23:06.000000 MDRefine-0.0.1/MDRefine.egg-info/top_level.txt
--rw-r--r--   0 bussi      (503) staff       (20)      705 2024-05-15 15:23:06.629339 MDRefine-0.0.1/PKG-INFO
--rw-r--r--   0 bussi      (503) staff       (20)       62 2024-05-15 15:18:58.000000 MDRefine-0.0.1/README.md
--rw-r--r--   0 bussi      (503) staff       (20)       38 2024-05-15 15:23:06.629601 MDRefine-0.0.1/setup.cfg
--rw-r--r--   0 bussi      (503) staff       (20)     1139 2024-05-15 15:21:59.000000 MDRefine-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:28.058858 MDRefine-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:28.058858 MDRefine-0.0.2/MDRefine/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 18:53:58.000000 MDRefine-0.0.2/MDRefine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 18:53:58.000000 MDRefine-0.0.2/MDRefine/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:28.058858 MDRefine-0.0.2/MDRefine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-15 18:54:28.000000 MDRefine-0.0.2/MDRefine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-15 18:54:28.000000 MDRefine-0.0.2/MDRefine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:54:28.000000 MDRefine-0.0.2/MDRefine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 18:54:28.000000 MDRefine-0.0.2/MDRefine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 18:54:28.000000 MDRefine-0.0.2/MDRefine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-15 18:54:28.058858 MDRefine-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 18:53:58.000000 MDRefine-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:54:28.058858 MDRefine-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 18:53:58.000000 MDRefine-0.0.2/setup.py
```

### Comparing `MDRefine-0.0.1/MDRefine.egg-info/PKG-INFO` & `MDRefine-0.0.2/MDRefine.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MDRefine
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to perform refinement of MD simulation trajectories.
 Home-page: https://github.com/bussilab/MDRefine
 Author: Ivan Gilardoni
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `MDRefine-0.0.1/PKG-INFO` & `MDRefine-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MDRefine
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to perform refinement of MD simulation trajectories.
 Home-page: https://github.com/bussilab/MDRefine
 Author: Ivan Gilardoni
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `MDRefine-0.0.1/setup.py` & `MDRefine-0.0.2/setup.py`

 * *Files identical despite different names*

