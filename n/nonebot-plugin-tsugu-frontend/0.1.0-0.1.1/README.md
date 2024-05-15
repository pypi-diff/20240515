# Comparing `tmp/nonebot_plugin_tsugu_frontend-0.1.0.tar.gz` & `tmp/nonebot_plugin_tsugu_frontend-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tsugu_frontend-0.1.0.tar", last modified: Sun May 12 07:27:12 2024, max compression
+gzip compressed data, was "nonebot_plugin_tsugu_frontend-0.1.1.tar", last modified: Wed May 15 14:49:10 2024, max compression
```

## Comparing `nonebot_plugin_tsugu_frontend-0.1.0.tar` & `nonebot_plugin_tsugu_frontend-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4556 2024-05-12 07:26:45.437514 nonebot_plugin_tsugu_frontend-0.1.0/README.md
--rw-r--r--   0        0        0     2637 2024-05-12 07:26:45.441514 nonebot_plugin_tsugu_frontend-0.1.0/nonebot_plugin_tsugu_frontend/__init__.py
--rw-r--r--   0        0        0     1825 2024-05-12 07:26:45.441514 nonebot_plugin_tsugu_frontend-0.1.0/nonebot_plugin_tsugu_frontend/config.py
--rw-r--r--   0        0        0      552 2024-05-12 07:27:12.145470 nonebot_plugin_tsugu_frontend-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_frontend-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4556 2024-05-15 14:48:46.413753 nonebot_plugin_tsugu_frontend-0.1.1/README.md
+-rw-r--r--   0        0        0     2887 2024-05-15 14:48:46.413753 nonebot_plugin_tsugu_frontend-0.1.1/nonebot_plugin_tsugu_frontend/__init__.py
+-rw-r--r--   0        0        0     2529 2024-05-15 14:48:46.413753 nonebot_plugin_tsugu_frontend-0.1.1/nonebot_plugin_tsugu_frontend/config.py
+-rw-r--r--   0        0        0      552 2024-05-15 14:49:10.161979 nonebot_plugin_tsugu_frontend-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_frontend-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_tsugu_frontend-0.1.0/README.md` & `nonebot_plugin_tsugu_frontend-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_frontend-0.1.0/nonebot_plugin_tsugu_frontend/__init__.py` & `nonebot_plugin_tsugu_frontend-0.1.1/nonebot_plugin_tsugu_frontend/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import nonebot
-import tsugu.handler
+import tsugu_async.handler
 from nonebot import require
 from nonebot import on_message
 from nonebot.log import logger
 from nonebot.params import Depends
-from nonebot.utils import run_sync
 from nonebot.adapters import Event, Bot
-from tsugu.config import config as tsugu_config
+from tsugu_async.config import config as tsugu_config
+from tsugu_api_async import settings as tsugu_api_config
 from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_userinfo")
 
 from nonebot_plugin_userinfo import get_user_info
 from nonebot_plugin_alconna import UniMessage, Target, Image, Text, At
@@ -28,30 +28,34 @@
 else:
     plugin_config_dict = plugin_config.dict()
 
 
 __plugin_meta__ = PluginMetadata(
     name="BanG Dream! Tsugu Frontend",
     description="基于 tsugu-python-frontend 的 tsugu-bangdream-bot 插件",
-    usage="\n".join([f"{k}:\n{v}" for k, v in tsugu_config.help_doc_dict.items()]),
+    usage="\n".join([f"{k}:\n{v}" for k, v in tsugu_config._help_doc_dict.items()]),
     type="application",
     homepage="https://github.com/zhaomaoniu/nonebot-plugin-tsugu-frontend",
     config=Config,
     supported_adapters=inherit_supported_adapters(
         "nonebot_plugin_alconna", "nonebot_plugin_userinfo"
     ),
 )
 
 
+# 更新配置对象
 for key, value in plugin_config_dict.items():
-    if hasattr(tsugu_config, key.replace("tsugu_", "")):
-        setattr(tsugu_config, key.replace("tsugu_", ""), value)
-
-
-tsugu_handler_async = run_sync(tsugu.handler)
+    if key.startswith("tsugu_api_"):
+        attr_name = key.replace("tsugu_api_", "")
+        if hasattr(tsugu_api_config, attr_name):
+            setattr(tsugu_api_config, attr_name, value)
+    elif key.startswith("tsugu_"):
+        attr_name = key.replace("tsugu_", "")
+        if hasattr(tsugu_config, attr_name):
+            setattr(tsugu_config, attr_name, value)
 
 
 async def get_target(event: Event, bot: Bot):
     return UniMessage.get_target(event, bot)
 
 
 @on_message(priority=10, block=False).handle()
@@ -62,18 +66,18 @@
 ):
     user_info = await get_user_info(bot, event, event.get_user_id())
 
     if not user_info:
         logger.warning("Failed to get user info")
         return None
 
-    result = await tsugu_handler_async(
+    result = await tsugu_async.handler(
         message=event.get_message().extract_plain_text(),
         user_id=user_info.user_id,
-        platform=plugin_config.tsugu_platform,
+        platform=plugin_config.platform,
         channel_id=(
             target.id if (target.channel or not target.private) else user_info.user_id
         ),
     )
 
     if not result:
         return None
@@ -82,8 +86,8 @@
 
     for content in result:
         if isinstance(content, str):
             message.append(Text(content))
         elif isinstance(content, bytes):
             message.append(Image(raw=content))
 
-    await message.send(target, bot)
+    await message.send(target, bot)
```

### Comparing `nonebot_plugin_tsugu_frontend-0.1.0/pyproject.toml` & `nonebot_plugin_tsugu_frontend-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-tsugu-frontend"
-version = "0.1.0"
+version = "0.1.1"
 description = "基于 tsugu-python-frontend 的 tsugu-bangdream-bot NoneBot 插件"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "nonebot-plugin-alconna>=0.42.4",
```

### Comparing `nonebot_plugin_tsugu_frontend-0.1.0/PKG-INFO` & `nonebot_plugin_tsugu_frontend-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tsugu-frontend
-Version: 0.1.0
+Version: 0.1.1
 Summary: 基于 tsugu-python-frontend 的 tsugu-bangdream-bot NoneBot 插件
 Author-Email: zhaomaoniu <2667292003@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: nonebot-plugin-alconna>=0.42.4
 Requires-Dist: tsugu>=0.6.0
```

