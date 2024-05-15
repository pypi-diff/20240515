# Comparing `tmp/cxalio_studio_tools-0.1.9.tar.gz` & `tmp/cxalio_studio_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxalio_studio_tools-0.1.9.tar", max compression
+gzip compressed data, was "cxalio_studio_tools-0.2.0.tar", max compression
```

## Comparing `cxalio_studio_tools-0.1.9.tar` & `cxalio_studio_tools-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,44 @@
--rw-r--r--   0        0        0    35821 2023-12-06 11:01:10.654584 cxalio_studio_tools-0.1.9/LICENSE
--rw-r--r--   0        0        0     1038 2024-04-28 10:56:52.641372 cxalio_studio_tools-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      927 2024-04-28 10:56:00.485481 cxalio_studio_tools-0.1.9/README.md
--rw-r--r--   0        0        0      186 2024-04-28 10:56:00.486497 cxalio_studio_tools-0.1.9/src/cx_core/__init__.py
--rw-r--r--   0        0        0      145 2024-01-27 13:17:34.142188 cxalio_studio_tools-0.1.9/src/cx_core/abstract_app.py
--rw-r--r--   0        0        0      838 2024-01-27 12:52:22.610811 cxalio_studio_tools-0.1.9/src/cx_core/abstract_env.py
--rw-r--r--   0        0        0     1286 2024-01-27 17:09:17.423551 cxalio_studio_tools-0.1.9/src/cx_core/app_logger.py
--rw-r--r--   0        0        0     2024 2024-01-27 13:17:34.143187 cxalio_studio_tools-0.1.9/src/cx_core/datapackage.py
--rw-r--r--   0        0        0     1826 2024-01-27 12:52:22.611806 cxalio_studio_tools-0.1.9/src/cx_core/ffmpeg_progress_parser.py
--rw-r--r--   0        0        0     1462 2024-01-27 12:52:22.612805 cxalio_studio_tools-0.1.9/src/cx_core/folder_expander.py
--rw-r--r--   0        0        0      465 2024-04-28 10:56:00.486497 cxalio_studio_tools-0.1.9/src/cx_core/osinfo.py
--rw-r--r--   0        0        0     2991 2024-02-05 14:10:41.883203 cxalio_studio_tools-0.1.9/src/cx_core/timecode.py
--rw-r--r--   0        0        0     1640 2024-02-05 14:10:41.883203 cxalio_studio_tools-0.1.9/src/cx_core/timepoint.py
--rw-r--r--   0        0        0      466 2024-03-06 11:11:33.875444 cxalio_studio_tools-0.1.9/src/cx_core/tui_elements.py
--rw-r--r--   0        0        0      956 2024-01-27 13:17:34.143187 cxalio_studio_tools-0.1.9/src/cx_core/utils.py
--rw-r--r--   0        0        0       83 2024-02-05 14:10:41.884204 cxalio_studio_tools-0.1.9/src/cx_subtitle/__init__.py
--rw-r--r--   0        0        0     4611 2024-02-05 14:10:41.884204 cxalio_studio_tools-0.1.9/src/cx_subtitle/loader.py
--rw-r--r--   0        0        0     4579 2024-02-05 14:10:41.885202 cxalio_studio_tools-0.1.9/src/cx_subtitle/saver.py
--rw-r--r--   0        0        0      482 2024-02-05 14:10:41.885202 cxalio_studio_tools-0.1.9/src/cx_subtitle/subtitle.py
--rw-r--r--   0        0        0     3271 2024-02-05 14:10:41.885202 cxalio_studio_tools-0.1.9/src/cx_subtitle/subtitle_formatter.py
--rw-r--r--   0        0        0       35 2024-01-27 12:52:22.618965 cxalio_studio_tools-0.1.9/src/media_killer/__init__.py
--rw-r--r--   0        0        0     1377 2024-03-06 11:11:33.876366 cxalio_studio_tools-0.1.9/src/media_killer/env.py
--rw-r--r--   0        0        0     1840 2024-01-27 13:17:34.144189 cxalio_studio_tools-0.1.9/src/media_killer/example_project.toml
--rw-r--r--   0        0        0     4004 2024-04-28 10:56:00.487502 cxalio_studio_tools-0.1.9/src/media_killer/help.md
--rw-r--r--   0        0        0     7178 2024-04-28 10:56:00.487502 cxalio_studio_tools-0.1.9/src/media_killer/media_killer_app.py
--rw-r--r--   0        0        0     3719 2024-01-27 17:09:17.424592 cxalio_studio_tools-0.1.9/src/media_killer/planner.py
--rw-r--r--   0        0        0     5006 2024-04-28 10:56:00.488481 cxalio_studio_tools-0.1.9/src/media_killer/profile_loader.py
--rw-r--r--   0        0        0     2382 2024-01-27 13:17:34.146188 cxalio_studio_tools-0.1.9/src/media_killer/script_writer.py
--rw-r--r--   0        0        0     2791 2024-01-27 13:17:34.146188 cxalio_studio_tools-0.1.9/src/media_killer/source_adapter.py
--rw-r--r--   0        0        0     3773 2024-03-06 11:11:33.877362 cxalio_studio_tools-0.1.9/src/media_killer/transcoder.py
--rw-r--r--   0        0        0       30 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.9/src/sub_conv/__init__.py
--rw-r--r--   0        0        0      278 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.9/src/sub_conv/env.py
--rw-r--r--   0        0        0       44 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.9/src/sub_conv/exceptions.py
--rw-r--r--   0        0        0     2937 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.9/src/sub_conv/help.md
--rw-r--r--   0        0        0     7432 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.9/src/sub_conv/subconv_app.py
--rw-r--r--   0        0        0        0 2024-04-28 10:56:00.488481 cxalio_studio_tools-0.1.9/src/systools/__init__.py
--rw-r--r--   0        0        0      278 2024-04-28 10:56:00.489483 cxalio_studio_tools-0.1.9/src/systools/env.py
--rw-r--r--   0        0        0     3715 2024-04-28 10:56:00.489483 cxalio_studio_tools-0.1.9/src/systools/update_githubhosts.py
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-16 07:18:25.822233 cxalio_studio_tools-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1064 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1204 2024-05-15 04:56:11.309783 cxalio_studio_tools-0.2.0/README.md
+-rw-r--r--   0        0        0      188 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.0/src/cx_core/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/abstract_app.py
+-rw-r--r--   0        0        0      838 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/abstract_env.py
+-rw-r--r--   0        0        0     1286 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/app_logger.py
+-rw-r--r--   0        0        0     2024 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/datapackage.py
+-rw-r--r--   0        0        0     1826 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/ffmpeg_progress_parser.py
+-rw-r--r--   0        0        0     1462 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/folder_expander.py
+-rw-r--r--   0        0        0      465 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.0/src/cx_core/osinfo.py
+-rw-r--r--   0        0        0     1421 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.0/src/cx_core/tag_replacer.py
+-rw-r--r--   0        0        0     2991 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/timecode.py
+-rw-r--r--   0        0        0     1640 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_core/timepoint.py
+-rw-r--r--   0        0        0      466 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.0/src/cx_core/tui_elements.py
+-rw-r--r--   0        0        0     2813 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.0/src/cx_core/utils.py
+-rw-r--r--   0        0        0      101 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.0/src/cx_subtitle/__init__.py
+-rw-r--r--   0        0        0     4611 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/cx_subtitle/loader.py
+-rw-r--r--   0        0        0     5394 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.0/src/cx_subtitle/saver.py
+-rw-r--r--   0        0        0      731 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.0/src/cx_subtitle/subtitle.py
+-rw-r--r--   0        0        0     2858 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.0/src/cx_subtitle/subtitle_formatter.py
+-rw-r--r--   0        0        0       35 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/media_killer/__init__.py
+-rw-r--r--   0        0        0     1312 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.0/src/media_killer/env.py
+-rw-r--r--   0        0        0     2958 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.0/src/media_killer/example_project.toml
+-rw-r--r--   0        0        0      364 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.0/src/media_killer/exceptions.py
+-rw-r--r--   0        0        0     5453 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.0/src/media_killer/help.md
+-rw-r--r--   0        0        0     7891 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.0/src/media_killer/media_killer_app.py
+-rw-r--r--   0        0        0     6476 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.0/src/media_killer/mission.py
+-rw-r--r--   0        0        0     1269 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.0/src/media_killer/option_package.py
+-rw-r--r--   0        0        0     3827 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.0/src/media_killer/planner.py
+-rw-r--r--   0        0        0     3319 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.0/src/media_killer/profile_loader.py
+-rw-r--r--   0        0        0     1762 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.0/src/media_killer/script_writer.py
+-rw-r--r--   0        0        0     2793 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.0/src/media_killer/source_adapter.py
+-rw-r--r--   0        0        0     3887 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.0/src/media_killer/transcoder.py
+-rw-r--r--   0        0        0       30 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/sub_conv/__init__.py
+-rw-r--r--   0        0        0     1132 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/sub_conv/env.py
+-rw-r--r--   0        0        0       44 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.0/src/sub_conv/exceptions.py
+-rw-r--r--   0        0        0     3316 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/sub_conv/help.md
+-rw-r--r--   0        0        0     9947 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/sub_conv/subconv_app.py
+-rw-r--r--   0        0        0     1624 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/sub_conv/subtitle_translator.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.0/src/systools/__init__.py
+-rw-r--r--   0        0        0      278 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.0/src/systools/env.py
+-rw-r--r--   0        0        0     3722 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.0/src/systools/update_githubhosts.py
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.0/PKG-INFO
```

### Comparing `cxalio_studio_tools-0.1.9/LICENSE` & `cxalio_studio_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.9/pyproject.toml` & `cxalio_studio_tools-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "cxalio-studio-tools"
-version = "0.1.9"
+version = "0.2.0"
 description = "Scripts for po studio made by cxalio"
 authors = ["xiii_1991 <xiii_1991@163.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cx_core", from = "src" },
     { include = "media_killer", from = "src" },
     { include = "cx_subtitle", from = "src" },
     { include = "sub_conv", from = "src" },
