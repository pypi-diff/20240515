# Comparing `tmp/atcform-0.1.3.tar.gz` & `tmp/atcform-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atcform-0.1.3.tar", last modified: Tue May 14 16:39:44 2024, max compression
+gzip compressed data, was "atcform-0.1.4.tar", last modified: Wed May 15 06:06:15 2024, max compression
```

## Comparing `atcform-0.1.3.tar` & `atcform-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 16:39:44.771198 atcform-0.1.3/
--rw-rw-rw-   0        0        0     1082 2024-05-14 15:47:09.000000 atcform-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1565 2024-05-14 16:39:44.769951 atcform-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      868 2024-05-14 16:36:41.000000 atcform-0.1.3/README.md
--rw-rw-rw-   0        0        0       86 2024-05-14 11:46:25.000000 atcform-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 16:39:44.771198 atcform-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1050 2024-05-14 16:39:31.000000 atcform-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:39:44.739318 atcform-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 16:39:44.759926 atcform-0.1.3/src/ATCForm/
--rw-rw-rw-   0        0        0    24411 2024-05-14 16:37:54.000000 atcform-0.1.3/src/ATCForm/AUTO_FORM.py
--rw-rw-rw-   0        0        0      140 2024-05-14 16:38:01.000000 atcform-0.1.3/src/ATCForm/__init__.py
--rw-rw-rw-   0        0        0     1873 2024-05-14 16:37:56.000000 atcform-0.1.3/src/ATCForm/examlpe.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:39:44.768856 atcform-0.1.3/src/ATCForm.egg-info/
--rw-rw-rw-   0        0        0     1565 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 06:06:15.281627 atcform-0.1.4/
+-rw-rw-rw-   0        0        0     1082 2024-05-14 15:47:09.000000 atcform-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1567 2024-05-15 06:06:15.280629 atcform-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2024-05-15 06:03:52.000000 atcform-0.1.4/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 11:46:25.000000 atcform-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 06:06:15.281627 atcform-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1050 2024-05-15 06:05:50.000000 atcform-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:06:15.256106 atcform-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 06:06:15.269113 atcform-0.1.4/src/ATCForm/
+-rw-rw-rw-   0        0        0    24411 2024-05-14 16:37:54.000000 atcform-0.1.4/src/ATCForm/AUTO_FORM.py
+-rw-rw-rw-   0        0        0      140 2024-05-14 16:38:01.000000 atcform-0.1.4/src/ATCForm/__init__.py
+-rw-rw-rw-   0        0        0     1873 2024-05-14 16:37:56.000000 atcform-0.1.4/src/ATCForm/examlpe.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:06:15.279627 atcform-0.1.4/src/ATCForm.egg-info/
+-rw-rw-rw-   0        0        0     1567 2024-05-15 06:06:15.000000 atcform-0.1.4/src/ATCForm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-15 06:06:15.000000 atcform-0.1.4/src/ATCForm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 06:06:15.000000 atcform-0.1.4/src/ATCForm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-15 06:06:15.000000 atcform-0.1.4/src/ATCForm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 06:06:15.000000 atcform-0.1.4/src/ATCForm.egg-info/top_level.txt
```

### Comparing `atcform-0.1.3/LICENSE` & `atcform-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atcform-0.1.3/PKG-INFO` & `atcform-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATCForm
-Version: 0.1.3
+Version: 0.1.4
 Summary: ATCFrom - Automatically fill in the collection form 自动化表单填写工具
 Home-page: https://github.com/YKONGCO/ATCForm
 Author: YKONGCO
 Author-email: 1570585752@qq.com
 Maintainer: YKONGCO
 Maintainer-email: 1570585752@qq.com
 License: MIT License
@@ -17,14 +17,15 @@
 License-File: LICENSE
 Requires-Dist: webdriver_manager
 Requires-Dist: selenium>=4.0
 
 ## ATCForm - Automatically fill in the collection form 自动化表单填写工具
 ATCForm is a tool that automatically fills in the collection form.
 supported: jin data ,tx data
+
 ![](https://img.shields.io/github/release/YKONGCO0/ATCFrom)
 #### 1.data.txt 格式要求
 ```
 {
         "学号姓名":"",
         "学号":"",
         "姓名":"",
```

### Comparing `atcform-0.1.3/README.md` & `atcform-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ## ATCForm - Automatically fill in the collection form 自动化表单填写工具
 ATCForm is a tool that automatically fills in the collection form.
 supported: jin data ,tx data
+
 ![](https://img.shields.io/github/release/YKONGCO0/ATCFrom)
 #### 1.data.txt 格式要求
 ```
 {
         "学号姓名":"",
         "学号":"",
         "姓名":"",
```

### Comparing `atcform-0.1.3/setup.py` & `atcform-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ATCForm",
-    version="0.1.3",
+    version="0.1.4",
     description="ATCFrom - Automatically fill in the collection form 自动化表单填写工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/YKONGCO/ATCForm",
     author="YKONGCO",
     author_email="1570585752@qq.com",
     maintainer="YKONGCO",
```

### Comparing `atcform-0.1.3/src/ATCForm/AUTO_FORM.py` & `atcform-0.1.4/src/ATCForm/AUTO_FORM.py`

 * *Files identical despite different names*

### Comparing `atcform-0.1.3/src/ATCForm/examlpe.py` & `atcform-0.1.4/src/ATCForm/examlpe.py`

 * *Files identical despite different names*

### Comparing `atcform-0.1.3/src/ATCForm.egg-info/PKG-INFO` & `atcform-0.1.4/src/ATCForm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATCForm
-Version: 0.1.3
+Version: 0.1.4
 Summary: ATCFrom - Automatically fill in the collection form 自动化表单填写工具
 Home-page: https://github.com/YKONGCO/ATCForm
 Author: YKONGCO
 Author-email: 1570585752@qq.com
 Maintainer: YKONGCO
 Maintainer-email: 1570585752@qq.com
 License: MIT License
@@ -17,14 +17,15 @@
 License-File: LICENSE
 Requires-Dist: webdriver_manager
 Requires-Dist: selenium>=4.0
 
 ## ATCForm - Automatically fill in the collection form 自动化表单填写工具
 ATCForm is a tool that automatically fills in the collection form.
 supported: jin data ,tx data
+
 ![](https://img.shields.io/github/release/YKONGCO0/ATCFrom)
 #### 1.data.txt 格式要求
 ```
 {
         "学号姓名":"",
         "学号":"",
         "姓名":"",
```

