# Comparing `tmp/ncmlistdownloader-1.1.0.240506.tar.gz` & `tmp/ncmlistdownloader-2.0.0.240515a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.1.0.240506.tar", last modified: Mon May  6 05:09:57 2024, max compression
+gzip compressed data, was "ncmlistdownloader-2.0.0.240515a1.tar", last modified: Wed May 15 14:50:40 2024, max compression
```

## Comparing `ncmlistdownloader-1.1.0.240506.tar` & `ncmlistdownloader-2.0.0.240515a1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 05:09:57.086328 ncmlistdownloader-1.1.0.240506/
--rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.1.0.240506/LICENSE
--rw-rw-rw-   0        0        0     1409 2024-05-06 05:09:57.085360 ncmlistdownloader-1.1.0.240506/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 05:09:57.023690 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1852 2024-05-06 05:06:28.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 05:09:57.056626 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     1789 2024-04-29 10:16:10.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/__init__.py
--rw-rw-rw-   0        0        0      651 2024-04-29 10:21:56.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/common.py
--rw-rw-rw-   0        0        0     1685 2024-04-29 10:22:02.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/download.py
--rw-rw-rw-   0        0        0     2689 2024-04-29 10:22:08.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/find_from_id.py
--rw-rw-rw-   0        0        0     1664 2024-04-29 10:23:33.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-05-06 05:09:57.069616 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2862 2024-04-29 10:21:37.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2161 2024-04-29 10:21:11.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2376 2024-05-06 05:09:23.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1791 2024-04-29 10:20:35.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-05-06 05:09:57.074575 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6233 2024-04-29 10:20:23.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/downloader/__init__.py
--rw-rw-rw-   0        0        0     1110 2024-04-30 04:27:30.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/downloader/json_list_io.py
-drwxrwxrwx   0        0        0        0 2024-05-06 05:09:57.077000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     4034 2024-05-05 14:27:08.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 05:09:57.077000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2296 2024-04-29 10:19:56.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 05:09:57.077000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     9580 2024-05-05 14:27:08.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 05:09:57.084333 ncmlistdownloader-1.1.0.240506/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1409 2024-05-06 05:09:56.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      822 2024-05-06 05:09:56.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 05:09:56.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-06 05:09:56.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-05-06 05:09:56.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 05:09:56.000000 ncmlistdownloader-1.1.0.240506/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 05:09:57.087331 ncmlistdownloader-1.1.0.240506/setup.cfg
--rw-rw-rw-   0        0        0     1923 2024-05-06 05:08:59.000000 ncmlistdownloader-1.1.0.240506/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.986467 ncmlistdownloader-2.0.0.240515a1/
+-rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-2.0.0.240515a1/LICENSE
+-rw-rw-rw-   0        0        0     1297 2024-05-15 14:50:40.984455 ncmlistdownloader-2.0.0.240515a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.906993 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1880 2024-05-10 14:55:05.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.943906 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     1789 2024-04-29 10:16:10.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-04-29 10:21:56.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/common.py
+-rw-rw-rw-   0        0        0     1685 2024-04-29 10:22:02.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/download.py
+-rw-rw-rw-   0        0        0     2689 2024-04-29 10:22:08.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-04-29 10:23:33.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.957703 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2862 2024-04-29 10:21:37.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2161 2024-04-29 10:21:11.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2376 2024-05-06 05:09:23.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1791 2024-04-29 10:20:35.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.964687 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6233 2024-04-29 10:20:23.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/__init__.py
+-rw-rw-rw-   0        0        0     1110 2024-04-30 04:27:30.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/json_list_io.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.968675 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     4034 2024-05-05 14:27:08.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.970670 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2296 2024-04-29 10:19:56.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.974465 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     9580 2024-05-05 14:27:08.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/song/__init__.py
+-rw-rw-rw-   0        0        0     8233 2024-05-15 14:49:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/song/cleaned.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.980466 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1297 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      856 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:50:40.986467 ncmlistdownloader-2.0.0.240515a1/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-05-15 14:50:09.000000 ncmlistdownloader-2.0.0.240515a1/setup.py
```

### Comparing `ncmlistdownloader-1.1.0.240506/LICENSE` & `ncmlistdownloader-2.0.0.240515a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/PKG-INFO` & `ncmlistdownloader-2.0.0.240515a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.1.0.240506
+Version: 2.0.0.240515a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: CD Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Editors
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
```

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/__init__.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 ncmlistdownloader/__init__.py
-Core.Ver.1.1.0.240506
+Core.Ver.1.1.1.240510
 Author: CooooldWind_
 """
 
 from pathlib import Path
 import time
+import getpass
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.global_args import *
 
 
 def main():
     for i in CMD_START_WORDS:
         print(i)
     print(f"[*]{CORE_VERSION}")
-    c = {"MUSIC_U": str(input("Cookies(Press Enter if you have not): "))}
+    c = {"MUSIC_U": str(getpass.getpass("Cookies(Press Enter if you have not): ", ))}
     id = str(input("ID: "))
     p = Playlist(id)
     if c['MUSIC_U'] == "":
         p.get_info()
     else:
         p.get_info(cookies=c)
     print("Playlist info-reading succeed.")
```

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/__init__.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/common.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/common.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/download.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/download.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/find_from_id.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/find_from_id.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/cmd/json_io.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/json_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/global_args.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/downloader/json_list_io.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/json_list_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/song/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.1.0.240506
+Version: 2.0.0.240515a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: CD Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Editors
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
```

### Comparing `ncmlistdownloader-1.1.0.240506/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 ncmlistdownloader/common/encode_sec_key.py
 ncmlistdownloader/common/global_args.py
 ncmlistdownloader/common/thread_test.py
 ncmlistdownloader/downloader/__init__.py
 ncmlistdownloader/downloader/json_list_io.py
 ncmlistdownloader/editer/__init__.py
 ncmlistdownloader/playlist/__init__.py
-ncmlistdownloader/song/__init__.py
+ncmlistdownloader/song/__init__.py
+ncmlistdownloader/song/cleaned.py
```

### Comparing `ncmlistdownloader-1.1.0.240506/setup.py` & `ncmlistdownloader-2.0.0.240515a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # from ncmlistdownloader.common.global_args import CORE_VERSION_SETUP
 setup(
     classifiers=[
         # 发展时期
-        # 'Development Status :: 3 - Alpha',
+        'Development Status :: 3 - Alpha',
         # 'Development Status :: 4 - Beta',
-        "Development Status :: 5 - Production/Stable",
+        # "Development Status :: 5 - Production/Stable",
         # 开发的目标用户
         "Intended Audience :: Customer Service",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         # 属于什么类型
         "Topic :: Communications :: File Sharing",
         "Topic :: Internet",
@@ -18,25 +18,23 @@
         "Topic :: Multimedia :: Graphics",
         "Topic :: Multimedia :: Sound/Audio",
         "Topic :: Multimedia :: Sound/Audio :: CD Audio",
         "Topic :: Multimedia :: Sound/Audio :: Editors",
         # 许可证信息
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         # 目标 Python 版本
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     name="ncmlistdownloader",
-    version="1.1.0.240506",
+    version="2.0.0.240515a1",
     description="获取网易云音乐歌单数据，下载音乐，主动添加元信息。",
     author="CooooldWind_",
     url="https://gitee.com/Cooooldwind/163ListDownloader_NexT",
     packages=find_packages(),
     install_requires=[
         "pycryptodome",
         "pillow",
```

