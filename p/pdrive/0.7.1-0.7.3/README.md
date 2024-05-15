# Comparing `tmp/pdrive-0.7.1.tar.gz` & `tmp/pdrive-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdrive-0.7.1.tar", last modified: Tue May 14 14:26:27 2024, max compression
+gzip compressed data, was "pdrive-0.7.3.tar", last modified: Tue May 14 16:21:40 2024, max compression
```

## Comparing `pdrive-0.7.1.tar` & `pdrive-0.7.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.138133 pdrive-0.7.1/
--rw-r--r--   0 huy        (501) staff       (20)    35147 2020-07-09 21:03:22.000000 pdrive-0.7.1/LICENSE
--rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-14 14:26:27.137688 pdrive-0.7.1/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)     1274 2020-07-20 21:16:34.000000 pdrive-0.7.1/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.109977 pdrive-0.7.1/pdrive/
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.115310 pdrive-0.7.1/pdrive/backend/
--rw-r--r--   0 huy        (501) staff       (20)      730 2020-07-09 21:03:22.000000 pdrive-0.7.1/pdrive/backend/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)     5792 2024-05-14 14:01:30.000000 pdrive-0.7.1/pdrive/backend/web.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.116295 pdrive-0.7.1/pdrive/frontend/
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.119381 pdrive-0.7.1/pdrive/frontend/dist/
--rw-r--r--   0 huy        (501) staff       (20)    28200 2020-07-18 04:41:27.000000 pdrive-0.7.1/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff
--rw-r--r--   0 huy        (501) staff       (20)    55956 2020-07-18 04:41:27.000000 pdrive-0.7.1/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf
--rw-r--r--   0 huy        (501) staff       (20)  6999766 2020-07-18 04:41:27.000000 pdrive-0.7.1/pdrive/frontend/dist/build.js
--rw-r--r--   0 huy        (501) staff       (20)     1145 2020-07-09 21:03:22.000000 pdrive-0.7.1/pdrive/frontend/index.html
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.114266 pdrive-0.7.1/pdrive.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      460 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)       52 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/entry_points.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2020-07-18 01:29:51.000000 pdrive-0.7.1/pdrive.egg-info/not-zip-safe
--rw-r--r--   0 huy        (501) staff       (20)        6 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/requires.txt
--rw-r--r--   0 huy        (501) staff       (20)        7 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-14 14:26:27.138328 pdrive-0.7.1/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)     1621 2024-05-14 14:25:49.000000 pdrive-0.7.1/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.466794 pdrive-0.7.3/
+-rw-r--r--   0 huy        (501) staff       (20)    35147 2020-07-09 21:03:22.000000 pdrive-0.7.3/LICENSE
+-rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-14 16:21:40.466228 pdrive-0.7.3/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)     1274 2020-07-20 21:16:34.000000 pdrive-0.7.3/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.429696 pdrive-0.7.3/pdrive/
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.437557 pdrive-0.7.3/pdrive/backend/
+-rw-r--r--   0 huy        (501) staff       (20)      730 2020-07-09 21:03:22.000000 pdrive-0.7.3/pdrive/backend/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)     7011 2024-05-14 16:17:44.000000 pdrive-0.7.3/pdrive/backend/web.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.438509 pdrive-0.7.3/pdrive/frontend/
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.442856 pdrive-0.7.3/pdrive/frontend/dist/
+-rw-r--r--   0 huy        (501) staff       (20)    28200 2020-07-18 04:41:27.000000 pdrive-0.7.3/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff
+-rw-r--r--   0 huy        (501) staff       (20)    55956 2020-07-18 04:41:27.000000 pdrive-0.7.3/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf
+-rw-r--r--   0 huy        (501) staff       (20)  6999766 2020-07-18 04:41:27.000000 pdrive-0.7.3/pdrive/frontend/dist/build.js
+-rw-r--r--   0 huy        (501) staff       (20)     1145 2020-07-09 21:03:22.000000 pdrive-0.7.3/pdrive/frontend/index.html
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.436021 pdrive-0.7.3/pdrive.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      460 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)       52 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/entry_points.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2020-07-18 01:29:51.000000 pdrive-0.7.3/pdrive.egg-info/not-zip-safe
+-rw-r--r--   0 huy        (501) staff       (20)        6 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/requires.txt
+-rw-r--r--   0 huy        (501) staff       (20)        7 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-14 16:21:40.467061 pdrive-0.7.3/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)     1621 2024-05-14 16:19:31.000000 pdrive-0.7.3/setup.py
```

### Comparing `pdrive-0.7.1/LICENSE` & `pdrive-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.1/PKG-INFO` & `pdrive-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdrive
-Version: 0.7.1
+Version: 0.7.3
 Summary: A simple file manager
 Home-page: https://github.com/huyng/pdrive
 Author: Huy Nguyen
 Author-email: 121183+huyng@users.noreply.github.com
 License: UNKNOWN
 Description: # pdrive
