# Comparing `tmp/xcloudforlinux-0.1.0.tar.gz` & `tmp/xcloudforlinux-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcloudforlinux-0.1.0.tar", last modified: Tue May 14 15:46:24 2024, max compression
+gzip compressed data, was "xcloudforlinux-0.2.0.tar", last modified: Tue May 14 15:51:44 2024, max compression
```

## Comparing `xcloudforlinux-0.1.0.tar` & `xcloudforlinux-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 15:46:24.260345 xcloudforlinux-0.1.0/
--rw-rw-rw-   0        0        0       38 2024-05-14 15:45:57.000000 xcloudforlinux-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2909 2024-05-14 15:46:24.257316 xcloudforlinux-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2574 2024-05-06 06:00:51.000000 xcloudforlinux-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 15:46:24.261317 xcloudforlinux-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-05-14 15:44:21.000000 xcloudforlinux-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:46:24.234006 xcloudforlinux-0.1.0/xcloudClients/
--rw-rw-rw-   0        0        0      166 2024-05-14 15:43:53.000000 xcloudforlinux-0.1.0/xcloudClients/__init__.py
--rw-rw-rw-   0        0        0     7579 2024-05-14 15:45:26.000000 xcloudforlinux-0.1.0/xcloudClients/xcloudforlinux.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:46:24.253316 xcloudforlinux-0.1.0/xcloudforlinux.egg-info/
--rw-rw-rw-   0        0        0     2909 2024-05-14 15:46:23.000000 xcloudforlinux-0.1.0/xcloudforlinux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-14 15:46:24.000000 xcloudforlinux-0.1.0/xcloudforlinux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 15:46:23.000000 xcloudforlinux-0.1.0/xcloudforlinux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 15:46:23.000000 xcloudforlinux-0.1.0/xcloudforlinux.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 15:46:23.000000 xcloudforlinux-0.1.0/xcloudforlinux.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 15:51:44.071187 xcloudforlinux-0.2.0/
+-rw-rw-rw-   0        0        0       38 2024-05-14 15:45:57.000000 xcloudforlinux-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2909 2024-05-14 15:51:44.068184 xcloudforlinux-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2574 2024-05-06 06:00:51.000000 xcloudforlinux-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 15:51:44.072186 xcloudforlinux-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-05-14 15:51:01.000000 xcloudforlinux-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:51:43.965184 xcloudforlinux-0.2.0/xcloudforlinux/
+-rw-rw-rw-   0        0        0      166 2024-05-14 15:51:13.000000 xcloudforlinux-0.2.0/xcloudforlinux/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:51:44.061184 xcloudforlinux-0.2.0/xcloudforlinux/resources/
+-rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloudforlinux-0.2.0/xcloudforlinux/resources/XCloudJDBC-2.10.6.7.jar
+-rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloudforlinux-0.2.0/xcloudforlinux/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
+-rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloudforlinux-0.2.0/xcloudforlinux/resources/libthrift-0.9.2.jar
+-rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloudforlinux-0.2.0/xcloudforlinux/resources/log4j-1.2.17.jar
+-rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloudforlinux-0.2.0/xcloudforlinux/resources/lz4-1.3.0.jar
+-rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloudforlinux-0.2.0/xcloudforlinux/resources/slf4j-api-1.7.5.jar
+-rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloudforlinux-0.2.0/xcloudforlinux/resources/slf4j-log4j12-1.7.5.jar
+-rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloudforlinux-0.2.0/xcloudforlinux/resources/slf4j-simple-1.7.5.jar
+-rw-rw-rw-   0        0        0     7579 2024-05-14 15:45:26.000000 xcloudforlinux-0.2.0/xcloudforlinux/xcloudforlinux.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:51:43.992185 xcloudforlinux-0.2.0/xcloudforlinux.egg-info/
+-rw-rw-rw-   0        0        0     2909 2024-05-14 15:51:42.000000 xcloudforlinux-0.2.0/xcloudforlinux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2024-05-14 15:51:43.000000 xcloudforlinux-0.2.0/xcloudforlinux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:51:42.000000 xcloudforlinux-0.2.0/xcloudforlinux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 15:51:42.000000 xcloudforlinux-0.2.0/xcloudforlinux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 15:51:43.000000 xcloudforlinux-0.2.0/xcloudforlinux.egg-info/top_level.txt
```

### Comparing `xcloudforlinux-0.1.0/PKG-INFO` & `xcloudforlinux-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcloudforlinux
-Version: 0.1.0
+Version: 0.2.0
 Summary: 这是一个国信行云数据库并发查询python程序,主要应用于自动通报
 Home-page: https://github.com/bailulue
 Author: bailu
 Author-email: yabailu@chinatelecom.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xcloudforlinux-0.1.0/README.md` & `xcloudforlinux-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.1.0/setup.py` & `xcloudforlinux-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xcloudforlinux',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages(),
     package_data={
         'xcloudforlinux': ['resources/*.jar'],
     },
     include_package_data=True,
     install_requires=[
         'JPype1==1.5.0'
```

### Comparing `xcloudforlinux-0.1.0/xcloudClients/xcloudforlinux.py` & `xcloudforlinux-0.2.0/xcloudforlinux/xcloudforlinux.py`

 * *Files identical despite different names*

### Comparing `xcloudforlinux-0.1.0/xcloudforlinux.egg-info/PKG-INFO` & `xcloudforlinux-0.2.0/xcloudforlinux.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcloudforlinux
-Version: 0.1.0
+Version: 0.2.0
 Summary: 这是一个国信行云数据库并发查询python程序,主要应用于自动通报
 Home-page: https://github.com/bailulue
 Author: bailu
 Author-email: yabailu@chinatelecom.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

