# Comparing `tmp/polyclash-0.0.3.tar.gz` & `tmp/polyclash-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyclash-0.0.3.tar", last modified: Fri May 10 09:05:14 2024, max compression
+gzip compressed data, was "polyclash-0.0.4.tar", last modified: Wed May 15 09:32:06 2024, max compression
```

## Comparing `polyclash-0.0.3.tar` & `polyclash-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-10 09:05:14.338797 polyclash-0.0.3/
--rw-r--r--   0 mingli     (501) staff       (20)     1068 2024-04-19 08:22:50.000000 polyclash-0.0.3/LICENSE
--rw-r--r--   0 mingli     (501) staff       (20)     3218 2024-05-10 09:05:14.339179 polyclash-0.0.3/PKG-INFO
--rw-r--r--   0 mingli     (501) staff       (20)     2551 2024-05-10 05:31:03.000000 polyclash-0.0.3/README.md
-drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-10 09:05:14.321741 polyclash-0.0.3/polyclash/
--rw-r--r--   0 mingli     (501) staff       (20)        0 2024-04-19 08:22:50.000000 polyclash-0.0.3/polyclash/__init__.py
--rw-r--r--   0 mingli     (501) staff       (20)      881 2024-05-10 09:05:01.000000 polyclash-0.0.3/polyclash/client.py
-drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-10 09:05:14.324826 polyclash-0.0.3/polyclash/data/
--rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/data/__init__.py
--rw-r--r--   0 mingli     (501) staff       (20)    42697 2024-05-10 05:31:03.000000 polyclash-0.0.3/polyclash/data/data.py
-drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-10 09:05:14.328998 polyclash-0.0.3/polyclash/game/
--rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/game/__init__.py
--rw-r--r--   0 mingli     (501) staff       (20)    11244 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/game/board.py
--rw-r--r--   0 mingli     (501) staff       (20)     4936 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/game/controller.py
--rw-r--r--   0 mingli     (501) staff       (20)     2036 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/game/player.py
--rw-r--r--   0 mingli     (501) staff       (20)      922 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/game/timer.py
-drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-10 09:05:14.335048 polyclash-0.0.3/polyclash/gui/
--rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/gui/__init__.py
--rw-r--r--   0 mingli     (501) staff       (20)      574 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/gui/constants.py
--rw-r--r--   0 mingli     (501) staff       (20)    11012 2024-05-10 05:31:03.000000 polyclash-0.0.3/polyclash/gui/dialogs.py
--rw-r--r--   0 mingli     (501) staff       (20)    34645 2024-05-10 05:31:03.000000 polyclash-0.0.3/polyclash/gui/icons.py
--rw-r--r--   0 mingli     (501) staff       (20)     6268 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/gui/main.py
--rw-r--r--   0 mingli     (501) staff       (20)     1728 2024-05-10 05:31:03.000000 polyclash-0.0.3/polyclash/gui/mesh.py
--rw-r--r--   0 mingli     (501) staff       (20)     2291 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/gui/overly_info.py
--rw-r--r--   0 mingli     (501) staff       (20)     2920 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/gui/overly_map.py
--rw-r--r--   0 mingli     (501) staff       (20)     5563 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/gui/view_sphere.py
--rw-r--r--   0 mingli     (501) staff       (20)     8843 2024-05-10 09:05:01.000000 polyclash-0.0.3/polyclash/server.py
-drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-10 09:05:14.336990 polyclash-0.0.3/polyclash/util/
--rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/util/__init__.py
--rw-r--r--   0 mingli     (501) staff       (20)     3870 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/util/api.py
--rw-r--r--   0 mingli     (501) staff       (20)     1001 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/util/logging.py
--rw-r--r--   0 mingli     (501) staff       (20)    12983 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/util/storage.py
-drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-10 09:05:14.338282 polyclash-0.0.3/polyclash/workers/
--rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/workers/__init__.py
--rw-r--r--   0 mingli     (501) staff       (20)     1608 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/workers/ai_play.py
--rw-r--r--   0 mingli     (501) staff       (20)     1928 2024-05-09 16:20:03.000000 polyclash-0.0.3/polyclash/workers/network.py
-drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-10 09:05:14.324099 polyclash-0.0.3/polyclash.egg-info/
--rw-r--r--   0 mingli     (501) staff       (20)     3218 2024-05-10 09:05:14.000000 polyclash-0.0.3/polyclash.egg-info/PKG-INFO
--rw-r--r--   0 mingli     (501) staff       (20)      897 2024-05-10 09:05:14.000000 polyclash-0.0.3/polyclash.egg-info/SOURCES.txt
--rw-r--r--   0 mingli     (501) staff       (20)        1 2024-05-10 09:05:14.000000 polyclash-0.0.3/polyclash.egg-info/dependency_links.txt
--rw-r--r--   0 mingli     (501) staff       (20)      100 2024-05-10 09:05:14.000000 polyclash-0.0.3/polyclash.egg-info/entry_points.txt
--rw-r--r--   0 mingli     (501) staff       (20)      188 2024-05-10 09:05:14.000000 polyclash-0.0.3/polyclash.egg-info/requires.txt
--rw-r--r--   0 mingli     (501) staff       (20)       10 2024-05-10 09:05:14.000000 polyclash-0.0.3/polyclash.egg-info/top_level.txt
--rw-r--r--   0 mingli     (501) staff       (20)      103 2024-05-10 09:05:14.339776 polyclash-0.0.3/setup.cfg
--rw-r--r--   0 mingli     (501) staff       (20)     1581 2024-05-10 09:05:01.000000 polyclash-0.0.3/setup.py
+drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-15 09:32:06.594707 polyclash-0.0.4/
+-rw-r--r--   0 mingli     (501) staff       (20)     1068 2024-04-19 08:22:50.000000 polyclash-0.0.4/LICENSE
+-rw-r--r--   0 mingli     (501) staff       (20)     3218 2024-05-15 09:32:06.595203 polyclash-0.0.4/PKG-INFO
+-rw-r--r--   0 mingli     (501) staff       (20)     2551 2024-05-10 05:31:03.000000 polyclash-0.0.4/README.md
+drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-15 09:32:06.575334 polyclash-0.0.4/polyclash/
+-rw-r--r--   0 mingli     (501) staff       (20)        0 2024-04-19 08:22:50.000000 polyclash-0.0.4/polyclash/__init__.py
+-rw-r--r--   0 mingli     (501) staff       (20)      881 2024-05-10 09:05:01.000000 polyclash-0.0.4/polyclash/client.py
+drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-15 09:32:06.579377 polyclash-0.0.4/polyclash/data/
+-rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/data/__init__.py
+-rw-r--r--   0 mingli     (501) staff       (20)    42697 2024-05-10 05:31:03.000000 polyclash-0.0.4/polyclash/data/data.py
+drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-15 09:32:06.583265 polyclash-0.0.4/polyclash/game/
+-rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/game/__init__.py
+-rw-r--r--   0 mingli     (501) staff       (20)    11244 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/game/board.py
+-rw-r--r--   0 mingli     (501) staff       (20)     4936 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/game/controller.py
+-rw-r--r--   0 mingli     (501) staff       (20)     2036 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/game/player.py
+-rw-r--r--   0 mingli     (501) staff       (20)      922 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/game/timer.py
+drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-15 09:32:06.589637 polyclash-0.0.4/polyclash/gui/
+-rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/gui/__init__.py
+-rw-r--r--   0 mingli     (501) staff       (20)      574 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/gui/constants.py
+-rw-r--r--   0 mingli     (501) staff       (20)    11014 2024-05-15 09:31:52.000000 polyclash-0.0.4/polyclash/gui/dialogs.py
+-rw-r--r--   0 mingli     (501) staff       (20)    34645 2024-05-10 05:31:03.000000 polyclash-0.0.4/polyclash/gui/icons.py
+-rw-r--r--   0 mingli     (501) staff       (20)     6268 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/gui/main.py
+-rw-r--r--   0 mingli     (501) staff       (20)     1728 2024-05-10 05:31:03.000000 polyclash-0.0.4/polyclash/gui/mesh.py
+-rw-r--r--   0 mingli     (501) staff       (20)     2291 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/gui/overly_info.py
+-rw-r--r--   0 mingli     (501) staff       (20)     2920 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/gui/overly_map.py
+-rw-r--r--   0 mingli     (501) staff       (20)     5563 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/gui/view_sphere.py
+-rw-r--r--   0 mingli     (501) staff       (20)     8842 2024-05-15 09:31:52.000000 polyclash-0.0.4/polyclash/server.py
+drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-15 09:32:06.592134 polyclash-0.0.4/polyclash/util/
+-rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/util/__init__.py
+-rw-r--r--   0 mingli     (501) staff       (20)     3870 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/util/api.py
+-rw-r--r--   0 mingli     (501) staff       (20)     1001 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/util/logging.py
+-rw-r--r--   0 mingli     (501) staff       (20)    12983 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/util/storage.py
+drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-15 09:32:06.594121 polyclash-0.0.4/polyclash/workers/
+-rw-r--r--   0 mingli     (501) staff       (20)        0 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/workers/__init__.py
+-rw-r--r--   0 mingli     (501) staff       (20)     1608 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/workers/ai_play.py
+-rw-r--r--   0 mingli     (501) staff       (20)     1928 2024-05-09 16:20:03.000000 polyclash-0.0.4/polyclash/workers/network.py
+drwxr-xr-x   0 mingli     (501) staff       (20)        0 2024-05-15 09:32:06.578490 polyclash-0.0.4/polyclash.egg-info/
+-rw-r--r--   0 mingli     (501) staff       (20)     3218 2024-05-15 09:32:06.000000 polyclash-0.0.4/polyclash.egg-info/PKG-INFO
+-rw-r--r--   0 mingli     (501) staff       (20)      897 2024-05-15 09:32:06.000000 polyclash-0.0.4/polyclash.egg-info/SOURCES.txt
+-rw-r--r--   0 mingli     (501) staff       (20)        1 2024-05-15 09:32:06.000000 polyclash-0.0.4/polyclash.egg-info/dependency_links.txt
+-rw-r--r--   0 mingli     (501) staff       (20)      100 2024-05-15 09:32:06.000000 polyclash-0.0.4/polyclash.egg-info/entry_points.txt
+-rw-r--r--   0 mingli     (501) staff       (20)      188 2024-05-15 09:32:06.000000 polyclash-0.0.4/polyclash.egg-info/requires.txt
+-rw-r--r--   0 mingli     (501) staff       (20)       10 2024-05-15 09:32:06.000000 polyclash-0.0.4/polyclash.egg-info/top_level.txt
+-rw-r--r--   0 mingli     (501) staff       (20)      103 2024-05-15 09:32:06.596033 polyclash-0.0.4/setup.cfg
+-rw-r--r--   0 mingli     (501) staff       (20)     1581 2024-05-15 09:31:52.000000 polyclash-0.0.4/setup.py
```

### Comparing `polyclash-0.0.3/LICENSE` & `polyclash-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/PKG-INFO` & `polyclash-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyclash
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python 3d spherical Go game on a snub dodecahedron board
 Home-page: https://github.com/spherical-go/polyclash
 Author: Mingli Yuan
 Author-email: mingli.yuan@gmail.com
 Project-URL: Documentation, https://github.com/spherical-go/polyclash
 Project-URL: Source, https://github.com/spherical-go/polyclash
 Project-URL: Tracker, https://github.com/spherical-go/polyclash/issues
