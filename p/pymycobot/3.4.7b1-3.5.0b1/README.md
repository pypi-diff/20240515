# Comparing `tmp/pymycobot-3.4.7b1.tar.gz` & `tmp/pymycobot-3.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.4.7b1.tar", last modified: Sat May 11 02:02:17 2024, max compression
+gzip compressed data, was "pymycobot-3.5.0b1.tar", last modified: Wed May 15 03:50:54 2024, max compression
```

## Comparing `pymycobot-3.4.7b1.tar` & `pymycobot-3.5.0b1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 02:02:17.635812 pymycobot-3.4.7b1/
--rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/LICENSE
--rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/MANIFEST.in
--rw-rw-rw-   0        0        0    63944 2024-05-11 02:02:17.633812 pymycobot-3.4.7b1/PKG-INFO
--rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.4.7b1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 02:02:17.593803 pymycobot-3.4.7b1/pymycobot/
--rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     2171 2024-05-11 02:02:09.000000 pymycobot-3.4.7b1/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.4.7b1/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    24941 2024-04-25 03:16:52.000000 pymycobot-3.4.7b1/pymycobot/common.py
--rw-rw-rw-   0        0        0    12842 2024-05-11 02:01:09.000000 pymycobot-3.4.7b1/pymycobot/elephantrobot.py
--rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/error.py
--rw-rw-rw-   0        0        0    42593 2024-04-18 11:13:01.000000 pymycobot-3.4.7b1/pymycobot/generate.py
--rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.4.7b1/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.4.7b1/pymycobot/log.py
--rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.4.7b1/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mecharmsocket.py
--rw-rw-rw-   0        0        0     7695 2024-04-12 11:33:10.000000 pymycobot-3.4.7b1/pymycobot/mercury.py
--rw-rw-rw-   0        0        0    16855 2024-04-23 03:10:49.000000 pymycobot-3.4.7b1/pymycobot/mercury_api.py
--rw-rw-rw-   0        0        0     6460 2024-04-25 03:16:52.000000 pymycobot-3.4.7b1/pymycobot/mercurychassis.py
--rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.4.7b1/pymycobot/mercurysocket.py
--rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.4.7b1/pymycobot/myagv.py
--rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    16475 2024-05-07 11:28:46.000000 pymycobot-3.4.7b1/pymycobot/myarm_api.py
--rw-rw-rw-   0        0        0      273 2024-04-22 09:29:51.000000 pymycobot-3.4.7b1/pymycobot/myarmc.py
--rw-rw-rw-   0        0        0     3186 2024-04-18 11:13:01.000000 pymycobot-3.4.7b1/pymycobot/myarmm.py
--rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/myarmsocket.py
--rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4544 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0    87447 2024-05-11 02:01:09.000000 pymycobot-3.4.7b1/pymycobot/mycobotpro630.py
--rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.4.7b1/pymycobot/public.py
--rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.4.7b1/pymycobot/robot_limit.json
--rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.4.7b1/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:02:17.632811 pymycobot-3.4.7b1/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    63944 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1093 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.4.7b1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 02:02:17.635812 pymycobot-3.4.7b1/setup.cfg
--rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.4.7b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:02:17.629810 pymycobot-3.4.7b1/tests/
--rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/tests/test_api.py
--rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/tests/test_generator.py
--rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/tests/test_socket.py
--rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 03:50:54.556720 pymycobot-3.5.0b1/
+-rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/MANIFEST.in
+-rw-rw-rw-   0        0        0    63942 2024-05-15 03:50:54.555721 pymycobot-3.5.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.5.0b1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 03:50:54.519817 pymycobot-3.5.0b1/pymycobot/
+-rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     2171 2024-05-15 03:49:56.000000 pymycobot-3.5.0b1/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.5.0b1/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    25589 2024-05-14 06:55:47.000000 pymycobot-3.5.0b1/pymycobot/common.py
+-rw-rw-rw-   0        0        0    12842 2024-05-11 02:01:09.000000 pymycobot-3.5.0b1/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/error.py
+-rw-rw-rw-   0        0        0    42593 2024-05-11 08:44:46.000000 pymycobot-3.5.0b1/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.5.0b1/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.5.0b1/pymycobot/log.py
+-rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.5.0b1/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mecharmsocket.py
+-rw-rw-rw-   0        0        0    14353 2024-05-15 03:44:23.000000 pymycobot-3.5.0b1/pymycobot/mercury.py
+-rw-rw-rw-   0        0        0    26397 2024-05-15 03:44:49.000000 pymycobot-3.5.0b1/pymycobot/mercury_api.py
+-rw-rw-rw-   0        0        0     6460 2024-04-25 03:16:52.000000 pymycobot-3.5.0b1/pymycobot/mercurychassis.py
+-rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.5.0b1/pymycobot/mercurysocket.py
+-rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.5.0b1/pymycobot/myagv.py
+-rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    16475 2024-05-07 11:28:46.000000 pymycobot-3.5.0b1/pymycobot/myarm_api.py
+-rw-rw-rw-   0        0        0      273 2024-04-22 09:29:51.000000 pymycobot-3.5.0b1/pymycobot/myarmc.py
+-rw-rw-rw-   0        0        0     3186 2024-04-18 11:13:01.000000 pymycobot-3.5.0b1/pymycobot/myarmm.py
+-rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/myarmsocket.py
+-rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4544 2024-05-13 10:58:22.000000 pymycobot-3.5.0b1/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0    87447 2024-05-11 02:01:09.000000 pymycobot-3.5.0b1/pymycobot/mycobotpro630.py
+-rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.5.0b1/pymycobot/public.py
+-rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.5.0b1/pymycobot/robot_limit.json
+-rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.5.0b1/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 03:50:54.554722 pymycobot-3.5.0b1/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    63942 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1093 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.5.0b1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 03:50:54.557721 pymycobot-3.5.0b1/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.5.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 03:50:54.552724 pymycobot-3.5.0b1/tests/
+-rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/tests/test_api.py
+-rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/tests/test_generator.py
+-rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/tests/test_socket.py
+-rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/tests/test_utils.py
```

### Comparing `pymycobot-3.4.7b1/LICENSE` & `pymycobot-3.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/PKG-INFO` & `pymycobot-3.5.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.7b1
+Version: 3.5.0b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -1594,15 +1594,15 @@
 
 ### Client
 
 ```python
 # demo
 from pymycobot import MyCobotSocket
 # Port 9000 is used by default
-mc = MyCobotSocket("192.168.10.10","9000")
+mc = MyCobotSocket("192.168.10.10",9000)
 
 res = mc.get_angles()
 print(res)
 
 mc.send_angles([0,0,0,0,0,0],20)
 ...
```

### Comparing `pymycobot-3.4.7b1/README.md` & `pymycobot-3.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/Interface.py` & `pymycobot-3.5.0b1/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/__init__.py` & `pymycobot-3.5.0b1/pymycobot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.4.7b1"
+__version__ = "3.5.0b1"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.4.7b1/pymycobot/bluet.py` & `pymycobot-3.5.0b1/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/common.py` & `pymycobot-3.5.0b1/pymycobot/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 
     # JOG MODE AND OPERATION
     JOG_ANGLE = 0x30
     JOG_ABSOLUTE = 0x31
     JOG_COORD = 0x32
     JOG_INCREMENT = 0x33
     JOG_STOP = 0x34
+    JOG_INCREMENT_COORD = 0x34
     
     COBOTX_GET_SOLUTION_ANGLES = 0x35
     COBOTX_SET_SOLUTION_ANGLES = 0x36
     
     SET_ENCODER = 0x3A
     GET_ENCODER = 0x3B
     SET_ENCODERS = 0x3C
