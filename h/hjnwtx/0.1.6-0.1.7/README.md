# Comparing `tmp/hjnwtx-0.1.6.tar.gz` & `tmp/hjnwtx-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hjnwtx-0.1.6.tar", last modified: Sat Apr 20 09:03:10 2024, max compression
+gzip compressed data, was "hjnwtx-0.1.7.tar", last modified: Wed May 15 03:23:26 2024, max compression
```

## Comparing `hjnwtx-0.1.6.tar` & `hjnwtx-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-04-20 09:03:10.517207 hjnwtx-0.1.6/
--rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-04-20 09:03:10.517207 hjnwtx-0.1.6/PKG-INFO
--rw-rw-r--   0 hjn       (1003) hjn       (1003)       16 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/README.md
-drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-04-20 09:03:10.517207 hjnwtx-0.1.6/hjnwtx/
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    17426 2024-01-23 02:42:51.000000 hjnwtx-0.1.6/hjnwtx/H8mess.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      171 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/__init__.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    23455 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/cinradHJN.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     1163 2024-01-06 12:54:45.000000 hjnwtx-0.1.6/hjnwtx/colormap.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    11590 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/examMeso.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      800 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/hjnDAAS.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2927 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/hjnFTP.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    12118 2024-03-05 02:10:16.000000 hjnwtx-0.1.6/hjnwtx/hjnGIS.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      516 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/hjnGPU.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2362 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/hjnIDW.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2395 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/hjnKDTree.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     1975 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/hjnLAPSTransform.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2193 2024-04-20 09:02:38.000000 hjnwtx-0.1.6/hjnwtx/hjnLog.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     6580 2024-01-23 02:47:03.000000 hjnwtx-0.1.6/hjnwtx/hjnMiscellaneous.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     5753 2024-01-23 02:42:52.000000 hjnwtx-0.1.6/hjnwtx/hjnProj.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     1290 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/inotify.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     3343 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/matplotlibMess.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    24653 2024-01-24 03:29:07.000000 hjnwtx-0.1.6/hjnwtx/mkNCHJN.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    23449 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/newTypeRadar.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)       80 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/test.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     5119 2024-01-03 00:18:24.000000 hjnwtx-0.1.6/hjnwtx/tlogP.py
-drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-04-20 09:03:10.517207 hjnwtx-0.1.6/hjnwtx.egg-info/
--rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-04-20 09:03:10.000000 hjnwtx-0.1.6/hjnwtx.egg-info/PKG-INFO
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      581 2024-04-20 09:03:10.000000 hjnwtx-0.1.6/hjnwtx.egg-info/SOURCES.txt
--rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-04-20 09:03:10.000000 hjnwtx-0.1.6/hjnwtx.egg-info/dependency_links.txt
--rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-01-03 00:19:56.000000 hjnwtx-0.1.6/hjnwtx.egg-info/not-zip-safe
--rw-rw-r--   0 hjn       (1003) hjn       (1003)        7 2024-04-20 09:03:10.000000 hjnwtx-0.1.6/hjnwtx.egg-info/top_level.txt
--rw-rw-r--   0 hjn       (1003) hjn       (1003)       38 2024-04-20 09:03:10.517207 hjnwtx-0.1.6/setup.cfg
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      250 2024-04-20 09:02:49.000000 hjnwtx-0.1.6/setup.py
+drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-05-15 03:23:26.936907 hjnwtx-0.1.7/
+-rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-05-15 03:23:26.936907 hjnwtx-0.1.7/PKG-INFO
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)       16 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/README.md
+drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-05-15 03:23:26.924907 hjnwtx-0.1.7/hjnwtx/
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    17426 2024-01-23 02:42:51.000000 hjnwtx-0.1.7/hjnwtx/H8mess.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      171 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/__init__.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    23455 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/cinradHJN.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     1163 2024-01-06 12:54:45.000000 hjnwtx-0.1.7/hjnwtx/colormap.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    11590 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/examMeso.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      800 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnDAAS.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     2927 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnFTP.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    12118 2024-03-05 02:10:16.000000 hjnwtx-0.1.7/hjnwtx/hjnGIS.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      516 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnGPU.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     2362 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnIDW.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     2395 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnKDTree.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     1975 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnLAPSTransform.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     2193 2024-04-20 09:02:38.000000 hjnwtx-0.1.7/hjnwtx/hjnLog.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     6580 2024-01-23 02:47:03.000000 hjnwtx-0.1.7/hjnwtx/hjnMiscellaneous.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     5753 2024-01-23 02:42:52.000000 hjnwtx-0.1.7/hjnwtx/hjnProj.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     1290 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/inotify.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     3343 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/matplotlibMess.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    24653 2024-01-24 03:29:07.000000 hjnwtx-0.1.7/hjnwtx/mkNCHJN.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    23449 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/newTypeRadar.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)       80 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/test.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     5119 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/tlogP.py
+drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-05-15 03:23:26.936907 hjnwtx-0.1.7/hjnwtx.egg-info/
+-rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-05-15 03:23:26.000000 hjnwtx-0.1.7/hjnwtx.egg-info/PKG-INFO
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      581 2024-05-15 03:23:26.000000 hjnwtx-0.1.7/hjnwtx.egg-info/SOURCES.txt
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-05-15 03:23:26.000000 hjnwtx-0.1.7/hjnwtx.egg-info/dependency_links.txt
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-01-03 00:19:56.000000 hjnwtx-0.1.7/hjnwtx.egg-info/not-zip-safe
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)        7 2024-05-15 03:23:26.000000 hjnwtx-0.1.7/hjnwtx.egg-info/top_level.txt
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)       38 2024-05-15 03:23:26.936907 hjnwtx-0.1.7/setup.cfg
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      250 2024-05-15 03:21:46.000000 hjnwtx-0.1.7/setup.py
```

### Comparing `hjnwtx-0.1.6/hjnwtx/H8mess.py` & `hjnwtx-0.1.7/hjnwtx/H8mess.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/cinradHJN.py` & `hjnwtx-0.1.7/hjnwtx/cinradHJN.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/colormap.py` & `hjnwtx-0.1.7/hjnwtx/colormap.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/examMeso.py` & `hjnwtx-0.1.7/hjnwtx/examMeso.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnDAAS.py` & `hjnwtx-0.1.7/hjnwtx/hjnDAAS.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnFTP.py` & `hjnwtx-0.1.7/hjnwtx/hjnFTP.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnGIS.py` & `hjnwtx-0.1.7/hjnwtx/hjnGIS.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnGPU.py` & `hjnwtx-0.1.7/hjnwtx/hjnGPU.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnIDW.py` & `hjnwtx-0.1.7/hjnwtx/hjnIDW.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnKDTree.py` & `hjnwtx-0.1.7/hjnwtx/hjnKDTree.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnLAPSTransform.py` & `hjnwtx-0.1.7/hjnwtx/hjnLAPSTransform.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnLog.py` & `hjnwtx-0.1.7/hjnwtx/hjnLog.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnMiscellaneous.py` & `hjnwtx-0.1.7/hjnwtx/hjnMiscellaneous.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/hjnProj.py` & `hjnwtx-0.1.7/hjnwtx/hjnProj.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/inotify.py` & `hjnwtx-0.1.7/hjnwtx/inotify.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/matplotlibMess.py` & `hjnwtx-0.1.7/hjnwtx/matplotlibMess.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/mkNCHJN.py` & `hjnwtx-0.1.7/hjnwtx/mkNCHJN.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/newTypeRadar.py` & `hjnwtx-0.1.7/hjnwtx/newTypeRadar.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx/tlogP.py` & `hjnwtx-0.1.7/hjnwtx/tlogP.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.6/hjnwtx.egg-info/SOURCES.txt` & `hjnwtx-0.1.7/hjnwtx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