```

### Comparing `polyclash-0.0.3/README.md` & `polyclash-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/client.py` & `polyclash-0.0.4/polyclash/client.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/data/data.py` & `polyclash-0.0.4/polyclash/data/data.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/game/board.py` & `polyclash-0.0.4/polyclash/game/board.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/game/controller.py` & `polyclash-0.0.4/polyclash/game/controller.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/game/player.py` & `polyclash-0.0.4/polyclash/game/player.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/game/timer.py` & `polyclash-0.0.4/polyclash/game/timer.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/gui/constants.py` & `polyclash-0.0.4/polyclash/gui/constants.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/gui/dialogs.py` & `polyclash-0.0.4/polyclash/gui/dialogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     def __init__(self, parent=None):
         super(NetworkGameDialog, self).__init__(parent)
         self.setWindowTitle('Create A Network Game Room')
         layout = QVBoxLayout(self)
 
         # Server input (only enabled for Network mode)
         self.server_input = QLineEdit(self)
-        self.server_input.setPlaceholderText("http://127.0.0.1:5000")
+        self.server_input.setPlaceholderText("https://sphericalgo.org")
         layout.addWidget(QLabel('Server'))
         layout.addWidget(self.server_input)
 
         self.token = QLineEdit(self)
         layout.addWidget(QLabel('Token'))
         layout.addWidget(self.token)
