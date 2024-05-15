# Comparing `tmp/qtmodel-0.3.0.tar.gz` & `tmp/qtmodel-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.3.0.tar", last modified: Wed May 15 02:29:54 2024, max compression
+gzip compressed data, was "qtmodel-0.3.1.tar", last modified: Wed May 15 05:49:13 2024, max compression
```

## Comparing `qtmodel-0.3.0.tar` & `qtmodel-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 02:29:54.481358 qtmodel-0.3.0/
--rw-rw-rw-   0        0        0    37701 2024-05-15 02:29:54.481358 qtmodel-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 02:29:54.473493 qtmodel-0.3.0/qtmodel/
--rw-rw-rw-   0        0        0       93 2024-05-15 02:13:58.000000 qtmodel-0.3.0/qtmodel/__init__.py
--rw-rw-rw-   0        0        0    82085 2024-05-15 02:18:41.000000 qtmodel-0.3.0/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     3834 2024-05-15 02:13:47.000000 qtmodel-0.3.0/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.3.0/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:29:54.479365 qtmodel-0.3.0/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    37701 2024-05-15 02:29:53.000000 qtmodel-0.3.0/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-15 02:29:54.000000 qtmodel-0.3.0/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 02:29:53.000000 qtmodel-0.3.0/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 02:29:54.000000 qtmodel-0.3.0/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 02:29:54.481358 qtmodel-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-15 02:29:33.000000 qtmodel-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:49:13.271619 qtmodel-0.3.1/
+-rw-rw-rw-   0        0        0    37701 2024-05-15 05:49:13.270553 qtmodel-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 05:49:13.248896 qtmodel-0.3.1/qtmodel/
+-rw-rw-rw-   0        0        0       93 2024-05-15 02:13:58.000000 qtmodel-0.3.1/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0    82085 2024-05-15 02:46:03.000000 qtmodel-0.3.1/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     3834 2024-05-15 02:13:47.000000 qtmodel-0.3.1/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.3.1/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:49:13.268158 qtmodel-0.3.1/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    37701 2024-05-15 05:49:12.000000 qtmodel-0.3.1/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-05-15 05:49:13.000000 qtmodel-0.3.1/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 05:49:12.000000 qtmodel-0.3.1/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 05:49:12.000000 qtmodel-0.3.1/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 05:49:13.271619 qtmodel-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-15 05:49:09.000000 qtmodel-0.3.1/setup.py
```

### Comparing `qtmodel-0.3.0/PKG-INFO` & `qtmodel-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.0
+Version: 0.3.1
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.3.0/README.md` & `qtmodel-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.0/qtmodel/qt_mdb.py` & `qtmodel-0.3.1/qtmodel/qt_mdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def save_file(file_path: str):
         """
             保存bfmd文件
             example:
                     mdb.save_file("a.bfmd")
             Returns: 无
         """
-        qt_model.OpenFile(file_path)
+        qt_model.SaveFile(file_path)
 
     @staticmethod
     def close_project():
         """
             关闭项目
             example:
                 mdb.close_project()
```

### Comparing `qtmodel-0.3.0/qtmodel/qt_odb.py` & `qtmodel-0.3.1/qtmodel/qt_odb.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.0/qtmodel/res_db.py` & `qtmodel-0.3.1/qtmodel/res_db.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.0/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.3.1/qtmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.0
+Version: 0.3.1
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.3.0/setup.py` & `qtmodel-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.3.0",
+    version="0.3.1",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
     description="python modeling for qt  24/05/06 ",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
```

