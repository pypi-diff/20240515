# Comparing `tmp/atcform-0.1.2.tar.gz` & `tmp/atcform-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atcform-0.1.2.tar", last modified: Tue May 14 16:11:58 2024, max compression
+gzip compressed data, was "atcform-0.1.3.tar", last modified: Tue May 14 16:39:44 2024, max compression
```

## Comparing `atcform-0.1.2.tar` & `atcform-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:58.781194 atcform-0.1.2/
--rw-rw-rw-   0        0        0     1082 2024-05-14 15:47:09.000000 atcform-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1565 2024-05-14 16:11:58.779191 atcform-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      868 2024-05-14 16:07:04.000000 atcform-0.1.2/README.md
--rw-rw-rw-   0        0        0       86 2024-05-14 11:46:25.000000 atcform-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 16:11:58.781194 atcform-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1050 2024-05-14 16:11:41.000000 atcform-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:58.759962 atcform-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:58.778190 atcform-0.1.2/src/ATCForm.egg-info/
--rw-rw-rw-   0        0        0     1565 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 16:11:58.776184 atcform-0.1.2/src/ATCFrom/
--rw-rw-rw-   0        0        0    24411 2024-05-14 16:04:01.000000 atcform-0.1.2/src/ATCFrom/AUTO_FROM.py
--rw-rw-rw-   0        0        0      140 2024-05-14 16:08:36.000000 atcform-0.1.2/src/ATCFrom/__init__.py
--rw-rw-rw-   0        0        0     1873 2024-05-14 16:04:29.000000 atcform-0.1.2/src/ATCFrom/examlpe.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:39:44.771198 atcform-0.1.3/
+-rw-rw-rw-   0        0        0     1082 2024-05-14 15:47:09.000000 atcform-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1565 2024-05-14 16:39:44.769951 atcform-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2024-05-14 16:36:41.000000 atcform-0.1.3/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 11:46:25.000000 atcform-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 16:39:44.771198 atcform-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1050 2024-05-14 16:39:31.000000 atcform-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:39:44.739318 atcform-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 16:39:44.759926 atcform-0.1.3/src/ATCForm/
+-rw-rw-rw-   0        0        0    24411 2024-05-14 16:37:54.000000 atcform-0.1.3/src/ATCForm/AUTO_FORM.py
+-rw-rw-rw-   0        0        0      140 2024-05-14 16:38:01.000000 atcform-0.1.3/src/ATCForm/__init__.py
+-rw-rw-rw-   0        0        0     1873 2024-05-14 16:37:56.000000 atcform-0.1.3/src/ATCForm/examlpe.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:39:44.768856 atcform-0.1.3/src/ATCForm.egg-info/
+-rw-rw-rw-   0        0        0     1565 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 16:39:44.000000 atcform-0.1.3/src/ATCForm.egg-info/top_level.txt
```

### Comparing `atcform-0.1.2/LICENSE` & `atcform-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atcform-0.1.2/PKG-INFO` & `atcform-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATCForm
-Version: 0.1.2
+Version: 0.1.3
 Summary: ATCFrom - Automatically fill in the collection form 自动化表单填写工具
 Home-page: https://github.com/YKONGCO/ATCForm
 Author: YKONGCO
 Author-email: 1570585752@qq.com
 Maintainer: YKONGCO
 Maintainer-email: 1570585752@qq.com
 License: MIT License
@@ -14,16 +14,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: webdriver_manager
 Requires-Dist: selenium>=4.0
 
