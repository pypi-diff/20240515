# Comparing `tmp/pyview_web-0.0.7a0.tar.gz` & `tmp/pyview_web-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyview_web-0.0.7a0.tar", max compression
+gzip compressed data, was "pyview_web-0.0.8a0.tar", max compression
```

## Comparing `pyview_web-0.0.7a0.tar` & `pyview_web-0.0.8a0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
--rw-r--r--   0        0        0     1071 2023-05-02 00:38:29.733278 pyview_web-0.0.7a0/LICENSE
--rw-r--r--   0        0        0     2032 2023-06-14 00:15:29.628194 pyview_web-0.0.7a0/pyproject.toml
--rw-r--r--   0        0        0      223 2023-06-02 16:20:26.327598 pyview_web-0.0.7a0/pyview/__init__.py
--rw-r--r--   0        0        0     2508 2023-05-02 00:38:29.742232 pyview_web-0.0.7a0/pyview/assets/js/app.js
--rw-r--r--   0        0        0     2425 2023-05-02 00:38:29.742415 pyview_web-0.0.7a0/pyview/assets/package-lock.json
--rw-r--r--   0        0        0      151 2023-05-02 00:38:29.742554 pyview_web-0.0.7a0/pyview/assets/package.json
--rw-r--r--   0        0        0       46 2023-05-02 00:38:29.742781 pyview_web-0.0.7a0/pyview/changesets/__init__.py
--rw-r--r--   0        0        0     1747 2023-05-02 00:38:29.743020 pyview_web-0.0.7a0/pyview/changesets/changesets.py
--rw-r--r--   0        0        0      789 2023-06-13 01:17:27.976763 pyview_web-0.0.7a0/pyview/csrf.py
--rw-r--r--   0        0        0      125 2023-06-02 16:20:26.327913 pyview_web-0.0.7a0/pyview/events.py
--rw-r--r--   0        0        0      751 2023-05-02 00:38:29.743473 pyview_web-0.0.7a0/pyview/js.py
--rw-r--r--   0        0        0      498 2023-05-02 00:38:29.743607 pyview_web-0.0.7a0/pyview/live_routes.py
--rw-r--r--   0        0        0     3314 2023-06-02 16:20:26.328472 pyview_web-0.0.7a0/pyview/live_socket.py
--rw-r--r--   0        0        0     1255 2023-06-13 20:41:53.657377 pyview_web-0.0.7a0/pyview/live_view.py
--rw-r--r--   0        0        0     3801 2023-06-14 00:15:09.733211 pyview_web-0.0.7a0/pyview/pyview.py
--rw-r--r--   0        0        0      363 2023-06-13 01:17:27.979329 pyview_web-0.0.7a0/pyview/secret.py
--rw-r--r--   0        0        0      432 2023-06-13 01:17:27.980035 pyview_web-0.0.7a0/pyview/session.py
--rw-r--r--   0        0        0   199984 2023-05-02 00:38:29.745551 pyview_web-0.0.7a0/pyview/static/assets/app.js
--rw-r--r--   0        0        0      124 2023-05-02 00:38:29.745832 pyview_web-0.0.7a0/pyview/template/__init__.py
--rw-r--r--   0        0        0     1864 2023-05-02 00:38:29.745961 pyview_web-0.0.7a0/pyview/template/live_template.py
--rw-r--r--   0        0        0      826 2023-05-02 00:38:29.746088 pyview_web-0.0.7a0/pyview/template/serializer.py
--rw-r--r--   0        0        0      684 2023-05-02 00:38:29.746210 pyview_web-0.0.7a0/pyview/test_csrf.py
--rw-r--r--   0        0        0        0 2023-05-02 00:38:29.746312 pyview_web-0.0.7a0/pyview/vendor/__init__.py
--rw-r--r--   0        0        0       39 2023-05-02 00:38:29.746495 pyview_web-0.0.7a0/pyview/vendor/flet/pubsub/__init__.py
--rw-r--r--   0        0        0    10184 2023-05-02 00:38:29.746630 pyview_web-0.0.7a0/pyview/vendor/flet/pubsub/pub_sub.py
--rw-r--r--   0        0        0      455 2023-05-02 00:38:29.746775 pyview_web-0.0.7a0/pyview/vendor/ibis/__init__.py
--rw-r--r--   0        0        0     7220 2023-05-02 00:38:29.746901 pyview_web-0.0.7a0/pyview/vendor/ibis/compiler.py
--rw-r--r--   0        0        0     3613 2023-05-02 00:38:29.747013 pyview_web-0.0.7a0/pyview/vendor/ibis/context.py
--rw-r--r--   0        0        0     1531 2023-05-02 00:38:29.747126 pyview_web-0.0.7a0/pyview/vendor/ibis/errors.py
--rw-r--r--   0        0        0     7042 2023-05-02 00:38:29.747263 pyview_web-0.0.7a0/pyview/vendor/ibis/filters.py
--rw-r--r--   0        0        0     3457 2023-05-02 00:38:29.747371 pyview_web-0.0.7a0/pyview/vendor/ibis/loaders.py
--rw-r--r--   0        0        0    25128 2023-05-02 00:38:29.747569 pyview_web-0.0.7a0/pyview/vendor/ibis/nodes.py
--rw-r--r--   0        0        0     2314 2023-05-02 00:38:29.747704 pyview_web-0.0.7a0/pyview/vendor/ibis/template.py
--rw-r--r--   0        0        0     2293 2023-05-02 00:38:29.747817 pyview_web-0.0.7a0/pyview/vendor/ibis/tree.py
--rw-r--r--   0        0        0     2768 2023-05-02 00:38:29.747930 pyview_web-0.0.7a0/pyview/vendor/ibis/utils.py
--rw-r--r--   0        0        0     4707 2023-06-14 00:15:09.733494 pyview_web-0.0.7a0/pyview/ws_handler.py
--rw-r--r--   0        0        0     3154 2023-06-13 01:17:27.982729 pyview_web-0.0.7a0/readme.md
--rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 pyview_web-0.0.7a0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-02 00:38:29.733278 pyview_web-0.0.8a0/LICENSE
+-rw-r--r--   0        0        0     2032 2024-05-15 00:40:24.073292 pyview_web-0.0.8a0/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-06-02 16:20:26.327598 pyview_web-0.0.8a0/pyview/__init__.py
+-rw-r--r--   0        0        0     2508 2023-05-02 00:38:29.742232 pyview_web-0.0.8a0/pyview/assets/js/app.js
+-rw-r--r--   0        0        0     2425 2023-05-02 00:38:29.742415 pyview_web-0.0.8a0/pyview/assets/package-lock.json
+-rw-r--r--   0        0        0      151 2023-05-02 00:38:29.742554 pyview_web-0.0.8a0/pyview/assets/package.json
+-rw-r--r--   0        0        0      109 2023-06-14 00:18:12.775162 pyview_web-0.0.8a0/pyview/auth/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-14 00:18:12.775807 pyview_web-0.0.8a0/pyview/auth/provider.py
+-rw-r--r--   0        0        0     1223 2023-06-14 00:18:12.776363 pyview_web-0.0.8a0/pyview/auth/required.py
+-rw-r--r--   0        0        0       46 2023-05-02 00:38:29.742781 pyview_web-0.0.8a0/pyview/changesets/__init__.py
+-rw-r--r--   0        0        0     1747 2023-05-02 00:38:29.743020 pyview_web-0.0.8a0/pyview/changesets/changesets.py
+-rw-r--r--   0        0        0      789 2023-06-13 01:17:27.976763 pyview_web-0.0.8a0/pyview/csrf.py
+-rw-r--r--   0        0        0      125 2023-06-02 16:20:26.327913 pyview_web-0.0.8a0/pyview/events.py
+-rw-r--r--   0        0        0      751 2023-05-02 00:38:29.743473 pyview_web-0.0.8a0/pyview/js.py
+-rw-r--r--   0        0        0      498 2023-05-02 00:38:29.743607 pyview_web-0.0.8a0/pyview/live_routes.py
+-rw-r--r--   0        0        0     3314 2023-06-30 19:20:12.827751 pyview_web-0.0.8a0/pyview/live_socket.py
+-rw-r--r--   0        0        0     1255 2023-06-13 20:41:53.657377 pyview_web-0.0.8a0/pyview/live_view.py
+-rw-r--r--   0        0        0     2302 2024-05-15 00:18:19.445788 pyview_web-0.0.8a0/pyview/pyview.py
+-rw-r--r--   0        0        0      363 2023-06-13 01:17:27.979329 pyview_web-0.0.8a0/pyview/secret.py
+-rw-r--r--   0        0        0      432 2023-06-13 01:17:27.980035 pyview_web-0.0.8a0/pyview/session.py
+-rw-r--r--   0        0        0   199984 2023-05-02 00:38:29.745551 pyview_web-0.0.8a0/pyview/static/assets/app.js
+-rw-r--r--   0        0        0      206 2024-05-15 00:06:35.328321 pyview_web-0.0.8a0/pyview/template/__init__.py
+-rw-r--r--   0        0        0     1864 2023-06-21 01:27:08.244253 pyview_web-0.0.8a0/pyview/template/live_template.py
+-rw-r--r--   0        0        0     1876 2024-05-15 00:33:27.966402 pyview_web-0.0.8a0/pyview/template/root_template.py
+-rw-r--r--   0        0        0      826 2023-05-02 00:38:29.746088 pyview_web-0.0.8a0/pyview/template/serializer.py
+-rw-r--r--   0        0        0      684 2023-05-02 00:38:29.746210 pyview_web-0.0.8a0/pyview/test_csrf.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:38:29.746312 pyview_web-0.0.8a0/pyview/vendor/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-02 00:38:29.746495 pyview_web-0.0.8a0/pyview/vendor/flet/pubsub/__init__.py
+-rw-r--r--   0        0        0    10184 2023-05-02 00:38:29.746630 pyview_web-0.0.8a0/pyview/vendor/flet/pubsub/pub_sub.py
+-rw-r--r--   0        0        0      455 2023-05-02 00:38:29.746775 pyview_web-0.0.8a0/pyview/vendor/ibis/__init__.py
+-rw-r--r--   0        0        0     7220 2023-05-02 00:38:29.746901 pyview_web-0.0.8a0/pyview/vendor/ibis/compiler.py
+-rw-r--r--   0        0        0     3613 2023-05-02 00:38:29.747013 pyview_web-0.0.8a0/pyview/vendor/ibis/context.py
+-rw-r--r--   0        0        0     1531 2023-05-02 00:38:29.747126 pyview_web-0.0.8a0/pyview/vendor/ibis/errors.py
+-rw-r--r--   0        0        0     7042 2023-05-02 00:38:29.747263 pyview_web-0.0.8a0/pyview/vendor/ibis/filters.py
+-rw-r--r--   0        0        0     3457 2023-05-02 00:38:29.747371 pyview_web-0.0.8a0/pyview/vendor/ibis/loaders.py
+-rw-r--r--   0        0        0    25128 2023-05-02 00:38:29.747569 pyview_web-0.0.8a0/pyview/vendor/ibis/nodes.py
+-rw-r--r--   0        0        0     2314 2023-06-30 19:20:12.828275 pyview_web-0.0.8a0/pyview/vendor/ibis/template.py
+-rw-r--r--   0        0        0     2293 2023-05-02 00:38:29.747817 pyview_web-0.0.8a0/pyview/vendor/ibis/tree.py
+-rw-r--r--   0        0        0     2768 2023-05-02 00:38:29.747930 pyview_web-0.0.8a0/pyview/vendor/ibis/utils.py
+-rw-r--r--   0        0        0     4738 2023-06-15 02:43:05.038205 pyview_web-0.0.8a0/pyview/ws_handler.py
+-rw-r--r--   0        0        0     3154 2023-06-13 01:17:27.982729 pyview_web-0.0.8a0/readme.md
+-rw-r--r--   0        0        0     4970 1970-01-01 00:00:00.000000 pyview_web-0.0.8a0/PKG-INFO
```

### Comparing `pyview_web-0.0.7a0/LICENSE` & `pyview_web-0.0.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyproject.toml` & `pyview_web-0.0.8a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "pyview-web"
 
 packages = [
   { include = "pyview" },
 ]
 
