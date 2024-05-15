# Comparing `tmp/py_music_editer-0.1.0a24050801.tar.gz` & `tmp/py_music_editer-0.1.0a24051001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_music_editer-0.1.0a24050801.tar", last modified: Wed May  8 14:59:31 2024, max compression
+gzip compressed data, was "py_music_editer-0.1.0a24051001.tar", last modified: Wed May 15 14:49:08 2024, max compression
```

## Comparing `py_music_editer-0.1.0a24050801.tar` & `py_music_editer-0.1.0a24051001.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 14:59:31.508318 py_music_editer-0.1.0a24050801/
--rw-rw-rw-   0        0        0    11558 2024-05-07 14:40:26.000000 py_music_editer-0.1.0a24050801/LICENSE
--rw-rw-rw-   0        0        0     1192 2024-05-08 14:59:31.508318 py_music_editer-0.1.0a24050801/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-05-07 14:46:08.000000 py_music_editer-0.1.0a24050801/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 14:59:31.508318 py_music_editer-0.1.0a24050801/py_music_editer/
--rw-rw-rw-   0        0        0      238 2024-05-08 14:56:48.000000 py_music_editer-0.1.0a24050801/py_music_editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:59:31.508318 py_music_editer-0.1.0a24050801/py_music_editer.egg-info/
--rw-rw-rw-   0        0        0     1192 2024-05-08 14:59:31.000000 py_music_editer-0.1.0a24050801/py_music_editer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-08 14:59:31.000000 py_music_editer-0.1.0a24050801/py_music_editer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 14:59:31.000000 py_music_editer-0.1.0a24050801/py_music_editer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-08 14:59:31.000000 py_music_editer-0.1.0a24050801/py_music_editer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 14:59:31.508318 py_music_editer-0.1.0a24050801/setup.cfg
--rw-rw-rw-   0        0        0     1558 2024-05-08 14:58:37.000000 py_music_editer-0.1.0a24050801/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:49:08.094374 py_music_editer-0.1.0a24051001/
+-rw-rw-rw-   0        0        0    11558 2024-05-07 14:40:26.000000 py_music_editer-0.1.0a24051001/LICENSE
+-rw-rw-rw-   0        0        0     1192 2024-05-15 14:49:08.091370 py_music_editer-0.1.0a24051001/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-07 14:46:08.000000 py_music_editer-0.1.0a24051001/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 14:49:08.074429 py_music_editer-0.1.0a24051001/py_music_editer/
+-rw-rw-rw-   0        0        0      220 2024-05-10 14:28:07.000000 py_music_editer-0.1.0a24051001/py_music_editer/__init__.py
+-rw-rw-rw-   0        0        0      376 2024-05-10 14:28:07.000000 py_music_editer-0.1.0a24051001/py_music_editer/music.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:49:08.089376 py_music_editer-0.1.0a24051001/py_music_editer.egg-info/
+-rw-rw-rw-   0        0        0     1192 2024-05-15 14:49:08.000000 py_music_editer-0.1.0a24051001/py_music_editer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-15 14:49:08.000000 py_music_editer-0.1.0a24051001/py_music_editer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:49:08.000000 py_music_editer-0.1.0a24051001/py_music_editer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-15 14:49:08.000000 py_music_editer-0.1.0a24051001/py_music_editer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:49:08.095361 py_music_editer-0.1.0a24051001/setup.cfg
+-rw-rw-rw-   0        0        0     1558 2024-05-10 14:25:05.000000 py_music_editer-0.1.0a24051001/setup.py
```

### Comparing `py_music_editer-0.1.0a24050801/LICENSE` & `py_music_editer-0.1.0a24051001/LICENSE`

 * *Files identical despite different names*

### Comparing `py_music_editer-0.1.0a24050801/PKG-INFO` & `py_music_editer-0.1.0a24051001/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_music_editer
-Version: 0.1.0a24050801
+Version: 0.1.0a24051001
 Summary: 提供主流音乐文件数据与属性管理，读取与修改，以及工具集的Python库。
 Home-page: https://gitee.com/CooooldWind/PyMusicEditer
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `py_music_editer-0.1.0a24050801/py_music_editer.egg-info/PKG-INFO` & `py_music_editer-0.1.0a24051001/py_music_editer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_music_editer
-Version: 0.1.0a24050801
+Version: 0.1.0a24051001
 Summary: 提供主流音乐文件数据与属性管理，读取与修改，以及工具集的Python库。
 Home-page: https://gitee.com/CooooldWind/PyMusicEditer
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `py_music_editer-0.1.0a24050801/setup.py` & `py_music_editer-0.1.0a24051001/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     name="py_music_editer",
-    version="0.1.0.alpha24050801",
+    version="0.1.0.alpha24051001",
     description="提供主流音乐文件数据与属性管理，读取与修改，以及工具集的Python库。",
     author="CooooldWind_",
     url="https://gitee.com/CooooldWind/PyMusicEditer",
     packages=find_packages(),
     install_requires=[
     ],
 )
```

