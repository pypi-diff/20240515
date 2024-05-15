# Comparing `tmp/l2dexapi-1.1.tar.gz` & `tmp/l2dexapi-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2dexapi-1.1.tar", last modified: Wed May 15 12:48:00 2024, max compression
+gzip compressed data, was "l2dexapi-1.2.tar", last modified: Wed May 15 08:03:25 2024, max compression
```

## Comparing `l2dexapi-1.1.tar` & `l2dexapi-1.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:48:00.545850 l2dexapi-1.1/
-drwxrwxrwx   0        0        0        0 2024-05-15 12:48:00.532786 l2dexapi-1.1/L2dvExApi/
--rw-rw-rw-   0        0        0     1463 2024-05-15 12:38:42.000000 l2dexapi-1.1/L2dvExApi/ApiList.py
--rw-rw-rw-   0        0        0     8305 2024-05-15 12:40:52.000000 l2dexapi-1.1/L2dvExApi/__init__.py
--rw-rw-rw-   0        0        0     1167 2024-05-15 12:48:00.544857 l2dexapi-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      509 2024-05-15 12:46:39.000000 l2dexapi-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 12:48:00.542843 l2dexapi-1.1/l2dexapi.egg-info/
--rw-rw-rw-   0        0        0     1167 2024-05-15 12:48:00.000000 l2dexapi-1.1/l2dexapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-15 12:48:00.000000 l2dexapi-1.1/l2dexapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:48:00.000000 l2dexapi-1.1/l2dexapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-15 08:03:25.000000 l2dexapi-1.1/l2dexapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-05-15 12:48:00.000000 l2dexapi-1.1/l2dexapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-15 12:48:00.000000 l2dexapi-1.1/l2dexapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 12:48:00.546852 l2dexapi-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1205 2024-05-15 12:47:45.000000 l2dexapi-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:03:25.507957 l2dexapi-1.2/
+drwxrwxrwx   0        0        0        0 2024-05-15 08:03:25.486528 l2dexapi-1.2/L2dvExApi/
+-rw-rw-rw-   0        0        0     8306 2024-05-15 06:42:41.000000 l2dexapi-1.2/L2dvExApi/__init__.py
+-rw-rw-rw-   0        0        0     1463 2024-05-14 11:58:38.000000 l2dexapi-1.2/L2dvExApi/msg_list.py
+-rw-rw-rw-   0        0        0      551 2024-05-15 08:03:25.504527 l2dexapi-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 08:03:25.502958 l2dexapi-1.2/l2dexapi.egg-info/
+-rw-rw-rw-   0        0        0      551 2024-05-15 08:03:25.000000 l2dexapi-1.2/l2dexapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-15 08:03:25.000000 l2dexapi-1.2/l2dexapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 08:03:25.000000 l2dexapi-1.2/l2dexapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-15 08:03:25.000000 l2dexapi-1.2/l2dexapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2024-05-15 08:03:25.000000 l2dexapi-1.2/l2dexapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 08:03:25.000000 l2dexapi-1.2/l2dexapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 08:03:25.507957 l2dexapi-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2024-05-15 08:02:51.000000 l2dexapi-1.2/setup.py
```

### Comparing `l2dexapi-1.1/L2dvExApi/ApiList.py` & `l2dexapi-1.2/L2dvExApi/msg_list.py`

 * *Files identical despite different names*

### Comparing `l2dexapi-1.1/L2dvExApi/__init__.py` & `l2dexapi-1.2/L2dvExApi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .ApiList import Msg_name_to_code
+from .msg_list import Msg_name_to_code
 import websocket, json
 
 class WebSocket:
 
     def __init__(self,url:str=None,**options) -> None:
         self.ws = websocket.WebSocket()
         self.url = url
```

### Comparing `l2dexapi-1.1/setup.py` & `l2dexapi-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 from setuptools import setup, find_packages
 
 setup(
     # 包名
     name='l2dexapi',
 
     # 版本号
-    version='1.1',
+    version='1.2',
 
     # 简短描述
-    description='API for Live2DViewerEX',
-    keywords=("live2d", "api"),
+    description='与Live2DViewerEX相互通信',
 
-    # 详细描述
-    long_description_content_type='text/markdown',
-    long_description=open('README.md',"r",encoding='utf-8').read(),
 
     # 项目主页
     url='http://www.icedream.space',
 
     # 作者信息
     author='Esdrin',
     author_email='esdrin@icedream.space',
 
-    # 许可证
+    # 许可证（您没有提供许可证信息，这里暂时留空）
     license='MIT License',
 
     # 包含的包（find_packages() 会自动查找所有包和子包）
     packages=find_packages(
         include=['L2dvExApi']
         ),
 
     # 依赖列表
     install_requires=[
-        'websocket-client',
+        'websocket',
     ],
 
     # 其他选项，如zip_safe等
     zip_safe=False,
-    
-    # 平台
-    platforms="any",
 
     # 类别
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