@@ -433,21 +434,23 @@
 
         return processed_args
 
     def _is_frame_header(self, data, pos1, pos2):
         return data[pos1] == ProtocolCode.HEADER and data[pos2] == ProtocolCode.HEADER
 
     def _process_received(self, data, genre, arm=6):
-        if not data:
-            return []
         if genre == 177:
             data = str(data)[2:-1].split(": ")
             return data[1][0:-9], data[-1]
-        if not data:
+        elif not data:
             return []
+        elif data == b'\xfe\xfe\x04[\x01\r\x87':
+            # 水星到位反馈
+            return 1
+        
         data = bytearray(data)
         data_len = len(data)
         # Get valid header: 0xfe0xfe
         header_i, header_j = 0, 1
         while header_j < data_len - 4:
             if self._is_frame_header(data, header_i, header_j):
                 if arm in [6, 7, 14, 8]:
@@ -603,21 +606,22 @@
             for i in range(len(res)):
                 res[i] /= 1000
         return res
 
     def _process_single(self, data):
         return data[0] if data else -1
 
-def check_python_version():
-    if sys.version_info.major == 2:
-        return 2
-    elif sys.version_info.major == 3:
-        return 3
-    else:
-        return -1
+    @staticmethod
+    def check_python_version():
+        if sys.version_info.major == 2:
+            return 2
+        elif sys.version_info.major == 3:
+            return 3
+        else:
+            return -1
 
 
 def write(self, command, method=None):
     if len(command) > 3 and command[3] == 176 and len(command) > 5:
         command = "'" + command[4] + "'" + "(" + command[5] + ")"
         command = command.encode()
     if method == "socket":
@@ -663,14 +667,16 @@
         wait_time = timeout
     if _class in ["Mercury", "MercurySocket"]:
         if genre == ProtocolCode.POWER_ON:
             wait_time = 8
         elif genre in [ProtocolCode.POWER_OFF, ProtocolCode.RELEASE_ALL_SERVOS, ProtocolCode.FOCUS_ALL_SERVOS,
                        ProtocolCode.RELEASE_SERVO, ProtocolCode.FOCUS_SERVO, ProtocolCode.STOP]:
             wait_time = 3
+        elif genre in [ProtocolCode.SEND_ANGLE, ProtocolCode.SEND_ANGLES, ProtocolCode.SEND_COORD, ProtocolCode.SEND_COORDS, ProtocolCode.JOG_ANGLE, ProtocolCode.JOG_COORD, ProtocolCode.JOG_INCREMENT, ProtocolCode.JOG_INCREMENT_COORD, ProtocolCode.COBOTX_SET_SOLUTION_ANGLES]:
+            wait_time = 300
     if method is not None:
         if genre == 177:
             while True:
                 data = self.sock.recv(1024)
                 if b"password" in data:
                     break
         elif genre == 192:
@@ -705,15 +711,19 @@
             time.sleep(0.1)
             if self._serial_port.inWaiting() > 0:
                 datas = self._serial_port.read(self._serial_port.inWaiting())
             return datas
         elif genre == ProtocolCode.GET_ACCEI_DATA:
             wait_time = 1
         while True and time.time() - t < wait_time:
+            if genre != ProtocolCode.STOP and self.is_stop:
+                break
+            # print(genre)
             data = self._serial_port.read()
+            print(genre, data)
             k += 1
             if _class in ["Mercury", "MercurySocket"]:
                 if data_len == 3:
                     datas += data
                     crc = self._serial_port.read(2)
                     if DataProcessor.crc_check(datas) == [v for v in crc]:
                         datas+=crc
@@ -741,15 +751,16 @@
                     if k - 1 == pre:
                         datas += data
                     else:
                         datas = b"\xfe"
                         pre = k
         else:
             datas = b''
-        if check_python_version() == 2:
+        print("datas", datas)
+        if DataProcessor.check_python_version() == 2:
             command_log = ""
             for d in datas:
                 command_log += hex(ord(d))[2:] + " "
             self.log.debug("_read : {}".format(command_log))
         else:
             command_log = ""
             for d in datas:
```

### Comparing `pymycobot-3.4.7b1/pymycobot/elephantrobot.py` & `pymycobot-3.5.0b1/pymycobot/elephantrobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/error.py` & `pymycobot-3.5.0b1/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/generate.py` & `pymycobot-3.5.0b1/pymycobot/generate.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/log.py` & `pymycobot-3.5.0b1/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mecharmsocket.py` & `pymycobot-3.5.0b1/pymycobot/mecharmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mercury.py` & `pymycobot-3.5.0b1/pymycobot/mercurysocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 # coding=utf-8
 
 import time
+import socket
 import threading
 
 from pymycobot.mercury_api import MercuryCommandGenerator
 from pymycobot.common import ProtocolCode, write, read
 from pymycobot.error import calibration_parameters
 
 
-class Mercury(MercuryCommandGenerator):
+class MercurySocket(MercuryCommandGenerator):
     _write = write
     _read = read
-    def __init__(self, port, baudrate="115200", timeout=0.1, debug=False):
+    def __init__(self, ip, netport=9000, debug=False):
         """
         Args:
-            port     : port string
-            baudrate : baud rate string, default '115200'
-            timeout  : default 0.1
-            debug    : whether show debug info
+            ip: Server ip
+            netport: Server port(default 9000)
         """
-        super(Mercury, self).__init__(debug)
+        super(MercurySocket, self).__init__(debug)
         self.calibration_parameters = calibration_parameters
-        import serial
-
-        self._serial_port = serial.Serial()
-        self._serial_port.port = port
-        self._serial_port.baudrate = baudrate
-        self._serial_port.timeout = timeout
-        self._serial_port.rts = False
-        self._serial_port.open()
+        self.SERVER_IP = ip
+        self.SERVER_PORT = netport
+        self.sock = self.connect_socket()
         self.lock = threading.Lock()
-        self.has_reply_command = []
-        
+
+    def connect_socket(self):
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.connect((self.SERVER_IP, self.SERVER_PORT))
+        return sock
         
 
     def _mesg(self, genre, *args, **kwargs):
         """
 
         Args:
             genre: command type (Command)
             *args: other data.
                    It is converted to octal by default.
                    If the data needs to be encapsulated into hexadecimal,
                    the array is used to include them. (Data cannot be nested)
             **kwargs: support `has_reply`
                 has_reply: Whether there is a return value to accept.
         """
-        real_command, has_reply = super(Mercury, self)._mesg(genre, *args, **kwargs)
+        real_command, has_reply = super(MercurySocket, self)._mesg(genre, *args, **kwargs)
         with self.lock:
-            self._write(self._flatten(real_command))
+            self._write(self._flatten(real_command), "socket")
 
             if has_reply:
-                data = self._read(genre, _class=self.__class__.__name__)
+                data = self._read(genre, _class=self.__class__.__name__, method='socket')
                 if genre == ProtocolCode.SET_SSID_PWD:
                     return None
                 res = self._process_received(data, genre, 14)
                 if res == []:
                     return None
                 if genre in [
                     ProtocolCode.ROBOT_VERSION,
@@ -139,39 +136,27 @@
                             for i in range(1, len(res)):
                                 if res[i] == 1:
                                     r.append(i)
                     return r
                 elif genre in [ProtocolCode.COBOTX_GET_ANGLE, ProtocolCode.COBOTX_GET_SOLUTION_ANGLES]:
                         return self._int2angle(res[0])
                 elif genre == ProtocolCode.MERCURY_ROBOT_STATUS:
-                    if self._serial_port.port == "/dev/ttyTHS0":
-                        i = 9
-                        for i in range(9, len(res)):
-                            if res[i] != 0:
-                                data = bin(res[i])[2:]
-                                res[i] = []
-                                while len(data) != 16:
-                                    data = "0"+data
-                                for j in range(16):
-                                    if data[j] != "0":
-                                        res[i].append(15-j)
-                        return res
-                    else:
-                        for i in range(10, len(res)):
-                            if res[i] != 0:
-                                data = bin(res[i])[2:]
-                                res[i] = []
-                                while len(data) != 16:
-                                    data = "0"+data
-                                for j in range(16):
-                                    if data[j] != "0":
-                                        res[i].append(15-j)
-                        return res
+                    i = 9
+                    for i in range(9, len(res)):
+                        if res[i] != 0:
+                            data = bin(res[i])[2:]
+                            res[i] = []
+                            while len(data) != 16:
+                                data = "0"+data
+                            for j in range(16):
+                                if data[j] != "0":
+                                    res[i].append(15-j)
+                    return res
                 else:
                     return res
             return None
     
     def open(self):
-        self._serial_port.open()
+        self.sock = self.connect_socket()
         
     def close(self):
-        self._serial_port.close()
+        self.sock.close()
```

### Comparing `pymycobot-3.4.7b1/pymycobot/mercury_api.py` & `pymycobot-3.5.0b1/pymycobot/mybuddy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,485 +1,439 @@
-
 # coding=utf-8
 
-import sys
-import logging
+from __future__ import division
 import time
+import math
+import logging
+import threading
+import struct
 
 from pymycobot.log import setup_logging
+from pymycobot.Interface import MyBuddyCommandGenerator
+from pymycobot.common import ProtocolCode, write, read
 from pymycobot.error import calibration_parameters
-from pymycobot.generate import CommandGenerator
-from pymycobot.generate import ProtocolCode
 
 
-class MercuryCommandGenerator(CommandGenerator):
-    def __init__(self, debug=False):
-        super(MercuryCommandGenerator, self).__init__(debug)
-        self.calibration_parameters = calibration_parameters
-        
-    def set_solution_angles(self, angle, speed):
-        """Set zero space deflection angle value
+class MyBuddy(MyBuddyCommandGenerator):
+    """MyCobot Python API Serial communication class.
 
-        Args:
-            angle: Angle of joint 1. The angle range is -90 ~ 90
-            speed: 1 - 100.
-        """
-        self.calibration_parameters(
-            class_name=self.__class__.__name__, speed=speed, solution_angle=angle
-        )
-        return self._mesg(
-            ProtocolCode.COBOTX_SET_SOLUTION_ANGLES, [self._angle2int(angle)], speed
-        )
-
-    def get_solution_angles(self):
-        """Get zero space deflection angle value"""
-        return self._mesg(ProtocolCode.COBOTX_GET_SOLUTION_ANGLES, has_reply=True)
-
-    def write_move_c(self, transpoint, endpoint, speed):
-        """_summary_
-
-        Args:
-            transpoint (list): Arc passing point coordinates
-            endpoint (list): Arc end point coordinates
-            speed (int): 1 ~ 100
-        """
-        start = []
-        end = []
-        for index in range(6):
-            if index < 3:
-                start.append(self._coord2int(transpoint[index]))
-                end.append(self._coord2int(endpoint[index]))
-            else:
-                start.append(self._angle2int(transpoint[index]))
-                end.append(self._angle2int(endpoint[index]))
-        return self._mesg(ProtocolCode.WRITE_MOVE_C, start, end, speed)
-
-    def focus_all_servos(self):
-        """Lock all joints"""
-        return self._mesg(ProtocolCode.FOCUS_ALL_SERVOS, has_reply=True)
+    Supported methods:
 
-    def go_home(self, robot, speed=20):
-        """Control the machine to return to the zero position.
-        
-        Args:
-            robot (int): 
-                1 - Mercury A1 
-                2 - Mercury B1 or X1
-            speed (int): 1 ~ 100
-        Return:
-            1 : All motors return to zero position.
-            0 : failed.
-        """
-        if robot == 1:
-            return self.sync_send_angles([0, 0, 0, 0, 0, 90, 0], speed)
-        else:
-            self.send_angle(11, 0, speed)
-            self.send_angle(12, 0, speed)
-            self.send_angle(13, 0, speed)
-            return self.sync_send_angles([0, 0, 0, 0, 0, 90, 0], speed)
+        # Overall status
+            Look at parent class: `CommandGenerator`.
 
-    def get_angle(self, joint_id):
-        """Get single joint angle
+        # MDI mode and operation
+            get_radians()
+            send_radians()
+            sync_send_angles() *
+            sync_send_coords() *
+            Other look at parent class: `CommandGenerator`.
 
-        Args:
-            joint_id (int): 1 ~ 7 or 11 ~ 13.
-        """
-        self.calibration_parameters(class_name=self.__class__.__name__, id=joint_id)
-        return self._mesg(ProtocolCode.COBOTX_GET_ANGLE, joint_id, has_reply=True)
-    
-    def servo_restore(self, joint_id):
-        """Abnormal recovery of joints
+        # JOG mode and operation
+            Look at parent class: `CommandGenerator`.
 
-        Args:
-            joint_id (int): Joint ID.
-                arm : 1 ~ 7 
-                waist : 13
-                All joints: 254
-        """
-        self.calibration_parameters(
-            class_name=self.__class__.__name__, servo_restore=joint_id
-        )
-        self._mesg(ProtocolCode.SERVO_RESTORE, joint_id)
-        
-    def set_error_detect_mode(self, mode):
-        """Set error detection mode. Turn off without saving, default to open state
-        
-        Return:
-            mode : 0 - close 1 - open.
+        # Running status and Settings
+            Look at parent class: `CommandGenerator`.
+
+        # Servo control
+            Look at parent class: `CommandGenerator`.
+
+        # Atom IO
+            Look at parent class: `CommandGenerator`.
+
+        # Basic
+            Look at parent class: `CommandGenerator`.
+
+        # Other
+            wait() *
+    """
+
+    def __init__(self, port, baudrate="115200", timeout=0.1, debug=False):
         """
-        self.calibration_parameters(
-            class_name=self.__class__.__name__, mode=mode
-        )
-        self._mesg(ProtocolCode.SET_ERROR_DETECT_MODE, mode)
-        
-    def get_error_detect_mode(self):
-        """Set error detection mode"""
-        return self._mesg(ProtocolCode.GET_ERROR_DETECT_MODE, has_reply=True)
-    
-    def sync_send_angles(self, degrees, speed, timeout=15):
-        """Send the angle in synchronous state and return when the target point is reached
-            
         Args:
-            degrees: a list of degree values(List[float]), length 6.
-            speed: (int) 0 ~ 100
-            timeout: default 7s.
+            port     : port string
+            baudrate : baud rate string, default '115200'
+            timeout  : default 0.1
+            debug    : whether show debug info
         """
+        super(MyBuddy, self).__init__(debug)
+        self.calibration_parameters = calibration_parameters
+        import serial
+        self._serial_port = serial.Serial()
+        self._serial_port.port = port
+        self._serial_port.baudrate = baudrate
+        self._serial_port.timeout = timeout
+        self._serial_port.rts = False
+        self._serial_port.open()
+        self.lock = threading.Lock()
+
+    _write = write
+    
+    def _read(self):
+        datas = b''
+        data_len = -1
+        real_data = b''
+        check_digit = 0
+        k = 0
+        pre = 0
         t = time.time()
-        self.send_angles(degrees, speed)
-        while time.time() - t < timeout:
-            f = self.is_in_position(degrees, 0)
-            if f == 1:
-                return 1
-            time.sleep(0.1)
-        return 0
+        while True and time.time() - t < 0.1:
+            try:
+                data = self._serial_port.read()
+                k+=1
+                if data_len == 1:
+                    datas += data
+                    if struct.pack("B", check_digit & 0xff) == data:
+                        break
+                elif len(datas) == 3:
+                    data_len = struct.unpack("b",data)[0]
+                    datas += data
+                elif len(datas)>=2:
+                    datas += data
+                    if len(datas) == 5: 
+                        check_digit += self._decode_int8(data)
+                    elif len(datas)>5:
+                        real_data += data
+                    if real_data != b'':
+                        check_digit += self._decode_int8(real_data)
+                        real_data = b''
+                    data_len -= 1
+                elif data == b'\xfe':
+                    if datas == b'':
+                        datas += data
+                        pre = k
+                    else:
+                        if k-1 == pre:
+                            datas += data
+                        else:
+                            datas = b'\xfe'
+                            pre = k  
+            except:
+                break
+        else:
+            datas = b''
+        self.log.debug("_read: {}".format(datas))
+        return datas
+    
+    def _mesg(self, genre, *args, **kwargs):
+        """
+
+        Args:
+            genre: command type (Command)
+            *args: other data.
+                   It is converted to octal by default.
+                   If the data needs to be encapsulated into hexadecimal,
+                   the array is used to include them. (Data cannot be nested)
+            **kwargs: support `has_reply`
+                has_reply: Whether there is a return value to accept.
+        """
+        real_command, has_reply = super(
+            MyBuddy, self)._mesg(genre, *args, **kwargs)
+        with self.lock:
+            self._write(self._flatten(real_command))
+
+            if has_reply:
+                data = self._read()
+                res = self._process_received(data, genre, arm=12)
+                if res == []:
+                    return None
+                if genre in [
+                    ProtocolCode.ROBOT_VERSION,
+                    ProtocolCode.SOFTWARE_VERSION,
+                    ProtocolCode.GET_ROBOT_ID,
+                    ProtocolCode.IS_POWER_ON,
+                    ProtocolCode.IS_CONTROLLER_CONNECTED,
+                    ProtocolCode.IS_PAUSED,  # TODO have bug: return b''
+                    ProtocolCode.IS_IN_POSITION,
+                    ProtocolCode.IS_MOVING,
+                    ProtocolCode.IS_SERVO_ENABLE,
+                    ProtocolCode.IS_ALL_SERVO_ENABLE,
+                    ProtocolCode.GET_SERVO_DATA,
+                    ProtocolCode.GET_DIGITAL_INPUT,
+                    ProtocolCode.GET_GRIPPER_VALUE,
+                    ProtocolCode.IS_GRIPPER_MOVING,
+                    ProtocolCode.GET_SPEED,
+                    ProtocolCode.GET_ENCODER,
+                    ProtocolCode.GET_BASIC_INPUT,
+                    ProtocolCode.GET_TOF_DISTANCE,
+                    ProtocolCode.GET_END_TYPE,
+                    ProtocolCode.GET_MOVEMENT_TYPE,
+                    ProtocolCode.GET_REFERENCE_FRAME,
+                    ProtocolCode.GET_FRESH_MODE,
+                    ProtocolCode.SetHTSGripperTorque,
+                    ProtocolCode.GetHTSGripperTorque,
+                    ProtocolCode.GetGripperProtectCurrent,
+                    ProtocolCode.InitGripper,
+                    ProtocolCode.SET_FOUR_PIECES_ZERO
+                    # ProtocolCode.GET_SERVO_CURRENTS
+                ]:
+                    return self._process_single(res)
+                elif genre in [ProtocolCode.GET_ANGLES]:
+                    return [self._int2angle(angle) for angle in res]
+                elif genre in [ProtocolCode.GET_ANGLE]:
+                    return self._int2angle(res[0]) if res else None
+                elif genre in [ProtocolCode.GET_COORD]:
+                    if real_command[5] < 4:
+                        if real_command[2] == 3:
+                            return self._int2angle(res[0]) if res else None
+                        return self._int2coord(res[0]) if res else None
+                    else:
+                        return self._int2angle(res[0]) if res else None
+                elif genre in [ProtocolCode.GET_ALL_BASE_COORDS, ProtocolCode.GET_COORDS, ProtocolCode.GET_TOOL_REFERENCE, ProtocolCode.GET_WORLD_REFERENCE, ProtocolCode.GET_BASE_COORDS, ProtocolCode.GET_BASE_COORD, ProtocolCode.BASE_TO_SINGLE_COORDS]:
+                    if res:
+                        r = [] 
+                        for idx in range(3):
+                            r.append(self._int2coord(res[idx]))
+                        for idx in range(3, 6):
+                            r.append(self._int2angle(res[idx]))
+                        if len(res) == 12:
+                            r1 = []
+                            for idx in range(6, 9):
+                                r1.append(self._int2coord(res[idx]))
+                            for idx in range(9, 12):
+                                r1.append(self._int2angle(res[idx]))
+                            return [r, r1]
+                        return r
+                    else:
+                        return res
+                elif genre in [ProtocolCode.GET_JOINT_MAX_ANGLE, ProtocolCode.GET_JOINT_MIN_ANGLE]:
+                    return self._int2coord(res[0])
+                elif genre in [ProtocolCode.GET_SERVO_VOLTAGES, ProtocolCode.COLLISION]:
+                    return [self._int2coord(angle) for angle in res]
+                else:
+                    return res
+            return None
 
-    def sync_send_coords(self, coords, speed, mode=None, timeout=15):
-        """Send the coord in synchronous state and return when the target point is reached
+    def get_radians(self, id):
+        """Get the radians of all joints
+
+        Args: 
+            id: 1/2 (L/R)
             
-        Args:
-            coords: a list of coord values(List[float])
-            speed: (int) 0 ~ 100
-            mode: (int): 0 - angular（default）, 1 - linear
-            timeout: default 7s.
+        Return:
+            list: A list of float radians [radian1, ...]
         """
-        t = time.time()
-        self.send_coords(coords, speed, mode)
-        while time.time() - t < timeout:
-            if self.is_in_position(coords, 1) == 1:
-                return 1
-            time.sleep(0.1)
-        return 0
-        
-    def get_base_coords(self):
-        """get base coords"""
-        return self._mesg(ProtocolCode.MERCURY_GET_BASE_COORDS, has_reply=True)
-    
-    def send_base_coord(self, axis, coord, speed):
-        """_summary_
+        angles = self._mesg(ProtocolCode.GET_ANGLES, id, has_reply=True)
+        return [round(angle * (math.pi / 180), 3) for angle in angles]
 
-        Args:
-            axis (_type_): _description_
-            coord (_type_): _description_
-            speed (_type_): _description_
-        """
-        if axis < 4:
-            coord = self._coord2int(coord)
-        else:
-            coord = self._angle2int(coord)
-        return self._mesg(ProtocolCode.MERCURY_SET_BASE_COORD, axis, [coord], speed)
-    
-    def send_base_coords(self, coords, speed):
-        """_summary_
+    def send_radians(self, id, radians, speed):
+        """Send the radians of all joints to robot arm
 
         Args:
-            coords (_type_): _description_
-            speed (_type_): _description_
+            id: 1/2 (L/R).
+            radians: a list of radian values( List[float]), length 6
+            speed: (int )0 ~ 100
         """
-        coord_list = []
-        for idx in range(3):
-            coord_list.append(self._coord2int(coords[idx]))
-        for angle in coords[3:]:
-            coord_list.append(self._angle2int(angle))
-        return self._mesg(ProtocolCode.MERCURY_SET_BASE_COORDS, coord_list, speed)
-    
-    def jog_base_coord(self, axis, direction, speed):
-        """_summary_
+        # calibration_parameters(len6=radians, speed=speed)
+        degrees = [self._angle2int(radian * (180 / math.pi))
+                   for radian in radians]
+        return self._mesg(ProtocolCode.SEND_ANGLES, id, degrees, speed)
 
-        Args:
-            axis (_type_): _description_
-            direction (_type_): _description_
-            speed (_type_): _description_
-        """
-        return self._mesg(ProtocolCode.MERCURY_JOG_BASE_COORD, axis, direction, speed)
-    
-    def drag_teach_save(self):
-        """Start recording the dragging teaching point. In order to show the best sports effect, the recording time should not exceed 90 seconds."""
-        return self._mesg(ProtocolCode.MERCURY_DRAG_TECH_SAVE)
-    
-    def drag_teach_execute(self):
-        """Start dragging the teaching point and only execute it once."""
-        return self._mesg(ProtocolCode.MERCURY_DRAG_TECH_EXECUTE)
-    
-    def drag_teach_pause(self):
-        """Pause recording of dragging teaching point"""
-        self._mesg(ProtocolCode.MERCURY_DRAG_TECH_PAUSE)
+    # Basic for raspberry pi.
+    def set_gpio_init_mode(self, mode = 1):
+        """import RPiGPIO,Init GPIO mode
         
-    def is_gripper_moving(self, mode=None):
-        """Judge whether the gripper is moving or not
-        
-        Args:
-            mode: 1 - pro gripper(default)  2 - Parallel gripper
+            Args:
+                mode(int):0/1
+                0 = BCM
+                1 = BOAND
+        """
+        import RPi.GPIO as GPIO  # type: ignore
+        self.gpio = GPIO
+        if mode == 0:
+            self.gpio.setmode(GPIO.BCM)
+        else:
+            self.gpio.setmode(GPIO.BOAND)
 
-        Returns:
-            0 - not moving
-            1 - is moving
-            -1- error data
-        """
-        if mode:
-            return self._mesg(ProtocolCode.IS_GRIPPER_MOVING, mode, has_reply=True)
-        return self._mesg(ProtocolCode.IS_GRIPPER_MOVING, has_reply=True)
-    
-    def set_gripper_enabled(self, value):
-        """Pro adaptive gripper enable setting
+    def set_gpio_setup(self, pin_no, mode):
+        """Init GPIO module, and set BCM mode. 
 
         Args:
-            value (int): 
-                1 : enable
-                0 : release
-        """
-        self.calibration_parameters(class_name=self.__class__.__name__, value=value)
-        return self._mesg(ProtocolCode.SET_GRIPPER_ENABLED, value)
-    
-    def is_btn_clicked(self):
-        """Check if the end button has been pressed.
-        
-        Return:
-            1 : pressed.
-            0 : not pressed.
-        """
-        return self._mesg(ProtocolCode.IS_BTN_CLICKED, has_reply=True)
-        
-    def tool_serial_restore(self):
-        """485 factory reset
-        """
-        return self._mesg(ProtocolCode.TOOL_SERIAL_RESTORE)
-    
-    def tool_serial_ready(self):
-        """Set up 485 communication
-        
-        Return:
-            0 : not set
-            1 : Setup completed
-        """
-        return self._mesg(ProtocolCode.TOOL_SERIAL_READY, has_reply=True)
-    
-    def tool_serial_available(self):
-        """Read 485 buffer length
+            pin_no: (int)pin number 1-16.
         
-        Return:
-            485 buffer length available for reading
-        """
-        return self._mesg(ProtocolCode.TOOL_SERIAL_AVAILABLE, has_reply=True)
-    
-    def tool_serial_read_data(self, data_len):
-        """Read fixed length data. Before reading, read the buffer length first. After reading, the data will be cleared
+                PIN_NO = GPIO.BCM:  
 
-        Args:
-            data_len (int): The number of bytes to be read, range 1 ~ 45
-        """
-        self.calibration_parameters(class_name=self.__class__.__name__, data_len=data_len)
-        return self._mesg(ProtocolCode.TOOL_SERIAL_READ_DATA, data_len, has_reply=True)
-    
-    def tool_serial_write_data(self, command):
-        """End 485 sends data， Data length range is 1 ~ 45 bytes
+                |1 = G7  |  2 = G8  |  3 = G25 | 4 = G24  | 5 = G23  | 6 = G18   |
 
-        Args:
-            command : data instructions
-            
-        Return:
-            number of bytes received
-        """
-        return self._mesg(ProtocolCode.TOOL_SERIAL_WRITE_DATA, command, has_reply=True)
-    
-    def tool_serial_flush(self):
-        """Clear 485 buffer
-        """
-        return self._mesg(ProtocolCode.TOOL_SERIAL_FLUSH)
-    
-    def tool_serial_peek(self):
-        """View the first data in the buffer, the data will not be cleared
-        
-        Return:
-            1 byte data
-        """
-        return self._mesg(ProtocolCode.TOOL_SERIAL_PEEK, has_reply=True)
-    
-    def tool_serial_set_baud(self, baud=115200):
-        """Set 485 baud rate, default 115200
+                |7 = G11 |  8 = G9  |  9 = G10 | 10 =G22  | 11 =G27  | 12 = G17  |
 
-        Args:
-            baud (int): baud rate
-        """
-        return self._mesg(ProtocolCode.TOOL_SERIAL_SET_BAUD, baud)
-    
-    def tool_serial_set_timeout(self, max_time):
-        """Set 485 timeout in milliseconds, default 30ms
+                |Grove0:   |  SCL0 = 13 = G3    |     SDA0 = 14 = G2    |
 
-        Args:
-            max_time (int): timeout
-        """
-        self.calibration_parameters(class_name=self.__class__.__name__, max_time=max_time)
-        return self._mesg(ProtocolCode.TOOL_SERIAL_SET_TIME_OUT, max_time)
+                |Grove1:   |  SCL1 = 15 = G6    |     SDA1 = 16 = G5    |
 
-    def get_robot_status(self):
-        return self._mesg(ProtocolCode.MERCURY_ROBOT_STATUS, has_reply=True)
-    
-    def power_on(self):
-        """Open communication with Atom."""
-        return self._mesg(ProtocolCode.POWER_ON, has_reply=True)
-
-    def power_off(self):
-        """Close communication with Atom."""
-        return self._mesg(ProtocolCode.POWER_OFF, has_reply=True)
-    
-    def release_all_servos(self):
-        """Relax all joints
+            mode: 
+                0 - input
+                    define: pull_up_down = DOWN
+                1 - output
+                     define: initial = HIGH
         """
-        return self._mesg(ProtocolCode.RELEASE_ALL_SERVOS, has_reply=True)
-    
-    def focus_servo(self, servo_id):
-        """Power on designated servo
+        pin_no = self.base_io_to_gpio(pin_no)       
+        if mode == 1:
+            self.gpio.setup(pin_no, self.gpio.OUT)
+        else:
+            self.gpio.setup(pin_no, self.gpio.IN)
+            
+    def set_gpio_output(self, pin_no, v):
+        """Set GPIO output value.
 
         Args:
-            servo_id: int. joint id 1 - 7
+            pin_no: (int)pin number 1-16.
+            v: (int) 0 / 1
         """
-        self.calibration_parameters(class_name = self.__class__.__name__, id=servo_id)
-        return self._mesg(ProtocolCode.FOCUS_SERVO, servo_id, has_reply=True)
-    
-    def release_servo(self, servo_id):
-        """Power off designated servo
+        pin = self.base_io_to_gpio(pin_no)
+        self.gpio.output(pin, v)
+        
+    def get_gpio_input(self, pin_no):
+        """Get GPIO input value.
 
         Args:
-            servo_id: int. joint id 1 - 7
-        """
-        self.calibration_parameters(class_name = self.__class__.__name__, id=servo_id)
-        return self._mesg(ProtocolCode.RELEASE_SERVO, servo_id, has_reply=True)
-    
-    def stop(self):
-        """Stop moving"""
-        return self._mesg(ProtocolCode.STOP, has_reply=True)
-    
-    def get_robot_type(self):
-        """Get robot type
+            pin_no: (int)pin number 1-16.
         """
-        return self._mesg(ProtocolCode.GET_ROBOT_ID, has_reply=True)
-        
+        pin = self.base_io_to_gpio(pin_no)
+        return self.gpio.input(pin)
         
-    def get_zero_pos(self):
-        """Read the zero encoder value
+    def set_gpio_pwm_start(self, pin_no, freq = 0.5, dc = 0.5):
+        """Set GPIO PWM value.
 
-        Returns:
-            list: The values of the zero encoders of the seven joints
+        Args:
+            pin_no: (int)pin number 1-16.
+            freq: (float) 0.0 - 1000000.0
+            dc: (float) 0.0 - 100.0
         """
-        return self._mesg(ProtocolCode.GET_ZERO_POS, has_reply=True)
-    
-    def is_init_calibration(self):
-        """Check if the robot is initialized for calibration
+        pin = self.base_io_to_gpio(pin_no)
+        self.pwm = self.gpio.PWM(pin, freq)
+        self.pwm.start(dc)
 
-        Returns:
-            bool: True if the robot is initialized for calibration, False otherwise
-        """
-        return self._mesg(ProtocolCode.IS_INIT_CALIBRATION, has_reply=True)
-    
-    def set_break(self, joint_id, value):
-        """Set break point
+    def set_gpio_pwm_change_freq(self, freq):
+        """Reset GPIO PWM freq.
 
         Args:
-            joint_id: int. joint id 1 - 7
-            value: int. 0 - disable, 1 - enable
-            
-        Return:
-            0 : failed
-            1 : success 
-        """
-        self.calibration_parameters(class_name = self.__class__.__name__, id=joint_id, value=value)
-        return self._mesg(ProtocolCode.SET_BREAK, joint_id, value, has_reply=True)
-    
-    def over_limit_return_zero(self):
-        """Return to zero when the joint is over the limit
+            freq: (float) 0.0 - 1000000.0
         """
-        return self._mesg(ProtocolCode.OVER_LIMIT_RETURN_ZERO)
-    
-    def jog_increment_angle(self, joint_id, increment, speed):
-        """angle step mode
+        self.pwm.ChangeFrequency(freq)
 
-        Args:
-            joint_id: Joint id 1 - 7.
-            increment: 
-            speed: int (1 - 100)
-        """
-        self.calibration_parameters(class_name = self.__class__.__name__, id = joint_id, speed = speed)
-        return self._mesg(ProtocolCode.JOG_INCREMENT, joint_id, [self._angle2int(increment)], speed)
-    
-    def jog_increment_coord(self, coord_id, increment, speed):
-        """coord step mode
+    def set_gpio_pwm_change_dc(self, dc):
+        """Reset GPIO PWM DC.
 
         Args:
-            coord_id: axis id 1 - 6.
-            increment: 
-            speed: int (1 - 100)
+            dc: (float) 0.0 - 100.0
         """
-        self.calibration_parameters(class_name = self.__class__.__name__, id = coord_id, speed = speed)
-        value = self._coord2int(increment) if id <= 3 else self._angle2int(increment)
-        return self._mesg(ProtocolCode.JOG_INCREMENT, coord_id, [value], speed)
-    
-    def drag_teach_clean(self):
-        """clear sample
+        self.pwm.ChangeDutyCycle(dc)
+
+    def set_gpio_pwm_stop(self):
+        """Set GPIO PWM STOP OUTPUT.
         """
-        return self._mesg(ProtocolCode.MERCURY_DRAG_TEACH_CLEAN)
-    
-    def get_comm_error_counts(self, joint_id, _type):
-        """Read the number of communication exceptions
+        self.pwm.stop()
 
-        Args:
-            joint_id (int): joint ID
-            _type (int): Error type to be read, 1 ~ 4.
-                1-The number of exceptions sent by the joint
-                2-The number of exceptions obtained by the joint
-                3-The number of exceptions sent by the end
-                4-The number of exceptions read by the end
+    def set_iic_init(self, IIC_NO):
         """
-        return self._mesg(ProtocolCode.MERCURY_ERROR_COUNTS, joint_id, _type, has_reply=True)
-    
-    def set_pos_over_shoot(self, value):
-        """Set position deviation value
+            import SMBUS2
 
+            Open IIC_NO port
+
+            (For more use, please see
+            
+            pypilink: https://pypi.org/project/smbus2/,
+             
+            githublink: https://github.com/kplindegaard/smbus2)
+            
         Args:
-            value (_type_): _description_
+            IIC_NO(int) : 0/1 ,0 = iic0, 1=iic1
         """
-        return self._mesg(ProtocolCode.MERCURY_SET_POS_OVER_SHOOT, value)
+        from smbus2 import SMBus
+        # self.iic = SMBus(IIC_NO)
+        return SMBus(IIC_NO)
+
+    def base_io_to_gpio(self, pin):
+        """BASE_io = GPIO.BCM:   
+            1 = G7    |   7 = G11  
+            2 = G8    |   8 = G9  
+            3 = G25  |   9 = G10  
+            4 = G24  |  10 =G22  
+            5 = G23  |  11 =G27  
+            6 = G18  |  12 = G17  
+            GND       |  3V3  
+
+            Grove0:
+            SCL0 = 13 = G3  
+            SDA0 = 14 = G2  
+            5V  
+            GND  
+
+            Grove1:  
+            SCL1 = 15 = G6  
+            SDA1 = 16 = G5  
+            5V  
+            GND  
+        """
+        pin_dist = {1:7, 2:8, 3:25, 4:24, 5:23, 6:18, 
+                    7:11, 8:9, 9:10, 10:22, 11:27, 12:17,
+                    13:3, 14:2,'SCL0':3,"SDA0":2, 
+                    15:6, 16:5, 'SCL0':6,"SDA0":5}
+        if pin in pin_dist:
+            _pin = pin
+            pin = pin_dist.get(_pin)
+        else:
+            print('The IO definition exceeds the system support range, and the program exits automatically.')
+            pin = None
+        return pin
+
+    def set_gpio_clearup(self,pin_no = None):
+        """SET GPIO CLEANUP
+
+        Args:
+            pin_no :(int)pin number 1-16.
+            if pin_no = None : cleanup all gpio
+        """
+        if pin_no:
+            pin_no = self.base_io_to_gpio(pin_no)
+        self.gpio.cleanup(pin_no)
+   
+    # Other
+    def wait(self, t):
+        time.sleep(t)
+        return self
+
+    def close(self):
+        self._serial_port.close()   
+            
+    def open(self):
+        self._serial_port.open()
         
-    def get_pos_over_shoot(self):
-        """Get position deviation value
-        """
-        return self._mesg(ProtocolCode.MERCURY_GET_POS_OVER_SHOOT, has_reply=True)
+    def is_open(self):
+        return self._serial_port.is_open
     
-    def stop(self, deceleration=False):
-        """Robot stops moving
-
+    def sync_send_angles(self, id, degrees, speed, timeout=15):
+        """Send the angle in synchronous state and return when the target point is reached
+            
         Args:
-            deceleration (bool, optional): Whether to slow down and stop. Defaults to False.
-
-        Returns:
-            int: 1 - Stop completion
+            degrees: a list of degree values(List[float]), length 6.
+            speed: (int) 0 ~ 100
+            timeout: default 7s.
         """
-        if deceleration:
-            return self._mesg(ProtocolCode.STOP, has_reply=True)
-        else:
-            return self._mesg(ProtocolCode.STOP, 1, has_reply=True)
-        
-    def pause(self, deceleration=False):
-        """Robot pauses movement
+        t = time.time()
+        self.send_angles(id, degrees, speed)
+        time.sleep(0.5)
+        while time.time() - t < timeout:
+            f = self.is_in_position(id, degrees, 0)
+            if f == 1:
+                break
+            time.sleep(0.1)
+        return self
 
+    def sync_send_coords(self, id, coords, speed, mode=0, timeout=15):
+        """Send the coord in synchronous state and return when the target point is reached
+            
         Args:
-            deceleration (bool, optional): Whether to slow down and stop. Defaults to False.
-
-        Returns:
-            int: 1 - pause completion
+            coords: a list of coord values(List[float])
+            speed: (int) 0 ~ 100
+            mode: (int): 0 - angular（default）, 1 - linear
+            timeout: default 7s.
         """
-        if deceleration:
-            return self._mesg(ProtocolCode.PAUSE, has_reply=True)
-        else:
-            return self._mesg(ProtocolCode.PAUSE, 1, has_reply=True)
-        
-    def get_modified_version(self):
-        return self._mesg(ProtocolCode.ROBOT_VERSION, has_reply=True)
-    
-    def get_pos_over(self):
-        return self._mesg(ProtocolCode.GET_POS_OVER, has_reply=True)
-    
-    def clear_encoders_error(self):
-        return self._mesg(ProtocolCode.CLEAR_ENCODERS_ERROR)
-    
-    def get_down_encoders(self):
-        return self._mesg(ProtocolCode.GET_DOWN_ENCODERS, has_reply=True)
-        
+        t = time.time()
+        self.send_coords(id, coords, speed, mode)
+        time.sleep(0.5)
+        while time.time() - t < timeout:
+            if self.is_in_position(id, coords, 1) == 1:
+                break
+            time.sleep(0.1)
+        return self
```

### Comparing `pymycobot-3.4.7b1/pymycobot/mercurychassis.py` & `pymycobot-3.5.0b1/pymycobot/mercurychassis.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mercurysocket.py` & `pymycobot-3.5.0b1/pymycobot/mybuddybluetooth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,72 @@
-# coding=utf-8
+# coding: utf-8
 
-import time
-import socket
 import threading
 
-from pymycobot.mercury_api import MercuryCommandGenerator
+from pymycobot.Interface import MyBuddyCommandGenerator
 from pymycobot.common import ProtocolCode, write, read
 from pymycobot.error import calibration_parameters
+from pymycobot.bluet import BluetoothConnection
 
 
-class MercurySocket(MercuryCommandGenerator):
+class MyBuddyBlueTooth(MyBuddyCommandGenerator):
+    """MyBuddy bluetooth API"""
     _write = write
-    _read = read
-    def __init__(self, ip, netport=9000, debug=False):
-        """
+    def __init__(self, bt_address=None, port = 10):
+        """When bt_address is the default value of None, enter the Bluetooth search mode. There is a default Bluetooth search time of 5 seconds"""
+        super(MyBuddyBlueTooth).__init__()
+        self.ble = BluetoothConnection(bt_address, port)
+        self.sock = self.ble.connect_target_device()
+        self.lock = threading.Lock()
+        
+    def connect(self, serialport="/dev/ttyAMA0", baudrate="1000000", timeout='0.2'):
+        """Connect the robot arm through the serial port and baud rate
+        
         Args:
-            ip: Server ip
-            netport: Server port(default 9000)
+            serialport: (str) default /dev/ttyAMA0
+            baudrate: default 1000000
+            timeout: default 0.1
+        
         """
-        super(MercurySocket, self).__init__(debug)
-        self.calibration_parameters = calibration_parameters
-        self.SERVER_IP = ip
-        self.SERVER_PORT = netport
-        self.sock = self.connect_socket()
-        self.lock = threading.Lock()
-
-    def connect_socket(self):
-        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        sock.connect((self.SERVER_IP, self.SERVER_PORT))
-        return sock
+        self.rasp = True
+        self._write(serialport, "socket")
+        self._write(baudrate, "socket")
+        self._write(timeout, "socket")
+        # self._write([254, 254, 1, 2, 32, 32], "socket")
+        # self._write([254, 254, 1, 2, 32, 32], "socket")
+        # self._write([254, 254, 1, 2, 32, 32], "socket")
+        
+        # self._write(timeout, "socket")
+        # self._write(timeout, "socket")
+        
         
-
     def _mesg(self, genre, *args, **kwargs):
         """
 
         Args:
             genre: command type (Command)
             *args: other data.
                    It is converted to octal by default.
                    If the data needs to be encapsulated into hexadecimal,
                    the array is used to include them. (Data cannot be nested)
             **kwargs: support `has_reply`
                 has_reply: Whether there is a return value to accept.
         """
-        real_command, has_reply = super(MercurySocket, self)._mesg(genre, *args, **kwargs)
+        real_command, has_reply = super(
+            MyBuddyBlueTooth, self)._mesg(genre, *args, **kwargs)
         with self.lock:
-            self._write(self._flatten(real_command), "socket")
+            data = self._write(self._flatten(real_command), "socket")
 
-            if has_reply:
-                data = self._read(genre, _class=self.__class__.__name__, method='socket')
-                if genre == ProtocolCode.SET_SSID_PWD:
-                    return None
-                res = self._process_received(data, genre, 14)
+            if data:
+                res = self._process_received(data, genre, arm=12)
                 if res == []:
                     return None
                 if genre in [
                     ProtocolCode.ROBOT_VERSION,
+                    ProtocolCode.SOFTWARE_VERSION,
                     ProtocolCode.GET_ROBOT_ID,
                     ProtocolCode.IS_POWER_ON,
                     ProtocolCode.IS_CONTROLLER_CONNECTED,
                     ProtocolCode.IS_PAUSED,  # TODO have bug: return b''
                     ProtocolCode.IS_IN_POSITION,
                     ProtocolCode.IS_MOVING,
                     ProtocolCode.IS_SERVO_ENABLE,
@@ -72,91 +79,55 @@
                     ProtocolCode.GET_ENCODER,
                     ProtocolCode.GET_BASIC_INPUT,
                     ProtocolCode.GET_TOF_DISTANCE,
                     ProtocolCode.GET_END_TYPE,
                     ProtocolCode.GET_MOVEMENT_TYPE,
                     ProtocolCode.GET_REFERENCE_FRAME,
                     ProtocolCode.GET_FRESH_MODE,
-                    ProtocolCode.GET_GRIPPER_MODE,
-                    ProtocolCode.SET_SSID_PWD,
-                    ProtocolCode.COBOTX_IS_GO_ZERO,
-                    ProtocolCode.GET_ERROR_DETECT_MODE,
-                    ProtocolCode.POWER_ON,
-                    ProtocolCode.POWER_OFF,
-                    ProtocolCode.RELEASE_ALL_SERVOS,
-                    ProtocolCode.RELEASE_SERVO,
-                    ProtocolCode.FOCUS_ALL_SERVOS,
-                    ProtocolCode.FOCUS_SERVO,
-                    ProtocolCode.STOP,
-                    ProtocolCode.SET_BREAK,
-                    ProtocolCode.IS_BTN_CLICKED
+                    ProtocolCode.SetHTSGripperTorque,
+                    ProtocolCode.GetHTSGripperTorque,
+                    ProtocolCode.GetGripperProtectCurrent,
+                    ProtocolCode.InitGripper,
+                    ProtocolCode.SET_FOUR_PIECES_ZERO
+                    # ProtocolCode.GET_SERVO_CURRENTS
                 ]:
                     return self._process_single(res)
                 elif genre in [ProtocolCode.GET_ANGLES]:
                     return [self._int2angle(angle) for angle in res]
-                elif genre in [
-                    ProtocolCode.GET_COORDS,
-                    ProtocolCode.MERCURY_GET_BASE_COORDS,
-                    ProtocolCode.GET_TOOL_REFERENCE,
-                    ProtocolCode.GET_WORLD_REFERENCE,
-                ]:
+                elif genre in [ProtocolCode.GET_ANGLE]:
+                    return self._int2angle(res[0]) if res else None
+                elif genre in [ProtocolCode.GET_COORD]:
+                    if real_command[5] < 4:
+                        if real_command[2] == 3:
+                            return self._int2angle(res[0]) if res else None
+                        return self._int2coord(res[0]) if res else None
+                    else:
+                        return self._int2angle(res[0]) if res else None
+                elif genre in [ProtocolCode.GET_ALL_BASE_COORDS, ProtocolCode.GET_COORDS, ProtocolCode.GET_TOOL_REFERENCE, ProtocolCode.GET_WORLD_REFERENCE, ProtocolCode.GET_BASE_COORDS, ProtocolCode.GET_BASE_COORD, ProtocolCode.BASE_TO_SINGLE_COORDS]:
                     if res:
-                        r = []
+                        r = [] 
                         for idx in range(3):
                             r.append(self._int2coord(res[idx]))
                         for idx in range(3, 6):
                             r.append(self._int2angle(res[idx]))
+                        if len(res) == 12:
+                            r1 = []
+                            for idx in range(6, 9):
+                                r1.append(self._int2coord(res[idx]))
+                            for idx in range(9, 12):
+                                r1.append(self._int2angle(res[idx]))
+                            return [r, r1]
                         return r
                     else:
                         return res
-                elif genre in [ProtocolCode.GET_SERVO_VOLTAGES]:
-                    return [self._int2coord(angle) for angle in res]
-                elif genre in [ProtocolCode.GET_BASIC_VERSION, ProtocolCode.SOFTWARE_VERSION, ProtocolCode.GET_ATOM_VERSION]:
-                    return self._int2coord(self._process_single(res))
-                elif genre in [
-                    ProtocolCode.GET_JOINT_MAX_ANGLE,
-                    ProtocolCode.GET_JOINT_MIN_ANGLE,
-                ]:
+                elif genre in [ProtocolCode.GET_JOINT_MAX_ANGLE, ProtocolCode.GET_JOINT_MIN_ANGLE]:
                     return self._int2coord(res[0])
-                elif genre == ProtocolCode.GET_ANGLES_COORDS:
-                    r = []
-                    for index in range(len(res)):
-                        if index < 7:
-                            r.append(self._int2angle(res[index]))
-                        elif index < 10:
-                            r.append(self._int2coord(res[index]))
-                        else:
-                            r.append(self._int2angle(res[index]))
-                    return r
-                elif genre == ProtocolCode.GO_ZERO:
-                    r = []
-                    if res:
-                        if 1 not in res[1:]:
-                            return res[0]
-                        else:
-                            for i in range(1, len(res)):
-                                if res[i] == 1:
-                                    r.append(i)
-                    return r
-                elif genre in [ProtocolCode.COBOTX_GET_ANGLE, ProtocolCode.COBOTX_GET_SOLUTION_ANGLES]:
-                        return self._int2angle(res[0])
-                elif genre == ProtocolCode.MERCURY_ROBOT_STATUS:
-                    i = 9
-                    for i in range(9, len(res)):
-                        if res[i] != 0:
-                            data = bin(res[i])[2:]
-                            res[i] = []
-                            while len(data) != 16:
-                                data = "0"+data
-                            for j in range(16):
-                                if data[j] != "0":
-                                    res[i].append(15-j)
-                    return res
+                elif genre in [ProtocolCode.GET_SERVO_VOLTAGES, ProtocolCode.COLLISION]:
+                    return [self._int2coord(angle) for angle in res]
                 else:
                     return res
             return None
-    
-    def open(self):
-        self.sock = self.connect_socket()
         
     def close(self):
+        self._write("close","socket")
         self.sock.close()
+
```

### Comparing `pymycobot-3.4.7b1/pymycobot/myagv.py` & `pymycobot-3.5.0b1/pymycobot/myagv.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/myarm.py` & `pymycobot-3.5.0b1/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/myarm_api.py` & `pymycobot-3.5.0b1/pymycobot/myarm_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/myarmm.py` & `pymycobot-3.5.0b1/pymycobot/myarmm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/myarmsocket.py` & `pymycobot-3.5.0b1/pymycobot/myarmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mybuddyemoticon.py` & `pymycobot-3.5.0b1/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mybuddysocket.py` & `pymycobot-3.5.0b1/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mycobot.py` & `pymycobot-3.5.0b1/pymycobot/mycobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mycobotpro630.py` & `pymycobot-3.5.0b1/pymycobot/mycobotpro630.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mycobotsocket.py` & `pymycobot-3.5.0b1/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mypalletizer.py` & `pymycobot-3.5.0b1/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/mypalletizersocket.py` & `pymycobot-3.5.0b1/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/public.py` & `pymycobot-3.5.0b1/pymycobot/public.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/robot_limit.json` & `pymycobot-3.5.0b1/pymycobot/robot_limit.json`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/ultraArm.py` & `pymycobot-3.5.0b1/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot/utils.py` & `pymycobot-3.5.0b1/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.5.0b1/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.7b1
+Version: 3.5.0b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -1594,15 +1594,15 @@
 
 ### Client
 
 ```python
 # demo
 from pymycobot import MyCobotSocket
 # Port 9000 is used by default
-mc = MyCobotSocket("192.168.10.10","9000")
+mc = MyCobotSocket("192.168.10.10",9000)
 
 res = mc.get_angles()
 print(res)
 
 mc.send_angles([0,0,0,0,0,0],20)
 ...
```

### Comparing `pymycobot-3.4.7b1/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.5.0b1/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/setup.py` & `pymycobot-3.5.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/tests/test_api.py` & `pymycobot-3.5.0b1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/tests/test_generator.py` & `pymycobot-3.5.0b1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.7b1/tests/test_socket.py` & `pymycobot-3.5.0b1/tests/test_socket.py`

 * *Files identical despite different names*