-    { include = "systools", from = "src"}
+    { include = "systools", from = "src" },
 ]
 
 repository = "https://gitee.com/xiii_1991/cxalio-studio-tools.git"
 homepage = "https://gitee.com/xiii_1991/cxalio-studio-tools"
 keywords = ["ffmpeg", "tool"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 rich = "^13.7.0"
 chardet = "^5.2.0"
 rich-argparse = '^1.4.0'
 python-ffmpeg = "^2.0.10"
 python-docx = "^1.1.0"
 openpyxl = "^3.1.2"
+translators = "^5.9.2"
 
 [tool.poetry.scripts]
 mediakiller = 'media_killer:run'
 subconv = 'sub_conv:run'
 update_githubhosts = 'systools.update_githubhosts:run'
 
 [build-system]
```

### Comparing `cxalio_studio_tools-0.1.9/src/cx_core/abstract_env.py` & `cxalio_studio_tools-0.2.0/src/cx_core/abstract_env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.9/src/cx_core/app_logger.py` & `cxalio_studio_tools-0.2.0/src/cx_core/app_logger.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.9/src/cx_core/datapackage.py` & `cxalio_studio_tools-0.2.0/src/cx_core/datapackage.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.9/src/cx_core/ffmpeg_progress_parser.py` & `cxalio_studio_tools-0.2.0/src/cx_core/ffmpeg_progress_parser.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.9/src/cx_core/folder_expander.py` & `cxalio_studio_tools-0.2.0/src/cx_core/folder_expander.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.9/src/cx_core/timecode.py` & `cxalio_studio_tools-0.2.0/src/cx_core/timecode.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.9/src/cx_core/timepoint.py` & `cxalio_studio_tools-0.2.0/src/cx_core/timepoint.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.9/src/cx_subtitle/loader.py` & `cxalio_studio_tools-0.2.0/src/cx_subtitle/loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.9/src/cx_subtitle/subtitle_formatter.py` & `cxalio_studio_tools-0.2.0/src/cx_subtitle/subtitle_formatter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 
-from .subtitle import Subtitle
+from .subtitle import Subtitle,SubtitleProcessor
 
 
-class SubtitleFormatter:
+class SubtitleFormatter(SubtitleProcessor):
     def __init__(self, **kwargs):
+        super(SubtitleFormatter,self).__init__()
         self.replacements = {'\t': ' '}
         self.remove_tags = True
 
         self.normal_strip = True
         self.strip_quotes = True
         self.extra_strips = ''
 
@@ -63,39 +64,29 @@
         return result
 
     @staticmethod
     def __shrink_long_quotes(content: str):
         result = re.sub(r'([\'\"‘“”’])+', r'\1', content)
         return result
 
-    def format_subtitle(self, subtitle: Subtitle):
+    def __call__(self, subtitle: Subtitle):
         content = self.__basic_content_cleaning(subtitle.content)
         content = self.__strip(content)
         if self.remove_tags:
             content = self.__remove_tags(content)
         if self.remove_empty_lines:
             content = self.__remove_empty_lines(content)
         if self.shrink_long_spaces:
             content = self.__shrink_long_spaces(content)
         if self.shrink_long_quotes:
             content = self.__shrink_long_quotes(content)
-        subtitle.content = content
-        return subtitle
+        return subtitle.with_content(content)
 
     def is_subtitle_legal(self, subtitle: Subtitle):
         if self.remove_empty_subtitles and not subtitle.content:
             return False
         if self.remove_zero_duration_subtitles and subtitle.duration == 0:
             return False
         return True
 
-    def format_sequence(self, subtitles: list[Subtitle]):
-        result = [self.format_subtitle(sub) for sub in subtitles if self.is_subtitle_legal(sub)]
-        result = sorted(result, key=lambda x: x.start)
-        return result
 
-    def __call__(self, sth: Subtitle | list[Subtitle]):
-        if isinstance(sth, list):
-            return self.format_sequence(sth)
-        elif isinstance(sth, Subtitle):
-            return self.format_subtitle(sth)
-        return sth
+
```

### Comparing `cxalio_studio_tools-0.1.9/src/media_killer/env.py` & `cxalio_studio_tools-0.2.0/src/media_killer/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import signal
-import asyncio
 
-from rich.progress import Progress, SpinnerColumn, MofNCompleteColumn
+from rich.progress import Progress, SpinnerColumn
 
-from cx_core import AppLogger, AbstractEnv, LogLevel, DataPackage
+from cx_core import AppLogger, AbstractEnv, LogLevel
 
 
 class Env(AbstractEnv):
     def __init__(self):
-        super(Env,self).__init__()
+        super(Env, self).__init__()
         self._progress = Progress(
             SpinnerColumn(),
             # MofNCompleteColumn(),
             *Progress.get_default_columns(),
             expand=True,
             transient=True)
 
         self._logger = AppLogger(console=self._progress.console)
         self._logger.level = LogLevel.WARNING
 
         self.args = None
-        self.profile = DataPackage()
 
         self.current_ffmpeg = None
         self.wanna_quit = False
 
     def start(self):
         self._progress.start()
-        self.info('Started ...')
+        self.info('全局环境已启动')
 
     def stop(self):
         self._progress.stop()
         self.info('Bye~')
 
     @property
     def progress(self):
@@ -45,14 +43,14 @@
 env = Env()
 
 
 def signal_handler(sig, frame):
     if sig != signal.SIGINT:
         return
     env.info('接收到 SIGINT')
-    env.print("收到终止信号，准备退出...")
+    env.print("[red]收到终止信号，准备退出...[/red]")
     env.wanna_quit = True
     if env.current_ffmpeg:
         env.current_ffmpeg.terminate()
 
 
 signal.signal(signal.SIGINT, signal_handler)
```

### Comparing `cxalio_studio_tools-0.1.9/src/media_killer/example_project.toml` & `cxalio_studio_tools-0.2.0/src/media_killer/example_project.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,84 @@
 [general] # 通用选项
 
 # 使用 name 制定当前配置文件的名称，只是用来区分而已
 name = "example-profile"
 description = "示例配置，请勿直接使用"
 
-# 制定工作目录，如果不指定的话则会设置为此文件所在的目录
-# working_folder = "."
+# 设置调用的ffmpeg
+# 如果不指定，则使用系统环境中的 ffmpeg
+ffmpeg = 'ffmpeg'
+
+# 设置工作目录，如果不指定的话则会设置为此文件所在的目录
+# 如果使用的是相对路径，也会以此文件的所在位置为基准位置
+working_folder = "."
 
 # 指定硬件解码方式，如果不指定则使用软件解码
 hardware_accelerate = "auto"
 
 # 输出时覆盖目标文件，默认值为 false
 overwrite_existed = true
 
 # 指定全局参数,可使用多种样式
-options = ["-hide_banner"]
+options = "-hide_banner"
 
 
-[input] # 来源设置
+[source] # 来源设置
 
 # source.files 指定源文件列表，每项一个文件，建议使用绝对路径。
 # 源文件如果是 txt、csv 或 xml 文件，将会作为文件列表读取
 # 否则直接作为源文件添加进入任务列表
 # 如果指定的路径是一个目录，运行时将会自动展开
-files = ["a.txt", "b.csv", "c.fcpxml", "d.xml"]
+# 如果不指定此选项，则不会运行任何任务，但是可以在执行命令中指定来源
+# 所以不指定此选项的配置文件可以作为一个通用的配置文件
+# files = ["a.txt", "b.csv", "c.fcpxml", "d.xml"]
+files = []
 
 # 使用扩展名过滤来源文件
 # 黑名单和白名单会分别用于对内置的常用名单进行修正
 # 黑名单优先级更高
-# 别动这个选项如果你不明白自己在做什么
+# 如果你不明白自己在做什么，不要设置这些选项
 # 这两个属性同时支持字符串列表或空格分割的字符串
 suffix_includes = []
 suffix_excludes = []
 
-# 可以指定针对每个输入文件的选项
-# 但是目前可能没有什么用
-# options=''
+[target] # 目标设置
+# 程序将根据这些选项构建默认的目标路径
 
+# 指定输出文件的扩展名
+suffix = "mov"
+
+# 指定输出目录，建议使用绝对路径，如果是相对路径，则会相对于工作目录进行识别
+folder = "转码结果"
+
+# 输出时保留源文件上级目录的层级，0 为不保留，1 为保留一级
+keep_parent_level = 1
+
+[[input]] # 输入设置
 
-[output] # 目标设置
+# 输入和输出设置都是数组表
+# 你可以指定多组输入和输出，并在其中应用预置tag调用信息
+
+# 设置输入的文件，下面展示的是默认的
+# 你也可以通过标签选项设置其它的文件输入
+# 但是通常保持有一个输入为默认的输入
+# 如果你不懂，不要胡乱设置这个选项
+filename = '{source:absolute}'
+
+# 设置此输入的前置选项，用法参考 output 中的说明
+options = ''
+
+[[output]] # 目标设置
+
+# 手动指定输出文件模板
+# 多输出的时候可愚蠢用于指定不同的输出目标
+# target标签会基于前面的选项生成，所以如果你不懂的话，不要胡乱设置这个选项
+filename = '{target:absolute}'
 
 # 指定选项,可以使用多种格式
 #options = { "c:v" = "copy", "c:a" = "copy" }
 #options = ["-c:v", "copy", "-c:a", "copy"]
 options = "-c:v copy -c:a copy"
 
-# 指定输出文件的扩展名
-suffix = "mov"
 
-# 指定输出目录，建议使用绝对路径，如果是相对路径，则会相对于工作目录进行识别
-folder = "转码结果"
 
-# 输出时保留源文件上级目录的层级，0 为不保留，1 为保留一级
-keep_parent_level = 1
+
```

### Comparing `cxalio_studio_tools-0.1.9/src/media_killer/help.md` & `cxalio_studio_tools-0.2.0/src/media_killer/help.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,119 +1,165 @@
-# media-killer
-version=0.1.7
+# MediaKiller
 
-media-killer 可以通过配置文件操纵 ffmpeg 批量地对大量媒体文件转码。
+当前版本 0.2.0
 
->media-killer 并不能作为 ffmpeg 的替代。
+MediaKiller 可以通过配置文件操纵 ffmpeg 批量地对大量媒体文件转码。
 
-和直接使用 ffmpeg 相比， media-killer 有如下优缺点：
+> MediaKiller 并不能作为 ffmpeg 的替代。
+
+和直接使用 ffmpeg 相比， MediaKiller 有如下优缺点：
 
 - 可以进行大量视频批量处理
-- 使用**可复用的配置文件**进行操作管理
-- 每个转码任务**仅支持**单个文件输入和单个目标输出
+- 使用 **可复用的配置文件** 进行操作管理
+- 每个转码任务可以通过文本模板的形式支持多文件输入和多文件输出
 - 可以通过指定文件夹作为源文件的方式来批量添加任务
 - 可以根据源文件路径保留指定层级的上层目录结构
-- 可以读取 xml、fcpxml、csv等文件中提供的源文件信息
+- 可以读取`xml`、`fcpxml`、`csv`等文件中提供的源文件信息
 - 拥有漂亮的进度监控和提示信息
-- 无法指定输出的文件名（但可以指定扩展名）
 
-#### 配置文件
+## 配置文件
 
-media-killer 使用 toml 配置文件描述工作内容。
+MediaKiller 使用`toml配置文件`描述工作内容。
 
 使用配置文件可以方便地复用设置，
 你可以保存多个不同的配置文件，并在将来对不同的视频文件进行同样的操作；
 或者是在源文件修改后，一键重新运行转码任务，以快速更新目标文件。
 
 使用 `--generate` 选项生成一个示例文件：
 
 ```shell
-media-killer '文件名.toml' --generate
+mediakiller '文件名.toml' --generate
 # 或
-media-killer '文件名.toml' -g
+mediakiller '文件名.toml' -g
 ```
 
-在示例文件中包含所有选项的说明。
+> 在示例文件中包含所有选项的说明。
 
-#### 执行任务
+## 执行任务
 
 不加任何选项地，指定配置文件，即可执行任务。
 
+但是如果配置文件中未设置源文件，则仍需要使用`-a`选项添加任务，详情见下一章节。
+
 ```shell
-media-killer '文件名.toml'
+mediakiller '配置文件.toml'
+mediakiller '配置文件.toml' -a '需要转码的文件.mp4'
 ```
 
-#### 来源文件设置
+## 来源文件设置
+
+一种可能的情况是：配置文件中仅仅制定了转码选项和目标位置。
+（事实上这也是推荐的使用方式。）
 
-一种可能的情况是，配置文件中仅仅制定了转码选项和目标位置。
 这种情况下可以使用 `--add-source` 添加源文件，
 这种情况下增加的源文件会附加在配置文件中指定的源文件列表之后。
 
 例如，在配置文件 `example.toml` 中有如下设置：
 
 ```toml
+# example.toml
 [input]
 files = ['a.mov', 'b.mov', 'c.mov']
 ```
 
 那么运行下面的命令之后——
 
 ```shell
-media-killer 'example.toml' --add-source 'one.mp4' -a 'two.mp4'
+mediakiller 'example.toml' --add-source 'one.mp4' -a 'two.mp4'
 # -a 是 --add-source 的缩写
 ```
 
-—— media-killer 将会处理全部 5 个目标文件。
+—— MediaKiller 将会处理全部 5 个目标文件。
 
 所以，如果不在配置文件中制定源文件可以最大程度重复使用它们。
 
-#### 来源文件的解析
+> 注意：`--add-source`选项只能指定一个来源项目，
+> 但是你可以多次使用它，或直接指定一个文件夹。
+> 这样就可以添加多个源文件了。
 
-在使用来源文件之前将会进行一系列处理：
+## 来源文件的解析
 
-1. 遍历每一个`input.file`：
+在使用来源文件之前，MediaKiller 将会进行一系列处理：
+
+1. 将`--add-source`指定的文件项目添加到从`配置文件`中解析的来源文件列表之后。
+   此列表将会被存储为`input.file`。
+
+2. 遍历`input.file`中的每一项：
     - 若：文件扩展名是被支持的**列表文件**,
+
       则：读取其中包含的片段信息，并将它们添加到`源文件列表`
-    - 若：不是列表文件，则：直接添加到`源文件列表`
-2. 初始化`扩展名列表`，
-   将`配置文件`中的`input.suffix_includes`添加到`扩展名列表`，
-   将`配置文件`中的`input.suffix_excludes`中包含的项目从`扩展名列表`中移除
-3. 遍历`源文件列表`，并将所有的文件夹递归地展开，
+
+    - 若：不是列表文件，
+
+      则：直接添加到`源文件列表`
+
+3. 初始化`扩展名列表`，
+    - 将`配置文件`中的`input.suffix_includes`添加到`扩展名列表`，
+    - 将`配置文件`中的`input.suffix_excludes`中包含的项目从`扩展名列表`中移除
+
+4. 遍历`源文件列表`，并将所有的文件夹递归地展开，
    并将扩展名符合`扩展名列表`的文件添加到`源文件列表`
-4. 根据路径排序`源文件列表`
-5. 检查`源文件列表`，去除重复的或不存在的文件
+
+5. 根据路径排序`源文件列表`
+
+6. 检查`源文件列表`，去除重复的或不存在的文件
 
 之后才会根据`配置文件`的设置，依次处理来源文件。
 
-#### 相对路径
+## 相对路径 vs 绝对路径
 
 在配置文件中，所有的文件都可以使用相对路径指定，
 但是相对路径并非相对于当前的工作目录的，
 而是相对于`general.working_folder`所设定的目录，
 此目录默认为配置文件所在的目录。
 
 ```toml
 [general]
 working_folder = '.'
 ```
 
-这允许使用拷贝配置文件，并将它 "make" 为目标文件的使用逻辑成为可能。
+这允许将配置文件拷贝至不同位置后，
+作为一个 *make* 文件展开成为目标文件的用法成为可能。
 
-#### 生成 shell 脚本
+## 生成可执行脚本
 
-如果制定了`--make-script`选项，
-media-killer 不会自动转码，而是会生成一个脚本文件。
+如果指定了`--make-script`选项，
+MediaKiller 不会自动转码，而是会生成一个脚本文件。
 当然，**必须指定脚本文件的保存位置**。
 
+你可以使用任何手段对脚本文件进行编辑，
+也可以将脚本文件复制到没有安装 MediaKiller 的环境中运行。
+
 ```shell
-media-killer 'example.toml' -s 'script.sh'
+mediakiller 'example.toml' --make-script 'script.sh'
+# 或
+mediakiller 'example.toml' -s 'script.ps1'
 # -s 是 --make-script 的缩写
 ```
 
-生成的脚本文件仅仅是普通的文本文件而已，**不包含 shebang**，
+生成的脚本文件仅仅是普通的文本文件而已，
+既**不包含 shebang**，也**没有运行权限**。
 所以运行时你需要自己指定使用的 shell：
 
 ```shell
-media-killer 'example.toml' --make-script 'script.ps1'
+media 'example.toml' --make-script 'script.ps1'
 pwsh 'script.ps1'
 ```
 
+## 调试与测试
+
+MediaKiller 包含 2 个选项用于调试和测试目的。
+
+- `--pretend` `-p` 选项通知 MediaKiller 进入模拟运行状态。
+
+  此状态下会正常运行所有功能，但是并不会运行 ffmpeg 进行转码。
+  但是`--make-script`选项仍然会正常输出脚本。
+
+- `--debug` `-d` 选项为 MediaKiller 开启调试模式。
+
+调试模式下将会启用大量的运行细节输出，便于查找到底出了什么问题。
+
+-----
+项目主页: https://gitee.com/xiii_1991/cxalio-studio-tools
+
+作者: xiii_1991@163.com
+
```

### Comparing `cxalio_studio_tools-0.1.9/src/media_killer/media_killer_app.py` & `cxalio_studio_tools-0.2.0/src/media_killer/media_killer_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,86 +6,95 @@
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich_argparse import RichHelpFormatter
 
 from cx_core import AbstractApp
 from cx_core import DataPackage
 from cx_core.app_logger import LogLevel
+from cx_core.tui_elements import JobCounter
 from cx_core.utils import normalize_path
 from .env import env
+from .mission import MissionMaker
 from .planner import Planner
 from .profile_loader import ProfileLoader, ProfileNoFoundError
 from .script_writer import ScriptWriter
 from .transcoder import Transcoder
 
-from cx_core.tui_elements import JobCounter
-
 
 class MediaKillerApp(AbstractApp):
+    APP_VERSION = '0.2.0'
+    APP_NAME = 'mediakiller'
+
     def __init__(self):
-        super(MediaKillerApp,self).__init__()
+        super(MediaKillerApp, self).__init__()
         self.global_task = None
-        self.app_name = 'media-killer'
-        self.app_version = '0.1.8'
-        parser = ArgumentParser(prog=self.app_name, formatter_class=RichHelpFormatter,
-                                description='简单批量转码工具', epilog='Designed by xiii_1991')
+
+        parser = ArgumentParser(prog=MediaKillerApp.APP_NAME, formatter_class=RichHelpFormatter,
+                                description='基于配置文件的批量转码工具',
+                                epilog=f'Version {MediaKillerApp.APP_VERSION} Designed by xiii_1991')
         parser.add_argument('profile', help='指定配置文件路径', default=None, nargs='?')
         parser.add_argument('-g', '--generate-example-profile',
                             action="store_true", dest='generate_example',
                             help='生成范例文件')
         parser.add_argument('-a', '--add-source',
                             action='append', dest='sources', metavar='SOURCE_FILE',
                             help='增加来源文件')
         parser.add_argument('-s', '--make-script',
                             dest='script_output', metavar='SCRIPT_OUTPUT',
                             help='生成对应的脚本文件')
         parser.add_argument('-d', '--debug',
                             action='store_true', dest='debug', help='显示调试信息')
-        parser.add_argument('--dry-run',
-                            dest='dry_run', action='store_true', help='空转模式，不执行命令')
-        parser.add_argument('--man', help='显示详细的说明',
-                            dest='show_man', action='store_true')
-        parser.add_argument('-v', '--version', action='version', version=self.app_version,
+        parser.add_argument('--pretend', '-p',
+                            dest='pretend_mode', action='store_true', help='空转模式，不执行命令')
+        parser.add_argument('--full-help', help='显示详细的说明',
+                            dest='full_help', action='store_true')
+        parser.add_argument('-v', '--version', action='version', version=MediaKillerApp.APP_VERSION,
                             help='显示软件版本信息')
+        self.profile = None
         self._parser = parser
         self.args = None
 
     @staticmethod
-    def show_man():
+    def show_full_help():
+        """显示完整的说明文件"""
         data = pkgutil.get_data('media_killer', 'help.md').decode('utf_8')
-        env.console.print(Markdown(data))
+        panel = Panel(Markdown(data), width=80)
+        env.console.print(panel)
 
     @staticmethod
     def copy_example_profile(tgt):
         tgt = normalize_path(tgt)
         data = pkgutil.get_data('media_killer', 'example_project.toml')
         try:
             with open(tgt, 'xb') as file:
                 file.write(data)
-            env.print(f'模板配置文件已保存到 {env.args.profile} ，[red]请勿直接加载运行！[/red]')
+            env.print(f'模板配置文件已保存到 {env.args.profile} ，[red]请在修改后运行！[/red]')
         except FileExistsError:
-            env.error('文件 {0} 已存在，禁止覆盖文件'.format(tgt))
+            env.error('文件 {0} 已存在，[red]请手动删除它，或指定其它的目标文件[/red]'.format(tgt))
 
     def __enter__(self):
         env.start()
+        env.debug('env 环境已启动')
 
         _args = self._parser.parse_args()
         self.args = DataPackage(**vars(_args))
-
         env.debug('解析命令行参数：', self.args)
+
         env.log_level = LogLevel.DEBUG if self.args.debug else LogLevel.WARNING
         env.args = self.args
 
         self.global_task = env.progress.add_task(description='全局进度', start=False, visible=False)
+        env.debug('构建全局进度条')
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         env.progress.stop_task(self.global_task)
         env.progress.remove_task(self.global_task)
         self.global_task = None
+        env.debug('删除全局进度条')
 
         result = False
         if exc_type is None:
             pass
         elif issubclass(exc_type, ProfileNoFoundError):
             env.critical(exc_val)
             result = True
@@ -93,78 +102,82 @@
             env.error('参数输入有误:', exc_val)
             result = True
 
         env.stop()
         return result
 
     def run(self):
-        if env.args.show_man:
-            MediaKillerApp.show_man()
+        if env.args.full_help:
+            env.info('检测到 full_help 设置，打印帮助文件并退出')
+            MediaKillerApp.show_full_help()
             return
 
         if not env.args.profile:
+            env.info('未检测到项目文件选项')
             raise ProfileNoFoundError
 
         if env.args.generate_example:
-            env.debug('检测到 "--generate-example" 参数，拷贝配置文件模板')
+            env.info('检测到 "--generate-example" 参数，将拷贝配置文件模板')
             env.progress.update(task_id=self.global_task, description='正在输出配置文件', visible=True)
             self.copy_example_profile(env.args.profile)
             return
 
-        with ProfileLoader() as profile_loader:
-            datas = profile_loader.load(env.args.profile)
-            env.profile = datas
+        with ProfileLoader(env.args.profile) as profile_loader:
+            datas = profile_loader.load()
+            self.profile = datas
         env.info('配置信息已初始化')
 
-        if not env.profile.input.files:
-            env.error('未指定任何来源信息，无事可做')
+        if not self.profile.source.files:
+            env.error('[red]未指定任何来源信息，无事可做[/red]')
             return
 
-        planner = Planner()
+        planner = Planner(self.profile)
         env.progress.update(task_id=self.global_task, description='正在将来源信息加入计划', visible=True)
-        planner.load_sources(env.profile.input.files)
+        planner.load_sources(self.profile.source.files)
         env.info('已发现 {0} 项来源'.format(len(planner)))
 
         env.progress.update(task_id=self.global_task, description='正在整理来源信息', visible=True)
-        planner.arrange(env.profile)
+        planner.arrange()
         env.print(f'整理结束，已添加 {len(planner)} 项计划')
         if env.args.debug:
             col = Columns(
-                (Panel(Path(x).name, style='yellow', border_style='green', safe_box=True,
+                (Panel(Path(str(x)).name, style='yellow', border_style='green', safe_box=True,
                        title=f'#{i}', title_align='left')
                  for i, x in enumerate(planner)),
                 expand=True, equal=False, column_first=True
             )
             env.debug(col)
 
+        env.debug('构建 mission maker')
+        missions = MissionMaker(self.profile)
+
         if env.args.script_output is not None:
             env.progress.update(task_id=self.global_task, description='输出脚本文件', visible=True)
-            env.debug('检测到 "--script" 参数，进行脚本输出')
+            env.info('检测到 "--make-script" 参数，将进行脚本输出')
             output_file = normalize_path(env.args.script_output)
-            with ScriptWriter(output_file, env.profile) as writer:
-                for plan in env.progress.track(planner, description=env.args.script_output):
-                    writer.write(plan)
-            env.print('已输出脚本文件 “{0}”'.format(env.args.script_output))
+            with ScriptWriter(output_file) as writer:
+                for mission in env.progress.track(missions(planner.plans), description=env.args.script_output):
+                    writer.write_mission(mission)
+            env.print(f'已输出脚本文件 "{env.args.script_output}"')
             return
 
         env.progress.update(self.global_task, description='总体进度', visible=True, total=len(planner))
         env.progress.start_task(self.global_task)
 
         job_counter = JobCounter(len(planner))
-        for plan in planner:
+        for mission in missions(planner):
             job_counter.advance()
             if env.wanna_quit:
-                env.print('用户申请终止运行，取消未完成的任务')
+                env.print('正在取消未完成的任务...')
                 break
-            if env.args.dry_run:
-                env.print(plan)
+            if env.args.pretend_mode:
+                env.print(f'模拟运行: [yellow]{mission.source.name}[/yellow] 完毕')
             else:
-                with Transcoder(plan, env.profile) as coder:
+                with Transcoder(mission) as coder:
                     coder.run()
             env.progress.advance(self.global_task)
-            env.print(f'[yellow]{job_counter}[/yellow] "{Path(plan).name}" [blue]...[/blue] FINISHED')
-        env.print('任务执行结束')
+            env.print(f'[yellow]{job_counter}[/yellow] [cyan]{mission.source.name}[/cyan] 转换完成')
 
 
 def run():
     with MediaKillerApp() as media_killer:
         media_killer.run()
```

### Comparing `cxalio_studio_tools-0.1.9/src/media_killer/planner.py` & `cxalio_studio_tools-0.2.0/src/media_killer/planner.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 
 from cx_core.folder_expander import FolderExpander
 from .env import env
 from .source_adapter import adapters
 
 
 class Planner:
-    _DEFAULT_SUFFIXES = ("mov mkv mp4 flv 3gp 3gpp rmvb mp3 aac"
-                         " mxf mxf_op1a vob wmv wma srt ass aas ttml ogg oga ogv m4a"
-                         " m4v 3g2 mpeg mpg ts lrc h264 flac ast asf gif")
+    DEFAULT_SUFFIXES = ("mov mkv mp4 flv 3gp 3gpp rmvb mp3 aac"
+                        " mxf mxf_op1a vob wmv wma srt ass aas ttml ogg oga ogv m4a"
+                        " m4v 3g2 mpeg mpg ts lrc h264 flac ast asf gif")
 
-    def __init__(self):
+    def __init__(self, profile):
         self._loaded_file = set()
         self.plans = []
-        env.debug('Planner 初始化')
+        self.profile = profile
+        env.debug('初始化任务调度器')
 
     def __len__(self):
         return len(self.plans)
 
     def __iter__(self):
         return self.plans.__iter__()
 
     def load_source(self, filename):
         source = Path(filename)
         if not source.is_absolute():
-            source = env.profile.general.working_folder / source
+            source = self.profile.general.working_folder / source
         suffix = source.suffix.lower().strip('.')
         env.debug(f'文件 "{source}" 的扩展名为 "{suffix}"')
         if suffix in adapters:
             env.debug(f'已识别 "{source}" 为列表文件')
             try:
                 with adapters[suffix](source) as adp:
                     for item in adp.items():
@@ -47,30 +48,31 @@
 
     def load_sources(self, filenames):
         task = env.progress.add_task(description='读取来源文件...')
         for f in env.progress.track(filenames, task_id=task):
             self.load_source(f)
         env.progress.remove_task(task)
 
-    def arrange(self, profile=None):
-        if not profile:
-            profile = env.profile
+    def make_suffix_whitelist(self):
+        env.debug('开始构建扩展名白名单')
+        _basic_suffixes = {str(x).strip('.') for x in
+                           itertools.chain(Planner.DEFAULT_SUFFIXES.split(), self.profile.source.suffix_includes)}
+        _blacklist = {str(x).strip('.') for x in self.profile.source.suffix_excludes}
+        w_list = _basic_suffixes - _blacklist
+        env.debug(f'生成扩展名白名单 [cyan]{" ".join(w_list)}[/cyan]')
+        return w_list
 
+    def arrange(self):
         env.info('开始整理计划列表')
 
         env.debug('构建 Expander ...')
         expander = FolderExpander()
-        expander.working_directory = profile.general.work_folder
+        expander.working_directory = self.profile.general.working_folder
 
-        env.debug('构建扩展名白名单')
-        _basic_suffixes = {str(x).strip('.') for x in
-                           itertools.chain(Planner._DEFAULT_SUFFIXES.split(), profile.input.suffix_includes)}
-        _blacklist = {str(x).strip('.') for x in profile.input.suffix_excludes}
-        w_list = _basic_suffixes - _blacklist
-        env.debug('生成扩展名白名单 [cyan]{" ".join(w_list)}[/cyan]')
+        w_list = self.make_suffix_whitelist()
         expander.suffixes_whitelist = ['.' + x for x in w_list]
 
         env.info('开始展开文件夹')
         new_files = [Path(x) for x in expander.expand(*self.plans)]
         env.info('正在根据路径进行排序')
         new_files = sorted(new_files, key=lambda a: a.absolute())
 
@@ -82,11 +84,11 @@
             if not kk.exists():
                 env.warning(f'文件 "{kk}" 不存在，将从任务列表中去除')
                 continue
             arranged_files.append(kk)
             env.debug(f'重新添加 "{kk}"')
             count = len(list(v))
             if count > 1:
-                env.debug(f'发现 {count} 个重复的 "{k}" ，已经去除')
+                env.warning(f'发现 {count} 个重复的 "{k}" ，已经去除')
         env.progress.remove_task(task)
         self.plans = arranged_files
         env.info('计划列表自动整理完毕')
```

### Comparing `cxalio_studio_tools-0.1.9/src/media_killer/source_adapter.py` & `cxalio_studio_tools-0.2.0/src/media_killer/source_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import csv
 import urllib.parse
+import xml.etree.ElementTree as ET
+from abc import abstractmethod
 from pathlib import Path
+
 from cx_core.utils import detect_encoding
-from abc import abstractmethod
-import csv
 from .env import env
-import xml.etree.ElementTree as ET
 
 
 class AbstractAdapter:
     def __init__(self):
         self.filename = None
         self.file = None
         self.task = None
```

### Comparing `cxalio_studio_tools-0.1.9/src/sub_conv/help.md` & `cxalio_studio_tools-0.2.0/src/sub_conv/help.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,100 @@
-# subconv
+# SubConv
 
-subconv 用于批量转换字幕文件为台词本文档，
-附加地，也可以转换成其它格式的字幕文件，但不保证完整性。
+version: 0.2.0
+
+SubConv 用于批量转换字幕文件为台词本文档，
+附加地，也可以转换成其它格式的字幕文件，但**不保证完整性**。
 
 >subconv 不能当做一个完备的字幕文件转换器
 
 subconv 有以下特点：
 - 可以批量地对文件进行处理，可以自动展开文件夹
-- 目标文件自动防止在源文件旁边，最大化减少参数指定
+- 目标文件自动放置在源文件旁边，最大化减少参数指定
 - 也可以手动指定集中的输出文件夹
-- 支持 srt、ttml 等多种字幕文件读取
-- 输出台词本可以选择是否需要添加时间信息
+- 支持`srt`、`ttml` 等多种字幕格式
+- 输出台词本可以选择是否尽量保留时间信息
 - 内置一个简单的字幕内容检查器，将会自动进行简单的格式化处理
-- 可以输出字幕为表格( csv 或 xlsx )，以兼容其它工作流
+- 内置台词英文翻译功能(需要网络)
+- 可以输出字幕为表格(`csv`或`xlsx`)，以兼容其它工作流
 
-#### 基本使用
+## 基本使用
 
 直接在命令之后紧接源文件列表即可：
 
 ```shell
-sub_conv '字幕1.srt' '字幕2.ttml'
+subconv '字幕1.srt' '字幕2.ttml'
 ```
 
 以上命令将会在这两个字幕旁边生成同名的 'txt' 文件，
 其内容为提取的台词，每条一行。
 
-#### 高级用法
+> SubConv 输出的文件格式默认为`txt`。
+
+## 高级用法
 
-##### 文件夹输入
+### 文件夹输入
 
 如果输入的来源是一个文件夹，则会自动展开其中所有的文件夹，
 并将扩展名符合要求的文件列为输入文件。例如：
 
 ```shell
-sub_conv 'D:/给你的在这里/' '魔法小子第一季字幕'
+subconv 'D:/给你的在这里/' '魔法小子第一季字幕'
 ```
 
 上面的命令中指定的两个输入源都是文件夹，
 其中的字幕文件都会被添加。
 
-##### 指定输出位置
+### 指定输出位置
 
 使用 `--output-folder` 参数可以指定输出位置，
 输出的文件都会添加到这里。
 
 ```shell
-sub_conv '字幕1.srt' '字幕文件夹/' --output-folder '目标文件假/'
+subconv '字幕1.srt' '字幕文件夹/' --output-folder '目标文件夹/'
 # -o 是 --output-folder 的缩写
-sub_conv '字幕1.srt' '字幕文件夹/' -o '目标文件假/'
+subconv '字幕1.srt' '字幕文件夹/' -o '目标文件夹/'
 ```
 
-##### 指定输出格式
+### 指定输出格式
 
-默认情况下输出的目标文件是 utf-8 编码的 txt 文本文件，
+默认情况下输出的目标文件是`utf-8`编码的`txt文本文件`，
 可以使用 `--format` 参数设置输出格式, `--encoding` 用于设置编码。
 
 ```shell
-sub_conv '字幕.ttml' --format word 
-sub_conv '字幕.srt' -f csv --encoding 'gb18030'
-sub_conv '字幕.srt' -c 'utf-16'
+subconv '字幕.ttml' --format word 
+subconv '字幕.srt' -f csv --encoding 'gb18030'
+subconv '字幕.srt' -c 'utf-16'
 # -f 是 --format 的缩写
 # -c 是 --encoding 的缩写
 ```
 
 具体支持的输出格式，可以用`--help`参数打印帮助信息查看
 
-##### 关于自动格式化器
+### 关于自动格式化器
 
 subconv 内置了一个简单的格式化器，默认启用。它将会对字幕内容进行这些检查：
 - 自动去除字幕文件中携带的格式化标签（Davinci Resolve 输出的字幕通常都有）
 - 自动删除开头结尾的空格或回车
 - 自动缩减连续的多个空格或引号
-- 自动将；连续的多个回车合并为一个
+- 自动将连续的多个回车合并为一个
 
 如果不希望进行这些处理，可以使用 `--bypass-formatter` 参数禁用它。
 
-##### 测试运行
+### 自动翻译
+
+启用了 `--translate` 参数后，输出的字幕文本将自动转换为英文。
+
+英文翻译使用 bing 翻译服务完成，需要确保网络通畅。
+
+## 测试运行
 指定 `--dry-run` 参数可以启用干转模式，
 subconv 将会处理所有的内容，但是不会真的输出文件。
 
 也可以使用 `--debug` 参数，将会输出所有工作过程的信息，方便查看。
 
-两个选项可以一起使用。
+两个选项可以一起使用。
+
+-----
+项目主页: https://gitee.com/xiii_1991/cxalio-studio-tools
+
+作者: xiii_1991@163.com
```

### Comparing `cxalio_studio_tools-0.1.9/src/systools/update_githubhosts.py` & `cxalio_studio_tools-0.2.0/src/systools/update_githubhosts.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class GithubHostsUpdaterApp(AbstractApp):
     URL = "https://gitlab.com/ineo6/hosts/-/raw/master/next-hosts"
 
     def __init__(self):
         super(GithubHostsUpdaterApp, self).__init__()
         self.osinfo = OSInfo()
         self.app_name = 'update_githubhosts'
-        self.app_version = '0.1.8'
+        self.app_version = '0.1.10'
         parser = ArgumentParser(prog=self.app_name, formatter_class=RichHelpFormatter,
                                 description='自动更新githubhosts', epilog='Designed by xiii_1991')
         parser.add_argument('-p', '--pretend', action='store_true', dest='pretend',
                             help='模拟执行并输出结果')
         parser.add_argument('-s', '--save', action='append', dest='side_save', metavar='PATH',
                             help='输出到指定位置')
         self._parser = parser
@@ -27,15 +27,15 @@
 
     def refresh_dns(self):
         self.status.update('尝试刷新DNS...')
         if self.osinfo.system == 'Darwin':
             os.system("killall -HUP mDNSResponder")
             env.print('杀死 mDNSResponder')
         elif self.osinfo.system == 'Linux':
-            os.system("systemctl restart networking")
+            os.system("systemctl restart systemd-resolved")
             env.print('重启网络服务')
         elif self.osinfo.system == 'Windows':
             os.system("ipconfig /flushdns")
             env.print('刷新 DNS 信息')
         else:
             env.warning('无法识别操作系统，请手动刷新')
```

### Comparing `cxalio_studio_tools-0.1.9/PKG-INFO` & `cxalio_studio_tools-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxalio-studio-tools
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scripts for po studio made by cxalio
 Home-page: https://gitee.com/xiii_1991/cxalio-studio-tools
 License: GPL-3.0-or-later
 Keywords: ffmpeg,tool
 Author: xiii_1991
 Author-email: xiii_1991@163.com
 Requires-Python: >=3.11,<4.0
@@ -14,54 +14,64 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: python-docx (>=1.1.0,<2.0.0)
 Requires-Dist: python-ffmpeg (>=2.0.10,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: rich-argparse (>=1.4.0,<2.0.0)
+Requires-Dist: translators (>=5.9.2,<6.0.0)
 Project-URL: Repository, https://gitee.com/xiii_1991/cxalio-studio-tools.git
 Description-Content-Type: text/markdown
 
 # cxalio-studio-tools
 
-#### 介绍
+## 介绍
 
 这是一套用于简化影视后期工作的脚本合集。
 
 涉及各种繁复的资料处理工作，解放双手，减少出错。
 
-#### 安装
+## 安装
 
 ```shell
 pip --install cxalio-media-tools
 
 #推荐使用 pipx 安装
 pipx --install cxalio-media-tools
 ```
 
-#### 包含的工具
+## 包含的工具
 
-##### mediakiller
+### MediaKiller
 
-media-killer 可以通过配置文件操纵 ffmpeg 批量地对大量媒体文件转码，
+MediaKiller 可以通过配置文件操纵 ffmpeg 批量地对大量媒体文件转码，
 仅支持单文件输入，可以保留源文件的目录层级。
-请查看[具体说明](media_killer/help.md)
+请查看[具体说明](src/media_killer/help.md)
 
-##### subconv
+### SubConv
 
 subconv 是一个批量从字幕文件提取台词本的工具。
 请查看[具体说明](src/sub_conv/help.md)
 
-#### To-do
+### update_githubhosts
+
+一个自动更新hosts的小工具
+
+## To-do
 
 - media-inspector 解析媒体信息
 
-#### Change-log
+## Change-log
+
+### 0.2.0
+
+重新构建现有工具。
 
-- 0.1.8
+#### MediaKiller
 
-  增加 update-githubhosts 工具
+- 增加了标签替换系统
+- 增加了任务模块，统一转码和脚本生成功能
+- 修改配置文件，分开输入和输出两部分，并且`input`和`output`现在是表数组了。这样就支持了多个文件的输入和输出。
+- 大幅优化内存占用和性能
+- 大幅调整调试信息
 
-- 0.1.7
-  
-  media-killer 对map的设置进行了特殊处理，解决了无法重映射媒体流的bug
```

