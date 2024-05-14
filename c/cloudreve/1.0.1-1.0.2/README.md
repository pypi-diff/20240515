# Comparing `tmp/cloudreve-1.0.1.tar.gz` & `tmp/cloudreve-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudreve-1.0.1.tar", last modified: Wed May  1 03:40:30 2024, max compression
+gzip compressed data, was "cloudreve-1.0.2.tar", last modified: Tue May 14 23:12:52 2024, max compression
```

## Comparing `cloudreve-1.0.1.tar` & `cloudreve-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 03:40:30.837207 cloudreve-1.0.1/
--rw-rw-rw-   0        0        0    35823 2024-04-30 15:03:13.000000 cloudreve-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1926 2024-05-01 03:40:30.836206 cloudreve-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1052 2024-05-01 03:26:50.000000 cloudreve-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 03:40:30.837207 cloudreve-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1308 2024-05-01 03:40:08.000000 cloudreve-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:40:30.794603 cloudreve-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:40:30.804602 cloudreve-1.0.1/src/cloudreve/
--rw-rw-rw-   0        0        0       28 2024-04-30 17:10:56.000000 cloudreve-1.0.1/src/cloudreve/__init__.py
--rw-rw-rw-   0        0        0    11459 2024-05-01 03:39:59.000000 cloudreve-1.0.1/src/cloudreve/models.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:40:30.832638 cloudreve-1.0.1/src/cloudreve.egg-info/
--rw-rw-rw-   0        0        0     1926 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 23:12:52.052342 cloudreve-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-30 15:03:13.000000 cloudreve-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2023 2024-05-14 23:12:52.051834 cloudreve-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1149 2024-05-14 23:12:25.000000 cloudreve-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 23:12:52.053144 cloudreve-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1353 2024-05-14 23:12:15.000000 cloudreve-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 23:12:51.996770 cloudreve-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 23:12:52.008863 cloudreve-1.0.2/src/cloudreve/
+-rw-rw-rw-   0        0        0       28 2024-04-30 17:10:56.000000 cloudreve-1.0.2/src/cloudreve/__init__.py
+-rw-rw-rw-   0        0        0    11459 2024-05-01 03:39:59.000000 cloudreve-1.0.2/src/cloudreve/models.py
+drwxrwxrwx   0        0        0        0 2024-05-14 23:12:52.048601 cloudreve-1.0.2/src/cloudreve.egg-info/
+-rw-rw-rw-   0        0        0     2023 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/top_level.txt
```

### Comparing `cloudreve-1.0.1/LICENSE` & `cloudreve-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudreve-1.0.1/PKG-INFO` & `cloudreve-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudreve
-Version: 1.0.1
+Version: 1.0.2
 Summary: SDK for Cloudreve sites
 Home-page: https://github.com/yxzlwz/cloudreve-sdk
 Author: yxzlwz
 Author-email: yxzlwz@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,21 @@
 
 # Cloudreve SDK
 
 本项目为 [Cloudreve](https://github.com/cloudreve/Cloudreve) 社区版的 Python SDK。
 
 - 开源地址：https://github.com/yxzlwz/cloudreve-sdk
 - PyPI：https://pypi.org/project/cloudreve/
+- API文档：https://cloudreve.apifox.cn/
+
+## 安装
+
+```bash
+pip3 install cloudreve
+```
 
 ## 示例
 
 ```python
 from cloudreve import Cloudreve
 
 # 初始化
```

### Comparing `cloudreve-1.0.1/README.md` & `cloudreve-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Cloudreve SDK
 
 本项目为 [Cloudreve](https://github.com/cloudreve/Cloudreve) 社区版的 Python SDK。
 
 - 开源地址：https://github.com/yxzlwz/cloudreve-sdk
 - PyPI：https://pypi.org/project/cloudreve/
+- API文档：https://cloudreve.apifox.cn/
+
+## 安装
+
+```bash
+pip3 install cloudreve
+```
 
 ## 示例
 
 ```python
 from cloudreve import Cloudreve
 
 # 初始化
```

### Comparing `cloudreve-1.0.1/setup.py` & `cloudreve-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
 
 from setuptools import find_packages, setup
 
-with open(os.path.join(os.path.dirname(__file__), 'README.md')) as fh:
+with open(os.path.join(os.path.dirname(__file__), 'README.md'),
+          'r',
+          encoding='utf-8') as fh:
     readme = fh.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='cloudreve',
-    version='1.0.1',
+    version='1.0.2',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     include_package_data=True,
     license='GPLv3',
     description='SDK for Cloudreve sites',
     long_description=readme,
     long_description_content_type='text/markdown',
```

### Comparing `cloudreve-1.0.1/src/cloudreve/models.py` & `cloudreve-1.0.2/src/cloudreve/models.py`

 * *Files identical despite different names*

### Comparing `cloudreve-1.0.1/src/cloudreve.egg-info/PKG-INFO` & `cloudreve-1.0.2/src/cloudreve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudreve
-Version: 1.0.1
+Version: 1.0.2
 Summary: SDK for Cloudreve sites
 Home-page: https://github.com/yxzlwz/cloudreve-sdk
 Author: yxzlwz
 Author-email: yxzlwz@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,21 @@
 
 # Cloudreve SDK
 
 本项目为 [Cloudreve](https://github.com/cloudreve/Cloudreve) 社区版的 Python SDK。
 
 - 开源地址：https://github.com/yxzlwz/cloudreve-sdk
 - PyPI：https://pypi.org/project/cloudreve/
+- API文档：https://cloudreve.apifox.cn/
+
+## 安装
+
+```bash
+pip3 install cloudreve
+```
 
 ## 示例
 
 ```python
 from cloudreve import Cloudreve
 
 # 初始化
```

