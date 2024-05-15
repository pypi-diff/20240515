# Comparing `tmp/switchboard-1.6.5.tar.gz` & `tmp/switchboard-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switchboard-1.6.5.tar", last modified: Wed Oct 18 16:32:43 2023, max compression
+gzip compressed data, was "switchboard-1.6.6.tar", last modified: Wed May 15 15:47:00 2024, max compression
```

## Comparing `switchboard-1.6.5.tar` & `switchboard-1.6.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2023-10-18 16:32:43.797803 switchboard-1.6.5/
--rw-r--r--   0 brondsem   (501) staff       (20)    10834 2019-05-17 17:43:22.000000 switchboard-1.6.5/LICENSE
--rw-r--r--   0 brondsem   (501) staff       (20)       55 2019-07-10 21:43:35.000000 switchboard-1.6.5/MANIFEST.in
--rw-r--r--   0 brondsem   (501) staff       (20)     6101 2023-10-18 16:32:43.797519 switchboard-1.6.5/PKG-INFO
--rw-r--r--   0 brondsem   (501) staff       (20)     5065 2022-03-18 16:19:22.000000 switchboard-1.6.5/README.md
--rw-r--r--   0 brondsem   (501) staff       (20)       38 2023-10-18 16:32:43.797906 switchboard-1.6.5/setup.cfg
--rw-r--r--   0 brondsem   (501) staff       (20)     1597 2023-10-18 16:31:51.000000 switchboard-1.6.5/setup.py
-drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2023-10-18 16:32:43.788499 switchboard-1.6.5/switchboard/
--rw-r--r--   0 brondsem   (501) staff       (20)      376 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/__init__.py
-drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2023-10-18 16:32:43.792493 switchboard-1.6.5/switchboard/admin/
--rw-r--r--   0 brondsem   (501) staff       (20)     6493 2023-09-21 22:06:20.000000 switchboard-1.6.5/switchboard/admin/__init__.py
--rw-r--r--   0 brondsem   (501) staff       (20)    42936 2022-06-20 18:58:47.000000 switchboard-1.6.5/switchboard/admin/index.tpl
-drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2023-10-18 16:32:43.792909 switchboard-1.6.5/switchboard/admin/templates/
--rw-r--r--   0 brondsem   (501) staff       (20)        0 2019-05-17 17:43:22.000000 switchboard-1.6.5/switchboard/admin/templates/__init__.py
--rw-r--r--   0 brondsem   (501) staff       (20)     1650 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/admin/utils.py
--rw-r--r--   0 brondsem   (501) staff       (20)    10473 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/base.py
--rw-r--r--   0 brondsem   (501) staff       (20)     2217 2023-10-03 18:12:01.000000 switchboard-1.6.5/switchboard/builtins.py
--rw-r--r--   0 brondsem   (501) staff       (20)    13257 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/conditions.py
--rw-r--r--   0 brondsem   (501) staff       (20)      730 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/decorators.py
--rw-r--r--   0 brondsem   (501) staff       (20)     2549 2023-09-21 22:06:20.000000 switchboard-1.6.5/switchboard/helpers.py
--rw-r--r--   0 brondsem   (501) staff       (20)     9996 2022-06-20 18:58:47.000000 switchboard-1.6.5/switchboard/manager.py
--rw-r--r--   0 brondsem   (501) staff       (20)     1377 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/middleware.py
--rw-r--r--   0 brondsem   (501) staff       (20)    16441 2023-09-21 22:06:20.000000 switchboard-1.6.5/switchboard/models.py
--rw-r--r--   0 brondsem   (501) staff       (20)     1183 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/proxy.py
--rw-r--r--   0 brondsem   (501) staff       (20)     1329 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/settings.py
--rw-r--r--   0 brondsem   (501) staff       (20)     2533 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/signals.py
--rw-r--r--   0 brondsem   (501) staff       (20)      812 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/template_helpers.py
-drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2023-10-18 16:32:43.796275 switchboard-1.6.5/switchboard/tests/
--rw-r--r--   0 brondsem   (501) staff       (20)        0 2019-05-17 17:43:22.000000 switchboard-1.6.5/switchboard/tests/__init__.py
-drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2023-10-18 16:32:43.796964 switchboard-1.6.5/switchboard/tests/admin/
--rw-r--r--   0 brondsem   (501) staff       (20)        0 2019-07-31 20:55:21.000000 switchboard-1.6.5/switchboard/tests/admin/__init__.py
--rw-r--r--   0 brondsem   (501) staff       (20)     2270 2023-09-21 22:06:20.000000 switchboard-1.6.5/switchboard/tests/admin/test_utils.py
--rw-r--r--   0 brondsem   (501) staff       (20)    14236 2023-01-10 17:46:12.000000 switchboard-1.6.5/switchboard/tests/test_base.py
--rw-r--r--   0 brondsem   (501) staff       (20)     5427 2023-06-05 16:36:27.000000 switchboard-1.6.5/switchboard/tests/test_builtins.py
--rw-r--r--   0 brondsem   (501) staff       (20)    13989 2023-01-10 17:46:12.000000 switchboard-1.6.5/switchboard/tests/test_conditions.py
--rw-r--r--   0 brondsem   (501) staff       (20)      917 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/tests/test_decorators.py
--rw-r--r--   0 brondsem   (501) staff       (20)    27738 2023-01-10 17:46:12.000000 switchboard-1.6.5/switchboard/tests/test_manager.py
--rw-r--r--   0 brondsem   (501) staff       (20)     1277 2023-01-10 17:46:12.000000 switchboard-1.6.5/switchboard/tests/test_middleware.py
--rw-r--r--   0 brondsem   (501) staff       (20)    17541 2023-09-21 22:06:20.000000 switchboard-1.6.5/switchboard/tests/test_models.py
--rw-r--r--   0 brondsem   (501) staff       (20)     1547 2023-01-10 17:46:12.000000 switchboard-1.6.5/switchboard/tests/test_testutils.py
--rw-r--r--   0 brondsem   (501) staff       (20)     1872 2022-06-20 18:02:43.000000 switchboard-1.6.5/switchboard/testutils.py
-drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2023-10-18 16:32:43.790106 switchboard-1.6.5/switchboard.egg-info/
--rw-r--r--   0 brondsem   (501) staff       (20)     6101 2023-10-18 16:32:43.000000 switchboard-1.6.5/switchboard.egg-info/PKG-INFO
--rw-r--r--   0 brondsem   (501) staff       (20)     1094 2023-10-18 16:32:43.000000 switchboard-1.6.5/switchboard.egg-info/SOURCES.txt
--rw-r--r--   0 brondsem   (501) staff       (20)        1 2023-10-18 16:32:43.000000 switchboard-1.6.5/switchboard.egg-info/dependency_links.txt
--rw-r--r--   0 brondsem   (501) staff       (20)        1 2019-07-12 18:45:29.000000 switchboard-1.6.5/switchboard.egg-info/not-zip-safe
--rw-r--r--   0 brondsem   (501) staff       (20)       60 2023-10-18 16:32:43.000000 switchboard-1.6.5/switchboard.egg-info/requires.txt
--rw-r--r--   0 brondsem   (501) staff       (20)       12 2023-10-18 16:32:43.000000 switchboard-1.6.5/switchboard.egg-info/top_level.txt
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-05-15 15:47:00.614857 switchboard-1.6.6/
+-rw-r--r--   0 brondsem   (501) staff       (20)    10834 2019-05-17 17:43:22.000000 switchboard-1.6.6/LICENSE
+-rw-r--r--   0 brondsem   (501) staff       (20)       55 2019-07-10 21:43:35.000000 switchboard-1.6.6/MANIFEST.in
+-rw-r--r--   0 brondsem   (501) staff       (20)     6101 2024-05-15 15:47:00.614627 switchboard-1.6.6/PKG-INFO
+-rw-r--r--   0 brondsem   (501) staff       (20)     5065 2022-03-18 16:19:22.000000 switchboard-1.6.6/README.md
+-rw-r--r--   0 brondsem   (501) staff       (20)       38 2024-05-15 15:47:00.614909 switchboard-1.6.6/setup.cfg
+-rw-r--r--   0 brondsem   (501) staff       (20)     1590 2024-05-15 15:46:21.000000 switchboard-1.6.6/setup.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-05-15 15:47:00.609419 switchboard-1.6.6/switchboard/
+-rw-r--r--   0 brondsem   (501) staff       (20)      359 2024-05-15 15:46:09.000000 switchboard-1.6.6/switchboard/__init__.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-05-15 15:47:00.611384 switchboard-1.6.6/switchboard/admin/
+-rw-r--r--   0 brondsem   (501) staff       (20)     6493 2023-09-21 22:06:20.000000 switchboard-1.6.6/switchboard/admin/__init__.py
+-rw-r--r--   0 brondsem   (501) staff       (20)    42936 2022-06-20 18:58:47.000000 switchboard-1.6.6/switchboard/admin/index.tpl
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-05-15 15:47:00.611622 switchboard-1.6.6/switchboard/admin/templates/
+-rw-r--r--   0 brondsem   (501) staff       (20)        0 2019-05-17 17:43:22.000000 switchboard-1.6.6/switchboard/admin/templates/__init__.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1650 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/admin/utils.py
+-rw-r--r--   0 brondsem   (501) staff       (20)    10473 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/base.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     2217 2023-10-03 18:12:01.000000 switchboard-1.6.6/switchboard/builtins.py
+-rw-r--r--   0 brondsem   (501) staff       (20)    13257 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/conditions.py
+-rw-r--r--   0 brondsem   (501) staff       (20)      730 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/decorators.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     2549 2023-09-21 22:06:20.000000 switchboard-1.6.6/switchboard/helpers.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     9996 2022-06-20 18:58:47.000000 switchboard-1.6.6/switchboard/manager.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1377 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/middleware.py
+-rw-r--r--   0 brondsem   (501) staff       (20)    16441 2023-09-21 22:06:20.000000 switchboard-1.6.6/switchboard/models.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1183 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/proxy.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1329 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/settings.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     2533 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/signals.py
+-rw-r--r--   0 brondsem   (501) staff       (20)      812 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/template_helpers.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-05-15 15:47:00.613770 switchboard-1.6.6/switchboard/tests/
+-rw-r--r--   0 brondsem   (501) staff       (20)        0 2019-05-17 17:43:22.000000 switchboard-1.6.6/switchboard/tests/__init__.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-05-15 15:47:00.614093 switchboard-1.6.6/switchboard/tests/admin/
+-rw-r--r--   0 brondsem   (501) staff       (20)        0 2019-07-31 20:55:21.000000 switchboard-1.6.6/switchboard/tests/admin/__init__.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     2270 2023-09-21 22:06:20.000000 switchboard-1.6.6/switchboard/tests/admin/test_utils.py
+-rw-r--r--   0 brondsem   (501) staff       (20)    14236 2023-01-10 17:46:12.000000 switchboard-1.6.6/switchboard/tests/test_base.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     5427 2023-06-05 16:36:27.000000 switchboard-1.6.6/switchboard/tests/test_builtins.py
+-rw-r--r--   0 brondsem   (501) staff       (20)    13989 2023-01-10 17:46:12.000000 switchboard-1.6.6/switchboard/tests/test_conditions.py
+-rw-r--r--   0 brondsem   (501) staff       (20)      917 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/tests/test_decorators.py
+-rw-r--r--   0 brondsem   (501) staff       (20)    27738 2023-01-10 17:46:12.000000 switchboard-1.6.6/switchboard/tests/test_manager.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1277 2023-01-10 17:46:12.000000 switchboard-1.6.6/switchboard/tests/test_middleware.py
+-rw-r--r--   0 brondsem   (501) staff       (20)    17541 2023-09-21 22:06:20.000000 switchboard-1.6.6/switchboard/tests/test_models.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1547 2023-01-10 17:46:12.000000 switchboard-1.6.6/switchboard/tests/test_testutils.py
+-rw-r--r--   0 brondsem   (501) staff       (20)     1872 2022-06-20 18:02:43.000000 switchboard-1.6.6/switchboard/testutils.py
+drwxr-xr-x   0 brondsem   (501) staff       (20)        0 2024-05-15 15:47:00.614311 switchboard-1.6.6/switchboard.egg-info/
+-rw-r--r--   0 brondsem   (501) staff       (20)     6101 2024-05-15 15:47:00.000000 switchboard-1.6.6/switchboard.egg-info/PKG-INFO
+-rw-r--r--   0 brondsem   (501) staff       (20)     1094 2024-05-15 15:47:00.000000 switchboard-1.6.6/switchboard.egg-info/SOURCES.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)        1 2024-05-15 15:47:00.000000 switchboard-1.6.6/switchboard.egg-info/dependency_links.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)        1 2019-07-12 18:45:29.000000 switchboard-1.6.6/switchboard.egg-info/not-zip-safe
+-rw-r--r--   0 brondsem   (501) staff       (20)       60 2024-05-15 15:47:00.000000 switchboard-1.6.6/switchboard.egg-info/requires.txt
+-rw-r--r--   0 brondsem   (501) staff       (20)       12 2024-05-15 15:47:00.000000 switchboard-1.6.6/switchboard.egg-info/top_level.txt
```

### Comparing `switchboard-1.6.5/LICENSE` & `switchboard-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/PKG-INFO` & `switchboard-1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchboard
-Version: 1.6.5
+Version: 1.6.6
 Summary: Feature flipper for Pyramid, Pylons, or TurboGears apps.
 Home-page: https://github.com/switchboardpy/switchboard/
 Download-URL: https://github.com/switchboardpy/switchboard/releases
 Author: Kyle Adams
 Author-email: kadams54@users.noreply.github.com
 License: Apache License
 Keywords: switches feature flipper pyramid pylons turbogears
