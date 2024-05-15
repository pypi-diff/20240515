# Comparing `tmp/RPICommLink-1.1.1.tar.gz` & `tmp/RPICommLink-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RPICommLink-1.1.1.tar", last modified: Tue May  7 17:59:47 2024, max compression
+gzip compressed data, was "dist\RPICommLink-1.1.2.tar", last modified: Wed May 15 04:40:20 2024, max compression
```

## Comparing `RPICommLink-1.1.1.tar` & `RPICommLink-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 17:59:47.000000 RPICommLink-1.1.1/
--rw-rw-rw-   0        0        0     2244 2024-05-07 17:59:47.000000 RPICommLink-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 17:59:47.000000 RPICommLink-1.1.1/RPICommLink/
--rw-rw-rw-   0        0        0    19537 2024-05-07 17:59:14.000000 RPICommLink-1.1.1/RPICommLink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:59:47.000000 RPICommLink-1.1.1/RPICommLink.egg-info/
--rw-rw-rw-   0        0        0     2244 2024-05-07 17:59:47.000000 RPICommLink-1.1.1/RPICommLink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-05-07 17:59:47.000000 RPICommLink-1.1.1/RPICommLink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 17:59:47.000000 RPICommLink-1.1.1/RPICommLink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 17:59:47.000000 RPICommLink-1.1.1/RPICommLink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 17:59:47.000000 RPICommLink-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2234 2024-05-07 17:55:45.000000 RPICommLink-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:40:20.000000 RPICommLink-1.1.2/
+-rw-rw-rw-   0        0        0     2371 2024-05-15 04:40:20.000000 RPICommLink-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 04:40:20.000000 RPICommLink-1.1.2/RPICommLink/
+-rw-rw-rw-   0        0        0    19926 2024-05-15 04:38:13.000000 RPICommLink-1.1.2/RPICommLink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:40:20.000000 RPICommLink-1.1.2/RPICommLink.egg-info/
+-rw-rw-rw-   0        0        0     2371 2024-05-15 04:40:20.000000 RPICommLink-1.1.2/RPICommLink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-05-15 04:40:20.000000 RPICommLink-1.1.2/RPICommLink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 04:40:20.000000 RPICommLink-1.1.2/RPICommLink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-15 04:40:20.000000 RPICommLink-1.1.2/RPICommLink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 04:40:20.000000 RPICommLink-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2338 2024-05-15 04:40:07.000000 RPICommLink-1.1.2/setup.py
```

### Comparing `RPICommLink-1.1.1/PKG-INFO` & `RPICommLink-1.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: RPICommLink
-Version: 1.1.1
+Version: 1.1.2
 Summary: A library for communication on Raspberry Pi
 Home-page: UNKNOWN
 Author: adixu
 Author-email: adixu7@gmail.com
 License: UNKNOWN
 Description: RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
         
@@ -57,8 +57,14 @@
         1.1   -增加了传输摄像头帧的函数，需要自行下载opencv-python库。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。
         
         
         
         
         
         1.1.1 -修复了几个bug。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。
+        
+        
+        
+        
+        
+        1.1.2 -现在服务端与客户端都可以进行发送或接收了
 Platform: UNKNOWN
```

### Comparing `RPICommLink-1.1.1/RPICommLink/__init__.py` & `RPICommLink-1.1.2/RPICommLink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,32 +149,38 @@
         直到有数据被成功接收并存储在 self.return_data 中。
 
          一旦数据事件被设置，表示数据已经接收到，线程将继续执行。recv_data 方法将 self.return_data 中存储的数据返回给调用者，
          并将 self.return_data 设置为 None，以便下一次接收新的数据。
 
         :return:返回接收到的数据
         """
-        if self.wait():
-            for i in self.socket_list:
-                if i not in self.threading_now:
-                    recv_thread = threading.Thread(target=self._recv_threading, args=(i,), daemon=True)
-                    self.threading_now.append(i)
-                    recv_thread.start()
-            if len(self.threading_now) == 0:
-                try:
-                    recv_thread = threading.Thread(target=self._recv_threading, args=(self.socket_list[0],),
-                                                   daemon=True)
-                    recv_thread.start()
-                except Exception:
-                    pass
-            self.data_event.wait()  # 等待数据事件被设置
-            return_data = self.return_data
-            self.return_data = None
-            self.data_event.clear()
-            return return_data
+        sock_list = []
+        if self._device_state == 'client':
+            sock_list.append(self._send_server_socket)
+        else:
+            sock_list = self.socket_list
+            self.wait()
+
+        for i in sock_list:
+            if i not in self.threading_now:
+                recv_thread = threading.Thread(target=self._recv_threading, args=(i,), daemon=True)
+                self.threading_now.append(i)
+                recv_thread.start()
+        if len(self.threading_now) == 0:
+            try:
+                recv_thread = threading.Thread(target=self._recv_threading, args=(sock_list[0],),
+                                               daemon=True)
+                recv_thread.start()
+            except Exception:
+                pass
+        self.data_event.wait()  # 等待数据事件被设置
+        return_data = self.return_data
+        self.return_data = None
+        self.data_event.clear()
+        return return_data
 
     def _recv_threading(self, sock):
         """处理从客户端收到的数据的线程
 
         将当前处理的套接字 sock 添加到 self.threading_now 列表中，以便跟踪当前正在处理的线程。
 
         使用套接字对象的 recv 方法接收数据，如果没有接收到数据（recv_data 为空），说明连接已经关闭，