```

### Comparing `polyclash-0.0.3/polyclash/gui/icons.py` & `polyclash-0.0.4/polyclash/gui/icons.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/gui/main.py` & `polyclash-0.0.4/polyclash/gui/main.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/gui/mesh.py` & `polyclash-0.0.4/polyclash/gui/mesh.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/gui/overly_info.py` & `polyclash-0.0.4/polyclash/gui/overly_info.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/gui/overly_map.py` & `polyclash-0.0.4/polyclash/gui/overly_map.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/gui/view_sphere.py` & `polyclash-0.0.4/polyclash/gui/view_sphere.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/server.py` & `polyclash-0.0.4/polyclash/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,12 +267,12 @@
             delayed_thread = Thread(target=delayed_start, args=(game_id,))
             delayed_thread.start()
 
 
 def main():
     logger.info(f"Secret: {secret_key}")
     logger.info(f"Token: {server_token}")
-    socketio.run(app, host='localhost', port=5000, allow_unsafe_werkzeug=True, debug=True)
+    socketio.run(app, host='0.0.0.0', port=3302, allow_unsafe_werkzeug=True, debug=False)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `polyclash-0.0.3/polyclash/util/api.py` & `polyclash-0.0.4/polyclash/util/api.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/util/logging.py` & `polyclash-0.0.4/polyclash/util/logging.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/util/storage.py` & `polyclash-0.0.4/polyclash/util/storage.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/workers/ai_play.py` & `polyclash-0.0.4/polyclash/workers/ai_play.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash/workers/network.py` & `polyclash-0.0.4/polyclash/workers/network.py`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/polyclash.egg-info/PKG-INFO` & `polyclash-0.0.4/polyclash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyclash
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python 3d spherical Go game on a snub dodecahedron board
 Home-page: https://github.com/spherical-go/polyclash
 Author: Mingli Yuan
 Author-email: mingli.yuan@gmail.com
 Project-URL: Documentation, https://github.com/spherical-go/polyclash
 Project-URL: Source, https://github.com/spherical-go/polyclash
 Project-URL: Tracker, https://github.com/spherical-go/polyclash/issues
```

### Comparing `polyclash-0.0.3/polyclash.egg-info/SOURCES.txt` & `polyclash-0.0.4/polyclash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyclash-0.0.3/setup.py` & `polyclash-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="polyclash",
-    version="0.0.3",
+    version="0.0.4",
     author="Mingli Yuan",
     author_email="mingli.yuan@gmail.com",
     description="A python 3d spherical Go game on a snub dodecahedron board",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spherical-go/polyclash",
     project_urls={
```

