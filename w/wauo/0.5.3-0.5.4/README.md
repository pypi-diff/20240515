# Comparing `tmp/wauo-0.5.3.tar.gz` & `tmp/wauo-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wauo-0.5.3.tar", last modified: Mon May 13 14:44:02 2024, max compression
+gzip compressed data, was "wauo-0.5.4.tar", last modified: Wed May 15 15:37:57 2024, max compression
```

## Comparing `wauo-0.5.3.tar` & `wauo-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-13 14:44:02.198037 wauo-0.5.3/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1730 2024-05-13 14:44:02.197804 wauo-0.5.3/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     1471 2024-05-13 14:43:30.000000 wauo-0.5.3/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-13 14:44:02.198085 wauo-0.5.3/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      615 2024-05-13 14:43:30.000000 wauo-0.5.3/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-13 14:44:02.196785 wauo-0.5.3/wauo/
--rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.5.3/wauo/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.5.3/wauo/exceptions.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.5.3/wauo/response.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     5506 2024-05-13 14:43:30.000000 wauo-0.5.3/wauo/spiders.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-13 14:31:08.000000 wauo-0.5.3/wauo/test.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-13 14:44:02.197602 wauo-0.5.3/wauo.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1730 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-13 14:44:02.000000 wauo-0.5.3/wauo.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-15 15:37:57.991094 wauo-0.5.4/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1806 2024-05-15 15:37:57.990919 wauo-0.5.4/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1471 2024-05-13 14:43:30.000000 wauo-0.5.4/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-15 15:37:57.991124 wauo-0.5.4/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      615 2024-05-15 15:37:44.000000 wauo-0.5.4/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-15 15:37:57.989884 wauo-0.5.4/wauo/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.5.4/wauo/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.5.4/wauo/exceptions.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.5.4/wauo/response.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     5511 2024-05-15 15:36:08.000000 wauo-0.5.4/wauo/spiders.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-13 14:31:08.000000 wauo-0.5.4/wauo/test.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-15 15:37:57.990747 wauo-0.5.4/wauo.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1806 2024-05-15 15:37:57.000000 wauo-0.5.4/wauo.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-15 15:37:57.000000 wauo-0.5.4/wauo.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-15 15:37:57.000000 wauo-0.5.4/wauo.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-15 15:37:57.000000 wauo-0.5.4/wauo.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-15 15:37:57.000000 wauo-0.5.4/wauo.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-15 15:37:57.000000 wauo-0.5.4/wauo.egg-info/top_level.txt
```

### Comparing `wauo-0.5.3/PKG-INFO` & `wauo-0.5.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: wauo
-Version: 0.5.3
+Version: 0.5.4
 Summary: 爬虫者的贴心助手
 Home-page: https://github.com/markadc/wauo
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: python,requests,spider
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: fake_useragent
+Requires-Dist: loguru
 
 # 更新历史
 
 - 新增`jsonp2json`静态方法
 - 爬虫`默认保持会话`状态
 - 新增`get_uuid`、`base64加解密`静态方法
```

### Comparing `wauo-0.5.3/README.md` & `wauo-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `wauo-0.5.3/setup.py` & `wauo-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='wauo',
-    version='0.5.3',
+    version='0.5.4',
     description='爬虫者的贴心助手',
     url='https://github.com/markadc/wauo',
     author='WangTuo',
     author_email='markadc@126.com',
     packages=find_packages(),
     license='MIT',
     zip_safe=False,
```

### Comparing `wauo-0.5.3/wauo/response.py` & `wauo-0.5.4/wauo/response.py`

 * *Files identical despite different names*

### Comparing `wauo-0.5.3/wauo/spiders.py` & `wauo-0.5.4/wauo/spiders.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from wauo.response import Response
 
 
 class SpiderTools:
     """爬虫工具"""
 
     @staticmethod
-    def jsonp2json(jsonp):
+    def jsonp2json(jsonp: str):
         """jsonp转换为json"""
         data: dict = json.loads(re.match(".*?({.*}).*", jsonp, re.S).group(1))
         return data
 
     @staticmethod
     def get_uuid():
         """获取uuid"""
```

### Comparing `wauo-0.5.3/wauo.egg-info/PKG-INFO` & `wauo-0.5.4/wauo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: wauo
-Version: 0.5.3
+Version: 0.5.4
 Summary: 爬虫者的贴心助手
 Home-page: https://github.com/markadc/wauo
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: python,requests,spider
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: fake_useragent
+Requires-Dist: loguru
 
 # 更新历史
 
 - 新增`jsonp2json`静态方法
 - 爬虫`默认保持会话`状态
 - 新增`get_uuid`、`base64加解密`静态方法
```

