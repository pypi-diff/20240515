# Comparing `tmp/tsugu-api-python-1.1.1.tar.gz` & `tmp/tsugu-api-python-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.1.1.tar", last modified: Wed May 15 04:36:39 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.1.2.tar", last modified: Wed May 15 04:46:31 2024, max compression
```

## Comparing `tsugu-api-python-1.1.1.tar` & `tsugu-api-python-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:36:39.048784 tsugu-api-python-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-15 04:36:39.048784 tsugu-api-python-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:36:39.048784 tsugu-api-python-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:36:39.044784 tsugu-api-python-1.1.1/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:36:39.048784 tsugu-api-python-1.1.1/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-15 04:36:30.000000 tsugu-api-python-1.1.1/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:36:39.048784 tsugu-api-python-1.1.1/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-15 04:36:38.000000 tsugu-api-python-1.1.1/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 04:36:39.000000 tsugu-api-python-1.1.1/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:36:38.000000 tsugu-api-python-1.1.1/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 04:36:38.000000 tsugu-api-python-1.1.1/tsugu_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 04:36:38.000000 tsugu-api-python-1.1.1/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:46:31.990208 tsugu-api-python-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-15 04:46:31.990208 tsugu-api-python-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:46:31.990208 tsugu-api-python-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:46:31.986208 tsugu-api-python-1.1.2/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:46:31.986208 tsugu-api-python-1.1.2/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:46:31.990208 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.1.1/LICENSE` & `tsugu-api-python-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/PKG-INFO` & `tsugu-api-python-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.1 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.2 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.1/README.md` & `tsugu-api-python-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/setup.py` & `tsugu-api-python-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.1.1',
+    version='1.1.2',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-1.1.1/tsugu_api/__init__.py` & `tsugu-api-python-1.1.2/tsugu_api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 from ._tsugu import gacha_simulate as gacha_simulate
 from ._tsugu import search_character as search_character
 from ._tsugu import get_card_illustration as get_card_illustration
 
 from ._station import station_query_all_room as station_query_all_room
 from ._station import station_submit_room_number as station_submit_room_number
 
+from ._bandoristation import query_room_number as query_room_number
 from ._bandoristation import submit_room_number as submit_room_number
```

### Comparing `tsugu-api-python-1.1.1/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.1.2/tsugu_api/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api/_network.py` & `tsugu-api-python-1.1.2/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api/_station.py` & `tsugu-api-python-1.1.2/tsugu_api/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api/_tsugu.py` & `tsugu-api-python-1.1.2/tsugu_api/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api/_typing.py` & `tsugu-api-python-1.1.2/tsugu_api/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api/_user.py` & `tsugu-api-python-1.1.2/tsugu_api/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api/settings.py` & `tsugu-api-python-1.1.2/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api/utils.py` & `tsugu-api-python-1.1.2/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api_async/__init__.py` & `tsugu-api-python-1.1.2/tsugu_api_async/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 from ._tsugu import gacha_simulate as gacha_simulate
 from ._tsugu import search_character as search_character
 from ._tsugu import get_card_illustration as get_card_illustration
 
 from ._station import station_query_all_room as station_query_all_room
 from ._station import station_submit_room_number as station_submit_room_number
 
+from ._bandoristation import query_room_number as query_room_number
 from ._bandoristation import submit_room_number as submit_room_number
```

### Comparing `tsugu-api-python-1.1.1/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.1.2/tsugu_api_async/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api_async/_network.py` & `tsugu-api-python-1.1.2/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api_async/_station.py` & `tsugu-api-python-1.1.2/tsugu_api_async/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.1.2/tsugu_api_async/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api_async/_typing.py` & `tsugu-api-python-1.1.2/tsugu_api_async/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api_async/_user.py` & `tsugu-api-python-1.1.2/tsugu_api_async/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api_async/settings.py` & `tsugu-api-python-1.1.2/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api_async/utils.py` & `tsugu-api-python-1.1.2/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.1/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.1.2/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.1 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.2 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.1/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.1.2/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

