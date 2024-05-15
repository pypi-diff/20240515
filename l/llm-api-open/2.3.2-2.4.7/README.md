# Comparing `tmp/llm_api_open-2.3.2.tar.gz` & `tmp/llm_api_open-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_api_open-2.3.2.tar", last modified: Fri Apr 19 10:04:50 2024, max compression
+gzip compressed data, was "llm_api_open-2.4.7.tar", last modified: Wed May 15 07:05:08 2024, max compression
```

## Comparing `llm_api_open-2.3.2.tar` & `llm_api_open-2.4.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:50.137666 llm_api_open-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25156 2024-04-19 10:04:50.137666 llm_api_open-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23555 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:50.133666 llm_api_open-2.3.2/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/configs/chatgpt.json
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/configs/ms_copilot.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:04:50.137666 llm_api_open-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:50.129666 llm_api_open-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:50.133666 llm_api_open-2.3.2/src/llm_api_open.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25156 2024-04-19 10:04:50.000000 llm_api_open-2.3.2/src/llm_api_open.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-19 10:04:50.000000 llm_api_open-2.3.2/src/llm_api_open.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:04:50.000000 llm_api_open-2.3.2/src/llm_api_open.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 10:04:50.000000 llm_api_open-2.3.2/src/llm_api_open.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 10:04:50.000000 llm_api_open-2.3.2/src/llm_api_open.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 10:04:50.000000 llm_api_open-2.3.2/src/llm_api_open.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:50.133666 llm_api_open-2.3.2/src/lmao/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:50.133666 llm_api_open-2.3.2/src/lmao/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/chatgpt/assistantGetLastMessage.js
--rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/chatgpt/chatgpt_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/chatgpt/conversationSearch.js
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/chatgpt/proxy_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/external_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11895 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/module_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:50.133666 llm_api_open-2.3.2/src/lmao/ms_copilot/
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/ms_copilot/conversationManage.js
--rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/ms_copilot/conversationParser.js
--rw-r--r--   0 runner    (1001) docker     (127)    43383 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/ms_copilot/ms_copilot_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-19 10:04:44.000000 llm_api_open-2.3.2/src/lmao/ms_copilot/proxy_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:05:08.362650 llm_api_open-2.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25505 2024-05-15 07:05:08.358650 llm_api_open-2.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:05:08.358650 llm_api_open-2.4.7/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/configs/chatgpt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/configs/ms_copilot.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:05:08.362650 llm_api_open-2.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:05:08.354650 llm_api_open-2.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:05:08.358650 llm_api_open-2.4.7/src/llm_api_open.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25505 2024-05-15 07:05:08.000000 llm_api_open-2.4.7/src/llm_api_open.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 07:05:08.000000 llm_api_open-2.4.7/src/llm_api_open.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:05:08.000000 llm_api_open-2.4.7/src/llm_api_open.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 07:05:08.000000 llm_api_open-2.4.7/src/llm_api_open.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 07:05:08.000000 llm_api_open-2.4.7/src/llm_api_open.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 07:05:08.000000 llm_api_open-2.4.7/src/llm_api_open.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:05:08.358650 llm_api_open-2.4.7/src/lmao/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:05:08.358650 llm_api_open-2.4.7/src/lmao/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/chatgpt/assistantGetLastMessage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    40593 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/chatgpt/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/chatgpt/conversationSearch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/chatgpt/proxy_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21405 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/external_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11895 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/module_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:05:08.358650 llm_api_open-2.4.7/src/lmao/ms_copilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/ms_copilot/conversationManage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16663 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/ms_copilot/conversationParser.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43466 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/ms_copilot/ms_copilot_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-15 07:05:01.000000 llm_api_open-2.4.7/src/lmao/ms_copilot/proxy_extension.py
```

### Comparing `llm_api_open-2.3.2/LICENSE` & `llm_api_open-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_api_open-2.3.2/PKG-INFO` & `llm_api_open-2.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.3.2
+Version: 2.4.7
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -759,7 +759,16 @@
 2024-04-19 02:07:02 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
  * Running on all addresses (0.0.0.0)
  * Running on http://127.0.0.1:1312
  * Running on http://192.168.0.3:1312
 2024-04-19 02:07:02 INFO     Press CTRL+C to quit
 ...
 ```
+
+----------
+
+## 🐛 How to fix `Failed to establish a new connection` when using multiple modules
+
+1. Open `venv/lib/python3.XX/site-packages/undetected_chromedriver/patcher.py`
+2. Add `import secrets` to the imports
+3. In `def __init__` change `prefix = "undetected"` to `prefix = f"undetected{secrets.token_hex(4)}"`
+4. Save file and reload LMAO
```

