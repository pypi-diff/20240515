# Comparing `tmp/pywxdll-0.2.1.tar.gz` & `tmp/pywxdll-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywxdll-0.2.1.tar", last modified: Wed Dec 13 11:12:58 2023, max compression
+gzip compressed data, was "pywxdll-0.2.3.tar", last modified: Tue May 14 14:49:13 2024, max compression
```

## Comparing `pywxdll-0.2.1.tar` & `pywxdll-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-12-13 11:12:58.000000 pywxdll-0.2.1/
--rw-r--r--   0 henryyang   (501) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.2.1/LICENSE
--rw-rw-r--   0 henryyang   (501) staff       (20)       26 2023-05-01 18:24:33.000000 pywxdll-0.2.1/MANIFEST.in
--rw-r--r--   0 henryyang   (501) staff       (20)      735 2023-12-13 11:12:58.000000 pywxdll-0.2.1/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)    10479 2023-12-13 11:02:10.000000 pywxdll-0.2.1/README.md
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-12-13 11:12:58.000000 pywxdll-0.2.1/pywxdll/
--rw-r--r--   0 henryyang   (501) staff       (20)       72 2023-10-26 14:31:40.000000 pywxdll-0.2.1/pywxdll/__init__.py
--rw-r--r--   0 henryyang   (501) staff       (20)     7699 2023-12-13 10:44:30.000000 pywxdll-0.2.1/pywxdll/pywxdll.py
--rw-r--r--   0 henryyang   (501) staff       (20)     4020 2023-10-26 14:31:40.000000 pywxdll-0.2.1/pywxdll/pywxdll_json.py
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-12-13 11:12:58.000000 pywxdll-0.2.1/pywxdll.egg-info/
--rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-02 16:36:22.000000 pywxdll-0.2.1/pywxdll.egg-info/.gitignore
--rw-r--r--   0 henryyang   (501) staff       (20)      735 2023-12-13 11:12:58.000000 pywxdll-0.2.1/pywxdll.egg-info/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)      283 2023-12-13 11:12:58.000000 pywxdll-0.2.1/pywxdll.egg-info/SOURCES.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-12-13 11:12:58.000000 pywxdll-0.2.1/pywxdll.egg-info/dependency_links.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       26 2023-12-13 11:12:58.000000 pywxdll-0.2.1/pywxdll.egg-info/requires.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        8 2023-12-13 11:12:58.000000 pywxdll-0.2.1/pywxdll.egg-info/top_level.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       38 2023-12-13 11:12:58.000000 pywxdll-0.2.1/setup.cfg
--rw-r--r--   0 henryyang   (501) staff       (20)     3761 2023-12-13 10:57:17.000000 pywxdll-0.2.1/setup.py
+drwxr-xr-x   0 keren      (502) staff       (20)        0 2024-05-14 14:49:13.551266 pywxdll-0.2.3/
+-rw-r-----   0 keren      (502) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.2.3/LICENSE
+-rw-r-----   0 keren      (502) staff       (20)       26 2023-05-01 18:24:33.000000 pywxdll-0.2.3/MANIFEST.in
+-rw-r--r--   0 keren      (502) staff       (20)      735 2024-05-14 14:49:13.551163 pywxdll-0.2.3/PKG-INFO
+-rw-r-----   0 keren      (502) staff       (20)    10479 2023-12-13 11:02:10.000000 pywxdll-0.2.3/README.md
+drwxr-xr-x   0 keren      (502) staff       (20)        0 2024-05-14 14:49:13.550427 pywxdll-0.2.3/pywxdll/
+-rw-r-----   0 keren      (502) staff       (20)       72 2023-10-26 14:31:40.000000 pywxdll-0.2.3/pywxdll/__init__.py
+-rw-r-----   0 keren      (502) staff       (20)     9665 2024-05-14 14:40:13.000000 pywxdll-0.2.3/pywxdll/pywxdll.py
+-rw-r-----   0 keren      (502) staff       (20)     4064 2024-05-13 15:56:32.000000 pywxdll-0.2.3/pywxdll/pywxdll_json.py
+drwxr-xr-x   0 keren      (502) staff       (20)        0 2024-05-14 14:49:13.551033 pywxdll-0.2.3/pywxdll.egg-info/
+-rw-r--r--   0 keren      (502) staff       (20)      735 2024-05-14 14:49:13.000000 pywxdll-0.2.3/pywxdll.egg-info/PKG-INFO
+-rw-r--r--   0 keren      (502) staff       (20)      255 2024-05-14 14:49:13.000000 pywxdll-0.2.3/pywxdll.egg-info/SOURCES.txt
+-rw-r--r--   0 keren      (502) staff       (20)        1 2024-05-14 14:49:13.000000 pywxdll-0.2.3/pywxdll.egg-info/dependency_links.txt
+-rw-r--r--   0 keren      (502) staff       (20)       26 2024-05-14 14:49:13.000000 pywxdll-0.2.3/pywxdll.egg-info/requires.txt
+-rw-r--r--   0 keren      (502) staff       (20)        8 2024-05-14 14:49:13.000000 pywxdll-0.2.3/pywxdll.egg-info/top_level.txt
+-rw-r--r--   0 keren      (502) staff       (20)       38 2024-05-14 14:49:13.551302 pywxdll-0.2.3/setup.cfg
+-rw-r-----   0 keren      (502) staff       (20)     3761 2024-05-14 14:38:57.000000 pywxdll-0.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pywxdll-0.2.1/LICENSE` & `pywxdll-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pywxdll-0.2.1/PKG-INFO` & `pywxdll-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.2.1
+Version: 0.2.3
 Summary: A Python package for wechat robot, basing on dll hook.
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.2.1/README.md` & `pywxdll-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pywxdll-0.2.1/pywxdll/pywxdll.py` & `pywxdll-0.2.3/pywxdll/pywxdll.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import threading
 
 import requests
 import websocket
