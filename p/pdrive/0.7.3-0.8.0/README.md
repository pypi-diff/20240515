# Comparing `tmp/pdrive-0.7.3.tar.gz` & `tmp/pdrive-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdrive-0.7.3.tar", last modified: Tue May 14 16:21:40 2024, max compression
+gzip compressed data, was "pdrive-0.8.0.tar", last modified: Wed May 15 00:19:53 2024, max compression
```

## Comparing `pdrive-0.7.3.tar` & `pdrive-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.466794 pdrive-0.7.3/
--rw-r--r--   0 huy        (501) staff       (20)    35147 2020-07-09 21:03:22.000000 pdrive-0.7.3/LICENSE
--rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-14 16:21:40.466228 pdrive-0.7.3/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)     1274 2020-07-20 21:16:34.000000 pdrive-0.7.3/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.429696 pdrive-0.7.3/pdrive/
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.437557 pdrive-0.7.3/pdrive/backend/
--rw-r--r--   0 huy        (501) staff       (20)      730 2020-07-09 21:03:22.000000 pdrive-0.7.3/pdrive/backend/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)     7011 2024-05-14 16:17:44.000000 pdrive-0.7.3/pdrive/backend/web.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.438509 pdrive-0.7.3/pdrive/frontend/
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.442856 pdrive-0.7.3/pdrive/frontend/dist/
--rw-r--r--   0 huy        (501) staff       (20)    28200 2020-07-18 04:41:27.000000 pdrive-0.7.3/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff
--rw-r--r--   0 huy        (501) staff       (20)    55956 2020-07-18 04:41:27.000000 pdrive-0.7.3/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf
--rw-r--r--   0 huy        (501) staff       (20)  6999766 2020-07-18 04:41:27.000000 pdrive-0.7.3/pdrive/frontend/dist/build.js
--rw-r--r--   0 huy        (501) staff       (20)     1145 2020-07-09 21:03:22.000000 pdrive-0.7.3/pdrive/frontend/index.html
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 16:21:40.436021 pdrive-0.7.3/pdrive.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      460 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)       52 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/entry_points.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2020-07-18 01:29:51.000000 pdrive-0.7.3/pdrive.egg-info/not-zip-safe
--rw-r--r--   0 huy        (501) staff       (20)        6 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/requires.txt
--rw-r--r--   0 huy        (501) staff       (20)        7 2024-05-14 16:21:40.000000 pdrive-0.7.3/pdrive.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-14 16:21:40.467061 pdrive-0.7.3/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)     1621 2024-05-14 16:19:31.000000 pdrive-0.7.3/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-15 00:19:53.651972 pdrive-0.8.0/
+-rw-r--r--   0 huy        (501) staff       (20)    35147 2024-05-14 23:49:46.000000 pdrive-0.8.0/LICENSE
+-rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-15 00:19:53.651313 pdrive-0.8.0/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)     1274 2020-07-20 21:16:34.000000 pdrive-0.8.0/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-15 00:19:53.633270 pdrive-0.8.0/pdrive/
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-15 00:19:53.641932 pdrive-0.8.0/pdrive/backend/
+-rw-r--r--   0 huy        (501) staff       (20)      730 2020-07-09 21:03:22.000000 pdrive-0.8.0/pdrive/backend/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)     7036 2024-05-14 23:09:36.000000 pdrive-0.8.0/pdrive/backend/web.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-15 00:19:53.642763 pdrive-0.8.0/pdrive/frontend/
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-15 00:19:53.643467 pdrive-0.8.0/pdrive/frontend/dist/
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-15 00:19:53.645957 pdrive-0.8.0/pdrive/frontend/dist/assets/
+-rw-r--r--   0 huy        (501) staff       (20)   329225 2024-05-15 00:16:34.000000 pdrive-0.8.0/pdrive/frontend/dist/assets/index-C7BLSwOv.css
+-rw-r--r--   0 huy        (501) staff       (20)  1131675 2024-05-15 00:16:34.000000 pdrive-0.8.0/pdrive/frontend/dist/assets/index-Cbql13x9.js
+-rw-r--r--   0 huy        (501) staff       (20)     1257 2024-05-15 00:16:34.000000 pdrive-0.8.0/pdrive/frontend/dist/index.html
+-rw-r--r--   0 huy        (501) staff       (20)     1158 2024-05-14 22:02:59.000000 pdrive-0.8.0/pdrive/frontend/index.html
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-15 00:19:53.640665 pdrive-0.8.0/pdrive.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-15 00:19:53.000000 pdrive-0.8.0/pdrive.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      438 2024-05-15 00:19:53.000000 pdrive-0.8.0/pdrive.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-15 00:19:53.000000 pdrive-0.8.0/pdrive.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)       52 2024-05-15 00:19:53.000000 pdrive-0.8.0/pdrive.egg-info/entry_points.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-15 00:19:53.000000 pdrive-0.8.0/pdrive.egg-info/not-zip-safe
+-rw-r--r--   0 huy        (501) staff       (20)        6 2024-05-15 00:19:53.000000 pdrive-0.8.0/pdrive.egg-info/requires.txt
+-rw-r--r--   0 huy        (501) staff       (20)        7 2024-05-15 00:19:53.000000 pdrive-0.8.0/pdrive.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-15 00:19:53.652242 pdrive-0.8.0/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)     1638 2024-05-15 00:19:23.000000 pdrive-0.8.0/setup.py
```

### Comparing `pdrive-0.7.3/LICENSE` & `pdrive-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.3/PKG-INFO` & `pdrive-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdrive
-Version: 0.7.3
+Version: 0.8.0
 Summary: A simple file manager
 Home-page: https://github.com/huyng/pdrive
 Author: Huy Nguyen
 Author-email: 121183+huyng@users.noreply.github.com
 License: UNKNOWN
 Description: # pdrive
