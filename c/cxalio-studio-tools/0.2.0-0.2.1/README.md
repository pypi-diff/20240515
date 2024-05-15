# Comparing `tmp/cxalio_studio_tools-0.2.0.tar.gz` & `tmp/cxalio_studio_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxalio_studio_tools-0.2.0.tar", max compression
+gzip compressed data, was "cxalio_studio_tools-0.2.1.tar", max compression
```

## Comparing `cxalio_studio_tools-0.2.0.tar` & `cxalio_studio_tools-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35821 2024-04-16 07:18:25.822233 cxalio_studio_tools-0.2.0/LICENSE
--rw-r--r--   0        0        0     1064 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1204 2024-05-15 04:56:11.309783 cxalio_studio_tools-0.2.0/README.md
--rw-r--r--   0        0        0      188 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.0/src/cx_core/__init__.py
--rw-r--r--   0        0        0      145 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/abstract_app.py
--rw-r--r--   0        0        0      838 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/abstract_env.py
--rw-r--r--   0        0        0     1286 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/app_logger.py
--rw-r--r--   0        0        0     2024 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/datapackage.py
--rw-r--r--   0        0        0     1826 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/ffmpeg_progress_parser.py
--rw-r--r--   0        0        0     1462 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/folder_expander.py
--rw-r--r--   0        0        0      465 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.0/src/cx_core/osinfo.py
--rw-r--r--   0        0        0     1421 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.0/src/cx_core/tag_replacer.py
--rw-r--r--   0        0        0     2991 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/timecode.py
--rw-r--r--   0        0        0     1640 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/timepoint.py
--rw-r--r--   0        0        0      466 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.0/src/cx_core/tui_elements.py
--rw-r--r--   0        0        0     2813 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.0/src/cx_core/utils.py
--rw-r--r--   0        0        0      101 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.0/src/cx_subtitle/__init__.py
--rw-r--r--   0        0        0     4611 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_subtitle/loader.py
--rw-r--r--   0        0        0     5394 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.0/src/cx_subtitle/saver.py
--rw-r--r--   0        0        0      731 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.0/src/cx_subtitle/subtitle.py
--rw-r--r--   0        0        0     2858 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.0/src/cx_subtitle/subtitle_formatter.py
--rw-r--r--   0        0        0       35 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/media_killer/__init__.py
--rw-r--r--   0        0        0     1312 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.0/src/media_killer/env.py
--rw-r--r--   0        0        0     2958 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.0/src/media_killer/example_project.toml
--rw-r--r--   0        0        0      364 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.0/src/media_killer/exceptions.py
--rw-r--r--   0        0        0     5453 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.0/src/media_killer/help.md
--rw-r--r--   0        0        0     7891 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.0/src/media_killer/media_killer_app.py
--rw-r--r--   0        0        0     6476 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.0/src/media_killer/mission.py
--rw-r--r--   0        0        0     1269 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.0/src/media_killer/option_package.py
--rw-r--r--   0        0        0     3827 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.0/src/media_killer/planner.py
--rw-r--r--   0        0        0     3319 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.0/src/media_killer/profile_loader.py
--rw-r--r--   0        0        0     1762 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.0/src/media_killer/script_writer.py
--rw-r--r--   0        0        0     2793 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.0/src/media_killer/source_adapter.py
--rw-r--r--   0        0        0     3887 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.0/src/media_killer/transcoder.py
--rw-r--r--   0        0        0       30 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/sub_conv/__init__.py
--rw-r--r--   0        0        0     1132 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/sub_conv/env.py
--rw-r--r--   0        0        0       44 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/sub_conv/exceptions.py
--rw-r--r--   0        0        0     3316 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/sub_conv/help.md
--rw-r--r--   0        0        0     9947 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/sub_conv/subconv_app.py
--rw-r--r--   0        0        0     1624 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/sub_conv/subtitle_translator.py
--rw-r--r--   0        0        0        0 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/systools/__init__.py
--rw-r--r--   0        0        0      278 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.0/src/systools/env.py
--rw-r--r--   0        0        0     3722 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.0/src/systools/update_githubhosts.py
--rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-16 07:18:25.822233 cxalio_studio_tools-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1064 2024-05-15 05:50:23.704918 cxalio_studio_tools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1271 2024-05-15 05:50:23.701352 cxalio_studio_tools-0.2.1/README.md
+-rw-r--r--   0        0        0      188 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.1/src/cx_core/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/cx_core/abstract_app.py
+-rw-r--r--   0        0        0      838 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/cx_core/abstract_env.py
+-rw-r--r--   0        0        0     1286 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/cx_core/app_logger.py
+-rw-r--r--   0        0        0     2024 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/cx_core/datapackage.py
+-rw-r--r--   0        0        0     1826 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/cx_core/ffmpeg_progress_parser.py
+-rw-r--r--   0        0        0     1462 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/cx_core/folder_expander.py
+-rw-r--r--   0        0        0      465 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.1/src/cx_core/osinfo.py
+-rw-r--r--   0        0        0     1421 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.1/src/cx_core/tag_replacer.py
+-rw-r--r--   0        0        0     2991 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/cx_core/timecode.py
+-rw-r--r--   0        0        0     1640 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/cx_core/timepoint.py
+-rw-r--r--   0        0        0      466 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.1/src/cx_core/tui_elements.py
+-rw-r--r--   0        0        0     2813 2024-05-15 05:48:14.513139 cxalio_studio_tools-0.2.1/src/cx_core/utils.py
+-rw-r--r--   0        0        0      101 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.1/src/cx_subtitle/__init__.py
+-rw-r--r--   0        0        0     4611 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/cx_subtitle/loader.py
+-rw-r--r--   0        0        0     5394 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.1/src/cx_subtitle/saver.py
+-rw-r--r--   0        0        0      731 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.1/src/cx_subtitle/subtitle.py
+-rw-r--r--   0        0        0     2858 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.1/src/cx_subtitle/subtitle_formatter.py
+-rw-r--r--   0        0        0       35 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/media_killer/__init__.py
+-rw-r--r--   0        0        0     1312 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.1/src/media_killer/env.py
+-rw-r--r--   0        0        0     2958 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.1/src/media_killer/example_project.toml
+-rw-r--r--   0        0        0      364 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.1/src/media_killer/exceptions.py
+-rw-r--r--   0        0        0     5453 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.1/src/media_killer/help.md
+-rw-r--r--   0        0        0     7891 2024-05-15 05:49:51.333020 cxalio_studio_tools-0.2.1/src/media_killer/media_killer_app.py
+-rw-r--r--   0        0        0     6476 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.1/src/media_killer/mission.py
+-rw-r--r--   0        0        0     1269 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.1/src/media_killer/option_package.py
+-rw-r--r--   0        0        0     3827 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.1/src/media_killer/planner.py
+-rw-r--r--   0        0        0     3318 2024-05-15 05:47:04.568947 cxalio_studio_tools-0.2.1/src/media_killer/profile_loader.py
+-rw-r--r--   0        0        0     1762 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.1/src/media_killer/script_writer.py
+-rw-r--r--   0        0        0     2793 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.1/src/media_killer/source_adapter.py
+-rw-r--r--   0        0        0     3896 2024-05-15 05:49:39.518324 cxalio_studio_tools-0.2.1/src/media_killer/transcoder.py
+-rw-r--r--   0        0        0       30 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/sub_conv/__init__.py
+-rw-r--r--   0        0        0     1132 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.1/src/sub_conv/env.py
+-rw-r--r--   0        0        0       44 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.1/src/sub_conv/exceptions.py
+-rw-r--r--   0        0        0     3316 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.1/src/sub_conv/help.md
+-rw-r--r--   0        0        0     9947 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.1/src/sub_conv/subconv_app.py
+-rw-r--r--   0        0        0     1624 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.1/src/sub_conv/subtitle_translator.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.1/src/systools/__init__.py
+-rw-r--r--   0        0        0      278 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.1/src/systools/env.py
+-rw-r--r--   0        0        0     3722 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.1/src/systools/update_githubhosts.py
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.1/PKG-INFO
```

### Comparing `cxalio_studio_tools-0.2.0/LICENSE` & `cxalio_studio_tools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/pyproject.toml` & `cxalio_studio_tools-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cxalio-studio-tools"
-version = "0.2.0"
+version = "0.2.1"
 description = "Scripts for po studio made by cxalio"
 authors = ["xiii_1991 <xiii_1991@163.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cx_core", from = "src" },
     { include = "media_killer", from = "src" },
