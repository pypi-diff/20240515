# Comparing `tmp/wxauto-3.9.8.15.6.tar.gz` & `tmp/wxauto-3.9.8.15.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wxauto-3.9.8.15.6.tar", last modified: Tue May 14 06:00:52 2024, max compression
+gzip compressed data, was "dist\wxauto-3.9.8.15.7.tar", last modified: Wed May 15 15:31:45 2024, max compression
```

## Comparing `wxauto-3.9.8.15.6.tar` & `wxauto-3.9.8.15.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/
--rw-rw-rw-   0        0        0     3698 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/PKG-INFO
--rw-rw-rw-   0        0        0     3333 2024-05-14 06:00:05.000000 wxauto-3.9.8.15.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/setup.cfg
--rw-rw-rw-   0        0        0      732 2024-05-14 05:58:42.000000 wxauto-3.9.8.15.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto/
--rw-rw-rw-   0        0        0      148 2024-05-14 04:47:09.000000 wxauto-3.9.8.15.6/wxauto/__init__.py
--rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.6/wxauto/color.py
--rw-rw-rw-   0        0        0    24759 2024-05-14 05:52:10.000000 wxauto-3.9.8.15.6/wxauto/elements.py
--rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.6/wxauto/errors.py
--rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.6/wxauto/languages.py
--rw-rw-rw-   0        0        0   366752 2024-05-14 04:11:30.000000 wxauto-3.9.8.15.6/wxauto/uiautomation.py
--rw-rw-rw-   0        0        0    10935 2024-05-14 05:18:00.000000 wxauto-3.9.8.15.6/wxauto/utils.py
--rw-rw-rw-   0        0        0    29336 2024-05-14 05:36:01.000000 wxauto-3.9.8.15.6/wxauto/wxauto.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/
--rw-rw-rw-   0        0        0     3698 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/
+-rw-rw-rw-   0        0        0     3698 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3333 2024-05-14 06:00:05.000000 wxauto-3.9.8.15.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/setup.cfg
+-rw-rw-rw-   0        0        0      732 2024-05-15 15:31:27.000000 wxauto-3.9.8.15.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/wxauto/
+-rw-rw-rw-   0        0        0      148 2024-05-14 04:47:09.000000 wxauto-3.9.8.15.7/wxauto/__init__.py
+-rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.7/wxauto/color.py
+-rw-rw-rw-   0        0        0    24103 2024-05-15 12:26:26.000000 wxauto-3.9.8.15.7/wxauto/elements.py
+-rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.7/wxauto/errors.py
+-rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.7/wxauto/languages.py
+-rw-rw-rw-   0        0        0   366752 2024-05-14 04:11:30.000000 wxauto-3.9.8.15.7/wxauto/uiautomation.py
+-rw-rw-rw-   0        0        0    11545 2024-05-15 12:23:50.000000 wxauto-3.9.8.15.7/wxauto/utils.py
+-rw-rw-rw-   0        0        0    29323 2024-05-15 15:31:36.000000 wxauto-3.9.8.15.7/wxauto/wxauto.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/wxauto.egg-info/
+-rw-rw-rw-   0        0        0     3698 2024-05-15 15:31:44.000000 wxauto-3.9.8.15.7/wxauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-15 15:31:45.000000 wxauto-3.9.8.15.7/wxauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 15:31:44.000000 wxauto-3.9.8.15.7/wxauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-15 15:31:44.000000 wxauto-3.9.8.15.7/wxauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 15:31:44.000000 wxauto-3.9.8.15.7/wxauto.egg-info/top_level.txt
```

### Comparing `wxauto-3.9.8.15.6/PKG-INFO` & `wxauto-3.9.8.15.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.6
+Version: 3.9.8.15.7
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

