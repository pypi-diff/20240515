# Comparing `tmp/easyland-0.7.5.tar.gz` & `tmp/easyland-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyland-0.7.5.tar", last modified: Mon May 13 10:49:36 2024, max compression
+gzip compressed data, was "easyland-0.7.6.tar", last modified: Wed May 15 12:43:55 2024, max compression
```

## Comparing `easyland-0.7.5.tar` & `easyland-0.7.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-13 10:49:36.913548 easyland-0.7.5/
--rw-r--r--   0 ju        (1000) ju        (1000)     1066 2024-04-25 19:16:43.000000 easyland-0.7.5/LICENSE.txt
--rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-13 10:49:36.913548 easyland-0.7.5/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)    13475 2024-05-03 08:13:49.000000 easyland-0.7.5/README.md
--rw-r--r--   0 ju        (1000) ju        (1000)      968 2024-05-13 10:47:03.000000 easyland-0.7.5/pyproject.toml
--rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-05-13 10:49:36.913548 easyland-0.7.5/setup.cfg
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-13 10:49:36.913548 easyland-0.7.5/src/
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-13 10:49:36.913548 easyland-0.7.5/src/easyland/
--rw-r--r--   0 ju        (1000) ju        (1000)      142 2024-05-01 07:14:10.000000 easyland-0.7.5/src/easyland/__init__.py
--rw-r--r--   0 ju        (1000) ju        (1000)     2405 2024-05-01 17:31:04.000000 easyland-0.7.5/src/easyland/command.py
--rw-r--r--   0 ju        (1000) ju        (1000)     5209 2024-05-13 10:16:41.000000 easyland-0.7.5/src/easyland/daemon.py
--rw-r--r--   0 ju        (1000) ju        (1000)     2440 2024-05-13 09:00:58.000000 easyland-0.7.5/src/easyland/idle.py
--rw-r--r--   0 ju        (1000) ju        (1000)      236 2024-05-01 11:08:03.000000 easyland-0.7.5/src/easyland/log.py
--rwxr-xr-x   0 ju        (1000) ju        (1000)     1245 2024-05-13 10:46:52.000000 easyland-0.7.5/src/easyland/main.py
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-13 10:49:36.913548 easyland-0.7.5/src/easyland.egg-info/
--rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-13 10:49:36.000000 easyland-0.7.5/src/easyland.egg-info/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)      388 2024-05-13 10:49:36.000000 easyland-0.7.5/src/easyland.egg-info/SOURCES.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-05-13 10:49:36.000000 easyland-0.7.5/src/easyland.egg-info/dependency_links.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-05-13 10:49:36.000000 easyland-0.7.5/src/easyland.egg-info/entry_points.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       18 2024-05-13 10:49:36.000000 easyland-0.7.5/src/easyland.egg-info/requires.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-05-13 10:49:36.000000 easyland-0.7.5/src/easyland.egg-info/top_level.txt
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-15 12:43:55.667912 easyland-0.7.6/
+-rw-r--r--   0 ju        (1000) ju        (1000)     1066 2024-04-25 19:16:43.000000 easyland-0.7.6/LICENSE.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-15 12:43:55.667912 easyland-0.7.6/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)    13475 2024-05-03 08:13:49.000000 easyland-0.7.6/README.md
+-rw-r--r--   0 ju        (1000) ju        (1000)      968 2024-05-15 12:22:11.000000 easyland-0.7.6/pyproject.toml
+-rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-05-15 12:43:55.667912 easyland-0.7.6/setup.cfg
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-15 12:43:55.667912 easyland-0.7.6/src/
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-15 12:43:55.667912 easyland-0.7.6/src/easyland/
+-rw-r--r--   0 ju        (1000) ju        (1000)      142 2024-05-01 07:14:10.000000 easyland-0.7.6/src/easyland/__init__.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     2405 2024-05-15 10:04:28.000000 easyland-0.7.6/src/easyland/command.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     5290 2024-05-15 08:09:25.000000 easyland-0.7.6/src/easyland/daemon.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     2623 2024-05-15 09:18:10.000000 easyland-0.7.6/src/easyland/idle.py
+-rw-r--r--   0 ju        (1000) ju        (1000)      236 2024-05-01 11:08:03.000000 easyland-0.7.6/src/easyland/log.py
+-rwxr-xr-x   0 ju        (1000) ju        (1000)     1247 2024-05-15 12:19:58.000000 easyland-0.7.6/src/easyland/main.py
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-15 12:43:55.667912 easyland-0.7.6/src/easyland.egg-info/
+-rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-15 12:43:55.000000 easyland-0.7.6/src/easyland.egg-info/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)      388 2024-05-15 12:43:55.000000 easyland-0.7.6/src/easyland.egg-info/SOURCES.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-05-15 12:43:55.000000 easyland-0.7.6/src/easyland.egg-info/dependency_links.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-05-15 12:43:55.000000 easyland-0.7.6/src/easyland.egg-info/entry_points.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       18 2024-05-15 12:43:55.000000 easyland-0.7.6/src/easyland.egg-info/requires.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-05-15 12:43:55.000000 easyland-0.7.6/src/easyland.egg-info/top_level.txt
```

### Comparing `easyland-0.7.5/LICENSE.txt` & `easyland-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyland-0.7.5/PKG-INFO` & `easyland-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyland
-Version: 0.7.5
+Version: 0.7.6
 Summary: A python swiss-knife to manage wayand compositors like Hyprland and Sway
 Author-email: Julien Pro <contact@julienpro.com>
 Project-URL: Homepage, https://github.com/juienpro/easyland
 Project-URL: Issues, https://github.com/juienpro/easyland/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyland-0.7.5/README.md` & `easyland-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `easyland-0.7.5/pyproject.toml` & `easyland-0.7.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "easyland"
