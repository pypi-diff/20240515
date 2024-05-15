# Comparing `tmp/obs_waykey-0.1.2.tar.gz` & `tmp/obs_waykey-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs_waykey-0.1.2.tar", max compression
+gzip compressed data, was "obs_waykey-0.2.0.tar", max compression
```

## Comparing `obs_waykey-0.1.2.tar` & `obs_waykey-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-05-11 20:19:27.676324 obs_waykey-0.1.2/LICENSE
--rw-r--r--   0        0        0     1812 2024-05-12 11:42:25.815367 obs_waykey-0.1.2/README.md
--rw-r--r--   0        0        0      138 2024-05-14 08:55:24.472435 obs_waykey-0.1.2/obs_waykey/__init__.py
--rw-r--r--   0        0        0       49 2024-05-14 09:11:50.046072 obs_waykey-0.1.2/obs_waykey/ignition/__init__.py
--rw-r--r--   0        0        0      136 2024-05-11 21:41:27.152336 obs_waykey-0.1.2/obs_waykey/ignition/hotkeys.py
--rw-r--r--   0        0        0      256 2024-05-14 08:50:44.135006 obs_waykey-0.1.2/obs_waykey/toggles.py
--rw-r--r--   0        0        0      452 2024-05-14 09:16:10.037222 obs_waykey-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2347 1970-01-01 00:00:00.000000 obs_waykey-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-11 20:19:27.676324 obs_waykey-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1655 2024-05-15 16:16:16.347566 obs_waykey-0.2.0/README.md
+-rw-r--r--   0        0        0      193 2024-05-15 16:12:46.525133 obs_waykey-0.2.0/obs_waykey/__init__.py
+-rw-r--r--   0        0        0      394 2024-05-15 16:12:46.525133 obs_waykey-0.2.0/obs_waykey/toggles_ignition.py
+-rw-r--r--   0        0        0      994 2024-05-15 16:12:46.525133 obs_waykey-0.2.0/obs_waykey/toggles_logic.py
+-rw-r--r--   0        0        0      452 2024-05-15 16:13:47.471053 obs_waykey-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2190 1970-01-01 00:00:00.000000 obs_waykey-0.2.0/PKG-INFO
```

### Comparing `obs_waykey-0.1.2/LICENSE` & `obs_waykey-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obs_waykey-0.1.2/README.md` & `obs_waykey-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,32 @@
+Metadata-Version: 2.1
+Name: obs-waykey
+Version: 0.2.0
+Summary: OBS global shortcuts workaround for wayland using websocket
+Author: PolyCat
+Author-email: polycat@tuta.io
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: obsws-python (>=1.7.0,<2.0.0)
+Description-Content-Type: text/markdown
+
 # OBS WayKey
 
 Python script for setting up OBS global keybinds under wayland
 
 ## Requirements
 