```

### Comparing `cxalio_studio_tools-0.2.0/README.md` & `cxalio_studio_tools-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
+### 0.2.1
+
+修复了 duration 无法解析时崩溃的 bug。
+
 ### 0.2.0
 
 重新构建现有工具。
 
 #### MediaKiller
 
 - 增加了标签替换系统
```

### Comparing `cxalio_studio_tools-0.2.0/src/cx_core/abstract_env.py` & `cxalio_studio_tools-0.2.1/src/cx_core/abstract_env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_core/app_logger.py` & `cxalio_studio_tools-0.2.1/src/cx_core/app_logger.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_core/datapackage.py` & `cxalio_studio_tools-0.2.1/src/cx_core/datapackage.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_core/ffmpeg_progress_parser.py` & `cxalio_studio_tools-0.2.1/src/cx_core/ffmpeg_progress_parser.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_core/folder_expander.py` & `cxalio_studio_tools-0.2.1/src/cx_core/folder_expander.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_core/tag_replacer.py` & `cxalio_studio_tools-0.2.1/src/cx_core/tag_replacer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_core/timecode.py` & `cxalio_studio_tools-0.2.1/src/cx_core/timecode.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_core/timepoint.py` & `cxalio_studio_tools-0.2.1/src/cx_core/timepoint.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_core/utils.py` & `cxalio_studio_tools-0.2.1/src/cx_core/utils.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_subtitle/loader.py` & `cxalio_studio_tools-0.2.1/src/cx_subtitle/loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_subtitle/saver.py` & `cxalio_studio_tools-0.2.1/src/cx_subtitle/saver.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_subtitle/subtitle.py` & `cxalio_studio_tools-0.2.1/src/cx_subtitle/subtitle.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/cx_subtitle/subtitle_formatter.py` & `cxalio_studio_tools-0.2.1/src/cx_subtitle/subtitle_formatter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/env.py` & `cxalio_studio_tools-0.2.1/src/media_killer/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/example_project.toml` & `cxalio_studio_tools-0.2.1/src/media_killer/example_project.toml`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/help.md` & `cxalio_studio_tools-0.2.1/src/media_killer/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/media_killer_app.py` & `cxalio_studio_tools-0.2.1/src/media_killer/media_killer_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .planner import Planner
 from .profile_loader import ProfileLoader, ProfileNoFoundError
 from .script_writer import ScriptWriter
 from .transcoder import Transcoder
 
 
 class MediaKillerApp(AbstractApp):
-    APP_VERSION = '0.2.0'
+    APP_VERSION = '0.2.1'
     APP_NAME = 'mediakiller'
 
     def __init__(self):
         super(MediaKillerApp, self).__init__()
         self.global_task = None
 
         parser = ArgumentParser(prog=MediaKillerApp.APP_NAME, formatter_class=RichHelpFormatter,
```

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/mission.py` & `cxalio_studio_tools-0.2.1/src/media_killer/mission.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/option_package.py` & `cxalio_studio_tools-0.2.1/src/media_killer/option_package.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/planner.py` & `cxalio_studio_tools-0.2.1/src/media_killer/planner.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/profile_loader.py` & `cxalio_studio_tools-0.2.1/src/media_killer/profile_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return [x for x in str(a).split(' ')]
 
     def __check_data_package(self, package):
         env.progress.update(self.task_id, description='解析配置文件数据', completed=1, total=2)
         env.info('开始检查配置数据...')
 
         result = DataPackage(**package)
