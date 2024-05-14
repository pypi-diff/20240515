# Comparing `tmp/simple_threaded_tcp-1.2.tar.gz` & `tmp/simple_threaded_tcp-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_threaded_tcp-1.2.tar", last modified: Mon May 13 19:16:49 2024, max compression
+gzip compressed data, was "simple_threaded_tcp-1.3.tar", last modified: Tue May 14 23:28:21 2024, max compression
```

## Comparing `simple_threaded_tcp-1.2.tar` & `simple_threaded_tcp-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 19:16:49.707173 simple_threaded_tcp-1.2/
--rw-rw-rw-   0        0        0     5429 2024-05-13 19:16:49.702175 simple_threaded_tcp-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4914 2024-05-13 19:12:46.000000 simple_threaded_tcp-1.2/README.md
--rw-rw-rw-   0        0        0      597 2024-05-13 19:16:40.000000 simple_threaded_tcp-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 19:16:49.708171 simple_threaded_tcp-1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 19:16:49.646216 simple_threaded_tcp-1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 19:16:49.700177 simple_threaded_tcp-1.2/src/simple_threaded_tcp.egg-info/
--rw-rw-rw-   0        0        0     5429 2024-05-13 19:16:49.000000 simple_threaded_tcp-1.2/src/simple_threaded_tcp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-13 19:16:49.000000 simple_threaded_tcp-1.2/src/simple_threaded_tcp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 19:16:49.000000 simple_threaded_tcp-1.2/src/simple_threaded_tcp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-13 19:16:49.000000 simple_threaded_tcp-1.2/src/simple_threaded_tcp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 19:16:49.697177 simple_threaded_tcp-1.2/src/sttcp/
--rw-rw-rw-   0        0        0       64 2024-05-13 17:37:14.000000 simple_threaded_tcp-1.2/src/sttcp/__init__.py
--rw-rw-rw-   0        0        0     5587 2024-05-13 19:12:46.000000 simple_threaded_tcp-1.2/src/sttcp/client.py
--rw-rw-rw-   0        0        0     5950 2024-05-13 19:12:46.000000 simple_threaded_tcp-1.2/src/sttcp/server.py
+drwxrwxrwx   0        0        0        0 2024-05-14 23:28:21.841151 simple_threaded_tcp-1.3/
+-rw-rw-rw-   0        0        0     6699 2024-05-14 23:28:21.840152 simple_threaded_tcp-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6184 2024-05-14 23:24:21.000000 simple_threaded_tcp-1.3/README.md
+-rw-rw-rw-   0        0        0      597 2024-05-14 23:28:10.000000 simple_threaded_tcp-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 23:28:21.842155 simple_threaded_tcp-1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 23:28:21.793122 simple_threaded_tcp-1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 23:28:21.837155 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/
+-rw-rw-rw-   0        0        0     6699 2024-05-14 23:28:21.000000 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-14 23:28:21.000000 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 23:28:21.000000 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-14 23:28:21.000000 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 23:28:21.835156 simple_threaded_tcp-1.3/src/sttcp/
+-rw-rw-rw-   0        0        0       64 2024-05-13 17:37:14.000000 simple_threaded_tcp-1.3/src/sttcp/__init__.py
+-rw-rw-rw-   0        0        0     7135 2024-05-14 23:24:21.000000 simple_threaded_tcp-1.3/src/sttcp/client.py
+-rw-rw-rw-   0        0        0     8283 2024-05-14 23:24:21.000000 simple_threaded_tcp-1.3/src/sttcp/server.py
```

### Comparing `simple_threaded_tcp-1.2/PKG-INFO` & `simple_threaded_tcp-1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_threaded_tcp
-Version: 1.2
+Version: 1.3
 Summary: Client-Server threaded TCP connector. This project also uses socket library.
 Author-email: Emil <emilahmaboy@gmail.com>
 Project-URL: Homepage, https://github.com/EmilAhmaBoy/simple-threaded-tcp
 Project-URL: Issues, https://github.com/EmilAhmaBoy/simple-threaded-tcp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8
@@ -39,15 +39,22 @@
 def server_receive_handler(address: tuple, connection: socket.socket, data: bytes):
     received_string = data.decode('utf-8') # Decoding input data
     received_string += '!'
     connection.sendall(received_string.encode('utf-8')) # Sending encoded string to client
 
 # Defining disconnection behavior
 @server.disconnection_handler