```

### Comparing `switchboard-1.6.5/README.md` & `switchboard-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/setup.py` & `switchboard-1.6.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 from pathlib import Path
 
-VERSION = '1.6.5'
+VERSION = '1.6.6'
 INSTALL_REQUIRES = [
     'pymongo >= 3',
     'blinker >= 1.2',
     'WebOb >= 0.9',
     'Mako >= 0.9',
     'bottle >= 0.12.8',
 ]
@@ -39,11 +39,11 @@
     license='Apache License',
     packages=setuptools.find_packages(exclude=['ez_setup']),
     include_package_data=True,
     install_requires=INSTALL_REQUIRES,
     zip_safe=False,
     tests_require=[
         'pytest',
-        'selenium < 4.10',
+        'selenium',
         'splinter',
     ],
 )
```

### Comparing `switchboard-1.6.5/switchboard/admin/__init__.py` & `switchboard-1.6.6/switchboard/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/admin/index.tpl` & `switchboard-1.6.6/switchboard/admin/index.tpl`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/admin/utils.py` & `switchboard-1.6.6/switchboard/admin/utils.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/base.py` & `switchboard-1.6.6/switchboard/base.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/builtins.py` & `switchboard-1.6.6/switchboard/builtins.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/conditions.py` & `switchboard-1.6.6/switchboard/conditions.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/decorators.py` & `switchboard-1.6.6/switchboard/decorators.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/helpers.py` & `switchboard-1.6.6/switchboard/helpers.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/manager.py` & `switchboard-1.6.6/switchboard/manager.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/middleware.py` & `switchboard-1.6.6/switchboard/middleware.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/models.py` & `switchboard-1.6.6/switchboard/models.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/proxy.py` & `switchboard-1.6.6/switchboard/proxy.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/settings.py` & `switchboard-1.6.6/switchboard/settings.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/signals.py` & `switchboard-1.6.6/switchboard/signals.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/template_helpers.py` & `switchboard-1.6.6/switchboard/template_helpers.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/tests/admin/test_utils.py` & `switchboard-1.6.6/switchboard/tests/admin/test_utils.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/tests/test_base.py` & `switchboard-1.6.6/switchboard/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/tests/test_builtins.py` & `switchboard-1.6.6/switchboard/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/tests/test_conditions.py` & `switchboard-1.6.6/switchboard/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/tests/test_decorators.py` & `switchboard-1.6.6/switchboard/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/tests/test_manager.py` & `switchboard-1.6.6/switchboard/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/tests/test_middleware.py` & `switchboard-1.6.6/switchboard/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/tests/test_models.py` & `switchboard-1.6.6/switchboard/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/tests/test_testutils.py` & `switchboard-1.6.6/switchboard/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard/testutils.py` & `switchboard-1.6.6/switchboard/testutils.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.5/switchboard.egg-info/PKG-INFO` & `switchboard-1.6.6/switchboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchboard
-Version: 1.6.5
+Version: 1.6.6
 Summary: Feature flipper for Pyramid, Pylons, or TurboGears apps.
 Home-page: https://github.com/switchboardpy/switchboard/
 Download-URL: https://github.com/switchboardpy/switchboard/releases
 Author: Kyle Adams
 Author-email: kadams54@users.noreply.github.com
 License: Apache License
 Keywords: switches feature flipper pyramid pylons turbogears
```

### Comparing `switchboard-1.6.5/switchboard.egg-info/SOURCES.txt` & `switchboard-1.6.6/switchboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