@@ -297,17 +303,25 @@
                 print(f'\033[93mError:没有找到{target_name}设备或密码不正确 \033[0m')
 
     def send(self, msg: str):
         """向服务器发送消息的函数
 
         :param msg:发送的信息
         """
-        for sock in self._send_server_socket:
+        sock_list = []
+        if self._device_state == 'server':
+            sock_list = self.socket_list
+        elif self._device_state is None:
+            print(f'\033[91mError:未开启或连接服务器 \033[0m')
+        else:
+            sock_list.append(self._send_server_socket)
+
+        for sock in sock_list:
             try:
-                sock.send(msg.encode('utf-8'))
+                sock[0].send(msg.encode('utf-8'))
             except Exception:
                 print('\033[91mError:一个服务器发送失败！请确认是否有连接服务器 \033[0m')
                 self._send_server_socket.remove(sock)
                 if len(self._send_server_socket) == 0:
                     print('\033[91mError:无服务器连接 \033[0m')
                     sys.exit()
 
@@ -406,7 +420,8 @@
         else:
             print(f'\033[93mWarning：无法通过互联网或自身获取IP，请自行设置IP \033[0m')
             sys.exit()
 
 
 if __name__ == "__main__":
     pass
+
```

### Comparing `RPICommLink-1.1.1/RPICommLink.egg-info/PKG-INFO` & `RPICommLink-1.1.2/RPICommLink.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: RPICommLink
-Version: 1.1.1
+Version: 1.1.2
 Summary: A library for communication on Raspberry Pi
 Home-page: UNKNOWN
 Author: adixu
 Author-email: adixu7@gmail.com
 License: UNKNOWN
 Description: RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
         
@@ -57,8 +57,14 @@
         1.1   -增加了传输摄像头帧的函数，需要自行下载opencv-python库。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。
         
         
         
         
         
         1.1.1 -修复了几个bug。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。
+        
+        
+        
+        
+        
+        1.1.2 -现在服务端与客户端都可以进行发送或接收了
 Platform: UNKNOWN
```

### Comparing `RPICommLink-1.1.1/setup.py` & `RPICommLink-1.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='RPICommLink',
-    version='1.1.1',
+    version='1.1.2',
     author='adixu',
     author_email='adixu7@gmail.com',
     description='A library for communication on Raspberry Pi',
     long_description="RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。"
                      "灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。"
                      "具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。"
                      "使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。"
@@ -15,12 +15,13 @@
                      "\n\n\n\n\n\n1.0.2 -优化了函数的命名，发送模块不再进行死循环。"
                      "\n\n\n\n\n\n1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。"
                      "\n\n\n\n\n\n1.0.4 -重新了上传中文介绍。"
                      "\n\n\n\n\n\n1.0.5 -修复了无法在无互联网下获取IP的报错，修复了无法同时连接两个服务器的bug。"
                      "\n\n\n\n\n\n1.0.6 -修复了潜在bug"
                      "\n\n\n\n\n\n1.0.7 -轻量化"
                      "\n\n\n\n\n\n1.1   -增加了传输摄像头帧的函数，需要自行下载opencv-python库。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。"
-                     "\n\n\n\n\n\n1.1.1 -修复了几个bug。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。",
+                     "\n\n\n\n\n\n1.1.1 -修复了几个bug。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。"
+                     "\n\n\n\n\n\n1.1.2 -现在服务端与客户端都可以进行发送或接收了",
     packages=['RPICommLink'],
     include_package_data=True,
     install_requires=[],
 )
```

