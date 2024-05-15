# Comparing `tmp/clipshare-0.1.4.tar.gz` & `tmp/clipshare-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipshare-0.1.4.tar", last modified: Tue May 14 06:16:21 2024, max compression
+gzip compressed data, was "clipshare-0.1.5.tar", last modified: Wed May 15 17:36:35 2024, max compression
```

## Comparing `clipshare-0.1.4.tar` & `clipshare-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:16:21.365211 clipshare-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-14 06:16:17.000000 clipshare-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 06:16:17.000000 clipshare-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-14 06:16:21.365211 clipshare-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-14 06:16:17.000000 clipshare-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:16:21.361211 clipshare-0.1.4/clipShare/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32482 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/clipShare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:16:21.361211 clipshare-0.1.4/clipShare/web-interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/web-interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:16:21.357211 clipshare-0.1.4/clipShare/web-interface/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:16:21.361211 clipshare-0.1.4/clipShare/web-interface/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    73502 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/web-interface/static/images/clipShare.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/web-interface/static/images/help.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:16:21.361211 clipshare-0.1.4/clipShare/web-interface/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    48316 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/web-interface/static/js/crypto-js.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/web-interface/static/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)   185790 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/web-interface/static/js/socket.io.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:16:21.361211 clipshare-0.1.4/clipShare/web-interface/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-14 06:16:17.000000 clipshare-0.1.4/clipShare/web-interface/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:16:21.361211 clipshare-0.1.4/clipShare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-14 06:16:21.000000 clipshare-0.1.4/clipShare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-14 06:16:21.000000 clipshare-0.1.4/clipShare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:16:21.000000 clipshare-0.1.4/clipShare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 06:16:21.000000 clipshare-0.1.4/clipShare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 06:16:21.000000 clipshare-0.1.4/clipShare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 06:16:21.000000 clipshare-0.1.4/clipShare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:16:21.365211 clipshare-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-14 06:16:17.000000 clipshare-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:36:35.879017 clipshare-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-15 17:36:30.000000 clipshare-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 17:36:30.000000 clipshare-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-15 17:36:35.879017 clipshare-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-15 17:36:30.000000 clipshare-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:36:35.875017 clipshare-0.1.5/clipShare/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/clipShare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:36:35.879017 clipshare-0.1.5/clipShare/web-interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/web-interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:36:35.875017 clipshare-0.1.5/clipShare/web-interface/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:36:35.879017 clipshare-0.1.5/clipShare/web-interface/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    73502 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/web-interface/static/images/clipShare.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/web-interface/static/images/help.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:36:35.879017 clipshare-0.1.5/clipShare/web-interface/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    48316 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/web-interface/static/js/crypto-js.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/web-interface/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)   185790 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/web-interface/static/js/socket.io.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:36:35.879017 clipshare-0.1.5/clipShare/web-interface/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-15 17:36:30.000000 clipshare-0.1.5/clipShare/web-interface/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:36:35.879017 clipshare-0.1.5/clipShare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-15 17:36:35.000000 clipshare-0.1.5/clipShare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-15 17:36:35.000000 clipshare-0.1.5/clipShare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:36:35.000000 clipshare-0.1.5/clipShare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 17:36:35.000000 clipshare-0.1.5/clipShare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 17:36:35.000000 clipshare-0.1.5/clipShare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 17:36:35.000000 clipshare-0.1.5/clipShare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:36:35.879017 clipshare-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-15 17:36:30.000000 clipshare-0.1.5/setup.py
```

### Comparing `clipshare-0.1.4/LICENSE` & `clipshare-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clipshare-0.1.4/PKG-INFO` & `clipshare-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipShare
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sync clipboard between devices
 Home-page: https://github.com/avinashkarhana/clipShare
 Author: Avinash Karhana
 Author-email: avinashkarhana1@gmail.com
 License: LGPLv2.1
 Keywords: clipboardSync clipboard sync share encrypted secure clipShare
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipShare Version: 0.1.4 Summary: Sync clipboard
+Metadata-Version: 2.1 Name: clipShare Version: 0.1.5 Summary: Sync clipboard
 between devices Home-page: https://github.com/avinashkarhana/clipShare Author:
 Avinash Karhana Author-email: avinashkarhana1@gmail.com License: LGPLv2.1
 Keywords: clipboardSync clipboard sync share encrypted secure clipShare
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v2 (LGPLv2) Classifier: Natural Language :: English Classifier:
```

### Comparing `clipshare-0.1.4/README.md` & `clipshare-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `clipshare-0.1.4/clipShare/clipShare.py` & `clipshare-0.1.5/clipShare/clipShare.py`

 * *Files 9% similar despite different names*