-def server_disconnection_handler(address: tuple):
+def server_disconnection_handler(address: tuple, reason: Exception):
+    # Note
+    #
+    # Parameter `reason` is new in version 1.3 and means the reason of disconnection
+    # This is an Exception that was caught during the handler function execution
+    # Also it can be ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError,
+    # ConnectionError, OSError
+    # Parameter `reason` is None when connection was successful (client requested for connection closure)
     print(f'Disconnected by {":".join(map(str, address))}')
 
 # Defining universal behavior
 # It being executed at all request phases like Server.HandlerType.connection, Server.HandlerType.receive etc.  
 @server.universal_handler
 def server_universal_handler(handler_type: Server.HandlerType, address: tuple, connection: socket.socket, data: bytes):
     print('- Server', handler_type, sep=': ')
@@ -76,15 +83,16 @@
         connection.sendall('Really?'.encode('utf-8')) # Sending encoded string to server
         return True # Continuing connection for awaiting future response
     else:
         return False # Stopping connection
 
 # Defining disconnection with server behavior 
 @client.disconnection_handler
-def client_disconnection_handler(address: tuple):
+def client_disconnection_handler(address: tuple, reason: Exception):
+    # Reason parameter is the same as in `server_disconnection_handler`
     print(f'Disconnected from {":".join(map(str, address))}')
 
 # Defining exceptions handling behavior
 @client.unconnected_handler
 def client_unconnected_handler(address: tuple, exception: Exception):
     print(f'Could not connect to {":".join(map(str, address))}')
     raise exception
@@ -98,14 +106,21 @@
 
 client.start() # Launching client (execution started in parallel thread)
 
 
 server.keep_alive()
 # server.keep_alive() is only needed to keep thread alive until KeyboardInterrupt will not be raised
 # This is optional in cases of you have something like "while True" statement
+
+"""
+Also there are methods like `server.close()` and `client.close()` but they only needed to close a connection.
+
+server.close() awaits for all connections to stop and stops the server
+client.close() disconnects the server with the reason of `sttcp.client.Client.DestructionException`
+"""
 ```
 
 ## What's new?
 ### Version 1.0
 - Nothing :)
 ### Version 1.1
 - Now with README.md
@@ -118,14 +133,21 @@
 - Added new method `sttcp.client.Client.universal_handler`
 - Added new method `sttcp.client.Client.unconnected_handler`
 - Added new method `sttcp.server.Server.connection_handler`
 - Added new method `sttcp.server.Server.receive_handler`
 - Added new method `sttcp.server.Server.disconnection_handler`
 - Added new method `sttcp.server.Server.universal_handler`
 - Renamed method `sttcp.server.Server.mainloop` to `sttcp.server.Server.keep_alive`
+- Added new methods `sttcp.client.Client.start` and `sttcp.server.Server.start`
+
+### Version 1.3
+- Added new methods `sttcp.client.Client.stop` and `sttcp.server.Server.stop`
+- Now server handler exceptions don't make server unstoppable by KeyboardInterrupt
+- Added new parameter to `disconnection_handler` for both sides - disconnection reason (Union[None, Exception]) 
+- Added new exception `sttcp.client.Client.DestructionException`
 
 ## Contacts
 Discord: `@emilahmaboy`
 
 that is all :)
 
 ## P.s
```

### Comparing `simple_threaded_tcp-1.2/README.md` & `simple_threaded_tcp-1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -27,15 +27,22 @@
 def server_receive_handler(address: tuple, connection: socket.socket, data: bytes):
     received_string = data.decode('utf-8') # Decoding input data
     received_string += '!'
     connection.sendall(received_string.encode('utf-8')) # Sending encoded string to client
 
 # Defining disconnection behavior
 @server.disconnection_handler
-def server_disconnection_handler(address: tuple):
+def server_disconnection_handler(address: tuple, reason: Exception):
+    # Note
+    #
+    # Parameter `reason` is new in version 1.3 and means the reason of disconnection
+    # This is an Exception that was caught during the handler function execution
+    # Also it can be ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError,
+    # ConnectionError, OSError
+    # Parameter `reason` is None when connection was successful (client requested for connection closure)
     print(f'Disconnected by {":".join(map(str, address))}')
 
 # Defining universal behavior
 # It being executed at all request phases like Server.HandlerType.connection, Server.HandlerType.receive etc.  
 @server.universal_handler
 def server_universal_handler(handler_type: Server.HandlerType, address: tuple, connection: socket.socket, data: bytes):
     print('- Server', handler_type, sep=': ')