### Comparing `llm_api_open-2.3.2/README.md` & `llm_api_open-2.4.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -721,7 +721,16 @@
 2024-04-19 02:07:02 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
  * Running on all addresses (0.0.0.0)
  * Running on http://127.0.0.1:1312
  * Running on http://192.168.0.3:1312
 2024-04-19 02:07:02 INFO     Press CTRL+C to quit
 ...
 ```
+
+----------
+
+## 🐛 How to fix `Failed to establish a new connection` when using multiple modules
+
+1. Open `venv/lib/python3.XX/site-packages/undetected_chromedriver/patcher.py`
+2. Add `import secrets` to the imports
+3. In `def __init__` change `prefix = "undetected"` to `prefix = f"undetected{secrets.token_hex(4)}"`
+4. Save file and reload LMAO
```

### Comparing `llm_api_open-2.3.2/configs/chatgpt.json` & `llm_api_open-2.4.7/configs/ms_copilot.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888157894736842%*

 * *Differences: {"'__comment01__'": "'Microsoft Copilot module config file "*

 * *                    "<https://github.com/F33RNI/LlM-Api-Open>'",*

 * * "'__comment02__'": "'File for loading and saving cookies. (Possibly not required anymore) Install "*

 * *                    "editor extension:'",*

 * * "'__comment04__'": "'Go to <https://copilot.microsoft.com/> log in and ask about something. Wait "*

 * *                    "for response'",*

 * * "'__comment11__'": '"It\'s recommended to leave this empty"',*

 * * "'__comment17__'": "'MS Copilot Web page a […]*

```diff
@@ -1,48 +1,57 @@
 {
-    "__comment01__": "ChatGPT module config file <https://github.com/F33RNI/LlM-Api-Open>",
-    "__comment02__": "File for loading and saving cookies. Install cookie editor extension, for example:",
+    "__comment01__": "Microsoft Copilot module config file <https://github.com/F33RNI/LlM-Api-Open>",
+    "__comment02__": "File for loading and saving cookies. (Possibly not required anymore) Install editor extension:",
     "__comment03__": "<https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm>",
-    "__comment04__": "Go to <https://chat.openai.com/> and ask ChatGPT about something",
+    "__comment04__": "Go to <https://copilot.microsoft.com/> log in and ask about something. Wait for response",
     "__comment05__": "Open the extension, click Export on the bottom right, then Export as JSON",
     "__comment06__": "(This saves your cookies to clipboard). Create a new .json file and paste cookies into it",
     "__comment07__": "save file and specify path to it here. File also must have write permissions",
     "__comment08__": "Path to browser executable or empty to auto-detect (ex. /usr/bin/google-chrome-stable)",
     "__comment09__": "Major version of browser to pass as version_main argument or null to auto-detect (ex. 122)",
     "__comment10__": "Path to driver executable to pass as driver_executable_path argument or empty for auto",
-    "__comment11__": "It's recommended ot leave this empty",
+    "__comment11__": "It's recommended to leave this empty",
     "__comment12__": "Set to true to enable proxy",
     "__comment13__": "Proxy host (ip) as string",
     "__comment14__": "Proxy port as integer",
     "__comment15__": "Proxy username or empty",
     "__comment16__": "Proxy password or empty",
-    "__comment17__": "ChatGPT Web page address",
+    "__comment17__": "MS Copilot Web page address",
     "__comment18__": "Start browser in headless mode (without GUI)",
     "__comment19__": "Chrome arguments",
     "__comment20__": "--headless= argument. Leave empty to use default value",
     "__comment21__": "Time (s) for automatically refresh page if no new prompts or responses (to update session)",
     "__comment22__": "Set to 0 to disable auto-refresher",
     "__comment23__": "User agent to prevent detection of headless chrome. Leave empty to disable it",
-    "auto_refresh_interval": 120,
-    "base_url": "https://chat.openai.com/",
+    "auto_refresh_interval": 300,
+    "base_url": "https://copilot.microsoft.com/",
     "browser_executable_path": "",
     "chrome_options": [
         "--disable-infobars",
         "--ignore-ssl-errors=yes",
         "--ignore-certificate-errors",
         "--disable-default-apps",
         "--disable-notifications",
         "--disable-popup-window",
         "--no-sandbox",
         "--auto-open-devtools-for-tabs",
         "--dns-prefetch-disable",
         "--disable-gpu",
+        "--disable-dev-shm-usage",
+        "--disable-renderer-backgrounding",
+        "--disable-background-timer-throttling",
+        "--disable-backgrounding-occluded-windows",
+        "--disable-client-side-phishing-detection",
+        "--disable-crash-reporter",
+        "--disable-oopr-debug-crash-dump",
+        "--no-crash-upload",
+        "--disable-low-res-tiling",
         "--window-size=1920x960"
     ],
-    "cookies_file": "ChatGPT_cookies.json",
+    "cookies_file": "MS_Copilot_cookies.json",
     "driver_executable_path": "",
     "headless": true,
     "headless_mode": "old",
     "proxy_enabled": false,
     "proxy_host": "123.45.67.89",
     "proxy_password": "",
     "proxy_port": 8080,
```

### Comparing `llm_api_open-2.3.2/configs/ms_copilot.json` & `llm_api_open-2.4.7/configs/chatgpt.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888157894736842%*

 * *Differences: {"'__comment01__'": "'ChatGPT module config file <https://github.com/F33RNI/LlM-Api-Open>'",*

 * * "'__comment02__'": "'File for loading and saving cookies. (Possibly not required anymore) Install "*

 * *                    "editor extension:'",*

 * * "'__comment04__'": "'Go to <https://chat.openai.com/> and ask ChatGPT about something'",*

 * * "'__comment11__'": '"It\'s recommended to leave this empty"',*

 * * "'__comment17__'": "'ChatGPT Web page address'",*

 * * "'auto_refresh_interval'": '120',*

 * * "'base_url'": "'https://chat.openai.c […]*

```diff
@@ -1,48 +1,57 @@
 {
-    "__comment01__": "Microsoft Copilot module config file <https://github.com/F33RNI/LlM-Api-Open>",
-    "__comment02__": "File for loading and saving cookies. Install cookie editor extension, for example:",
+    "__comment01__": "ChatGPT module config file <https://github.com/F33RNI/LlM-Api-Open>",
+    "__comment02__": "File for loading and saving cookies. (Possibly not required anymore) Install editor extension:",
     "__comment03__": "<https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm>",
-    "__comment04__": "Go to <https://copilot.microsoft.com/> log in and ask about something. Wait for response",
+    "__comment04__": "Go to <https://chat.openai.com/> and ask ChatGPT about something",
     "__comment05__": "Open the extension, click Export on the bottom right, then Export as JSON",
     "__comment06__": "(This saves your cookies to clipboard). Create a new .json file and paste cookies into it",
     "__comment07__": "save file and specify path to it here. File also must have write permissions",
     "__comment08__": "Path to browser executable or empty to auto-detect (ex. /usr/bin/google-chrome-stable)",
     "__comment09__": "Major version of browser to pass as version_main argument or null to auto-detect (ex. 122)",
     "__comment10__": "Path to driver executable to pass as driver_executable_path argument or empty for auto",
-    "__comment11__": "It's recommended ot leave this empty",
+    "__comment11__": "It's recommended to leave this empty",
     "__comment12__": "Set to true to enable proxy",
     "__comment13__": "Proxy host (ip) as string",
     "__comment14__": "Proxy port as integer",
     "__comment15__": "Proxy username or empty",
     "__comment16__": "Proxy password or empty",
-    "__comment17__": "MS Copilot Web page address",
+    "__comment17__": "ChatGPT Web page address",
     "__comment18__": "Start browser in headless mode (without GUI)",
     "__comment19__": "Chrome arguments",
     "__comment20__": "--headless= argument. Leave empty to use default value",
     "__comment21__": "Time (s) for automatically refresh page if no new prompts or responses (to update session)",
     "__comment22__": "Set to 0 to disable auto-refresher",
     "__comment23__": "User agent to prevent detection of headless chrome. Leave empty to disable it",
-    "auto_refresh_interval": 300,
-    "base_url": "https://copilot.microsoft.com/",
+    "auto_refresh_interval": 120,
+    "base_url": "https://chat.openai.com/",
     "browser_executable_path": "",
     "chrome_options": [
         "--disable-infobars",
         "--ignore-ssl-errors=yes",
         "--ignore-certificate-errors",
         "--disable-default-apps",
         "--disable-notifications",
         "--disable-popup-window",
         "--no-sandbox",
         "--auto-open-devtools-for-tabs",
         "--dns-prefetch-disable",
         "--disable-gpu",
+        "--disable-dev-shm-usage",
+        "--disable-renderer-backgrounding",
+        "--disable-background-timer-throttling",
+        "--disable-backgrounding-occluded-windows",
+        "--disable-client-side-phishing-detection",
+        "--disable-crash-reporter",
+        "--disable-oopr-debug-crash-dump",
+        "--no-crash-upload",
+        "--disable-low-res-tiling",
         "--window-size=1920x960"
     ],
-    "cookies_file": "MS_Copilot_cookies.json",
+    "cookies_file": "ChatGPT_cookies.json",
     "driver_executable_path": "",
     "headless": true,
     "headless_mode": "old",
     "proxy_enabled": false,
     "proxy_host": "123.45.67.89",
     "proxy_password": "",
     "proxy_port": 8080,
```

### Comparing `llm_api_open-2.3.2/setup.py` & `llm_api_open-2.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `llm_api_open-2.3.2/src/llm_api_open.egg-info/PKG-INFO` & `llm_api_open-2.4.7/src/llm_api_open.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.3.2
+Version: 2.4.7
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -759,7 +759,16 @@
 2024-04-19 02:07:02 INFO     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
  * Running on all addresses (0.0.0.0)
  * Running on http://127.0.0.1:1312
  * Running on http://192.168.0.3:1312
 2024-04-19 02:07:02 INFO     Press CTRL+C to quit
 ...
 ```
+
+----------
+
+## 🐛 How to fix `Failed to establish a new connection` when using multiple modules
+
+1. Open `venv/lib/python3.XX/site-packages/undetected_chromedriver/patcher.py`
+2. Add `import secrets` to the imports
+3. In `def __init__` change `prefix = "undetected"` to `prefix = f"undetected{secrets.token_hex(4)}"`
+4. Save file and reload LMAO
```

### Comparing `llm_api_open-2.3.2/src/llm_api_open.egg-info/SOURCES.txt` & `llm_api_open-2.4.7/src/llm_api_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm_api_open-2.3.2/src/lmao/_version.py` & `llm_api_open-2.4.7/src/lmao/_version.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-__version__ = "2.3.2"
+__version__ = "2.4.7"
```

### Comparing `llm_api_open-2.3.2/src/lmao/chatgpt/assistantGetLastMessage.js` & `llm_api_open-2.4.7/src/lmao/chatgpt/assistantGetLastMessage.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -104,15 +104,15 @@
             // Get last one
             const assistantMessage = assistantMessages[assistantMessages.length - 1];
 
             // Extract message ID
             const assistantMessageID = assistantMessage.getAttribute("data-message-id");
 
             // Extract actual response parent
-            const responseContainer = assistantMessage.firstChild.cloneNode(true);
+            const responseContainer = assistantMessage.firstChild.firstChild.cloneNode(true);
 
             // result-thinking or result-streaming or markdown
             const responseContainerClassName = responseContainer.className;
 
             // {"code block placeholder": "code block content", ...}
             const codeBlocks = {};
```

### Comparing `llm_api_open-2.3.2/src/lmao/chatgpt/chatgpt_api.py` & `llm_api_open-2.4.7/src/lmao/chatgpt/chatgpt_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,20 +251,21 @@
         # Check if running
         if self.driver is not None:
             raise Exception("Error starting new session! Previous one is not closed! Please run session_close()")
 
         try:
             # Load cookies
             cookies_file = self.config.get("cookies_file")
-            logging.info(f"Loading cookies from {cookies_file}")
-            with open(cookies_file, "r", encoding="utf-8") as file:
-                self._cookies = json.load(file)
-                if self._cookies is None or not isinstance(self._cookies, list) or len(self._cookies) == 0:
-                    raise Exception("Empty or wrong cookies file")
-                logging.info(f"Loaded {len(self._cookies)} cookies")
+            if cookies_file and os.path.exists(cookies_file):
+                logging.info(f"Loading cookies from {cookies_file}")
+                with open(cookies_file, "r", encoding="utf-8") as file:
+                    self._cookies = json.load(file)
+                    if self._cookies is None or not isinstance(self._cookies, list):
+                        raise Exception("Wrong cookies file")
+                    logging.info(f"Loaded {len(self._cookies)} cookies")
 
             # Set driver options
             logging.info("Adding chrome options")
             chrome_options = undetected_chromedriver.ChromeOptions()
 
             # Proxy
             if self.config.get("proxy_enabled"):
@@ -320,14 +321,15 @@
             self.driver = undetected_chromedriver.Chrome(
                 browser_executable_path=browser_executable_path,
                 driver_executable_path=driver_executable_path,
                 version_main=version_main,
                 options=chrome_options,
                 headless=headless,
                 enable_cdp_events=True,
+                user_multi_procs=True,
                 **kwargs,
             )
             self.driver.set_page_load_timeout(_WAIT_TIMEOUT)
 
             # Add cookies
             logging.info(f"Trying to add {len(self._cookies)} cookies")
 
@@ -349,14 +351,21 @@
             base_url = self.config.get("base_url")
             logging.info(f"Loading {base_url}")
             self.driver.get(base_url)
 
             # Wait for textarea (New chat)
             self._wait_for_prompt_textarea()
 
+            # Wait
+            logging.info("Waiting 5 extra seconds")
+            time.sleep(5)
+
+            # Close welcome back dialogue
+            self._welcome_back_resolve()
+
             # Prevent "element not interactable" error
             self._remove_new_chat_button()
 
             # Save cookies before starting refresher
             self.cookies_save()
 
             # Start auto-refresher if needed
@@ -445,22 +454,34 @@
 
             # Get prompt area
             prompt_textarea = self.driver.find_element(By.ID, "prompt-textarea")
 
             # Paste -> click -> move cursor to the end -> add space -> erase space
             logging.info("Pasting prompt into textarea")
             self.driver.execute_script(_TYPE_INTO_TEXTAREA, prompt_textarea, prompt)
+            time.sleep(0.1)
             prompt_textarea.click()
+            time.sleep(0.1)
             self.driver.execute_script(_MOVE_CURSOR_TEXTAREA, prompt_textarea)
+            time.sleep(0.1)
             prompt_textarea.send_keys(Keys.SPACE)
+            time.sleep(0.1)
             prompt_textarea.send_keys(Keys.BACKSPACE)
+            time.sleep(0.1)
 
             # Click send prompt button
             logging.info("Clinking on send-button")
-            self.driver.find_element(By.XPATH, "//*[@data-testid='send-button']").click()
+            send_buttons_old = self.driver.find_elements(By.XPATH, "//*[@data-testid='send-button']")
+            if len(send_buttons_old) != 0:
+                send_buttons_old[0].click()
+            else:
+                self.driver.find_element(
+                    By.XPATH,
+                    '//button[@class="mb-1 mr-1 flex h-8 w-8 items-center justify-center rounded-full bg-black text-white transition-colors hover:opacity-70 focus-visible:outline-none focus-visible:outline-black disabled:bg-[#D7D7D7] disabled:text-[#f4f4f4] disabled:hover:opacity-100 dark:bg-white dark:text-black dark:focus-visible:outline-white disabled:dark:bg-token-text-quaternary dark:disabled:text-token-main-surface-secondary"]',
+                ).click()
 
             # Wait until assistant starts responding
             logging.info("Waiting for assistant to start responding")
             time_start = time.time()
             while True:
                 # Check timeout
                 if time.time() - time_start > _WAIT_TIMEOUT:
@@ -543,15 +564,15 @@
                 message_id, class_name, response_text, code_blocks = response
 
                 # Check response type
                 if class_name.startswith("result-streaming"):
                     finished = False
                 elif class_name.startswith("markdown"):
                     finished = True
-                elif not class_name.startswith("result-thinking"):
+                elif "result-thinking" not in class_name:
                     raise Exception(f"Unknown response type: {class_name}")
 
                 response_parsed = {"finished": finished}
 
                 def _code_language_callback(element_) -> str or None:
                     """Extracts language name from lang attribute
 
@@ -629,14 +650,17 @@
         if self.driver is None:
             raise Exception("No opened session! Please call session_start() first")
 
         try:
             # Pause auto-refresher
             self._refresher_pause_resume(pause=True)
 
+            # Close welcome back dialogue
+            self._welcome_back_resolve()
+
             # Prevent "element not interactable" error
             self._remove_new_chat_button()
 
             # Search chat and get it's <a> tag and expand button
             logging.info("Executing conversation search script. Please wait")
             self.driver.set_script_timeout(_WAIT_TIMEOUT)
             search_result = self.driver.execute_async_script(self._conversation_search_js, conversation_id)
@@ -646,15 +670,15 @@
                 raise Exception(search_result)
             chat_a_tag, chat_expand_button = search_result
 
             # Click on expand button
             action_chains = ActionChains(self.driver)
             time.sleep(0.1)
             logging.info("Moving to the a tag")
-            action_chains.move_to_element(chat_a_tag).perform()
+            action_chains.move_to_element(chat_a_tag).click().perform()
             time.sleep(0.5)
             logging.info("Clicking on expand button")
             chat_expand_button.click()
             time.sleep(0.5)
 
             # List all menu items
             menu_items = self.driver.find_elements(By.XPATH, "//*[@role='menuitem']")
@@ -787,26 +811,58 @@
             self.driver.execute_script(_INJECT_JS, self._assistant_get_last_message_js)
             logging.info(f"Injected? {self.driver.execute_script('return isGetLastMessageInjected();')}")
 
         # Execute script and return result
         raw = "true" if raw else "false"
         return self.driver.execute_script(f"return conversationGetLastMessage({raw});")
 
+    def _welcome_back_resolve(self) -> None:
+        """Clicks on "Stay logged out" in welcome back dialogue"""
+        welcome_back_dialogues = self.driver.find_elements(By.XPATH, "//div[@role='dialog' and @id='radix-:r7:']")
+        if len(welcome_back_dialogues) == 0:
+            return
+        welcome_back_dialogue = welcome_back_dialogues[0]
+        try:
+            logging.info('Clicking on "Stay logged out"')
+            welcome_back_dialogue.find_element(By.XPATH, "//a[starts-with(@class, 'cursor-pointer')]").click()
+            logging.info("Waiting extra 5 seconds")
+            time.sleep(5)
+        except Exception as e:
+            logging.warning(f'Unable to clock on "Stay logged out": {e}')
+
     def _remove_new_chat_button(self) -> None:
         """Removes "New chat" button because it intercepts side chat buttons"""
+        # Expand histories
+        expand_buttons = self.driver.find_elements(
+            By.XPATH,
+            '//button[@class="h-10 rounded-lg px-2.5 text-token-text-secondary focus-visible:outline-0 hover:bg-token-main-surface-secondary focus-visible:bg-token-main-surface-secondary"]',
+        )
+        if len(expand_buttons) != 0:
+            logging.info("Expanding histories")
+            expand_buttons[0].click()
+            time.sleep(1)
+
+        # Old version
         sticky_divs = self.driver.find_elements(By.XPATH, "//div[starts-with(@class, 'sticky')]")
         for sticky_div in sticky_divs:
             try:
                 if "New chat" in sticky_div.get_attribute("innerText"):
                     logging.info('Removing "New chat" button')
                     self.driver.execute_script("arguments[0].remove();", sticky_div)
                     break
             except:
                 pass
 
+        # New version
+        try:
+            self.driver.execute_script("")
+            logging.info('"New chat" button removed')
+        except:
+            pass
+
     def _wait_for_prompt_textarea(self) -> None:
         """Waits for prompt textarea to become visible and 1 extra second to make sure it's loaded and clickable"""
         logging.info("Waiting for page to load (waiting for prompt-textarea element)")
         WebDriverWait(self.driver, _WAIT_TIMEOUT).until(
             expected_conditions.presence_of_element_located((By.ID, "prompt-textarea"))
         )
         time.sleep(1)
```

### Comparing `llm_api_open-2.3.2/src/lmao/chatgpt/conversationSearch.js` & `llm_api_open-2.4.7/src/lmao/chatgpt/conversationSearch.js`

 * *Files identical despite different names*

### Comparing `llm_api_open-2.3.2/src/lmao/chatgpt/proxy_extension.py` & `llm_api_open-2.4.7/src/lmao/chatgpt/proxy_extension.py`

 * *Files identical despite different names*

### Comparing `llm_api_open-2.3.2/src/lmao/external_api.py` & `llm_api_open-2.4.7/src/lmao/external_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 for module_name, module in self.modules.items():
                     try:
                         statuses.append(
                             {
                                 "module": module_name,
                                 "status_code": module.status,
                                 "status_name": STATUS_TO_STR[module.status],
-                                "error": module.error if module.error is not None else "",
+                                "error": str(module.error) if module.error is not None else "",
                             }
                         )
                     except Exception as e:
                         logging.warning(f"Can't read {module_name} status: {e}")
                 return jsonify(statuses), 200
             except Exception as e:
                 logging.error(f"/status error: {e}")
```

### Comparing `llm_api_open-2.3.2/src/lmao/main.py` & `llm_api_open-2.4.7/src/lmao/main.py`

 * *Files identical despite different names*

### Comparing `llm_api_open-2.3.2/src/lmao/module_wrapper.py` & `llm_api_open-2.4.7/src/lmao/module_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,29 +193,29 @@
 
             # Re-yield response
             for response in self._module_class.response_read_stream(request.get("convert_to_markdown")):
                 yield response
 
         # Clear status back to IDLE
         finally:
-            self.status = STATUS_IDLE
+            self.status = STATUS_IDLE if self._module_class is not None else STATUS_NOT_INITIALIZED
 
     def response_stop(self) -> None:
         """Wrapper for response_stop() function
 
         Raises:
             Exception: module error
         """
         self.status = STATUS_BUSY
         try:
             self._module_class.response_stop()
 
         # Clear status back to IDLE
         finally:
-            self.status = STATUS_IDLE
+            self.status = STATUS_IDLE if self._module_class is not None else STATUS_NOT_INITIALIZED
 
     def delete_conversation(self, conversation: Dict) -> None:
         """Wrapper for conversation_delete() function
 
         Args:
             conversation (Dict): conversation data to delete
             For chatgpt / ms_copilot: {
@@ -227,8 +227,8 @@
         """
         self.status = STATUS_BUSY
         try:
             self._module_class.conversation_delete(conversation.get("conversation_id"))
 
         # Clear status back to IDLE
         finally:
-            self.status = STATUS_IDLE
+            self.status = STATUS_IDLE if self._module_class is not None else STATUS_NOT_INITIALIZED
```

### Comparing `llm_api_open-2.3.2/src/lmao/ms_copilot/conversationManage.js` & `llm_api_open-2.4.7/src/lmao/ms_copilot/conversationManage.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -62,22 +62,49 @@
         }
     }
     console.error("No conversation with id: " + conversationID);
     return null;
 }
 
 /**
- * Focuses on chat container and presses rename button
+ * Focuses on chat container -> waits 100ms -> presses rename button -> waits 500ms
+ * -> renames and confirms -> return the same conversation ID
+ * @param {string} conversationID new unique chat name
  */
