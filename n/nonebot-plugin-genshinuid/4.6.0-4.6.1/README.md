# Comparing `tmp/nonebot_plugin_genshinuid-4.6.0.tar.gz` & `tmp/nonebot_plugin_genshinuid-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshinuid-4.6.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshinuid-4.6.1.tar", max compression
```

## Comparing `nonebot_plugin_genshinuid-4.6.0.tar` & `nonebot_plugin_genshinuid-4.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    27245 2024-03-18 03:59:20.687734 nonebot_plugin_genshinuid-4.6.0/GenshinUID/__init__.py
--rw-r--r--   0        0        0     1241 2024-03-18 03:42:09.945510 nonebot_plugin_genshinuid-4.6.0/GenshinUID/auto_install.py
--rw-r--r--   0        0        0    53583 2024-03-18 03:42:41.172209 nonebot_plugin_genshinuid-4.6.0/GenshinUID/client.py
--rw-r--r--   0        0        0     1043 2023-11-14 11:45:37.543193 nonebot_plugin_genshinuid-4.6.0/GenshinUID/models.py
--rw-r--r--   0        0        0      336 2023-11-07 03:46:26.313902 nonebot_plugin_genshinuid-4.6.0/GenshinUID/path.py
--rw-r--r--   0        0        0      201 2023-11-14 11:45:37.545146 nonebot_plugin_genshinuid-4.6.0/GenshinUID/utils.py
--rw-r--r--   0        0        0    35823 2023-11-07 03:46:26.314931 nonebot_plugin_genshinuid-4.6.0/LICENSE
--rw-r--r--   0        0        0     1739 2024-03-18 04:06:59.454615 nonebot_plugin_genshinuid-4.6.0/pyproject.toml
--rw-r--r--   0        0        0     3318 2023-11-07 03:46:26.314931 nonebot_plugin_genshinuid-4.6.0/README.md
--rw-r--r--   0        0        0     4593 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0    29463 2024-05-15 20:42:35.965512 nonebot_plugin_genshinuid-4.6.1/GenshinUID/__init__.py
+-rw-r--r--   0        0        0     1241 2024-03-26 17:58:55.852956 nonebot_plugin_genshinuid-4.6.1/GenshinUID/auto_install.py
+-rw-r--r--   0        0        0    53583 2024-03-26 17:58:55.853960 nonebot_plugin_genshinuid-4.6.1/GenshinUID/client.py
+-rw-r--r--   0        0        0     1043 2023-11-07 19:36:18.179923 nonebot_plugin_genshinuid-4.6.1/GenshinUID/models.py
+-rw-r--r--   0        0        0      336 2023-09-13 16:21:07.373051 nonebot_plugin_genshinuid-4.6.1/GenshinUID/path.py
+-rw-r--r--   0        0        0      201 2023-11-07 19:17:06.110424 nonebot_plugin_genshinuid-4.6.1/GenshinUID/utils.py
+-rw-r--r--   0        0        0    35823 2023-09-13 16:21:07.374051 nonebot_plugin_genshinuid-4.6.1/LICENSE
+-rw-r--r--   0        0        0     1739 2024-05-15 20:38:04.040090 nonebot_plugin_genshinuid-4.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3318 2023-09-13 16:21:07.376052 nonebot_plugin_genshinuid-4.6.1/README.md
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.6.1/PKG-INFO
```

### Comparing `nonebot_plugin_genshinuid-4.6.0/GenshinUID/__init__.py` & `nonebot_plugin_genshinuid-4.6.1/GenshinUID/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Any, List, Union, Optional
 
 import aiofiles
 from nonebot.log import logger
 from nonebot.adapters import Bot
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
+from nonebot.plugin import PluginMetadata
 from nonebot.internal.adapter import Event
 from websockets.exceptions import ConnectionClosed
 from nonebot import on, require, on_notice, on_message, on_fullmatch
 
 require('nonebot_plugin_apscheduler')
 
 from nonebot_plugin_apscheduler import scheduler  # noqa:E402
@@ -23,31 +24,64 @@
 from .client import GsClient, driver  # noqa:E402
 from .auto_install import start, install  # noqa:E402
 from .models import Message, MessageReceive  # noqa:E402
 
 get_message = on_message(priority=999)
 get_notice = on_notice(priority=999)
 get_tn = on('inline')
