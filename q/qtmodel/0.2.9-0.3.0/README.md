# Comparing `tmp/qtmodel-0.2.9.tar.gz` & `tmp/qtmodel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.2.9.tar", last modified: Tue May 14 08:32:59 2024, max compression
+gzip compressed data, was "qtmodel-0.3.0.tar", last modified: Wed May 15 02:29:54 2024, max compression
```

## Comparing `qtmodel-0.2.9.tar` & `qtmodel-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:32:59.352196 qtmodel-0.2.9/
--rw-rw-rw-   0        0        0    37701 2024-05-14 08:32:59.352196 qtmodel-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 08:32:59.330210 qtmodel-0.2.9/qtmodel/
--rw-rw-rw-   0        0        0      117 2024-05-14 06:05:14.000000 qtmodel-0.2.9/qtmodel/__init__.py
--rw-rw-rw-   0        0        0    82266 2024-05-14 08:25:47.000000 qtmodel-0.2.9/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     3834 2024-05-13 05:54:03.000000 qtmodel-0.2.9/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0      939 2024-05-14 06:03:36.000000 qtmodel-0.2.9/qtmodel/qt_post.py
--rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.2.9/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:32:59.349151 qtmodel-0.2.9/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    37701 2024-05-14 08:32:58.000000 qtmodel-0.2.9/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-14 08:32:59.000000 qtmodel-0.2.9/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:32:58.000000 qtmodel-0.2.9/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-14 08:32:59.000000 qtmodel-0.2.9/qtmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 08:32:59.000000 qtmodel-0.2.9/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 08:32:59.352196 qtmodel-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      860 2024-05-14 08:32:52.000000 qtmodel-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:29:54.481358 qtmodel-0.3.0/
+-rw-rw-rw-   0        0        0    37701 2024-05-15 02:29:54.481358 qtmodel-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 02:29:54.473493 qtmodel-0.3.0/qtmodel/
+-rw-rw-rw-   0        0        0       93 2024-05-15 02:13:58.000000 qtmodel-0.3.0/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0    82085 2024-05-15 02:18:41.000000 qtmodel-0.3.0/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     3834 2024-05-15 02:13:47.000000 qtmodel-0.3.0/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.3.0/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:29:54.479365 qtmodel-0.3.0/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    37701 2024-05-15 02:29:53.000000 qtmodel-0.3.0/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-05-15 02:29:54.000000 qtmodel-0.3.0/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 02:29:53.000000 qtmodel-0.3.0/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 02:29:54.000000 qtmodel-0.3.0/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 02:29:54.481358 qtmodel-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-15 02:29:33.000000 qtmodel-0.3.0/setup.py
```

### Comparing `qtmodel-0.2.9/PKG-INFO` & `qtmodel-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.2.9
+Version: 0.3.0
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.2.9/README.md` & `qtmodel-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.9/qtmodel/qt_mdb.py` & `qtmodel-0.3.0/qtmodel/qt_mdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1289,16 +1289,16 @@
         example:
             mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
         Returns: 无
         """
         qt_model.RemoveNodalDisplacement(caseName=case_name, nodeId=-node_id)
 
     @staticmethod
-    def add_beam_load(beam_id: int = 1, case_name: str = "", load_type: int = 1, coord_system: int = 3, list_x: list[tuple[float, float]] = None,
-                      list_load: list[tuple[float, float]] = None, group_name="默认荷载组"):
+    def add_beam_load(beam_id: int = 1, case_name: str = "", load_type: int = 1, coord_system: int = 3, list_x: list[float, float] = None,
+                      list_load: list[float, float] = None, group_name="默认荷载组"):
         """
         添加梁单元荷载
         Args:
             beam_id:单元编号
             case_name:荷载工况名
             load_type:荷载类型
                _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩
@@ -1670,23 +1670,14 @@
         if name != "":
             qt_model.DeleteLoadCase(name=name)
         elif index != -1:
             qt_model.DeleteLoadCase(id=index)
         else:
             qt_model.DeleteAllLoadCase()
 
-    @staticmethod
-    def test_print():
-        """
-        测试运行
-        Returns: 无
-        """
-        print(1)
-        raise Exception("错误")
-
     # endregion
 
     # region 施工阶段
     @staticmethod
     def add_construction_stage(name: str = "", duration: int = 0,
                                active_structures: list[tuple[str, int, int, int]] = None,
                                delete_structures: list[str] = None,
```

### Comparing `qtmodel-0.2.9/qtmodel/qt_odb.py` & `qtmodel-0.3.0/qtmodel/qt_odb.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.9/qtmodel/res_db.py` & `qtmodel-0.3.0/qtmodel/res_db.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.9/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.3.0/qtmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.2.9
+Version: 0.3.0
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.2.9/setup.py` & `qtmodel-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,24 +3,21 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.2.9",
+    version="0.3.0",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
     description="python modeling for qt  24/05/06 ",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
-    install_requires=[
-        'requests>=2.23.0',      # 一个有版本要求的依赖项
-    ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         "Operating System :: OS Independent",
     ],
 )
```