-function startRenameMode() {
+function startRenameMode(conversationID) {
     const cibThreadContainer = document.querySelector("#b_sydConvCont > cib-serp").shadowRoot.querySelector("#cib-conversation-main > cib-side-panel").shadowRoot.querySelector("#cib-threads-container > cib-thread:nth-child(1)").shadowRoot;
     const loadChatBtn = cibThreadContainer.querySelector("div > div > button");
     loadChatBtn.focus();
-    const renameBtn = cibThreadContainer.querySelector("div > div > div.controls > button.edit.icon-button");
-    renameBtn.click();
+
+    setTimeout(function() {
+        try {
+            const cibThreadContainer_ = document.querySelector("#b_sydConvCont > cib-serp").shadowRoot.querySelector("#cib-conversation-main > cib-side-panel").shadowRoot.querySelector("#cib-threads-container > cib-thread:nth-child(1)").shadowRoot;
+            const renameBtn = cibThreadContainer_.querySelector("div > div > div.controls > button.edit.icon-button");
+            renameBtn.click();
+
+            setTimeout(function() {
+                try {
+                    renameChatAndConfirm(conversationID);
+                    callback("" + conversationID);
+                }
+
+                // Log and return error as string
+                catch (error) {
+                    console.error(error);
+                    callback("" + error);
+                }
+            }, 500);
+        }
+
+        // Log and return error as string
+        catch (error) {
+            console.error(error);
+            callback("" + error);
+        }
+    }, 100);
 }
 
 /**
  * Renames last chat and confirms it's name (call startRenameMode() before)
  * @param {string} conversationID new unique chat name
  */
 function renameChatAndConfirm(conversationID) {
@@ -127,20 +154,15 @@
             deleteChatBtn.click();
             callback("" + conversationID);
         }, 500);
     }
 
     // Rename conversation
     else if (action === "rename") {
-        // Enter edit mode -> wait 500ms -> rename and confirm -> return the same conversation ID
-        startRenameMode();
-        setTimeout(function() {
-            renameChatAndConfirm(conversationID);
-            callback("" + conversationID);
-        }, 500);
+        startRenameMode(conversationID);
     }
 }
 
 // Log and return error as string
 catch (error) {
     console.error(error);
     callback("" + error);
```

### Comparing `llm_api_open-2.3.2/src/lmao/ms_copilot/conversationParser.js` & `llm_api_open-2.4.7/src/lmao/ms_copilot/conversationParser.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -414,23 +414,24 @@
                 return false;
             }
 
             // Button is disabled -> check for image loading
             const lastMessageGroupBot = getLastMessageGroupBot();
             const cibMessages = lastMessageGroupBot.shadowRoot.querySelectorAll("cib-message");
             for (const cibMessage of cibMessages) {
-                if (cibMessage.getAttribute("content") !== "IMAGE") {
+                if (cibMessage.hasAttribute("content") && cibMessage.getAttribute("content") !== "IMAGE") {
                     continue;
                 }
                 const cibMessageIframe = cibMessage.shadowRoot.querySelector("cib-shared > iframe");
                 if (cibMessageIframe === null) {
                     continue;
                 }
                 const iframeDocument = cibMessageIframe.contentWindow.document;
-                if (iframeDocument.querySelector("#giloader").getAttribute("style") === "display: flex;") {
+                const giLoader = iframeDocument.querySelector("#giloader");
+                if (giLoader && giLoader.getAttribute("style") === "display: flex;") {
                     return false;
                 }
             }
             return true;
         }
     }