-install_core = on_fullmatch('gs一键安装', permission=SUPERUSER, block=True)
-start_core = on_fullmatch('启动core', permission=SUPERUSER, block=True)
+install_core = on_fullmatch(
+    'gs一键安装',
+    permission=SUPERUSER,
+    block=True,
+)
+start_core = on_fullmatch(
+    '启动core',
+    permission=SUPERUSER,
+    block=True,
+)
 connect_core = on_fullmatch(
-    ('连接core', '链接core'), permission=SUPERUSER, block=True
+    ('连接core', '链接core'),
+    permission=SUPERUSER,
+    block=True,
+)
+
+__plugin_meta__ = PluginMetadata(
+    name="GenshinUID",
+    description="SayuCore连接器, 支持大部分适配器的全功能插件",
+    usage="支持大部分适配器连接SayuCore",
+    type="application",
+    homepage="https://docs.sayu-bot.com",
+    supported_adapters=None,
 )
 
 gsclient: Optional[GsClient] = None
 command_start = deepcopy(driver.config.command_start)
 command_start.discard('')
 msg_id_cache = OrderedDict()
 
 if hasattr(driver.config, 'gsuid_core_repeat'):
     is_repeat = True
 else:
     is_repeat = False
 
 
+async def file_to_base64(file_path: Path):
+    # 读取文件内容
+    async with aiofiles.open(str(file_path), 'rb') as file:
+        file_content = await file.read()
+
+    # 将文件内容转换为base64编码
+    base64_encoded = b64encode(file_content)
+
+    # 将base64编码的字节转换为字符串
+    base64_string = base64_encoded.decode('utf-8')
+
+    return base64_string
+
+
 @get_tn.handle()
 @get_notice.handle()
 async def get_notice_message(bot: Bot, ev: Event):
     if gsclient is None:
         return await connect()
     try:
         await gsclient.ws.ping()
@@ -86,15 +120,32 @@
     user_type = 'group' if group_id else 'direct'
 
     if bot.adapter.get_name() == 'OneBot V11':
         if 'notice_type' in raw_data and raw_data['notice_type'] in [
             'group_upload',
             'offline_file',
         ]:
-            val = raw_data['file']['url']
+            if 'url' in raw_data['file']:
+                val = raw_data['file']['url']
+            elif 'id' in raw_data['file']:
+                if raw_data['file']['size'] <= 1024 * 1024 * 4:
+                    val_data = await bot.call_api(
+                        'get_file',
+                        file_id=raw_data['file']['id'],
+                    )
+                    if 'base64' in val_data and val_data['base64']:
+                        val = val_data['base64']
+                    else:
+                        path = Path(val_data['file'])
+                        val = await file_to_base64(path)
+            else:
+                logger.debug(raw_data)
+                logger.warning('[文件上传] 不支持的协议端')
+                return
+
             name = raw_data['file']['name']
             message = [Message('file', f'{name}|{val}')]
             # onebot_v11
         else:
             return
     elif bot.adapter.get_name() == 'DoDo':
         from nonebot.adapters.dodo.event import CardMessageButtonClickEvent
@@ -315,15 +366,15 @@
             sp_bot_id = 'qqgroup'
             user_type = 'group'
             group_id = str(ev.group_openid)
             msg_id = ev.id
             sender = ev.author.dict()
             sender = {
                 'avatar': 'https://q.qlogo.cn/qqapp/'
-                f'{self_id}/{str(user_id)}/0'
+                f'{self_id}/{str(user_id)}/0',
             }
             msg_id_cache[user_id] = msg_id
         elif isinstance(ev, C2CMessageCreateEvent):
             sp_bot_id = 'qqgroup'
             user_type = 'direct'
             group_id = None
             msg_id = ev.id
@@ -656,15 +707,15 @@
 
     # 如果有at提及，增加AT
     if ev.is_tome():
         message.append(Message('at', self_id))
 
     # 处理消息
     for index, _msg in enumerate(messages):
