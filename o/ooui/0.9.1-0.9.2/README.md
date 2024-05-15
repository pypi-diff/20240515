# Comparing `tmp/ooui-0.9.1.tar.gz` & `tmp/ooui-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooui-0.9.1.tar", last modified: Tue May 14 13:39:13 2024, max compression
+gzip compressed data, was "ooui-0.9.2.tar", last modified: Tue May 14 15:59:54 2024, max compression
```

## Comparing `ooui-0.9.1.tar` & `ooui-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:13.357871 ooui-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 13:39:04.000000 ooui-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 13:39:04.000000 ooui-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 13:39:13.357871 ooui-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 13:39:04.000000 ooui-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:13.357871 ooui-0.9.1/ooui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:13.357871 ooui-0.9.1/ooui/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/graph/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/graph/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/graph/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/graph/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/graph/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9469 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/graph/timerange.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:13.357871 ooui-0.9.1/ooui/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/helpers/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-14 13:39:04.000000 ooui-0.9.1/ooui/helpers/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:39:13.357871 ooui-0.9.1/ooui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 13:39:13.000000 ooui-0.9.1/ooui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 13:39:13.000000 ooui-0.9.1/ooui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:39:13.000000 ooui-0.9.1/ooui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 13:39:13.000000 ooui-0.9.1/ooui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 13:39:13.000000 ooui-0.9.1/ooui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 13:39:04.000000 ooui-0.9.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 13:39:04.000000 ooui-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:39:13.357871 ooui-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-14 13:39:04.000000 ooui-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:59:54.654172 ooui-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 15:59:46.000000 ooui-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 15:59:46.000000 ooui-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 15:59:54.654172 ooui-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 15:59:46.000000 ooui-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:59:54.650172 ooui-0.9.2/ooui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:59:54.654172 ooui-0.9.2/ooui/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/graph/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/graph/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/graph/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/graph/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/graph/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/graph/timerange.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:59:54.654172 ooui-0.9.2/ooui/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/helpers/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-14 15:59:46.000000 ooui-0.9.2/ooui/helpers/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:59:54.654172 ooui-0.9.2/ooui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 15:59:54.000000 ooui-0.9.2/ooui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 15:59:54.000000 ooui-0.9.2/ooui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:59:54.000000 ooui-0.9.2/ooui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 15:59:54.000000 ooui-0.9.2/ooui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 15:59:54.000000 ooui-0.9.2/ooui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 15:59:46.000000 ooui-0.9.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 15:59:46.000000 ooui-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:59:54.654172 ooui-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-14 15:59:46.000000 ooui-0.9.2/setup.py
```

### Comparing `ooui-0.9.1/LICENSE` & `ooui-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/graph/__init__.py` & `ooui-0.9.2/ooui/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/graph/axis.py` & `ooui-0.9.2/ooui/graph/axis.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/graph/base.py` & `ooui-0.9.2/ooui/graph/base.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/graph/chart.py` & `ooui-0.9.2/ooui/graph/chart.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/graph/fields.py` & `ooui-0.9.2/ooui/graph/fields.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/graph/indicator.py` & `ooui-0.9.2/ooui/graph/indicator.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/graph/processor.py` & `ooui-0.9.2/ooui/graph/processor.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/graph/timerange.py` & `ooui-0.9.2/ooui/graph/timerange.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,16 @@
 
     :rtype: str
     :returns: The appropriate date format string compatible with
         `datetime.strptime`.
     """
     if ':' in date_str:
         return '%Y-%m-%d %H:%M:%S'
+    elif date_str.count('-') == 1:
+        return '%Y-%m'
     else:
         return '%Y-%m-%d'
 
 
 def get_unique_values_grouped_by(values, group_by):
     """
     Group values by unique keys determined by the grouping criteria.
```

### Comparing `ooui-0.9.1/ooui/helpers/__init__.py` & `ooui-0.9.2/ooui/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/helpers/conditions.py` & `ooui-0.9.2/ooui/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/ooui/helpers/domain.py` & `ooui-0.9.2/ooui/helpers/domain.py`

 * *Files identical despite different names*

### Comparing `ooui-0.9.1/setup.py` & `ooui-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     name='ooui',
     description='Open Object User Interface',
     author='GISCE',
     author_email='devel@gisce.net',
     url='https://github.com/gisce/python-ooui',
-    version='0.9.1',
+    version='0.9.2',
     license='MIT',
     long_description='''Open Object User Interface for GISCE-ERP''',
     provides=['ooui'],
     install_requires=requirements,
     tests_require=requirements_dev,
     packages=find_packages()
 )
```