-version = "0.0.7a"
+version = "0.0.8a"
 description = "LiveView in Python"
 authors = ["Larry Ogrodnek <ogrodnek@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://pyview.rocks"
 repository = "https://github.com/ogrodnek/pyview"
 keywords = ["web", "api", "LiveView"]
```

### Comparing `pyview_web-0.0.7a0/pyview/assets/js/app.js` & `pyview_web-0.0.8a0/pyview/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/assets/package-lock.json` & `pyview_web-0.0.8a0/pyview/assets/package-lock.json`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/changesets/changesets.py` & `pyview_web-0.0.8a0/pyview/changesets/changesets.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/csrf.py` & `pyview_web-0.0.8a0/pyview/csrf.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/js.py` & `pyview_web-0.0.8a0/pyview/js.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/live_socket.py` & `pyview_web-0.0.8a0/pyview/live_socket.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/live_view.py` & `pyview_web-0.0.8a0/pyview/live_view.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/static/assets/app.js` & `pyview_web-0.0.8a0/pyview/static/assets/app.js`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/template/live_template.py` & `pyview_web-0.0.8a0/pyview/template/live_template.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/template/serializer.py` & `pyview_web-0.0.8a0/pyview/template/serializer.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/test_csrf.py` & `pyview_web-0.0.8a0/pyview/test_csrf.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/flet/pubsub/pub_sub.py` & `pyview_web-0.0.8a0/pyview/vendor/flet/pubsub/pub_sub.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/ibis/compiler.py` & `pyview_web-0.0.8a0/pyview/vendor/ibis/compiler.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/ibis/context.py` & `pyview_web-0.0.8a0/pyview/vendor/ibis/context.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/ibis/errors.py` & `pyview_web-0.0.8a0/pyview/vendor/ibis/errors.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/ibis/filters.py` & `pyview_web-0.0.8a0/pyview/vendor/ibis/filters.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/ibis/loaders.py` & `pyview_web-0.0.8a0/pyview/vendor/ibis/loaders.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/ibis/nodes.py` & `pyview_web-0.0.8a0/pyview/vendor/ibis/nodes.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/ibis/template.py` & `pyview_web-0.0.8a0/pyview/vendor/ibis/template.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/ibis/tree.py` & `pyview_web-0.0.8a0/pyview/vendor/ibis/tree.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/vendor/ibis/utils.py` & `pyview_web-0.0.8a0/pyview/vendor/ibis/utils.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/pyview/ws_handler.py` & `pyview_web-0.0.8a0/pyview/ws_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,40 +2,50 @@
 from fastapi import WebSocket, WebSocketDisconnect
 import json
 from urllib.parse import urlparse, parse_qs
 from pyview.live_socket import LiveViewSocket
 from pyview.live_routes import LiveViewLookup
 from pyview.csrf import validate_csrf_token
 from pyview.session import deserialize_session
+from pyview.auth import AuthProviderFactory
+
+
+class AuthException(Exception):
+    pass
 
 
 class LiveSocketHandler:
     def __init__(self, routes: LiveViewLookup):
         self.routes = routes
         self.manager = ConnectionManager()
         self.sessions = 0
 
+    async def check_auth(self, websocket: WebSocket, lv):
+        if not await AuthProviderFactory.get(lv).has_required_auth(websocket):
+            raise AuthException()
+
     async def handle(self, websocket: WebSocket):
         await self.manager.connect(websocket)
 
         self.sessions += 1
         topic = None
         socket: Optional[LiveViewSocket] = None
 
         try:
             data = await websocket.receive_text()
             [joinRef, mesageRef, topic, event, payload] = json.loads(data)
             if event == "phx_join":
+                if not validate_csrf_token(payload["params"]["_csrf_token"], topic):
+                    raise AuthException("Invalid CSRF token")
+
                 url = urlparse(payload["url"])
                 lv = self.routes.get(url.path)
+                await self.check_auth(websocket, lv)
                 socket = LiveViewSocket(websocket, topic, lv)
 
-                if not validate_csrf_token(payload["params"]["_csrf_token"], topic):
-                    raise Exception("Invalid CSRF token")
-
                 session = {}
                 if "session" in payload:
                     session = deserialize_session(payload["session"])
 
                 await lv.mount(socket, session)
                 await lv.handle_params(url, parse_qs(url.query), socket)
 
@@ -49,18 +59,20 @@
                     {"response": {"rendered": rendered}, "status": "ok"},
                 ]
 
                 await self.manager.send_personal_message(json.dumps(resp), websocket)
                 await self.handle_connected(socket)
 
         except WebSocketDisconnect:
-            self.manager.disconnect(websocket)
             if socket:
                 await socket.close()
             self.sessions -= 1
+        except AuthException:
+            await websocket.close()
+            self.sessions -= 1
 
     async def handle_connected(self, socket: LiveViewSocket):
         while True:
             data = await socket.websocket.receive_text()
             [joinRef, mesageRef, topic, event, payload] = json.loads(data)
 
             if event == "heartbeat":
@@ -118,22 +130,14 @@
         socket.live_title = None
 
     return rendered
 
 
 class ConnectionManager:
     def __init__(self):
-        self.active_connections: list[WebSocket] = []
+        pass
 
     async def connect(self, websocket: WebSocket):
         await websocket.accept()
-        self.active_connections.append(websocket)
-
-    def disconnect(self, websocket: WebSocket):
-        self.active_connections.remove(websocket)
 
     async def send_personal_message(self, message: str, websocket: WebSocket):
         await websocket.send_text(message)
-
-    async def broadcast(self, message: str):
-        for connection in self.active_connections:
-            await connection.send_text(message)
```

### Comparing `pyview_web-0.0.7a0/readme.md` & `pyview_web-0.0.8a0/readme.md`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.7a0/PKG-INFO` & `pyview_web-0.0.8a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyview-web
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: LiveView in Python
 Home-page: https://pyview.rocks
 License: MIT
 Keywords: web,api,LiveView
 Author: Larry Ogrodnek
 Author-email: ogrodnek@gmail.com
 Requires-Python: >=3.9.16,<4.0.0
@@ -18,18 +18,16 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