-        env.print(f'开始解析配置文件：[cyan]{result.general.name}[/cyan]\n[yellow]{result.general.description}[/yellow]')
+        env.print(f'开始解析配置文件：[cyan]{result.general.name}[/cyan]:[yellow]{result.general.description}[/yellow]')
 
         if not result.general.ffmpeg:
             result.general.ffmpeg = 'ffmpeg'
             env.print('未指定 ffmpeg ，将调用系统环境中的 ffmpeg')
 
         if not result.general.working_folder:
             env.debug('配置文件未指定工作目录')
```

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/script_writer.py` & `cxalio_studio_tools-0.2.1/src/media_killer/script_writer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/source_adapter.py` & `cxalio_studio_tools-0.2.1/src/media_killer/source_adapter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/media_killer/transcoder.py` & `cxalio_studio_tools-0.2.1/src/media_killer/transcoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def __enter__(self):
         self.task = env.progress.add_task(description=f'{self.mission.source.name}...')
 
         ffprobe = FFmpeg(executable='ffprobe').input(self.mission.source, print_format='json', show_format=None)
         media = json.loads(asyncio.run(ffprobe.execute()))
         self.media_info = DataPackage(**media)
-        self.duration = float(self.media_info.format.duration)
+        self.duration = float(self.media_info.format.duration or -1)
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         env.progress.remove_task(self.task)
         self.task = None
         env.current_ffmpeg = None
@@ -58,15 +58,15 @@
             ffmpeg.output(output_.filename.absolute(), output_.raw_data)
             env.debug(f'添加输出选项： {output_.raw_data}')
 
         env.debug(f'全部任务选项输入完毕， ffmpeg 对象构建完成')
 
         @ffmpeg.on('progress')
         def on_progress(progress: Progress):
-            desc = f'{self.mission.source.name}... [yellow]x{round(progress.speed, 2)}[/yellow]'
+            desc = '{0} [yellow]x{1:.2f}[/yellow]'.format(self.mission.source.name, progress.speed)
             curr = progress.time.seconds
             env.progress.update(self.task, description=desc, completed=curr, total=self.duration)
 
         @ffmpeg.on('stderr')
         def on_stderr(line):
             env.debug(f'[grey]FFMPEG输出：[/grey] {line}')
```