```

### Comparing `pdrive-0.7.1/README.md` & `pdrive-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.1/pdrive/backend/__init__.py` & `pdrive-0.7.3/pdrive/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.1/pdrive/backend/web.py` & `pdrive-0.7.3/pdrive/backend/web.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import gunicorn.app.base
+import logging
+from flask import cli
 import sys
 import os.path as pth
 import os
 import json
 import shutil
 
 from argparse import ArgumentParser
@@ -152,25 +153,39 @@
         "type": node_type,
         "mimetype": mimetype,
         "size": statinfo.st_size,
         "mtime": datetime.datetime.utcfromtimestamp(statinfo.st_mtime).strftime("%Y-%M-%d %I:%M:%S %p")
     }
 
 
+def print_banner(args):
+    print("")
+    print("\x1b[32m================\x1b[0m")
+    print("\x1b[32m-    PDrive    -\x1b[0m")
+    print("\x1b[32m================\x1b[0m")
+    print("")
+    print(f"\x1b[32mStarting server at http://{args.host}:{args.port}\x1b[0m")
+    print("")
+
+
 def main():
     p = ArgumentParser()
-    p.add_argument("-H", "--host", default="127.0.0.1")
-    p.add_argument("-p", "--port", default=9999)
+    p.add_argument("-H", "--host", default="127.0.0.1",
+                   help="Host address to bind server to (default: 127.0.0.1)")
+    p.add_argument("-p", "--port", default=5000,
+                   help="Host port to bind server to (default: 9999)")
     a = p.parse_args()
 
     # If gunicorn is available use it rather than the
     # default dev server
-    try:
-        import gunicorn
+    import importlib
+    gunicorn_import_available = importlib.find_loader("gunicorn")
+    if gunicorn_import_available:
         import gunicorn.app.base
+        import multiprocessing
 
         class Application(gunicorn.app.base.BaseApplication):
 
             def __init__(self, app, options=None):
                 self.options = options or {}
                 self.application = app
                 super().__init__()
@@ -181,20 +196,37 @@
                 for key, value in config.items():
                     self.cfg.set(key.lower(), value)
 
             def load(self):
                 return self.application
 
         # start app
+        print_banner(a)
+
+        cpu_count = multiprocessing.cpu_count()
         options = {
             'bind': '%s:%s' % (a.host, a.port),
-            'workers': 3,
+            'workers': min(cpu_count, 3),
             'timeout': 120,
+            'threads': 3
         }
         Application(app, options).run()
+    else:
+        print_banner(a)
 
-    except ImportError:
+        print("")
+        print("\x1b[33mYou are running PDrive using a built-in minimal web server. For \n"
+              "better file upload & download performance, we recommend you install \n"
+              "the gunicorn web server python package. PDrive will automatically \n"
+              "use it if it is available:\x1b[0m")
+        print("")
+        print("    pip install gunicorn")
+        print("")
+
+        log = logging.getLogger('werkzeug')
+        log.disabled = True
+        cli.show_server_banner = lambda *_: None
         app.run(host=a.host, port=a.port)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pdrive-0.7.1/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff` & `pdrive-0.7.3/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.1/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf` & `pdrive-0.7.3/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.1/pdrive/frontend/dist/build.js` & `pdrive-0.7.3/pdrive/frontend/dist/build.js`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.1/pdrive/frontend/index.html` & `pdrive-0.7.3/pdrive/frontend/index.html`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.1/pdrive.egg-info/PKG-INFO` & `pdrive-0.7.3/pdrive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdrive
-Version: 0.7.1
+Version: 0.7.3
 Summary: A simple file manager
 Home-page: https://github.com/huyng/pdrive
 Author: Huy Nguyen
 Author-email: 121183+huyng@users.noreply.github.com
 License: UNKNOWN
 Description: # pdrive
```

### Comparing `pdrive-0.7.1/setup.py` & `pdrive-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='pdrive',
-      version='0.7.1',
+      version='0.7.3',
       description='A simple file manager',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Huy Nguyen',
       author_email='121183+huyng@users.noreply.github.com',
       packages=['pdrive', "pdrive.frontend", "pdrive.backend"],
       package_data={
```