```

### Comparing `pdrive-0.7.3/README.md` & `pdrive-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.3/pdrive/backend/__init__.py` & `pdrive-0.8.0/pdrive/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.3/pdrive/backend/web.py` & `pdrive-0.8.0/pdrive/backend/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,19 @@
 from flask import render_template
 from flask import send_file
 from flask import send_from_directory
 
 frontend_path = pth.join(
     pth.split(pth.split(pth.abspath(__file__))[0])[0], "frontend")
 
+print(frontend_path)
+
 app = Flask(__name__,
             static_folder=pth.join(frontend_path, "dist"),
-            static_url_path="/dist")
+            static_url_path="")
 
 
 basedir = os.path.abspath(os.curdir)
 
 
 @app.route("/api", methods=["GET", "POST"])
 def api():
@@ -122,15 +124,15 @@
     fd.save(fpath)
     node = process(fpath)
     return json.dumps(node)
 
 
 @app.route("/")
 def index_page():
-    return send_file(pth.join(frontend_path, "index.html"))
+    return send_file(pth.join(frontend_path, "dist", "index.html"))
 
 
 def process(path):
     import os
     import stat
     import datetime
     import mimetypes
```

### Comparing `pdrive-0.7.3/pdrive/frontend/index.html` & `pdrive-0.8.0/pdrive/frontend/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -28,10 +28,10 @@
     <style media="screen">
       html,body { height:100%; }
       #app {height: 100%}
     </style>
   </head>
   <body>
     <div id="app"></div>
-    <script src="dist/build.js"></script>
+    <script type="module" src="/src/main.js"></script>
   </body>
 </html>
```

### Comparing `pdrive-0.7.3/pdrive.egg-info/PKG-INFO` & `pdrive-0.8.0/pdrive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdrive
-Version: 0.7.3
+Version: 0.8.0
 Summary: A simple file manager
 Home-page: https://github.com/huyng/pdrive
 Author: Huy Nguyen
 Author-email: 121183+huyng@users.noreply.github.com
 License: UNKNOWN
 Description: # pdrive
```

### Comparing `pdrive-0.7.3/setup.py` & `pdrive-0.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='pdrive',
-      version='0.7.3',
+      version='0.8.0',
       description='A simple file manager',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Huy Nguyen',
       author_email='121183+huyng@users.noreply.github.com',
       packages=['pdrive', "pdrive.frontend", "pdrive.backend"],
       package_data={
-          'pdrive.frontend': ['index.html', 'dist/*']
+          'pdrive.frontend': ['index.html', 'dist/assets/*', 'dist/*']
       },
       entry_points={
           "console_scripts": [
               "pdrive = pdrive.backend.web:main"
           ]
       },
       install_requires=["Flask"],
```