-        message = convert_message(_msg, message, index)
+        message = await convert_message(_msg, message, index, bot)
 
     if not message:
         return
     msg = MessageReceive(
         bot_id=bot_id,
         bot_self_id=self_id,
         user_type=user_type,
@@ -721,27 +772,46 @@
             try:
                 await gsclient.ws.ensure_open()
             except ConnectionClosed:
                 return await connect()
         return
 
 
-def convert_message(_msg: Any, message: List[Message], index: int):
+async def convert_message(
+    _msg: Any,
+    message: List[Message],
+    index: int,
+    bot: Bot,
+):
     if _msg.type == 'text' or _msg.type == 'kmarkdown':
         data: str = (
             _msg.data['text'] if 'text' in _msg.data else _msg.data['content']
         )
 
         if index == 0 or index == 1:
             for word in command_start:
                 _data = data.strip()
                 if _data.startswith(word):
                     data = _data[len(word) :]  # noqa:E203
                     break
         message.append(Message('text', data))
+    elif _msg.type == 'file':
+        if 'file_id' in _msg.data:
+            name = _msg.data.get('file')
+            if float(_msg.data['file_size']) <= 1024 * 1024 * 4:
+                val_data = await bot.call_api(
+                    'get_file',
+                    file_id=_msg.data.get('file_id'),
+                )
+                if 'base64' in val_data and val_data['base64']:
+                    val = val_data['base64']
+                else:
+                    path = Path(val_data['file'])
+                    val = await file_to_base64(path)
+                message.append(Message('file', f'{name}|{val}'))
     elif _msg.type == 'image':
         file_id = _msg.data.get('file_id')
         if file_id in _msg.data.values():
             message.append(Message('image', _msg.data['file_id']))
             logger.debug('[OB12图片]', _msg.data['file_id'])
         elif 'path' in _msg.data:
             message.append(Message('image', _msg.data['path']))
```

### Comparing `nonebot_plugin_genshinuid-4.6.0/GenshinUID/auto_install.py` & `nonebot_plugin_genshinuid-4.6.1/GenshinUID/auto_install.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.6.0/GenshinUID/client.py` & `nonebot_plugin_genshinuid-4.6.1/GenshinUID/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.6.0/GenshinUID/models.py` & `nonebot_plugin_genshinuid-4.6.1/GenshinUID/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.6.0/LICENSE` & `nonebot_plugin_genshinuid-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.6.0/pyproject.toml` & `nonebot_plugin_genshinuid-4.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nonebot-plugin-genshinuid"
-version = "4.6.0"
+version = "4.6.1"
 description = "支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）、DoDo、Villa（米游社大别野）、Discord的全功能NoneBot2原神插件"
 authors = ["KimigaiiWuyi <444835641@qq.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2"
 repository = "https://github.com/KimigaiiWuyi/GenshinUID"
 documentation = "https://docs.gsuid.gbots.work/#/"
```

### Comparing `nonebot_plugin_genshinuid-4.6.0/README.md` & `nonebot_plugin_genshinuid-4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.6.0/PKG-INFO` & `nonebot_plugin_genshinuid-4.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshinuid
-Version: 4.6.0
+Version: 4.6.1
 Summary: 支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）、DoDo、Villa（米游社大别野）、Discord的全功能NoneBot2原神插件
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later
 Author: KimigaiiWuyi
 Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.1.0)
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: gitpython (>=3.1.27)
 Requires-Dist: msgspec (>=0.13.1)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0)
 Requires-Dist: nonebot2 (>=2.0.0b4)
 Requires-Dist: pillow (>=9.2.0)
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.6.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.6.1 Summary:
 æ¯æOneBot
 (QQ)ãOneBotV12ãQQé¢éãå¾®ä¿¡ãKOOKï¼å¼é»å¦ï¼ãTelegramï¼çµæ¥ï¼ãFeiShuï¼é£ä¹¦ï¼ãDoDoãVillaï¼ç±³æ¸¸ç¤¾å¤§å«éï¼ãDiscordçå¨åè½NoneBot2åç¥æä»¶
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later Author: KimigaiiWuyi Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: GNU
 General Public License v3 or later (GPLv3+) Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: aiofiles (>=23.1.0) Requires-Dist: aiohttp
-(>=3.9.3,<4.0.0) Requires-Dist: gitpython (>=3.1.27) Requires-Dist: msgspec
-(>=0.13.1) Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0) Requires-Dist:
-nonebot2 (>=2.0.0b4) Requires-Dist: pillow (>=9.2.0) Requires-Dist: pydantic
-(<2) Requires-Dist: websockets (>=11.0.1) Project-URL: Bug Tracker, https://
-github.com/KimigaiiWuyi/GenshinUID/issues Project-URL: Documentation, https://
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Dist: aiofiles (>=23.1.0) Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-
+Dist: gitpython (>=3.1.27) Requires-Dist: msgspec (>=0.13.1) Requires-Dist:
+nonebot-plugin-apscheduler (>=0.2.0) Requires-Dist: nonebot2 (>=2.0.0b4)
+Requires-Dist: pillow (>=9.2.0) Requires-Dist: pydantic (<2) Requires-Dist:
+websockets (>=11.0.1) Project-URL: Bug Tracker, https://github.com/
+KimigaiiWuyi/GenshinUID/issues Project-URL: Documentation, https://
 docs.gsuid.gbots.work/#/ Project-URL: Repository, https://github.com/
 KimigaiiWuyi/GenshinUID Description-Content-Type: text/markdown
                                  _[_G_e_n_s_h_i_n_U_I_D_]
                          ************ GGeennsshhiinnUUIIDD 44..00 ************
                               ****** ?â??¨?æ??¯?æ??OOnneeBBoott
  ((QQQQ))?ã??QQQQ?é?¢??é???ã???å?¾?®?ä?¿?¡?ã???å?¼??é?»??å??¦?ã??TTeelleeggrraamm?ç???å??¨?å???è??½?å???ç?¥?BBoott?æ???ä?»?¶?â??¨
                                       ******
```