-from cachetools import cached, TTLCache
 
 from .pywxdll_json import *
 
 HEART_BEAT = 5005
 RECV_TXT_MSG = 1
 RECV_PIC_MSG = 3
-NEW_FRIEND_REQUEST = 37
 RECV_TXT_CITE_MSG = 49
+NEW_FRIEND_REQUEST = 37
 PIC_MSG = 500
 AT_MSG = 550
 TXT_MSG = 555
+ATTATCH_FILE = 5003
 USER_LIST = 5000
 GET_USER_LIST_SUCCSESS = 5001
 GET_USER_LIST_FAIL = 5002
-ATTATCH_FILE = 5003
 CHATROOM_MEMBER = 5010
 CHATROOM_MEMBER_NICK = 5020
 DEBUG_SWITCH = 6000
 PERSONAL_INFO = 6500
 PERSONAL_DETAIL = 6550
 DESTROY_ALL = 9999
 JOIN_ROOM = 10000
@@ -36,22 +35,22 @@
         self.ip = ip
         self.port = port
         self._ws_url = f'ws://{ip}:{port}'  # websocket url
         self.msg_list = []
 
     def _thread_start(self):  # 监听hook The thread for listeing
         websocket.enableTrace(False)  # 开启调试？
-        ws = websocket.WebSocketApp(
+        self.ws = websocket.WebSocketApp(
             self._ws_url,
             on_open=self._on_open,
             on_message=self._on_message,
             on_error=self._on_error,
             on_close=self._on_close
         )
-        ws.run_forever()
+        self.ws.run_forever()
 
     def start(self):  # 开始监听 Start listening for incoming message
         '''
         开始监听微信消息 Start listening for incoming message
         :return:
         '''
         wxt = threading.Thread(target=self._thread_start)
@@ -62,15 +61,15 @@
         pass
 
     def _on_message(self, ws, message):  # For websocket
         recieve = json.loads(message)
         r_type = recieve['type']
         if r_type == 5005:
             pass
-        elif r_type == 1 or r_type == 3 or r_type == 49:
+        else:
             self.msg_list.append(self._recv_txt_handle(recieve))
 
     def _on_error(self, ws, error):  # For websocket
         raise error
 
     def _on_close(self, ws):  # For websocket
         pass
@@ -148,34 +147,31 @@
     # 获取唯一id
     def _getid(self):
         return time.strftime("%Y%m%d%H%M%S", time.localtime())
 
     def heartbeat(h):
         return h
 
-    @cached(cache=TTLCache(maxsize=10, ttl=15))
     def get_personal_detail(self, wxid: str):
         '''
         获取其他账号信息 get other user's information
         :param wxid: wxid(新用户的wxid以wxid_开头 老用户他们可能修改过 现在改不了) wechatid(start with wxid_)
         :return: Dictionary
         '''
         uri = '/api/get_personal_detail'
         return self._send_http(uri, json_get_personal_detail(wxid))['content']
 
-    @cached(cache=TTLCache(maxsize=5, ttl=15))
     def get_contact_list(self):
         '''
         获取微信通讯录用户名字和wxid get wechat address list username and wxid
         :return: Dictionary
         '''
         uri = '/api/getcontactlist'
         return self._send_http(uri, json_get_contact_list())['content']
 
-    @cached(cache=TTLCache(maxsize=100, ttl=15))
     def get_chatroom_nickname(self, roomid: str = 'null', wxid: str = 'ROOT'):
         '''
         获取群聊中用户昵称 Get chatroom's user's nickname
         :param roomid: 群号(以@chatroom结尾) groupchatid(end with@chatroom)
         :param wxid: wxid(新用户的wxid以wxid_开头 老用户他们可能修改过 现在改不了) wechatid(start with wxid_)
         :return: Dictionary
         '''
@@ -186,15 +182,14 @@
         '''
         获取朋友昵称 Get friend's nickname
         :param wxid: wxid(新用户的wxid以wxid_开头 老用户他们可能修改过 现在改不了) wechatid(start with wxid_)
         :return: Dictionary
         '''
         return self.get_chatroom_nickname(wxid=wxid)
 
-    @cached(cache=TTLCache(maxsize=5, ttl=30))
     def get_chatroom_memberlist(self, roomid: str = 'null'):
         '''
         获取群聊中用户列表 Get chatroom member list
         :param roomid: 群号(以@chatroom结尾) groupchatid(end with@chatroom)
         :return: List or Dictionary
         '''
         uri = '/api/get_charroom_member_list'
@@ -207,7 +202,69 @@
                     return i
             return result
 
     ######## 信息处理 ########
 
     def _recv_txt_handle(self, recieve):
         return recieve
+
+    ######## 解密图片 ########
+
+    # 感谢群友提供的代码
+
+    @staticmethod
+    def _get_xor(file_buffer, suffix_map):
+        for key in suffix_map.keys():
+            suffix = suffix_map[key]
+            hex_values = [key[i:i + 2] for i in range(0, len(key), 2)]
+            map_values = []
+            for a in range(3):
+                byte = file_buffer[a]
+                value = byte ^ int(hex_values[a], 16)
+                map_values.append(value)
+            if map_values[0] == map_values[1] == map_values[2]:
+                return {"value": format(map_values[0], 'x'), "suffix": suffix}
+        return None
+
+    def decrypt_wechat_picture(self, file_path: str, output_dir: str = '') -> str:
+        if not os.path.isdir(output_dir) and output_dir:
+            raise Exception('Output directory does not exist')
+        elif not os.path.isfile(file_path):
+            raise Exception('File does not exist')
+
+        file_path = os.path.abspath(file_path)
+
+        suffix_map = {
+            'ffd8ffe000104a464946': 'jpg',
+            '89504e470d0a1a0a0000': 'png',
+            '47494638396126026f01': 'gif',
+            '49492a00227105008037': 'tif',
+            '424d228c010000000000': 'bmp',
+            '424d8240090000000000': 'bmp',
+            '424d8e1b030000000000': 'bmp'
+        }
+
+        with open(file_path, 'rb') as file:
+            buffer = file.read()
+
+        if buffer:
+            xor1 = self._get_xor(buffer, suffix_map)
+            if not xor1:
+                raise Exception('Decrypt failed')
+
+            # 转换之后的文件流
+            new_buffer = bytearray()
+            # 遍历文件流
+            for value in buffer:
+                # 异或运算
+                new_buffer.append(value ^ int('0x' + xor1['value'], 16))
+
+            # 保存文件
+            save_file_name = os.path.join(output_dir,
+                                          os.path.splitext(os.path.basename(file_path))[0] + '.' + xor1['suffix'])
+            with open(save_file_name, 'wb') as file:
+                file.write(new_buffer)
+
+            return os.path.abspath(save_file_name)
+        else:
+            # 处理读取失败的情况
+            raise Exception('Read file failed')
```

### Comparing `pywxdll-0.2.1/pywxdll/pywxdll_json.py` & `pywxdll-0.2.3/pywxdll/pywxdll_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import time
+import os
 
 HEART_BEAT = 5005
 RECV_TXT_MSG = 1
 RECV_PIC_MSG = 3
 NEW_FRIEND_REQUEST = 37
 RECV_TXT_CITE_MSG = 49
 PIC_MSG = 500
@@ -39,15 +40,15 @@
 # 发送图片信息 wxid为用户id或群id path为发送图片的路径（建议用绝对路径） Send picture to wxid(perosnal or group)
 def json_send_pic_msg(wxid, path: str):
     qs = {
         'id': _getid(),
         'type': PIC_MSG,
         'wxid': wxid,
         'roomid': 'null',
-        'content': path,
+        'content': os.path.abspath(path),
         'nickname': "null",
         'ext': 'null'
     }
     s = json.dumps(qs)
     return s
 
 
@@ -69,15 +70,15 @@
 # 发送文件 wxid为用户id或者群id path为文件的路径 send attachment to chat or group
 def json_send_attach_msg(wxid, path):
     qs = {
         'id': _getid(),
         'type': ATTATCH_FILE,
         'wxid': wxid,
         'roomid': 'null',
-        'content': path,
+        'content': os.path.abspath(path),
         'nickname': "null",
         'ext': 'null'
     }
 
     s = json.dumps(qs)
     return s
```

### Comparing `pywxdll-0.2.1/pywxdll.egg-info/PKG-INFO` & `pywxdll-0.2.3/pywxdll.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.2.1
+Version: 0.2.3
 Summary: A Python package for wechat robot, basing on dll hook.
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.2.1/setup.py` & `pywxdll-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pywxdll'
 DESCRIPTION = 'A Python package for wechat robot, basing on dll hook.'
 URL = 'https://github.com/HenryXiaoYang/pywxdll'
 EMAIL = 'henryyang666@hotmal.com'
 AUTHOR = 'HenryXiaoYang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.1'
+VERSION = '0.2.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['websocket-client', 'requests']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