### Comparing `cxalio_studio_tools-0.2.0/src/sub_conv/env.py` & `cxalio_studio_tools-0.2.1/src/sub_conv/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/sub_conv/help.md` & `cxalio_studio_tools-0.2.1/src/sub_conv/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/sub_conv/subconv_app.py` & `cxalio_studio_tools-0.2.1/src/sub_conv/subconv_app.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/sub_conv/subtitle_translator.py` & `cxalio_studio_tools-0.2.1/src/sub_conv/subtitle_translator.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/src/systools/update_githubhosts.py` & `cxalio_studio_tools-0.2.1/src/systools/update_githubhosts.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.0/PKG-INFO` & `cxalio_studio_tools-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxalio-studio-tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Scripts for po studio made by cxalio
 Home-page: https://gitee.com/xiii_1991/cxalio-studio-tools
 License: GPL-3.0-or-later
 Keywords: ffmpeg,tool
 Author: xiii_1991
 Author-email: xiii_1991@163.com
 Requires-Python: >=3.11,<4.0
@@ -58,14 +58,18 @@
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
+### 0.2.1
+
+修复了 duration 无法解析时崩溃的 bug。
+
 ### 0.2.0
 
 重新构建现有工具。
 
 #### MediaKiller
 
 - 增加了标签替换系统
```