--   [OBS Studio](https://obsproject.com/)
--   [OBS Websocket v5 Plugin](https://github.com/obsproject/obs-websocket/releases/tag/5.0.0)
-    -   ATTENTION: For OBS version 28 and above Websocket plugin is included by default. If you run an older version it must be installed manually.
--   Python 3.9 or greater
+- [OBS Studio](https://obsproject.com/)
+- [OBS Websocket v5 Plugin](https://github.com/obsproject/obs-websocket/releases/tag/5.0.0)
+  - ATTENTION: For OBS version 28 and above Websocket plugin is included by default. If you run an older version it must be installed manually.
+- Python 3.9 or greater
 
 # Install and Setup
 
 ## Install
 
 I recommend installing via [pipx](https://github.com/pypa/pipx)
 
@@ -23,33 +38,29 @@
 
 ```
 pipx install <file-name>
 ```
 
 ## Setup
 
-ATTENTION: WebSocket authentication must be disabled for this script to work.
-
-You can find it under `Tools > WebSocket Server Settings > Enable Authentication`.
-
 1. Go to your Desktop settings (or WM config file)
 2. Go to where you configure keybinds
 3. Add a new custom keybind
 4. Name it what you want
-5. Use the command `obs-waykey <toggle>`
+5. Use the command `obs-waykey -t <toggle> -w <your-password>`
 6. Set your keybind
 
-### Here's how mine looks
+### Here's an example
 
 ![my keybind](https://github.com/PolyCatDev/obs-waykey/blob/main/.github/toggle-rec-config.png)
 
 ## Toggles
 
-1. `toggle-rec`
-2. `toggle-rec-pause`
+1. `toggle-record`
+2. `toggle-record-pause`
 
 # Build from source
 
 ATTENTION: This project was built with [poetry](https://python-poetry.org/) in mind.
 
 1. Clone the repo
 
@@ -76,11 +87,12 @@
 
 ```
 poetry build
 ```
 
 # To do
 
--   [ ] Add more toggles
--   [ ] Password Support
--   [ ] Alternative IP support
--   [ ] Alternative port support
+- [ ] Add more toggles
+- [x] Password Support
+- [ ] Alternative IP support
+- [ ] Alternative port support
+
```

### Comparing `obs_waykey-0.1.2/PKG-INFO` & `obs_waykey-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,17 @@
-Metadata-Version: 2.1
-Name: obs-waykey
-Version: 0.1.2
-Summary: OBS global shortcuts workaround for wayland using websocket
-Author: PolyCat
-Author-email: polycat@tuta.io
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: obsws-python (>=1.7.0,<2.0.0)
-Description-Content-Type: text/markdown
-
 # OBS WayKey
 
 Python script for setting up OBS global keybinds under wayland
 
 ## Requirements
 
--   [OBS Studio](https://obsproject.com/)
--   [OBS Websocket v5 Plugin](https://github.com/obsproject/obs-websocket/releases/tag/5.0.0)
-    -   ATTENTION: For OBS version 28 and above Websocket plugin is included by default. If you run an older version it must be installed manually.
--   Python 3.9 or greater
+- [OBS Studio](https://obsproject.com/)
+- [OBS Websocket v5 Plugin](https://github.com/obsproject/obs-websocket/releases/tag/5.0.0)
+  - ATTENTION: For OBS version 28 and above Websocket plugin is included by default. If you run an older version it must be installed manually.
+- Python 3.9 or greater
 
 # Install and Setup
 
 ## Install
 
 I recommend installing via [pipx](https://github.com/pypa/pipx)
 
@@ -38,33 +23,29 @@
 
 ```
 pipx install <file-name>
 ```
 
 ## Setup
 
-ATTENTION: WebSocket authentication must be disabled for this script to work.
-
-You can find it under `Tools > WebSocket Server Settings > Enable Authentication`.
-
 1. Go to your Desktop settings (or WM config file)
 2. Go to where you configure keybinds
 3. Add a new custom keybind
 4. Name it what you want
-5. Use the command `obs-waykey <toggle>`
+5. Use the command `obs-waykey -t <toggle> -w <your-password>`
 6. Set your keybind
 
-### Here's how mine looks
+### Here's an example
 
 ![my keybind](https://github.com/PolyCatDev/obs-waykey/blob/main/.github/toggle-rec-config.png)
 
 ## Toggles
 
-1. `toggle-rec`
-2. `toggle-rec-pause`
+1. `toggle-record`
+2. `toggle-record-pause`
 
 # Build from source
 
 ATTENTION: This project was built with [poetry](https://python-poetry.org/) in mind.
 
 1. Clone the repo
 
@@ -91,12 +72,11 @@
 
 ```
 poetry build
 ```
 
 # To do
 
--   [ ] Add more toggles
--   [ ] Password Support
--   [ ] Alternative IP support
--   [ ] Alternative port support
-
+- [ ] Add more toggles
+- [x] Password Support
+- [ ] Alternative IP support
+- [ ] Alternative port support
```