### Comparing `wxauto-3.9.8.15.6/README.md` & `wxauto-3.9.8.15.7/README.md`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.6/setup.py` & `wxauto-3.9.8.15.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wxauto',
-    version='3.9.8.15.6',
+    version='3.9.8.15.7',
     author='Cluic',
     author_email='tikic@qq.com',
     description='A simple wechat automation tool',
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `wxauto-3.9.8.15.6/wxauto/color.py` & `wxauto-3.9.8.15.7/wxauto/color.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.6/wxauto/elements.py` & `wxauto-3.9.8.15.7/wxauto/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,26 +72,15 @@
         if savepic:
             self._show()
             paths = list()
             ImgItems = [i for i in msgitems if i.Name == f"[{self._lang('图片')}]" and i.ButtonControl(Name='').Exists(maxSearchSeconds=0.1)]
             if not ImgItems:
                 return msgs
             imgcontrol = ImgItems[0].ButtonControl(Name='')
-            if imgcontrol.BoundingRectangle.top < self.C_MsgList.BoundingRectangle.top:
-                # 上滚动
-                while True:
-                    self.C_MsgList.WheelUp(wheelTimes=1, waitTime=0.1)
-                    if imgcontrol.BoundingRectangle.top > self.C_MsgList.BoundingRectangle.top:
-                        break
-            elif imgcontrol.BoundingRectangle.bottom > self.C_MsgList.BoundingRectangle.bottom:
-                # 下滚动
-                while True:
-                    self.C_MsgList.WheelDown(wheelTimes=1, waitTime=0.1)
-                    if imgcontrol.BoundingRectangle.bottom < self.C_MsgList.BoundingRectangle.bottom:
-                        break
+            RollIntoView(self.C_MsgList, imgcontrol)
             imgcontrol.Click(simulateMove=False)
             imgobj = WeChatImage()
             savepath = imgobj.Save()
             paths.append(savepath)
             while True:
                 if imgobj.Next(warning=False):
                     savepath = imgobj.Save()
```

### Comparing `wxauto-3.9.8.15.6/wxauto/languages.py` & `wxauto-3.9.8.15.7/wxauto/languages.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.6/wxauto/uiautomation.py` & `wxauto-3.9.8.15.7/wxauto/uiautomation.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.6/wxauto/utils.py` & `wxauto-3.9.8.15.7/wxauto/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 try:
     from anytree import Node, RenderTree
 
     def GetAllControl(ele):
         def findall(ele, n=0, node=None):
             nn = '\n'
-            nodename = f"[{ele.ControlTypeName}](\"{ele.ClassName}\", \"{ele.Name.replace(nn, '')}\")"
+            nodename = f"[{ele.ControlTypeName}](\"{ele.ClassName}\", \"{ele.Name.replace(nn, '')}\", \"{''.join([str(i) for i in ele.GetRuntimeId()])}\")"
             if not node:
                 node1 = Node(nodename)
             else:
                 node1 = Node(nodename, parent=node)
             eles = ele.GetChildren()
             for ele1 in eles:
                 findall(ele1, n+1, node1)
@@ -310,8 +310,24 @@
             wxpath = os.path.join(path, "WeChat.exe")
             if os.path.exists(wxpath):
                 os.system(f'start "" "{wxpath}"')
                 FixVersionError()
             else:
                 raise Exception('nof found')
         except WindowsError:
-            Warning("未找到微信安装路径，请先打开微信启动页面再次尝试运行该方法！")
+            Warning("未找到微信安装路径，请先打开微信启动页面再次尝试运行该方法！")
+
+
+def RollIntoView(win, ele):
+    if ele.BoundingRectangle.top < win.BoundingRectangle.top:
+        # 上滚动
+        while True:
+            win.WheelUp(wheelTimes=1, waitTime=0.1)
+            if ele.BoundingRectangle.top >= win.BoundingRectangle.top:
+                break
+
+    elif ele.BoundingRectangle.bottom >= win.BoundingRectangle.bottom:
+        # 下滚动
+        while True:
+            win.WheelDown(wheelTimes=1, waitTime=0.1)
+            if ele.BoundingRectangle.bottom < win.BoundingRectangle.bottom:
+                break
```

### Comparing `wxauto-3.9.8.15.6/wxauto/wxauto.py` & `wxauto-3.9.8.15.7/wxauto/wxauto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Cluic
-Update: 2024-05-14
-Version: 3.9.8.15.6
+Update: 2024-05-15
+Version: 3.9.8.15.7
 """
 
 from . import uiautomation as uia
 from .languages import *
 from .utils import *
 from .elements import *
 from .errors import *
@@ -91,15 +91,15 @@
             sessionname (str): 聊天对象名
             amount (int): 新消息条数
         """
         matchobj = re.search('\d+条新消息', SessionItem.Name)
         amount = 0
         if matchobj:
             try:
-                amount = int([i for i in SessionItem.GetChildren()[0].GetChildren() if type(i) == uia.uiautomation.TextControl][0].Name)
+                amount = int([i for i in SessionItem.GetChildren()[0].GetChildren() if type(i) == uia.TextControl][0].Name)
             except:
                 pass
         if amount:
             sessionname = SessionItem.Name.replace(f'{amount}条新消息','')
         else:
             sessionname = SessionItem.Name
         return sessionname, amount
```

### Comparing `wxauto-3.9.8.15.6/wxauto.egg-info/PKG-INFO` & `wxauto-3.9.8.15.7/wxauto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.6
+Version: 3.9.8.15.7
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