-version = "0.7.5"
+version = "0.7.6"
 authors = [
     { name="Julien Pro", email="contact@julienpro.com"}
 ]
 description = "A python swiss-knife to manage wayand compositors like Hyprland and Sway"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `easyland-0.7.5/src/easyland/command.py` & `easyland-0.7.6/src/easyland/command.py`

 * *Files identical despite different names*

### Comparing `easyland-0.7.5/src/easyland/daemon.py` & `easyland-0.7.6/src/easyland/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,21 +69,22 @@
     def launch_hyprland_daemon(self):
         logger.info('Launching hyprland daemon')
         socket = self.listeners['hyprland'].get('socket_path', '$XDG_RUNTIME_DIR/hypr/$HYPRLAND_INSTANCE_SIGNATURE/.socket2.sock')
         cmd = "socat -U - UNIX-CONNECT:"+socket
         # ps = subprocess.Popen(cmd,shell=True,stdout=subprocess.PIPE,stderr=subprocess.STDOUT)
         ps = subprocess.Popen(cmd,shell=True,stdout=subprocess.PIPE,stderr=subprocess.PIPE)
         while True:
-            if ps.returncode != 0:
+            if ps.returncode != 0 and ps.returncode is not None:
                 err = ps.stderr.read().decode("utf-8")
                 logger.error("Error while listening to Hyprland socket: " + err)
                 sys.exit(1)
             for line in iter(ps.stdout.readline, ""):
                 self.last_event_time = time.time()
                 decoded_line = line.decode("utf-8")
+                logger.debug(decoded_line.strip())
                 if '>>' in decoded_line:
                     data = decoded_line.split('>>')
                     self.call_handler('on_hyprland_event', data[0], data[1])
 
     def launch_sway_daemon(self, event_type):
         logger.info('Launching Sway daemon for event type: ' + event_type)
         cmd = "swaymsg -m -r -t subscribe '[\"" + event_type + "\"]'"
```

### Comparing `easyland-0.7.5/src/easyland/idle.py` & `easyland-0.7.6/src/easyland/idle.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,28 +17,31 @@
         self.command = command
         self._config = config
         self._display =  Display()
         self._display.connect()
         self._idle_notifier = None
         self._seat = None
         self._notifications = []
+        self._notifier_set = False
 
     # def _global_handler_init(self, reg, id_num, iface_name, version):
     #     if iface_name == 'wl_seat':
     #         self._seat = reg.bind(id_num, WlSeat, version)
 
     def _global_handler(self, reg, id_num, iface_name, version):
         if iface_name == 'wl_seat':
             self._seat = reg.bind(id_num, WlSeat, version)
         if iface_name == "ext_idle_notifier_v1":
             self._idle_notifier = reg.bind(id_num, ExtIdleNotifierV1, version)
 
-        if self._idle_notifier and self._seat:
+        if self._idle_notifier and self._seat and not self._notifier_set:
+            self._notifier_set = True
             for idx, c in enumerate(self._config):
                 self._notifications.append(None)
+                logger.info("Setting idle notifier for " + str(c[0]) + " seconds")
                 self._notifications[idx] = self._idle_notifier.get_idle_notification(c[0] * 1000, self._seat)
                 self._notifications[idx]._index = idx
                 self._notifications[idx].dispatcher['idled'] = self._idle_notifier_handler
                 self._notifications[idx].dispatcher['resumed'] = self._idle_notifier_resume_handler
 
     def _idle_notifier_handler(self, notification): 
         for command in self._config[notification._index][1]:
```

### Comparing `easyland-0.7.5/src/easyland/main.py` & `easyland-0.7.6/src/easyland/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib.util
 import importlib.machinery
 import sys
 import time
 import os
 from easyland.daemon import Daemon
 
-version = '0.7.5'
+version = '0.7.6'
 
 def import_from_path(path):
     module_name = os.path.basename(path).replace('-', '_').replace('.py', '')
     spec = importlib.util.spec_from_loader(module_name, importlib.machinery.SourceFileLoader(module_name, path))
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     sys.modules[module_name] = module
@@ -22,15 +22,15 @@
 
     parser = argparse.ArgumentParser(description="Easyland - A python swiss-knife to manage Wayland compositors like Hyprland and Sway")
     parser.add_argument("-c", "--config", help="Path to your config file")
     parser.add_argument("-v", "--version", action="store_true", help="Show the version")
     args = parser.parse_args()
 
     if args.version:
-        print('Pyland version: ' + version)
+        print('Easyland version: ' + version)
         sys.exit()
 
     if not args.config:
         print('Please provide a config file with the option -c')
         sys.exit(1)
 
     config = import_from_path(args.config)
```

### Comparing `easyland-0.7.5/src/easyland.egg-info/PKG-INFO` & `easyland-0.7.6/src/easyland.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyland
-Version: 0.7.5
+Version: 0.7.6
 Summary: A python swiss-knife to manage wayand compositors like Hyprland and Sway
 Author-email: Julien Pro <contact@julienpro.com>
 Project-URL: Homepage, https://github.com/juienpro/easyland
 Project-URL: Issues, https://github.com/juienpro/easyland/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