```diff
@@ -114,33 +114,33 @@
 def on_disconnect():
     global authenticated_clients
     found_client = False
     for client in authenticated_clients:
         if client['clientId'] == request.sid:
             found_client = True
             authenticated_clients.remove(client)
-            print(f'#> Client {request.sid} disconnected.')
+            print(f'{bcolors.OKBLUE}#> Client {request.sid} disconnected.{bcolors.ENDC}')
             break
     if not found_client:
-        print(f'#> Client {request.sid} disconnected without authentication.')
+        print(f'{bcolors.OKCYAN}#> Client {request.sid} disconnected without authentication.{bcolors.ENDC}')
 
 @socketio.on('authentication_from_client', namespace='/')
 def auth_request_from_client(data):
     global authenticated_clients
     if str(data.get('passcode')) == str(passcode):
         md5_hash = hashlib.md5(str(random.randint(0, 100000000)).encode()).hexdigest()
         emit('authentication_to_client', {'success': True, 'token': md5_hash, 'msg': 'Pass this token along all further requests'}, broadcast=False)
         for client in authenticated_clients:
             if client['clientId'] == request.sid:
                 authenticated_clients.remove(client)
         now_time = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
         authenticated_clients.append({ "clientId": request.sid, "hash": md5_hash, "ip": request.remote_addr, "connection_time": now_time })
-        print(f'#> Client {request.sid} from {request.remote_addr} authenticated successfully at {now_time}.')
+        print(f'{bcolors.OKGREEN}#> Client {request.sid} from {request.remote_addr} authenticated successfully at {now_time}.{bcolors.ENDC}')
     else:
-        print(f'#> Client {request.sid} authentication failed. Disconnecting...')
+        print(f'{bcolors.FAIL}#> Client {request.sid} authentication failed. Disconnecting...{bcolors.ENDC}')
         emit('authentication_to_client', {'success': False, 'msg': 'Authentication Failed due to inavlid passcode!'}, broadcast=False)
         disconnect(request.sid)
 
 @socketio.on('connect', namespace='/')
 def on_connect():
     print(f'#> Client Connection {request.sid}')
     for client in authenticated_clients:
@@ -246,22 +246,14 @@
         server_clipboard_thread_started = True
     except (KeyboardInterrupt, SystemExit):
         global QUITTING
         QUITTING = True
         print('\n# Received keyboard interrupt, quitting...')
         exit()
 
-def get_shortened_url(url):
-    # Make a request to bitly.ws to shorten the URL
-    shortne_service_url = f"https://shorter.me/page/shorten"
-    response = requests.post(shortne_service_url, data={'url': url})
-    if response.status_code == 200:
-        shortened_url = response.json()['data']
-        print(f' * Shortened URL: {shortened_url}')
-
 def run_server():
     global ADVERTISE_SERVER
     global QUITTING
     global server_port
     global server_name
     global public_url
     global SERVE_ON_NGROK_TUNNEL
@@ -278,14 +270,20 @@
     socketio.run(app, host='0.0.0.0', port=server_port)
     ADVERTISE_SERVER = False
     QUITTING = True
     print("\n# Server stopped.")
     if SERVE_ON_NGROK_TUNNEL:
         ngrok.disconnect(public_url)
         ngrok.kill()
+        if SERVE_ON_NGROK_TUNNEL:
+            try:
+                ngrok.disconnect(public_url)
+                ngrok.kill()
+            except:
+                print("Error stopping ngrok tunnel. But it will be stopped and process will be killed automatically when this process finishes.")
 
 def act_as_server():
     run_server()
 
 
 ##############################################################################################################
 # Web Client Code
@@ -576,16 +574,119 @@
         if QUITTING:
             exit()
 
     print("\nRunning as a client")
     run_client()
 
 ##############################################################################################################
-# Main
+# Main / Utility Code
 ##############################################################################################################
+class bcolors:
+    HEADER = '\033[95m'
+    OKBLUE = '\033[94m'
+    OKCYAN = '\033[96m'
+    OKGREEN = '\033[92m'
+    WARNING = '\033[93m'
+    FAIL = '\033[91m'
+    ENDC = '\033[0m'
+    BOLD = '\033[1m'
+    UNDERLINE = '\033[4m'
+
+def get_shortened_url(url, service_opt="1", custom="clipShare"):
+    custom += str(random.randint(1000, 9999))
+    error = False
+    possible_service_opts = [
+        "1",
+        "2",
+        "3",
+        "4"
+    ]
+    if service_opt not in possible_service_opts:
+        service_opt = possible_service_opts[0]
+    if str(service_opt) == "1":
+        # Make a request to shorter.me to shorten the URL
+        service_url = "https://shorter.me/page/shorten"
+        data = {'url': url}
+        try:
+            response = requests.post(service_url, data=data)
+            if response.status_code == 200:
+                shortened_url = response.json().get('data')
+                print(f' * Shortened URL (shorter.me): {shortened_url}')
+            else:
+                error = True
+        except:
+            error = True
+
+    elif service_opt == "2":
+        # Make a request to smolurl.com API to shorten the URL
+        api_url = "https://smolurl.com/api/links"
+        headers = {
+            "Accept": "application/json",
+            "Content-Type": "application/json"
+        }
+        data = {
+            "url": url
+        }
+        try:
+            response = requests.post(api_url, headers=headers, json=data)
+            if response.status_code >= 200 and response.status_code < 300:
+                shortened_url = response.json()['data']['short_url']
+                print(f' * Shortened URL (smolurl.com): {shortened_url}')
+            else:
+                error = True
+        except:
+            error = True
+    elif service_opt == "3":
+        base_url = "https://ulvis.net"
+        api_endpoint = "/api.php"
+        full_url = f"{base_url}{api_endpoint}?url={url}"
+        if custom:
+            full_url += f"&custom={custom}"
+        try:
+            response = requests.get(full_url)
+            if response.status_code == 200:
+                shortened_url = response.text
+                print(f' * Shortened URL (ulvis.net): {shortened_url}')
+            else:
+                error = True
+        except:
+            error = True
+    elif service_opt == "4":
+        # Make a request to api.encurtador.dev to shorten the URL
+        api_url = "https://api.encurtador.dev/encurtamentos"
+        headers = {
+            "Content-Type": "application/json"
+        }
+        data = {
+            "url": url,
+            "codigo": custom
+        }
+        try:
+            response = requests.post(api_url, headers=headers, json=data)
+            if response.status_code == 200:
+                shortened_url = response.json()['urlEncurtada']
+                if shortened_url[:8] != "https":
+                    shortened_url = f"https://{shortened_url}"
+                print(f' * Shortened URL (api.encurtador.dev): {shortened_url}')
+            else:
+                error = True
+        except:
+            error = True
+    else:
+        print(f"Invalid service specified. Please choose {possible_service_opts} as service options.")
+    if error:
+        # Try next service
+        current_service_index = possible_service_opts.index(service_opt)
+        next_service_index = current_service_index + 1
+        if next_service_index < len(possible_service_opts):
+            get_shortened_url(url, possible_service_opts[next_service_index])
+        else:
+            print("Couldn't shorten the URL. Please try again later.")
+            return
+
 def set_ngrok_auth_token():
     global SERVE_ON_NGROK_TUNNEL
     # Read ngrok auth token from file and set it if SERVE_ON_NGROK_TUNNEL is True
     if SERVE_ON_NGROK_TUNNEL:
         try:
             with open(f'{current_working_directory}/ngrok-auth-token.txt', 'r') as f:
                 ngrok_auth_token = f.read()
```