-## ATCFrom - Automatically fill in the collection form 自动化表单填写工具
-ATCFrom is a tool that automatically fills in the collection form.
+## ATCForm - Automatically fill in the collection form 自动化表单填写工具
+ATCForm is a tool that automatically fills in the collection form.
 supported: jin data ,tx data
 ![](https://img.shields.io/github/release/YKONGCO0/ATCFrom)
 #### 1.data.txt 格式要求
 ```
 {
         "学号姓名":"",
         "学号":"",
```

### Comparing `atcform-0.1.2/setup.py` & `atcform-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ATCForm",
-    version="0.1.2",
+    version="0.1.3",
     description="ATCFrom - Automatically fill in the collection form 自动化表单填写工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/YKONGCO/ATCForm",
     author="YKONGCO",
     author_email="1570585752@qq.com",
     maintainer="YKONGCO",
```

### Comparing `atcform-0.1.2/src/ATCForm.egg-info/PKG-INFO` & `atcform-0.1.3/src/ATCForm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATCForm
-Version: 0.1.2
+Version: 0.1.3
 Summary: ATCFrom - Automatically fill in the collection form 自动化表单填写工具
 Home-page: https://github.com/YKONGCO/ATCForm
 Author: YKONGCO
 Author-email: 1570585752@qq.com
 Maintainer: YKONGCO
 Maintainer-email: 1570585752@qq.com
 License: MIT License
@@ -14,16 +14,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: webdriver_manager
 Requires-Dist: selenium>=4.0
 
-## ATCFrom - Automatically fill in the collection form 自动化表单填写工具
-ATCFrom is a tool that automatically fills in the collection form.
+## ATCForm - Automatically fill in the collection form 自动化表单填写工具
+ATCForm is a tool that automatically fills in the collection form.
 supported: jin data ,tx data
 ![](https://img.shields.io/github/release/YKONGCO0/ATCFrom)
 #### 1.data.txt 格式要求
 ```
 {
         "学号姓名":"",
         "学号":"",
```

### Comparing `atcform-0.1.2/src/ATCFrom/AUTO_FROM.py` & `atcform-0.1.3/src/ATCForm/AUTO_FORM.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         os.remove(file_path)
     download_driver_path = EdgeChromiumDriverManager().install()
     print(download_driver_path)
     shutil.move(download_driver_path, folder_path)
 
 
 
-class AUTO_JSJ_FROM:
+class AUTO_JSJ_FORM:
     info_data={}
     select_list=[]
     wait_time :str 
     answer_list=[]
     
     def __init__(self,url : str ):
         options = webdriver.EdgeOptions()
@@ -256,15 +256,15 @@
         except Exception as e:
             print(e)
             
 
     def __del__(self):
         self.driver.quit()
 
-class AUTO_TX_FROM:
+class AUTO_TX_FORM:
     info_data={}
     select_list=[]
     wait_time :str 
     answer_list=[]
     
     def __init__(self,url : str ):
         options = webdriver.EdgeOptions()
@@ -580,15 +580,15 @@
     def run(self):
         self.AT1.wait_for_time()
         self.AT1.auto_input()
         self.AT1.auto_click_button()
         self.AT1.auto_submit_click_tx()
         
     def init(self):
-        self.AT1=AUTO_TX_FROM(self.url)
+        self.AT1=AUTO_TX_FORM(self.url)
         self.AT1.set_wait_time(input_time=self.start_time)
         self.AT1.wait_for_login()
         self.AT1.set_base_data(self.data_path)
         if(self.is_enable==False):
             self.AT1.select_list+=self.SELECT_LIST
         self.AT1.display_all_qus()
         self.AT1.Initializes_the_answer_list()
@@ -647,15 +647,15 @@
     def run(self):
         self.AJ1.wait_for_time()
         self.AJ1.auto_input()
         self.AJ1.auto_click_button()
         self.AJ1.auto_submit_click_JSJ()
         
     def init(self):
-        self.AJ1=AUTO_JSJ_FROM(self.url)
+        self.AJ1=AUTO_JSJ_FORM(self.url)
         time.sleep(1)
         self.AJ1.set_wait_time(input_time=self.start_time)
         self.AJ1.set_base_data(self.data_path)
         if(self.is_enable==False):
             self.AJ1.select_list+=self.SELECT_LIST
         self.AJ1.display_all_qus()
         self.AJ1.Initializes_the_answer_list()
```

### Comparing `atcform-0.1.2/src/ATCFrom/examlpe.py` & `atcform-0.1.3/src/ATCForm/examlpe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import ATCFrom as AT
+import ATCForm as AT
 import time
 # Args:
 #     url (str): 收集表地址
 #     data_path (str): 数据地址
 #     start_time (str): 开始时间 格式为202405121200 年月日时分(注意补零).
 #     is_enable (bool, optional): 是否提前输入需要选择内容 Defaults to True.
 #     SELECT_LIST (list, optional): 需要选择的内容. Defaults to [] 如["1","2"].
```