```

### Comparing `llm_api_open-2.3.2/src/lmao/ms_copilot/ms_copilot_api.py` & `llm_api_open-2.4.7/src/lmao/ms_copilot/ms_copilot_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 );
 return searchBox;
 """
 
 # JS script that sets conversation style (WORKS ONLY ON NEW CONVERSATIONS). Pass 1 / 2 / 3 as argument
 # (1 - Creative, 2 - Balanced, 3 - Precise)
 _SET_STYLE = """
-document.querySelector("#b_sydConvCont > cib-serp").shadowRoot.querySelector("#cib-conversation-main").shadowRoot.querySelector("#cib-chat-main > div > cib-welcome-container").shadowRoot.querySelector("div.controls > cib-tone-selector").shadowRoot.querySelector("#tone-options > li:nth-child(" + arguments[0] + ") > button").click();
+document.querySelector("#b_sydConvCont > cib-serp").shadowRoot.querySelector("#cib-conversation-main").shadowRoot.querySelector("#cib-chat-main > cib-welcome-container").shadowRoot.querySelector("div.controls > cib-tone-selector").shadowRoot.querySelector("#tone-options > li:nth-child(" + arguments[0] + ") > button").click();
 """
 
 # JS script that returns "Stop responding" button
 _STOP_RESPONDING = """
 return document.querySelector("#b_sydConvCont > cib-serp").shadowRoot.querySelector("#cib-action-bar-main").shadowRoot.querySelector("div > cib-typing-indicator").shadowRoot.querySelector("#stop-responding-button");
 """
 
@@ -227,20 +227,21 @@
         # Check if running
         if self.driver is not None:
             raise Exception("Error starting new session! Previous one is not closed! Please run session_close()")
 
         try:
             # Load cookies
             cookies_file = self.config.get("cookies_file")
-            logging.info(f"Loading cookies from {cookies_file}")
-            with open(cookies_file, "r", encoding="utf-8") as file:
-                self._cookies = json.load(file)
-                if self._cookies is None or not isinstance(self._cookies, list) or len(self._cookies) == 0:
-                    raise Exception("Empty or wrong cookies file")
-                logging.info(f"Loaded {len(self._cookies)} cookies")
+            if cookies_file and os.path.exists(cookies_file):
+                logging.info(f"Loading cookies from {cookies_file}")
+                with open(cookies_file, "r", encoding="utf-8") as file:
+                    self._cookies = json.load(file)
+                    if self._cookies is None or not isinstance(self._cookies, list):
+                        raise Exception("Wrong cookies file")
+                    logging.info(f"Loaded {len(self._cookies)} cookies")
 
             # Set driver options
             logging.info("Adding chrome options")
             chrome_options = undetected_chromedriver.ChromeOptions()
 
             # Hope this fill fix "Timed out receiving message from renderer" but it did't help :(
             # logging.info("Using eager page load strategy")
@@ -300,14 +301,15 @@
             self.driver = undetected_chromedriver.Chrome(
                 browser_executable_path=browser_executable_path,
                 driver_executable_path=driver_executable_path,
                 version_main=version_main,
                 options=chrome_options,
                 headless=headless,
                 enable_cdp_events=True,
+                user_multi_procs=True,
                 **kwargs,
             )
 
             # Add cookies
             logging.info(f"Trying to add {len(self._cookies)} cookies")
 
             # Enables network tracking so we may use Network.setCookie method
```

### Comparing `llm_api_open-2.3.2/src/lmao/ms_copilot/proxy_extension.py` & `llm_api_open-2.4.7/src/lmao/ms_copilot/proxy_extension.py`

 * *Files identical despite different names*

