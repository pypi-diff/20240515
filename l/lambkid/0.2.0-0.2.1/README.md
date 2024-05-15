# Comparing `tmp/lambkid-0.2.0.tar.gz` & `tmp/lambkid-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.2.0.tar", last modified: Sat May 11 14:14:15 2024, max compression
+gzip compressed data, was "lambkid-0.2.1.tar", last modified: Wed May 15 08:33:56 2024, max compression
```

## Comparing `lambkid-0.2.0.tar` & `lambkid-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 14:14:15.076256 lambkid-0.2.0/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2094 2024-05-11 14:14:15.075258 lambkid-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 14:14:14.971051 lambkid-0.2.0/docs/
--rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.0/docs/cli.md
--rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.0/docs/csv.md
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.0/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.0/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.0/docs/sshclient.md
--rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.0/docs/utils.md
-drwxrwxrwx   0        0        0        0 2024-05-11 14:14:14.973017 lambkid-0.2.0/lambkid/
--rw-rw-rw-   0        0        0      188 2024-04-25 02:53:27.000000 lambkid-0.2.0/lambkid/__init__.py
--rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.0/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:14:15.054339 lambkid-0.2.0/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.0/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1514 2024-04-29 07:44:19.000000 lambkid-0.2.0/lambkid/libs/log.py
--rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.2.0/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0     7344 2024-05-11 14:13:31.000000 lambkid-0.2.0/lambkid/libs/ssh.py
--rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.0/lambkid/libs/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:14:15.074261 lambkid-0.2.0/lambkid.egg-info/
--rw-rw-rw-   0        0        0     2094 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 14:14:15.076256 lambkid-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1834 2024-05-11 14:13:43.000000 lambkid-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.271175 lambkid-0.2.1/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2094 2024-05-15 08:33:56.269184 lambkid-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.107612 lambkid-0.2.1/docs/
+-rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.1/docs/cli.md
+-rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.1/docs/csv.md
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.1/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.1/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.1/docs/sshclient.md
+-rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.1/docs/utils.md
+drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.110604 lambkid-0.2.1/lambkid/
+-rw-rw-rw-   0        0        0      188 2024-04-25 02:53:27.000000 lambkid-0.2.1/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.1/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.202358 lambkid-0.2.1/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.1/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1514 2024-04-29 07:44:19.000000 lambkid-0.2.1/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.2.1/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     7346 2024-05-15 08:32:56.000000 lambkid-0.2.1/lambkid/libs/ssh.py
+-rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.1/lambkid/libs/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.240257 lambkid-0.2.1/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     2094 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 08:33:56.271175 lambkid-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-05-15 08:32:56.000000 lambkid-0.2.1/setup.py
```

### Comparing `lambkid-0.2.0/LICENSE` & `lambkid-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.0/PKG-INFO` & `lambkid-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.0
+Version: 0.2.1
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.0/README.md` & `lambkid-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.0/docs/log.md` & `lambkid-0.2.1/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.0/docs/sshclient.md` & `lambkid-0.2.1/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.0/lambkid/cli.py` & `lambkid-0.2.1/lambkid/cli.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.0/lambkid/libs/log.py` & `lambkid-0.2.1/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.0/lambkid/libs/minio_client.py` & `lambkid-0.2.1/lambkid/libs/minio_client.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.0/lambkid/libs/ssh.py` & `lambkid-0.2.1/lambkid/libs/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             self.__ssh.connect(hostname=self.__ip, port=self.__port, username=self.__username, password=self.__password,
                                timeout=self.__connect_timeout)
             self.__transport = self.__ssh.get_transport()
             self.__transport.set_keepalive(self.__keep_alive_interval)
             log.info(f" {self.__ip}:{self.__port} | successful to create ssh connect: OK.")
             return True
         except Exception as e:
-            log.error(f" {self.__ip}:{self.__port} | fail create ssh connect: Error.err msg is {str(e)}")
+            log.warning(f" {self.__ip}:{self.__port} | fail create ssh connect: Error.err msg is {str(e)}")
             return False
 
     def __reconnect(self):
         try:
             if self.__ssh:
                 del self.__ssh
         except:
```

### Comparing `lambkid-0.2.0/lambkid/libs/utils.py` & `lambkid-0.2.1/lambkid/libs/utils.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.0/lambkid.egg-info/PKG-INFO` & `lambkid-0.2.1/lambkid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.0
+Version: 0.2.1
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.0/setup.py` & `lambkid-0.2.1/setup.py`

 * *Files identical despite different names*

```diff
@@ -6,15 +6,15 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.2.0",
+    version="0.2.1",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
```

