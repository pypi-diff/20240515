# Comparing `tmp/xtn-tools-pro-1.0.0.1.1.tar.gz` & `tmp/xtn-tools-pro-1.0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtn-tools-pro-1.0.0.1.1.tar", last modified: Wed May 15 09:02:22 2024, max compression
+gzip compressed data, was "dist\xtn-tools-pro-1.0.0.1.2.tar", last modified: Wed May 15 09:08:37 2024, max compression
```

## Comparing `xtn-tools-pro-1.0.0.1.1.tar` & `xtn-tools-pro-1.0.0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 09:02:22.000000 xtn-tools-pro-1.0.0.1.1/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.1.1/LICENSE
--rw-rw-rw-   0        0        0      287 2024-05-15 09:02:22.000000 xtn-tools-pro-1.0.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 09:02:22.000000 xtn-tools-pro-1.0.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1271 2024-05-15 09:02:17.000000 xtn-tools-pro-1.0.0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:02:22.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/
--rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:02:22.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/db/
--rw-rw-rw-   0        0        0     5573 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/db/MongoDB.py
--rw-rw-rw-   0        0        0    13373 2024-05-12 14:20:54.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/db/MysqlDB.py
--rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/db/RedisDB.py
--rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:02:22.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/proxy/
--rw-rw-rw-   0        0        0    10223 2024-05-15 09:02:17.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/proxy/XiaoXiangProxy.py
--rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/proxy/__init__.py
--rw-rw-rw-   0        0        0     8703 2024-05-13 14:02:38.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/proxy/proxy.py
--rw-rw-rw-   0        0        0      542 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:02:22.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/
--rw-rw-rw-   0        0        0      418 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/__init__.py
--rw-rw-rw-   0        0        0     3190 2024-05-15 08:10:00.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/crypto.py
--rw-rw-rw-   0        0        0     1509 2024-05-12 16:32:12.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/file_utils.py
--rw-rw-rw-   0        0        0     3773 2024-05-15 07:34:46.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/helpers.py
--rw-rw-rw-   0        0        0     8139 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/log.py
--rw-rw-rw-   0        0        0     1657 2024-05-12 12:05:16.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/retry.py
--rw-rw-rw-   0        0        0     6263 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/sql.py
--rw-rw-rw-   0        0        0     4859 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/time_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:02:22.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro.egg-info/
--rw-rw-rw-   0        0        0      287 2024-05-15 09:02:21.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-05-15 09:02:22.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:02:21.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-15 09:02:21.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-15 09:02:21.000000 xtn-tools-pro-1.0.0.1.1/xtn_tools_pro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      287 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2024-05-15 09:08:31.000000 xtn-tools-pro-1.0.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/
+-rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/db/
+-rw-rw-rw-   0        0        0     5573 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/db/MongoDB.py
+-rw-rw-rw-   0        0        0    13373 2024-05-12 14:20:54.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/db/MysqlDB.py
+-rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/db/RedisDB.py
+-rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/proxy/
+-rw-rw-rw-   0        0        0    10720 2024-05-15 09:08:13.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/proxy/XiaoXiangProxy.py
+-rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/proxy/__init__.py
+-rw-rw-rw-   0        0        0     8703 2024-05-13 14:02:38.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/proxy/proxy.py
+-rw-rw-rw-   0        0        0      542 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/
+-rw-rw-rw-   0        0        0      418 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/__init__.py
+-rw-rw-rw-   0        0        0     3190 2024-05-15 08:10:00.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/crypto.py
+-rw-rw-rw-   0        0        0     1509 2024-05-12 16:32:12.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/file_utils.py
+-rw-rw-rw-   0        0        0     3773 2024-05-15 07:34:46.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/helpers.py
+-rw-rw-rw-   0        0        0     8139 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/log.py
+-rw-rw-rw-   0        0        0     1657 2024-05-12 12:05:16.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/retry.py
+-rw-rw-rw-   0        0        0     6263 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/sql.py
+-rw-rw-rw-   0        0        0     4859 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/time_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 09:08:37.000000 xtn-tools-pro-1.0.0.1.2/xtn_tools_pro.egg-info/top_level.txt
```

### Comparing `xtn-tools-pro-1.0.0.1.1/setup.py` & `xtn-tools-pro-1.0.0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtn-tools-pro",  # 模块名称
-    version="1.0.0.1.1",  # 版本
+    version="1.0.0.1.2",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/db/MongoDB.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/db/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/db/MysqlDB.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/db/MysqlDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/db/RedisDB.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/db/RedisDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/proxy/XiaoXiangProxy.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/proxy/XiaoXiangProxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,16 +159,23 @@
                 while True:
                     # 检查代理
                     self.__check_proxy()
                     # 获取小象代理
                     self.__get_api_proxy()
                     time.sleep(1)
                     # 判断时间是否超过当前23:59分时间戳
-                    if get_time_now_timestamp(is_time_10=True) >= self.__now_day59_timestamp:
-                        self.__log("时间23:59，结束循环，{t}".format(t=int(time.time())))
+                    t_a = get_time_now_timestamp(is_time_10=True)
+                    if t_a >= self.__now_day59_timestamp:
+                        self.__log(
+                            "时间23:59，结束循环，{t} {a} {a_v} {b} {b_v}".format(t=int(time.time()),
+                                                                          a=type(t_a),
+                                                                          a_v=t_a,
+                                                                          b=type(self.__now_day59_timestamp),
+                                                                          b_v=self.__now_day59_timestamp)
+                        )
                         break
             except Exception as eee:
                 self.__log("程序异常报错:{eee}".format(eee=eee))
                 # self.__del__()
 
     def get_proxy(self):
         """
```

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/proxy/proxy.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/tools.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/tools.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/crypto.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/file_utils.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/helpers.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/log.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/log.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/retry.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/retry.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/sql.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/sql.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro/utils/time_utils.py` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.1/xtn_tools_pro.egg-info/SOURCES.txt` & `xtn-tools-pro-1.0.0.1.2/xtn_tools_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

