# Comparing `tmp/dynamic_drf-0.1.tar.gz` & `tmp/dynamic_drf-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_drf-0.1.tar", last modified: Mon May  6 11:13:01 2024, max compression
+gzip compressed data, was "dynamic_drf-0.2.tar", last modified: Wed May 15 06:49:19 2024, max compression
```

## Comparing `dynamic_drf-0.1.tar` & `dynamic_drf-0.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 atitsharma   (501) staff       (20)        0 2024-05-06 11:13:01.503647 dynamic_drf-0.1/
--rw-r--r--   0 atitsharma   (501) staff       (20)      560 2024-05-06 11:13:01.503399 dynamic_drf-0.1/PKG-INFO
-drwxr-xr-x   0 atitsharma   (501) staff       (20)        0 2024-05-06 11:13:01.502115 dynamic_drf-0.1/dynamic_drf/
--rw-r--r--   0 atitsharma   (501) staff       (20)       76 2024-05-06 11:10:48.000000 dynamic_drf-0.1/dynamic_drf/__init__.py
--rw-r--r--   0 atitsharma   (501) staff       (20)     1099 2024-05-06 10:41:11.000000 dynamic_drf-0.1/dynamic_drf/dyn_settings.py
-drwxr-xr-x   0 atitsharma   (501) staff       (20)        0 2024-05-06 11:13:01.503134 dynamic_drf-0.1/dynamic_drf.egg-info/
--rw-r--r--   0 atitsharma   (501) staff       (20)      560 2024-05-06 11:13:01.000000 dynamic_drf-0.1/dynamic_drf.egg-info/PKG-INFO
--rw-r--r--   0 atitsharma   (501) staff       (20)      234 2024-05-06 11:13:01.000000 dynamic_drf-0.1/dynamic_drf.egg-info/SOURCES.txt
--rw-r--r--   0 atitsharma   (501) staff       (20)        1 2024-05-06 11:13:01.000000 dynamic_drf-0.1/dynamic_drf.egg-info/dependency_links.txt
--rw-r--r--   0 atitsharma   (501) staff       (20)       66 2024-05-06 11:13:01.000000 dynamic_drf-0.1/dynamic_drf.egg-info/requires.txt
--rw-r--r--   0 atitsharma   (501) staff       (20)       12 2024-05-06 11:13:01.000000 dynamic_drf-0.1/dynamic_drf.egg-info/top_level.txt
--rw-r--r--   0 atitsharma   (501) staff       (20)       38 2024-05-06 11:13:01.503712 dynamic_drf-0.1/setup.cfg
--rw-r--r--   0 atitsharma   (501) staff       (20)      688 2024-05-06 11:12:58.000000 dynamic_drf-0.1/setup.py
+drwxr-xr-x   0 atitsharma   (501) staff       (20)        0 2024-05-15 06:49:19.143711 dynamic_drf-0.2/
+-rw-r--r--   0 atitsharma   (501) staff       (20)      560 2024-05-15 06:49:19.143481 dynamic_drf-0.2/PKG-INFO
+drwxr-xr-x   0 atitsharma   (501) staff       (20)        0 2024-05-15 06:49:19.142299 dynamic_drf-0.2/dynamic_drf/
+-rw-r--r--   0 atitsharma   (501) staff       (20)      162 2024-05-15 06:45:29.000000 dynamic_drf-0.2/dynamic_drf/__init__.py
+-rw-r--r--   0 atitsharma   (501) staff       (20)      981 2024-05-15 06:44:31.000000 dynamic_drf-0.2/dynamic_drf/apps.py
+-rw-r--r--   0 atitsharma   (501) staff       (20)      553 2024-05-15 06:45:19.000000 dynamic_drf-0.2/dynamic_drf/auth.py
+-rw-r--r--   0 atitsharma   (501) staff       (20)     1686 2024-05-15 06:44:41.000000 dynamic_drf-0.2/dynamic_drf/dyn_settings.py
+-rw-r--r--   0 atitsharma   (501) staff       (20)     1088 2024-05-15 06:44:49.000000 dynamic_drf-0.2/dynamic_drf/models.py
+-rw-r--r--   0 atitsharma   (501) staff       (20)      912 2024-05-15 06:45:02.000000 dynamic_drf-0.2/dynamic_drf/serializers.py
+-rw-r--r--   0 atitsharma   (501) staff       (20)      546 2024-05-15 06:45:17.000000 dynamic_drf-0.2/dynamic_drf/views.py
+drwxr-xr-x   0 atitsharma   (501) staff       (20)        0 2024-05-15 06:49:19.143218 dynamic_drf-0.2/dynamic_drf.egg-info/
+-rw-r--r--   0 atitsharma   (501) staff       (20)      560 2024-05-15 06:49:19.000000 dynamic_drf-0.2/dynamic_drf.egg-info/PKG-INFO
+-rw-r--r--   0 atitsharma   (501) staff       (20)      344 2024-05-15 06:49:19.000000 dynamic_drf-0.2/dynamic_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 atitsharma   (501) staff       (20)        1 2024-05-15 06:49:19.000000 dynamic_drf-0.2/dynamic_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 atitsharma   (501) staff       (20)       66 2024-05-15 06:49:19.000000 dynamic_drf-0.2/dynamic_drf.egg-info/requires.txt
+-rw-r--r--   0 atitsharma   (501) staff       (20)       12 2024-05-15 06:49:19.000000 dynamic_drf-0.2/dynamic_drf.egg-info/top_level.txt
+-rw-r--r--   0 atitsharma   (501) staff       (20)       38 2024-05-15 06:49:19.143803 dynamic_drf-0.2/setup.cfg
+-rw-r--r--   0 atitsharma   (501) staff       (20)      688 2024-05-15 06:48:59.000000 dynamic_drf-0.2/setup.py
```

### Comparing `dynamic_drf-0.1/PKG-INFO` & `dynamic_drf-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_drf
-Version: 0.1
+Version: 0.2
 Summary: A package that overrides the default drf spectacular
 Author: Atit Sharma
 Requires-Dist: Django==5.0.4
 Requires-Dist: drf-spectacular==0.27.2
 Requires-Dist: djangorestframework==3.15.1
 
 This python package is for those developers who feels complex to include drf-spectacular in there project. Now simple add this 'dyn_drf' in your installed apps. Then in your project url import urlpatterns from urlpatterns          Simply do urlpatterns+=[             path('your-other-url',your_views),         ]
```

### Comparing `dynamic_drf-0.1/dynamic_drf.egg-info/PKG-INFO` & `dynamic_drf-0.2/dynamic_drf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_drf
-Version: 0.1
+Version: 0.2
 Summary: A package that overrides the default drf spectacular
 Author: Atit Sharma
 Requires-Dist: Django==5.0.4
 Requires-Dist: drf-spectacular==0.27.2
 Requires-Dist: djangorestframework==3.15.1
 
 This python package is for those developers who feels complex to include drf-spectacular in there project. Now simple add this 'dyn_drf' in your installed apps. Then in your project url import urlpatterns from urlpatterns          Simply do urlpatterns+=[             path('your-other-url',your_views),         ]
```

### Comparing `dynamic_drf-0.1/setup.py` & `dynamic_drf-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dynamic_drf',
-    version='0.1',
+    version='0.2',
     description="A package that overrides the default drf spectacular", \
     long_description="This python package is for those developers who feels complex to include drf-spectacular in there project. Now simple add this 'dyn_drf' in your installed apps. Then in your project url import urlpatterns from urlpatterns  \
         Simply do urlpatterns+=[ \
             path('your-other-url',your_views), \
         ]" ,
     author='Atit Sharma',
     packages=['dynamic_drf'],
```