### Comparing `clipshare-0.1.4/clipShare/web-interface/static/images/clipShare.jpeg` & `clipshare-0.1.5/clipShare/web-interface/static/images/clipShare.jpeg`

 * *Files identical despite different names*

### Comparing `clipshare-0.1.4/clipShare/web-interface/static/images/help.png` & `clipshare-0.1.5/clipShare/web-interface/static/images/help.png`

 * *Files identical despite different names*

### Comparing `clipshare-0.1.4/clipShare/web-interface/static/js/crypto-js.min.js` & `clipshare-0.1.5/clipShare/web-interface/static/js/crypto-js.min.js`

 * *Files identical despite different names*

### Comparing `clipshare-0.1.4/clipShare/web-interface/static/js/main.js` & `clipshare-0.1.5/clipShare/web-interface/static/js/main.js`

 * *Files identical despite different names*

### Comparing `clipshare-0.1.4/clipShare/web-interface/static/js/socket.io.js` & `clipshare-0.1.5/clipShare/web-interface/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `clipshare-0.1.4/clipShare/web-interface/templates/index.html` & `clipshare-0.1.5/clipShare/web-interface/templates/index.html`

 * *Files identical despite different names*

### Comparing `clipshare-0.1.4/clipShare.egg-info/PKG-INFO` & `clipshare-0.1.5/clipShare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipShare
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sync clipboard between devices
 Home-page: https://github.com/avinashkarhana/clipShare
 Author: Avinash Karhana
 Author-email: avinashkarhana1@gmail.com
 License: LGPLv2.1
 Keywords: clipboardSync clipboard sync share encrypted secure clipShare
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipShare Version: 0.1.4 Summary: Sync clipboard
+Metadata-Version: 2.1 Name: clipShare Version: 0.1.5 Summary: Sync clipboard
 between devices Home-page: https://github.com/avinashkarhana/clipShare Author:
 Avinash Karhana Author-email: avinashkarhana1@gmail.com License: LGPLv2.1
 Keywords: clipboardSync clipboard sync share encrypted secure clipShare
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v2 (LGPLv2) Classifier: Natural Language :: English Classifier:
```

### Comparing `clipshare-0.1.4/clipShare.egg-info/SOURCES.txt` & `clipshare-0.1.5/clipShare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipshare-0.1.4/setup.py` & `clipshare-0.1.5/setup.py`

 * *Files identical despite different names*

