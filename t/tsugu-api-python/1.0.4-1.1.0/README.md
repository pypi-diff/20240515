# Comparing `tmp/tsugu-api-python-1.0.4.tar.gz` & `tmp/tsugu-api-python-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.0.4.tar", last modified: Tue May 14 16:40:20 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.1.0.tar", last modified: Wed May 15 04:30:39 2024, max compression
```

## Comparing `tsugu-api-python-1.0.4.tar` & `tsugu-api-python-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:40:20.332352 tsugu-api-python-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-14 16:40:20.332352 tsugu-api-python-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:40:20.332352 tsugu-api-python-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:40:20.328353 tsugu-api-python-1.0.4/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:40:20.328353 tsugu-api-python-1.0.4/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-14 16:40:10.000000 tsugu-api-python-1.0.4/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:40:20.332352 tsugu-api-python-1.0.4/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-14 16:40:20.000000 tsugu-api-python-1.0.4/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 16:40:20.000000 tsugu-api-python-1.0.4/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:40:20.000000 tsugu-api-python-1.0.4/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 16:40:20.000000 tsugu-api-python-1.0.4/tsugu_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 16:40:20.000000 tsugu-api-python-1.0.4/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:30:39.426855 tsugu-api-python-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-15 04:30:39.426855 tsugu-api-python-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:30:39.426855 tsugu-api-python-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:30:39.422855 tsugu-api-python-1.1.0/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:30:39.422855 tsugu-api-python-1.1.0/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-15 04:30:30.000000 tsugu-api-python-1.1.0/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:30:39.426855 tsugu-api-python-1.1.0/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-15 04:30:39.000000 tsugu-api-python-1.1.0/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 04:30:39.000000 tsugu-api-python-1.1.0/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:30:39.000000 tsugu-api-python-1.1.0/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 04:30:39.000000 tsugu-api-python-1.1.0/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 04:30:39.000000 tsugu-api-python-1.1.0/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.0.4/LICENSE` & `tsugu-api-python-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/PKG-INFO` & `tsugu-api-python-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.0.4
+Version: 1.1.0
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
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.4 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.0 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.0.4/README.md` & `tsugu-api-python-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/setup.py` & `tsugu-api-python-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.0.4',
+    version='1.1.0',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-1.0.4/tsugu_api/__init__.py` & `tsugu-api-python-1.1.0/tsugu_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.1.0/tsugu_api/_bandoristation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from tsugu_api import settings
 from tsugu_api._network import Api
+from tsugu_api._typing import _StationRoom
 from tsugu_api.exception import RoomSubmitFailure
 
 BANDORI_STATION_URL = 'https://api.bandoristation.com/index.php'
 
 def submit_room_number(number: int, user_id: str, raw_message: str, source: str, token: str) -> None:
-    '''上传车牌号
+    '''上传房间号
 
     参数:
-        number (int): 车牌号
+        number (int): 房间号
         user_id (str): 用户 ID
-        raw_message (str): 原始消息，用作车牌号注释
-        source (str): 车牌来源，即令牌名称
+        raw_message (str): 原始消息，用作房间号注释
+        source (str): 房间来源，即令牌名称
         token (str): 上传用的车站令牌
     '''
     
     # 构建参数
     params = {
         'function': 'submit_room_number',
         'number': number,
@@ -28,7 +29,25 @@
     # 发送请求
     response = Api(
         BANDORI_STATION_URL,
         proxy=settings.backend_proxy
     ).get(params).json()
     if response['status'] == 'failure':
         raise RoomSubmitFailure(response['response'])
+
+def query_room_number() -> list[_StationRoom]:
+    '''获取房间号
+
+    返回:
+        list[_StationRoom]: 房间信息列表
+    '''
+    
+    # 构建参数
+    params = {
+        'function': 'query_room_number'
+    }
+    
+    # 发送请求
+    return Api(
+        BANDORI_STATION_URL,
+        proxy=settings.backend_proxy
+    ).get(params).json()
```

### Comparing `tsugu-api-python-1.0.4/tsugu_api/_network.py` & `tsugu-api-python-1.1.0/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api/_station.py` & `tsugu-api-python-1.1.0/tsugu_api/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api/_tsugu.py` & `tsugu-api-python-1.1.0/tsugu_api/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api/_typing.py` & `tsugu-api-python-1.1.0/tsugu_api_async/_typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 '''
 `tsugu_api._typing`
 
 定义了一些类型别名
 '''
 
 from typing import (
+    Any,
     Union,
     Literal,
     TypeAlias,
     TypedDict,
     NotRequired
 )
 
+from httpx import Response
+from aiohttp import ClientResponse
+
+_ApiResponse: TypeAlias = Union[Response, ClientResponse]
+
 _ServerId: TypeAlias = Literal[0, 1, 2, 3, 4]
 '''
 服务器 ID
 
 值:
     0: 日服
     1: 国际服