@@ -64,15 +71,16 @@
         connection.sendall('Really?'.encode('utf-8')) # Sending encoded string to server
         return True # Continuing connection for awaiting future response
     else:
         return False # Stopping connection
 
 # Defining disconnection with server behavior 
 @client.disconnection_handler
-def client_disconnection_handler(address: tuple):
+def client_disconnection_handler(address: tuple, reason: Exception):
+    # Reason parameter is the same as in `server_disconnection_handler`
     print(f'Disconnected from {":".join(map(str, address))}')
 
 # Defining exceptions handling behavior
 @client.unconnected_handler
 def client_unconnected_handler(address: tuple, exception: Exception):
     print(f'Could not connect to {":".join(map(str, address))}')
     raise exception
@@ -86,14 +94,21 @@
 
 client.start() # Launching client (execution started in parallel thread)
 
 
 server.keep_alive()
 # server.keep_alive() is only needed to keep thread alive until KeyboardInterrupt will not be raised
 # This is optional in cases of you have something like "while True" statement
+
+"""
+Also there are methods like `server.close()` and `client.close()` but they only needed to close a connection.
+
+server.close() awaits for all connections to stop and stops the server
+client.close() disconnects the server with the reason of `sttcp.client.Client.DestructionException`
+"""
 ```
 
 ## What's new?
 ### Version 1.0
 - Nothing :)
 ### Version 1.1
 - Now with README.md
@@ -106,14 +121,21 @@
 - Added new method `sttcp.client.Client.universal_handler`
 - Added new method `sttcp.client.Client.unconnected_handler`
 - Added new method `sttcp.server.Server.connection_handler`
 - Added new method `sttcp.server.Server.receive_handler`
 - Added new method `sttcp.server.Server.disconnection_handler`
 - Added new method `sttcp.server.Server.universal_handler`
 - Renamed method `sttcp.server.Server.mainloop` to `sttcp.server.Server.keep_alive`
+- Added new methods `sttcp.client.Client.start` and `sttcp.server.Server.start`
+
+### Version 1.3
+- Added new methods `sttcp.client.Client.stop` and `sttcp.server.Server.stop`
+- Now server handler exceptions don't make server unstoppable by KeyboardInterrupt
+- Added new parameter to `disconnection_handler` for both sides - disconnection reason (Union[None, Exception]) 
+- Added new exception `sttcp.client.Client.DestructionException`
 
 ## Contacts
 Discord: `@emilahmaboy`
 
 that is all :)
 
 ## P.s
```

### Comparing `simple_threaded_tcp-1.2/pyproject.toml` & `simple_threaded_tcp-1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simple_threaded_tcp"
-version = "1.2"
+version = "1.3"
 authors = [
     {name = "Emil", email = "emilahmaboy@gmail.com"}
 ]
 description = "Client-Server threaded TCP connector. This project also uses socket library."
 readme = "README.md"
 requires-python = ">3.8"
 classifiers = [
```

### Comparing `simple_threaded_tcp-1.2/src/simple_threaded_tcp.egg-info/PKG-INFO` & `simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_threaded_tcp
-Version: 1.2
+Version: 1.3
 Summary: Client-Server threaded TCP connector. This project also uses socket library.
 Author-email: Emil <emilahmaboy@gmail.com>
 Project-URL: Homepage, https://github.com/EmilAhmaBoy/simple-threaded-tcp
 Project-URL: Issues, https://github.com/EmilAhmaBoy/simple-threaded-tcp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8
@@ -39,15 +39,22 @@
 def server_receive_handler(address: tuple, connection: socket.socket, data: bytes):
     received_string = data.decode('utf-8') # Decoding input data
     received_string += '!'
     connection.sendall(received_string.encode('utf-8')) # Sending encoded string to client
 
 # Defining disconnection behavior
 @server.disconnection_handler
-def server_disconnection_handler(address: tuple):
+def server_disconnection_handler(address: tuple, reason: Exception):
+    # Note
+    #
+    # Parameter `reason` is new in version 1.3 and means the reason of disconnection
+    # This is an Exception that was caught during the handler function execution
+    # Also it can be ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError,
+    # ConnectionError, OSError
+    # Parameter `reason` is None when connection was successful (client requested for connection closure)
     print(f'Disconnected by {":".join(map(str, address))}')
 
 # Defining universal behavior
 # It being executed at all request phases like Server.HandlerType.connection, Server.HandlerType.receive etc.  
 @server.universal_handler
 def server_universal_handler(handler_type: Server.HandlerType, address: tuple, connection: socket.socket, data: bytes):
     print('- Server', handler_type, sep=': ')
@@ -76,15 +83,16 @@
         connection.sendall('Really?'.encode('utf-8')) # Sending encoded string to server
         return True # Continuing connection for awaiting future response
     else:
         return False # Stopping connection
 
 # Defining disconnection with server behavior 
 @client.disconnection_handler
-def client_disconnection_handler(address: tuple):
+def client_disconnection_handler(address: tuple, reason: Exception):
+    # Reason parameter is the same as in `server_disconnection_handler`
     print(f'Disconnected from {":".join(map(str, address))}')
 
 # Defining exceptions handling behavior
 @client.unconnected_handler
 def client_unconnected_handler(address: tuple, exception: Exception):
     print(f'Could not connect to {":".join(map(str, address))}')
     raise exception
@@ -98,14 +106,21 @@
 
 client.start() # Launching client (execution started in parallel thread)
 
 
 server.keep_alive()
 # server.keep_alive() is only needed to keep thread alive until KeyboardInterrupt will not be raised
 # This is optional in cases of you have something like "while True" statement
+
+"""
+Also there are methods like `server.close()` and `client.close()` but they only needed to close a connection.
+
+server.close() awaits for all connections to stop and stops the server
+client.close() disconnects the server with the reason of `sttcp.client.Client.DestructionException`
+"""
 ```
 
 ## What's new?
 ### Version 1.0
 - Nothing :)
 ### Version 1.1
 - Now with README.md
@@ -118,14 +133,21 @@
 - Added new method `sttcp.client.Client.universal_handler`
 - Added new method `sttcp.client.Client.unconnected_handler`
 - Added new method `sttcp.server.Server.connection_handler`
 - Added new method `sttcp.server.Server.receive_handler`
 - Added new method `sttcp.server.Server.disconnection_handler`
 - Added new method `sttcp.server.Server.universal_handler`
 - Renamed method `sttcp.server.Server.mainloop` to `sttcp.server.Server.keep_alive`
+- Added new methods `sttcp.client.Client.start` and `sttcp.server.Server.start`
+
+### Version 1.3
+- Added new methods `sttcp.client.Client.stop` and `sttcp.server.Server.stop`
+- Now server handler exceptions don't make server unstoppable by KeyboardInterrupt
+- Added new parameter to `disconnection_handler` for both sides - disconnection reason (Union[None, Exception]) 
+- Added new exception `sttcp.client.Client.DestructionException`
 
 ## Contacts
 Discord: `@emilahmaboy`
 
 that is all :)
 
 ## P.s
```

### Comparing `simple_threaded_tcp-1.2/src/sttcp/client.py` & `simple_threaded_tcp-1.3/src/sttcp/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import socket
 import threading
+import traceback
 import warnings
 from enum import Enum
 from typing import Union
 from . import screen_lock
 
 
-def _default_connection(addr: tuple, connection: socket.socket):
+def _default_connection(addr: tuple, connection: socket.socket) -> Union[bool, None]:
     connection.sendall(b'ok')
+    return None
 
 
 def _default_response(addr: tuple, connection: socket.socket, data: bytes):
     print(f'Received "{data.decode("utf-8")}"')
     return False
 
 
-def _default_disconnection(addr: tuple):
+def _default_disconnection(addr: tuple, reason: Union[None, Exception]):
     pass
 
 
 def _default_universal(handler_type, addr: Union[tuple, None], connection: Union[socket.socket, None],
                        data: Union[bytes, None]):
     return True
 
 
 def _default_unconnected(addr: tuple, e: Exception):
     print(f'Couldn\'t connect to {":".join(map(str, addr))}')
     raise e
 
 
 class Client:
+    class DestructionException(ConnectionAbortedError):
+        pass
+
     class HandlerType(Enum):
         connection = 1
         response = 2
         disconnection = 3
         unconnected = 4
 
     def __init__(self, host: str, port: Union[str, int], handler=None):
@@ -55,23 +60,42 @@
         def client():
             self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             s = self._socket
             try:
                 s.connect((self.host, self.port))
                 addr = s.getpeername()
 
+                disconnection_reason = None
                 data = None
                 while True:
                     screen_lock.acquire()
                     if data is None:
                         continue_request_alt = self._universal_handler(self.HandlerType.connection, addr, s, None)
                         continue_request = self._connection_handler(addr, s)
                     else:
-                        continue_request_alt = self._universal_handler(self.HandlerType.response, addr, s, data)
-                        continue_request = self._response_handler(addr, s, data)
+                        if not self._socket_thread.shutdown:
+                            try:
+                                continue_request_alt = self._universal_handler(self.HandlerType.response, addr, s, data)
+                                continue_request = self._response_handler(addr, s, data)
+                            except (ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError,
+                                    ConnectionError, OSError) as e:
+                                disconnection_reason = e
+                                break
+                            except Exception as e:
+                                print('\033[91mOh no! Something went wrong in your handler! Check it out and find '
+                                      'problems:\033[0m')
+                                print(traceback.format_exc())
+                                print('\033[91mDisconnecting the client\033[0m')
+                                disconnection_reason = e
+                                s.close()
+                                break
+                        else:
+                            s.close()
+                            disconnection_reason = self.DestructionException('Connection closed!')
+                            break
 
                     if self.handler is not None:
                         self.handler(addr, s, data)
 
                     screen_lock.release()
 
                     if continue_request is None:
@@ -84,31 +108,37 @@
                     try:
                         data = s.recv(1024)
                     except OSError:
                         data = b''
 
                     if not data:
                         break
-
+                screen_lock.release()
                 screen_lock.acquire()
                 self._universal_handler(self.HandlerType.disconnection, addr, None, None)
-                self._disconnection_handler(addr)
+                self._disconnection_handler(addr, disconnection_reason)
                 screen_lock.release()
-            except (ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError, ConnectionError) as e:
+            except (ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError, ConnectionError, OSError) \
+                    as e:
                 screen_lock.acquire()
                 self._universal_handler(self.HandlerType.unconnected, None, None, None)
                 self._unconnected_handler((self.host, self.port), e)
                 screen_lock.release()
 
         self._socket_thread = threading.Thread(target=client)
+        self._socket_thread.shutdown = False
 
     def start(self):
         """Starts TCP client"""
         self._socket_thread.start()
 
+    def close(self):
+        """Closes TCP client"""
+        self._socket_thread.shutdown = True
+
     def connection_handler(self, function) -> None:
         """
         Sets a connection handler for TCP client.
         :param function: Function handler parameter with `"address: tuple"`, `"connection: socket.socket"` parameters`
         """
         self._connection_handler = function
```

### Comparing `simple_threaded_tcp-1.2/src/sttcp/server.py` & `simple_threaded_tcp-1.3/src/sttcp/server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import socket
 import threading
+import traceback
 import warnings
 from enum import Enum
-from types import NoneType
 from typing import Union
 from . import screen_lock
 
 
-def _default_connection(addr: tuple, connection: socket.socket):
+def _default_connection(addr: tuple, connection: socket.socket) -> Union[bool, None]:
     print(f'Connected by {":".join(map(str, addr))}')
+    return None
 
 
 def _default_receive(addr: tuple, connection: socket.socket, data: bytes):
     pass
 
 
-def _default_disconnection(addr: tuple):
+def _default_disconnection(addr: tuple, disconnection_reason: Exception):
     print(f'Disconnected by {":".join(map(str, addr))}')
 
 
 def _default_universal(handler_type, addr: tuple, connection: Union[socket.socket, None], data: Union[bytes, None]):
     return True
 
 
@@ -43,69 +44,112 @@
         self.host = host
         self.port = port
         self.address = str(self.host) + ':' + str(self.port)
         self.is_listening = False
 
         def conn_handler(addr, conn: socket.socket):
             with conn:
+                disconnection_reason = None
                 while True:
                     try:
                         data = conn.recv(1024)
                     except OSError:
                         data = b''
 
                     if not data:
                         break
 
                     screen_lock.acquire()
-                    self._universal_handler(self.HandlerType.receive, addr, conn, data)
-                    self._receive_handler(addr, conn, data)
-                    if self.handler is not None:
-                        self.handler(addr, conn, data)
+                    try:
+                        self._universal_handler(self.HandlerType.receive, addr, conn, data)
+                        self._receive_handler(addr, conn, data)
+                        if self.handler is not None:
+                            self.handler(addr, conn, data)
+                    except (ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError,
+                            ConnectionError, OSError) as e:
+                        disconnection_reason = e
+                        break
+                    except Exception as e:
+                        print('\033[91mOh no! Something went wrong in your handler! Check it out and find '
+                              'problems:\033[0m')
+                        print(traceback.format_exc())
+                        print('\033[91mDisconnecting the client\033[0m')
+                        disconnection_reason = e
+                        conn.close()
+                        break
                     screen_lock.release()
 
                 screen_lock.acquire()
-                self._universal_handler(self.HandlerType.disconnection, addr, None, None)
-                self._disconnection_handler(addr)
+                try:
+                    self._universal_handler(self.HandlerType.disconnection, addr, None, None)
+                    self._disconnection_handler(addr, disconnection_reason)
+                except Exception:
+                    print('\033[91mOh no! Something went wrong in your handler! Check it out and find '
+                          'problems:\033[0m')
+                    print(traceback.format_exc())
                 screen_lock.release()
 
         def server():
             self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             s = self._socket
             s.bind((self.host, self.port))
             s.listen()
             screen_lock.acquire()
             print(f'Listening to {":".join(map(str, s.getsockname()))}')
             screen_lock.release()
             self.is_listening = True
-            while True:
+            while not self._socket_thread.shutdown:
                 try:
                     conn, addr = s.accept()
-                    screen_lock.acquire()
-                    connect_alt = self._universal_handler(self.HandlerType.connection, addr, None, None)
-                    connect = self._connection_handler(addr, conn)
-                    screen_lock.release()
-
-                    if connect is None:
-                        connect = connect_alt or True
-
-                    if connect:
-                        conn_thread = threading.Thread(target=conn_handler, args=(addr, conn))
-                        conn_thread.start()
-                    else:
-                        conn.close()
+                    if addr != self._socket_thread.shutdown_socket:
+                        screen_lock.acquire()
+                        try:
+                            connect_alt = self._universal_handler(self.HandlerType.connection, addr, None, None)
+                            connect = self._connection_handler(addr, conn)
+                        except (ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError,
+                                ConnectionError, OSError):
+                            continue
+
+                        screen_lock.release()
+
+                        if connect is None:
+                            connect = connect_alt or True
+
+                        if connect:
+                            conn_thread = threading.Thread(target=conn_handler, args=(addr, conn))
+                            conn_thread.start()
+                        else:
+                            conn.close()
                 except OSError:
                     break
+            screen_lock.acquire()
+            print(f'Closed {":".join(map(str, s.getsockname()))}')
+            screen_lock.release()
+            s.close()
+            self.closed = True
 
         self._socket_thread = threading.Thread(target=server, daemon=True)
+        self._socket_thread.shutdown = False
+        self._socket_thread.shutdown_socket = None
+        self.closed = False
 
     def start(self):
         """Starts TCP server"""
         self._socket_thread.start()
 
+    def close(self):
+        """Closes TCP server"""
+        self._socket_thread.shutdown = True
+        try:
+            closure_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            closure_socket.connect((self.host, self.port))
+            self._socket_thread.shutdown_socket = closure_socket.getsockname()
+        except (ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError, ConnectionError, OSError) as e:
+            raise e
+
     def set_handler(self, function):
         """
         Sets a handler for TCP server. Handler format:
 
         def server_handler(addr: tuple, conn: socket.socket, data: bytes): pass
         """
         self.handler = function
@@ -145,20 +189,21 @@
         """Use it to make server stoppable only by KeyboardInterrupt exception."""
         try:
             while not self.is_listening:
                 pass
             screen_lock.acquire()
             print('Press Ctrl + C to stop server!')
             screen_lock.release()
-            while True:
+            while not self.closed:
                 pass
         except KeyboardInterrupt:
             if hasattr(self, '_socket'):
                 screen_lock.acquire()
                 print('Stopping server...')
                 screen_lock.release()
-                self._socket: socket.socket
-                self._socket.close()
+                self.close()
+                while not self.closed:
+                    pass
 
     def mainloop(self):
         warnings.warn('This method is renamed to keep_alive', DeprecationWarning)
         self.keep_alive()
```