@@ -118,7 +124,30 @@
     status: _Status
     data: Union[str, _VerifyCode]
 
 class _BindPlayerVerificationResponse(TypedDict):
     '''`/user/bindPlayerVerification` 响应结果'''
     status: _Status
     data: str
+
+class _SourceInfo(TypedDict):
+    '''来源信息'''
+    name: str
+    type: str
+
+class _UserInfo(TypedDict):
+    '''用户信息'''
+    avatar: str
+    bandori_player_brief_info: Any
+    role: int
+    type: str
+    user_id: int
+    username: str
+
+class _StationRoom(TypedDict):
+    '''车站房间数据'''
+    number: int
+    raw_message: str
+    source_info: _SourceInfo
+    time: int
+    type: str
+    user_info: _UserInfo
```

### Comparing `tsugu-api-python-1.0.4/tsugu_api/_user.py` & `tsugu-api-python-1.1.0/tsugu_api/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api/settings.py` & `tsugu-api-python-1.1.0/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api/utils.py` & `tsugu-api-python-1.1.0/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api_async/__init__.py` & `tsugu-api-python-1.1.0/tsugu_api_async/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.1.0/tsugu_api_async/_bandoristation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from httpx import Response
 
 from tsugu_api_async import settings
 from tsugu_api_async._network import Api
+from tsugu_api_async._typing import _StationRoom
 from tsugu_api_async.exception import RoomSubmitFailure
 
 BANDORI_STATION_URL = 'https://api.bandoristation.com/index.php'
 
 async def submit_room_number(number: int, user_id: str, raw_message: str, source: str, token: str) -> None:
-    '''上传车牌号
+    '''上传房间号
 
     参数:
-        number (int): 车牌号
+        number (int): 房间号
         user_id (str): 用户 ID
-        raw_message (str): 原始消息，用作车牌号注释
-        source (str): 车牌来源，即令牌名称
+        raw_message (str): 原始消息，用作房间号注释
+        source (str): 房间来源，即令牌名称
         token (str): 上传用的车站令牌
     '''
     
     # 构建参数
     params = {
         'function': 'submit_room_number',
         'number': number,
@@ -32,7 +33,27 @@
             BANDORI_STATION_URL,
             proxy=settings.backend_proxy
     ).get(params)
     if isinstance(response, Response): response = response.json()
     else: response = await response.json()
     if response['status'] == 'failure':
         raise RoomSubmitFailure(response['response'])
+
+async def query_room_number() -> list[_StationRoom]:
+    '''获取房间号
+
+    返回:
+        list[_StationRoom]: 房间信息列表
+    '''
+    
+    # 构建参数
+    params = {
+        'function': 'query_room_number'
+    }
+    
+    # 发送请求
+    response = await Api(
+        BANDORI_STATION_URL,
+        proxy=settings.backend_proxy
+    ).get(params)
+    if isinstance(response, Response): return response.json()
+    else: return await response.json()
```

### Comparing `tsugu-api-python-1.0.4/tsugu_api_async/_network.py` & `tsugu-api-python-1.1.0/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api_async/_station.py` & `tsugu-api-python-1.1.0/tsugu_api_async/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.1.0/tsugu_api_async/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api_async/_typing.py` & `tsugu-api-python-1.1.0/tsugu_api/_typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 '''
 `tsugu_api._typing`
 
 定义了一些类型别名
 '''
 
 from typing import (
+    Any,
     Union,
     Literal,
     TypeAlias,
     TypedDict,
     NotRequired
 )
 
-from httpx import Response
-from aiohttp import ClientResponse
-
-_ApiResponse: TypeAlias = Union[Response, ClientResponse]
-
 _ServerId: TypeAlias = Literal[0, 1, 2, 3, 4]
 '''
 服务器 ID
 
 值:
     0: 日服
     1: 国际服
@@ -123,7 +119,30 @@
     status: _Status
     data: Union[str, _VerifyCode]
 
 class _BindPlayerVerificationResponse(TypedDict):
     '''`/user/bindPlayerVerification` 响应结果'''
     status: _Status
     data: str
+
+class _SourceInfo(TypedDict):
+    '''来源信息'''
+    name: str
+    type: str
+
+class _UserInfo(TypedDict):
+    '''用户信息'''
+    avatar: str
+    bandori_player_brief_info: Any
+    role: int
+    type: str
+    user_id: int
+    username: str
+
+class _StationRoom(TypedDict):
+    '''车站房间数据'''
+    number: int
+    raw_message: str
+    source_info: _SourceInfo
+    time: int
+    type: str
+    user_info: _UserInfo
```

### Comparing `tsugu-api-python-1.0.4/tsugu_api_async/_user.py` & `tsugu-api-python-1.1.0/tsugu_api_async/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api_async/settings.py` & `tsugu-api-python-1.1.0/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api_async/utils.py` & `tsugu-api-python-1.1.0/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.0.4/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.1.0/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.0.4
+Version: 1.1.0
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
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.4 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.0 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.0.4/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.1.0/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

