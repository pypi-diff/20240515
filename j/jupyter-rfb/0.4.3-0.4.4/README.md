# Comparing `tmp/jupyter_rfb-0.4.3.tar.gz` & `tmp/jupyter_rfb-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_rfb-0.4.3.tar", last modified: Fri May 10 07:45:19 2024, max compression
+gzip compressed data, was "jupyter_rfb-0.4.4.tar", last modified: Wed May 15 08:06:56 2024, max compression
```

## Comparing `jupyter_rfb-0.4.3.tar` & `jupyter_rfb-0.4.4.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.084814 jupyter_rfb-0.4.3/
--rw-r--r--   0 almar      (501) staff       (20)     1062 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/LICENSE
--rw-r--r--   0 almar      (501) staff       (20)      386 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/MANIFEST.in
--rw-r--r--   0 almar      (501) staff       (20)      824 2024-05-10 07:45:19.084887 jupyter_rfb-0.4.3/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     1880 2023-06-09 13:12:17.000000 jupyter_rfb-0.4.3/README.md
--rw-r--r--   0 almar      (501) staff       (20)      182 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/install.json
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.078490 jupyter_rfb-0.4.3/js/
--rw-r--r--   0 almar      (501) staff       (20)      455 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/js/.eslintrc.json
--rw-r--r--   0 almar      (501) staff       (20)      157 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/js/README.md
--rw-r--r--   0 almar      (501) staff       (20)      647 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.3/js/amd-public-path.js
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.078709 jupyter_rfb-0.4.3/js/dist/
--rw-r--r--   0 almar      (501) staff       (20)     8563 2024-05-10 07:45:10.000000 jupyter_rfb-0.4.3/js/dist/index.js
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.079274 jupyter_rfb-0.4.3/js/lib/
--rw-r--r--   0 almar      (501) staff       (20)      459 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.3/js/lib/extension.js
--rw-r--r--   0 almar      (501) staff       (20)      185 2024-05-10 07:44:48.000000 jupyter_rfb-0.4.3/js/lib/index.js
--rw-r--r--   0 almar      (501) staff       (20)      522 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.3/js/lib/labplugin.js
--rw-r--r--   0 almar      (501) staff       (20)    18725 2024-04-16 11:03:12.000000 jupyter_rfb-0.4.3/js/lib/widget.js
--rw-r--r--   0 almar      (501) staff       (20)     1505 2024-05-10 07:45:09.000000 jupyter_rfb-0.4.3/js/package.json
--rw-r--r--   0 almar      (501) staff       (20)     2828 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.3/js/webpack.config.js
--rw-r--r--   0 almar      (501) staff       (20)    94847 2024-05-10 07:45:09.000000 jupyter_rfb-0.4.3/js/yarn.lock
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.080896 jupyter_rfb-0.4.3/jupyter_rfb/
--rw-r--r--   0 almar      (501) staff       (20)     1842 2023-02-24 11:04:02.000000 jupyter_rfb-0.4.3/jupyter_rfb/__init__.py
--rw-r--r--   0 almar      (501) staff       (20)     3552 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.3/jupyter_rfb/_jpg.py
--rw-r--r--   0 almar      (501) staff       (20)     2416 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/jupyter_rfb/_png.py
--rw-r--r--   0 almar      (501) staff       (20)     4922 2023-11-07 10:12:10.000000 jupyter_rfb-0.4.3/jupyter_rfb/_utils.py
--rw-r--r--   0 almar      (501) staff       (20)      445 2024-05-10 07:34:08.000000 jupyter_rfb-0.4.3/jupyter_rfb/_version.py
--rw-r--r--   0 almar      (501) staff       (20)     5093 2024-05-10 07:32:58.000000 jupyter_rfb-0.4.3/jupyter_rfb/events.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.082365 jupyter_rfb-0.4.3/jupyter_rfb/labextension/
--rw-r--r--   0 almar      (501) staff       (20)     1621 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/package.json
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.083216 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/
--rw-r--r--   0 almar      (501) staff       (20)     8187 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/493.cb43b5d572b2f6b10c8e.js
--rw-r--r--   0 almar      (501) staff       (20)     7826 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/678.c748912b15ffb2656a49.js
--rw-r--r--   0 almar      (501) staff       (20)     6480 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/remoteEntry.0d5a3b6ccc7e17c1ed27.js
--rw-r--r--   0 almar      (501) staff       (20)      118 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/style.js
--rw-r--r--   0 almar      (501) staff       (20)       20 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.083576 jupyter_rfb-0.4.3/jupyter_rfb/nbextension/
--rw-r--r--   0 almar      (501) staff       (20)      531 2024-05-10 07:45:10.000000 jupyter_rfb-0.4.3/jupyter_rfb/nbextension/extension.js
--rw-r--r--   0 almar      (501) staff       (20)     8563 2024-05-10 07:45:10.000000 jupyter_rfb-0.4.3/jupyter_rfb/nbextension/index.js
--rw-r--r--   0 almar      (501) staff       (20)    17152 2024-05-10 07:32:58.000000 jupyter_rfb-0.4.3/jupyter_rfb/widget.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.082211 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/
--rw-r--r--   0 almar      (501) staff       (20)      824 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     1120 2024-05-10 07:45:19.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/SOURCES.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/dependency_links.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2022-02-04 09:25:53.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/not-zip-safe
--rw-r--r--   0 almar      (501) staff       (20)       46 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/requires.txt
--rw-r--r--   0 almar      (501) staff       (20)       12 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/top_level.txt
--rw-r--r--   0 almar      (501) staff       (20)       65 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/jupyter_rfb.json
--rw-r--r--   0 almar      (501) staff       (20)      153 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/pyproject.toml
--rw-r--r--   0 almar      (501) staff       (20)      460 2024-05-10 07:45:19.085186 jupyter_rfb-0.4.3/setup.cfg
--rw-r--r--   0 almar      (501) staff       (20)     2525 2023-04-30 21:11:03.000000 jupyter_rfb-0.4.3/setup.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.084570 jupyter_rfb-0.4.3/tests/
--rw-r--r--   0 almar      (501) staff       (20)     3443 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.3/tests/test_jpg.py
--rw-r--r--   0 almar      (501) staff       (20)     2614 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/tests/test_png.py
--rw-r--r--   0 almar      (501) staff       (20)     3670 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.3/tests/test_utils.py
--rw-r--r--   0 almar      (501) staff       (20)     8346 2024-04-16 11:03:12.000000 jupyter_rfb-0.4.3/tests/test_widget.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.159585 jupyter_rfb-0.4.4/
+-rw-r--r--   0 almar      (501) staff       (20)     1062 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.4/LICENSE
+-rw-r--r--   0 almar      (501) staff       (20)      386 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.4/MANIFEST.in
+-rw-r--r--   0 almar      (501) staff       (20)      824 2024-05-15 08:06:56.159688 jupyter_rfb-0.4.4/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     1880 2023-06-09 13:12:17.000000 jupyter_rfb-0.4.4/README.md
+-rw-r--r--   0 almar      (501) staff       (20)      182 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.4/install.json
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.146609 jupyter_rfb-0.4.4/js/
+-rw-r--r--   0 almar      (501) staff       (20)      455 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.4/js/.eslintrc.json
+-rw-r--r--   0 almar      (501) staff       (20)      157 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.4/js/README.md
+-rw-r--r--   0 almar      (501) staff       (20)      647 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.4/js/amd-public-path.js
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.149965 jupyter_rfb-0.4.4/js/dist/
+-rw-r--r--   0 almar      (501) staff       (20)     8541 2024-05-15 08:06:50.000000 jupyter_rfb-0.4.4/js/dist/index.js
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.151346 jupyter_rfb-0.4.4/js/lib/
+-rw-r--r--   0 almar      (501) staff       (20)      459 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.4/js/lib/extension.js
+-rw-r--r--   0 almar      (501) staff       (20)      433 2024-05-15 08:05:39.000000 jupyter_rfb-0.4.4/js/lib/index.js
+-rw-r--r--   0 almar      (501) staff       (20)      522 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.4/js/lib/labplugin.js
+-rw-r--r--   0 almar      (501) staff       (20)    18725 2024-04-16 11:03:12.000000 jupyter_rfb-0.4.4/js/lib/widget.js
+-rw-r--r--   0 almar      (501) staff       (20)   146009 2024-05-15 07:57:17.000000 jupyter_rfb-0.4.4/js/package-lock.json
+-rw-r--r--   0 almar      (501) staff       (20)     1509 2024-05-15 08:05:39.000000 jupyter_rfb-0.4.4/js/package.json
+-rw-r--r--   0 almar      (501) staff       (20)     2828 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.4/js/webpack.config.js
+-rw-r--r--   0 almar      (501) staff       (20)    94851 2024-05-15 08:06:48.000000 jupyter_rfb-0.4.4/js/yarn.lock
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.153843 jupyter_rfb-0.4.4/jupyter_rfb/
+-rw-r--r--   0 almar      (501) staff       (20)     1842 2023-02-24 11:04:02.000000 jupyter_rfb-0.4.4/jupyter_rfb/__init__.py
+-rw-r--r--   0 almar      (501) staff       (20)     3552 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.4/jupyter_rfb/_jpg.py
+-rw-r--r--   0 almar      (501) staff       (20)     2416 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.4/jupyter_rfb/_png.py
+-rw-r--r--   0 almar      (501) staff       (20)     4922 2023-11-07 10:12:10.000000 jupyter_rfb-0.4.4/jupyter_rfb/_utils.py
+-rw-r--r--   0 almar      (501) staff       (20)      445 2024-05-15 08:06:28.000000 jupyter_rfb-0.4.4/jupyter_rfb/_version.py
+-rw-r--r--   0 almar      (501) staff       (20)     5093 2024-05-10 07:32:58.000000 jupyter_rfb-0.4.4/jupyter_rfb/events.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.155846 jupyter_rfb-0.4.4/jupyter_rfb/labextension/
+-rw-r--r--   0 almar      (501) staff       (20)     1625 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb/labextension/package.json
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.157235 jupyter_rfb-0.4.4/jupyter_rfb/labextension/static/
+-rw-r--r--   0 almar      (501) staff       (20)     7816 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb/labextension/static/420.d43f6d92aa7a9fb70aad.js
+-rw-r--r--   0 almar      (501) staff       (20)     8183 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb/labextension/static/493.102804eff6eca0571ecf.js
+-rw-r--r--   0 almar      (501) staff       (20)     6516 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb/labextension/static/remoteEntry.cf57a6d7f00412526ea4.js
+-rw-r--r--   0 almar      (501) staff       (20)      118 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb/labextension/static/style.js
+-rw-r--r--   0 almar      (501) staff       (20)       20 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.157743 jupyter_rfb-0.4.4/jupyter_rfb/nbextension/
+-rw-r--r--   0 almar      (501) staff       (20)      531 2024-05-15 08:06:50.000000 jupyter_rfb-0.4.4/jupyter_rfb/nbextension/extension.js
+-rw-r--r--   0 almar      (501) staff       (20)     8541 2024-05-15 08:06:50.000000 jupyter_rfb-0.4.4/jupyter_rfb/nbextension/index.js
+-rw-r--r--   0 almar      (501) staff       (20)    17152 2024-05-10 07:32:58.000000 jupyter_rfb-0.4.4/jupyter_rfb/widget.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.155570 jupyter_rfb-0.4.4/jupyter_rfb.egg-info/
+-rw-r--r--   0 almar      (501) staff       (20)      824 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb.egg-info/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     1141 2024-05-15 08:06:56.000000 jupyter_rfb-0.4.4/jupyter_rfb.egg-info/SOURCES.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb.egg-info/dependency_links.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2022-02-04 09:25:53.000000 jupyter_rfb-0.4.4/jupyter_rfb.egg-info/not-zip-safe
+-rw-r--r--   0 almar      (501) staff       (20)       46 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb.egg-info/requires.txt
+-rw-r--r--   0 almar      (501) staff       (20)       12 2024-05-15 08:06:55.000000 jupyter_rfb-0.4.4/jupyter_rfb.egg-info/top_level.txt
+-rw-r--r--   0 almar      (501) staff       (20)       65 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.4/jupyter_rfb.json
+-rw-r--r--   0 almar      (501) staff       (20)      153 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.4/pyproject.toml
+-rw-r--r--   0 almar      (501) staff       (20)      460 2024-05-15 08:06:56.160138 jupyter_rfb-0.4.4/setup.cfg
+-rw-r--r--   0 almar      (501) staff       (20)     2525 2023-04-30 21:11:03.000000 jupyter_rfb-0.4.4/setup.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-15 08:06:56.159288 jupyter_rfb-0.4.4/tests/
+-rw-r--r--   0 almar      (501) staff       (20)     3443 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.4/tests/test_jpg.py
+-rw-r--r--   0 almar      (501) staff       (20)     2614 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.4/tests/test_png.py
+-rw-r--r--   0 almar      (501) staff       (20)     3670 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.4/tests/test_utils.py
+-rw-r--r--   0 almar      (501) staff       (20)     8346 2024-04-16 11:03:12.000000 jupyter_rfb-0.4.4/tests/test_widget.py
```

### Comparing `jupyter_rfb-0.4.3/LICENSE` & `jupyter_rfb-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/PKG-INFO` & `jupyter_rfb-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_rfb
-Version: 0.4.3
+Version: 0.4.4
 Summary: Remote Frame Buffer for Jupyter
 Home-page: https://github.com/vispy/jupyter_rfb
 Author: Almar Klein
 Author-email: almar@almarklein.org
 License: MIT
 Keywords: ipython,jupyter,widgets,visualization,remote frame buffer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jupyter_rfb-0.4.3/README.md` & `jupyter_rfb-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/js/amd-public-path.js` & `jupyter_rfb-0.4.4/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/js/dist/index.js` & `jupyter_rfb-0.4.4/js/dist/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,261 +1,10 @@
 define(["module", "@jupyter-widgets/base"], ((e, t) => (() => {
     "use strict";
     var i = {
-            747: (e, t, i) => {
-                var s = i(325);
-                const n = new URL(s.uri, document.location);
-                n.pathname = n.pathname.slice(0, n.pathname.lastIndexOf("/") + 1), i.p = `${n.origin}${n.pathname}`
-            },
-            681: (e, t, i) => {
-                i.r(t), i.d(t, {
-                    RemoteFrameBufferModel: () => n,
-                    RemoteFrameBufferView: () => o,
-                    version: () => _.i8
-                });
-                var s = i(146);
-                class n extends s.DOMWidgetModel {
-                    defaults() {
-                        return {
-                            ...super.defaults(),
-                            _model_name: "RemoteFrameBufferModel",
-                            _view_name: "RemoteFrameBufferView",
-                            _model_module: "jupyter_rfb",
-                            _view_module: "jupyter_rfb",
-                            _model_module_version: "0.1.0",
-                            _view_module_version: "0.1.0",
-                            frame_feedback: {},
-                            css_width: "500px",
-                            css_height: "300px",
-                            resizable: !0,
-                            has_visible_views: !1,
-                            cursor: "default"
-                        }
-                    }
-                    initialize() {
-                        super.initialize.apply(this, arguments), this.img_elements = [], this._intersection_observer = new IntersectionObserver(this._intersection_callback.bind(this)), window.setInterval(this.collect_view_img_elements.bind(this), 5e3), this.frames = [], this.on("msg:custom", this.on_msg, this), this.last_frame = {
-                            src: "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAADElEQVR42mOor68HAAL+AX6E2KOJAAAAAElFTkSuQmCC",
-                            index: 0,
-                            timestamp: 0
-                        }, this._img_update_pending = !1, this._request_animation_frame()
-                    }
-                    async collect_view_img_elements() {
-                        this._intersection_observer.disconnect();
-                        for (let e of this.img_elements) e.onload = null;
-                        this.img_elements = [];
-                        for (let e in this.views) {
-                            let t = await this.views[e];
-                            this._intersection_observer.observe(t.img), this.img_elements.push(t.img), t.img.onload = this._request_animation_frame.bind(this)
-                        }
-                        this._request_animation_frame()
-                    }
-                    on_msg(e, t) {
-                        "framebufferdata" === e.type && this.frames.push({
-                            ...e,
-                            buffers: t
-                        })
-                    }
-                    _intersection_callback(e, t) {
-                        for (let t of e) t.target._is_visible = t.isIntersecting;
-                        let i = 0;
-                        for (let e of this.img_elements) e._is_visible && (i += 1);
-                        let s = i > 0;
-                        s != this.get("has_visible_views") && (this.set("has_visible_views", s), this.save_changes())
-                    }
-                    _send_response() {
-                        let e = this.last_frame,
-                            t = {
-                                index: e.index,
-                                timestamp: e.timestamp,
-                                localtime: Date.now() / 1e3
-                            };
-                        this.set("frame_feedback", t), this.save_changes()
-                    }
-                    _request_animation_frame() {
-                        if (!this._img_update_pending) {
-                            this._img_update_pending = !0;
-                            let e = this._animate.bind(this);
-                            window.setTimeout(window.requestAnimationFrame, 5, e)
-                        }
-                    }
-                    _animate() {
-                        if (this._img_update_pending = !1, !this.frames.length) return void this._request_animation_frame();
-                        let e, t = this.frames.shift();
-                        if (t.buffers.length > 0) {
-                            let i = new Blob([t.buffers[0].buffer], {
-                                type: t.mimetype
-                            });
-                            e = URL.createObjectURL(i)
-                        } else e = t.data_b64;
-                        let i = this.img_elements?.[0]?.src;
-                        i.startsWith("blob:") && URL.revokeObjectURL(i);
-                        for (let t of this.img_elements) t.src = e;
-                        this.last_frame = t, this._send_response(), 0 === this.img_elements.length && this._request_animation_frame()
-                    }
-                    close() {
-                        this.send({
-                            event_type: "close",
-                            time_stamp: a()
-                        }), super.close.apply(this, arguments)
-                    }
-                }
-                class o extends s.DOMWidgetView {
-                    render() {
-                        var e = this;
-
-                        function t() {
-                            let t = e._wheel_state.e,
-                                i = e.img.getBoundingClientRect(),
-                                s = {
-                                    event_type: "wheel",
-                                    x: Number(t.clientX - i.left),
-                                    y: Number(t.clientY - i.top),
-                                    dx: e._wheel_state.dx,
-                                    dy: e._wheel_state.dy,
-                                    buttons: e._last_buttons,
-                                    modifiers: r(t),
-                                    time_stamp: a()
-                                };
-                            e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
-                        }
-
-                        function i(t) {
-                            if (null === e.el.offsetParent) return;
-                            let i = {
-                                event_type: "key_" + t.type.slice(3),
-                                key: l[t.key] || t.key,
-                                modifiers: r(t),
-                                time_stamp: a()
-                            };
-                            t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
-                        }
-                        this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
-                            if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
-                        }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this.el.style.cursor = this.model.get("cursor"), this.model.on("change:cursor", (function() {
-                            this.el.style.cursor = this.model.get("cursor")
-                        }), this), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
-                            this.el.style.width = this.model.get("css_width")
-                        }), this), this.model.on("change:css_height", (function() {
-                            this.el.style.height = this.model.get("css_height")
-                        }), this), this.model.on("change:resizable", (function() {
-                            this.el.style.resize = this.model.get("resizable") ? "both" : "none"
-                        }), this), this._current_size = [0, 0, 1], this._resizeObserver = new ResizeObserver(this._check_resize.bind(e)), this._resizeObserver.observe(this.img), window.addEventListener("resize", this._check_resize.bind(this)), this._pointers = {}, this._last_buttons = [], this.img.addEventListener("pointerdown", (function(t) {
-                            e.focus_el.focus(), e.img.setPointerCapture(t.pointerId), e._pointers[t.pointerId] = t;
-                            let i = h(e.img, t, e._pointers, "pointer_down");
-                            e._last_buttons = i.buttons, e.send(i), t.altKey || t.preventDefault()
-                        })), this.img.addEventListener("lostpointercapture", (function(t) {
-                            let i = h(e.img, t, e._pointers, "pointer_up");
-                            delete e._pointers[t.pointerId], e._last_buttons = i.buttons, e.send(i)
-                        })), this.img.addEventListener("pointermove", (function(t) {
-                            if (void 0 === e._pointers[t.pointerId] && Object.keys(e._pointers).length > 0) return;
-                            let i = h(e.img, t, e._pointers, "pointer_move");
-                            e.send_throttled(i, 20)
-                        })), this.img.addEventListener("dblclick", (function(t) {
-                            let i = h(e.img, t, {}, "double_click");
-                            delete i.touches, delete i.ntouches, e.send(i), t.altKey || t.preventDefault()
-                        })), this._wheel_state = {
-                            dx: 0,
-                            dy: 0,
-                            e: null,
-                            pending: !1
-                        }, this.img.addEventListener("wheel", (function(i) {
-                            if (window.document.activeElement !== e.focus_el) return;
-                            let s = [1 / window.devicePixelRatio, 16, 600][i.deltaMode];
-                            e._wheel_state.dx += i.deltaX * s, e._wheel_state.dy += i.deltaY * s, e._wheel_state.pending || (e._wheel_state.pending = !0, e._wheel_state.e = i, window.setTimeout(t, 20)), i.altKey || i.preventDefault()
-                        })), this.focus_el.addEventListener("keydown", i, !0), this.focus_el.addEventListener("keyup", i, !0)
-                    }
-                    remove() {
-                        super.remove.apply(this, arguments), window.setTimeout(this.model.collect_view_img_elements.bind(this.model), 10)
-                    }
-                    _check_resize() {
-                        if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.maxWidth = Math.max(1024, window.innerWidth) + "px", void(this.el.style.maxHeight = Math.max(1024, window.innerHeight) + "px");
-                        let e = this.img.clientWidth,
-                            t = this.img.clientHeight,
-                            i = window.devicePixelRatio;
-                        0 === e && 0 === t || this._current_size[0] === e && this._current_size[1] === t && this._current_size[2] === i || (this._current_size = [e, t, i], this.send_throttled({
-                            event_type: "resize",
-                            width: e,
-                            height: t,
-                            pixel_ratio: i,
-                            time_stamp: a()
-                        }, 200))
-                    }
-                    send_throttled(e, t) {
-                        let i = e.event_type || "",
-                            s = this._throttlers[i];
-                        void 0 === s && (s = function(e, t) {
-                            var i, s, n, o = null,
-                                l = 0,
-                                r = function() {
-                                    l = Date.now(), o = null, n = e.apply(i, s), o || (i = s = null)
-                                };
-                            return function() {
-                                var h = Date.now(),
-                                    a = t - (h - l);
-                                return i = this, s = arguments, a <= 0 || a > t ? (o && (clearTimeout(o), o = null), l = h, n = e.apply(i, s), o || (i = s = null)) : o || (o = setTimeout(r, a)), n
-                            }
-                        }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
-                    }
-                }
-                var l = {
-                    Ctrl: "Control",
-                    Del: "Delete",
-                    Esc: "Escape"
-                };
-
-                function r(e) {
-                    return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => l[e] || e))
-                }
-
-                function h(e, t, i, s) {
-                    let n = e.getBoundingClientRect(),
-                        o = [n.left, n.top],
-                        l = Number(t.clientX - o[0]),
-                        h = Number(t.clientY - o[1]),
-                        _ = {},
-                        d = 0;
-                    for (let e in i) {
-                        let t = i[e],
-                            s = {
-                                x: Number(t.clientX - o[0]),
-                                y: Number(t.clientY - o[1]),
-                                pressure: t.pressure
-                            };
-                        _[t.pointerId] = s, d += 1
-                    }
-                    var m = {
-                            0: 1,
-                            1: 3,
-                            2: 2,
-                            3: 4,
-                            4: 5,
-                            5: 6
-                        } [t.button] || 0,
-                        u = [];
-                    for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && u.push(e + 1);
-                    return {
-                        event_type: s,
-                        x: l,
-                        y: h,
-                        button: m,
-                        buttons: u,
-                        modifiers: r(t),
-                        ntouches: d,
-                        touches: _,
-                        time_stamp: a()
-                    }
-                }
-
-                function a() {
-                    return Date.now() / 1e3
-                }
-                const _ = {
-                    i8: "0.4.3"
-                }
-            },
             146: e => {
                 e.exports = t
             },
             325: t => {
                 t.exports = e
             }
         },
@@ -265,15 +14,15 @@
         var t = s[e];
         if (void 0 !== t) return t.exports;
         var o = s[e] = {
             exports: {}
         };
         return i[e](o, o.exports, n), o.exports
     }
-    return n.n = e => {
+    n.n = e => {
         var t = e && e.__esModule ? () => e.default : () => e;
         return n.d(t, {
             a: t
         }), t
     }, n.d = (e, t) => {
         for (var i in t) n.o(t, i) && !n.o(e, i) && Object.defineProperty(e, i, {
             enumerable: !0,
@@ -281,9 +30,258 @@
         })
     }, n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, n.p = "", n(747), n(681)
+    }, n.p = "";
+    var o = {};
+    return (() => {
+        var e = n(325);
+        const t = new URL(e.uri, document.location);
+        t.pathname = t.pathname.slice(0, t.pathname.lastIndexOf("/") + 1), n.p = `${t.origin}${t.pathname}`
+    })(), (() => {
+        n.r(o), n.d(o, {
+            RemoteFrameBufferModel: () => t,
+            RemoteFrameBufferView: () => i,
+            version: () => a
+        });
+        var e = n(146);
+        class t extends e.DOMWidgetModel {
+            defaults() {
+                return {
+                    ...super.defaults(),
+                    _model_name: "RemoteFrameBufferModel",
+                    _view_name: "RemoteFrameBufferView",
+                    _model_module: "jupyter_rfb",
+                    _view_module: "jupyter_rfb",
+                    _model_module_version: "0.1.0",
+                    _view_module_version: "0.1.0",
+                    frame_feedback: {},
+                    css_width: "500px",
+                    css_height: "300px",
+                    resizable: !0,
+                    has_visible_views: !1,
+                    cursor: "default"
+                }
+            }
+            initialize() {
+                super.initialize.apply(this, arguments), this.img_elements = [], this._intersection_observer = new IntersectionObserver(this._intersection_callback.bind(this)), window.setInterval(this.collect_view_img_elements.bind(this), 5e3), this.frames = [], this.on("msg:custom", this.on_msg, this), this.last_frame = {
+                    src: "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAADElEQVR42mOor68HAAL+AX6E2KOJAAAAAElFTkSuQmCC",
+                    index: 0,
+                    timestamp: 0
+                }, this._img_update_pending = !1, this._request_animation_frame()
+            }
+            async collect_view_img_elements() {
+                this._intersection_observer.disconnect();
+                for (let e of this.img_elements) e.onload = null;
+                this.img_elements = [];
+                for (let e in this.views) {
+                    let t = await this.views[e];
+                    this._intersection_observer.observe(t.img), this.img_elements.push(t.img), t.img.onload = this._request_animation_frame.bind(this)
+                }
+                this._request_animation_frame()
+            }
+            on_msg(e, t) {
+                "framebufferdata" === e.type && this.frames.push({
+                    ...e,
+                    buffers: t
+                })
+            }
+            _intersection_callback(e, t) {
+                for (let t of e) t.target._is_visible = t.isIntersecting;
+                let i = 0;
+                for (let e of this.img_elements) e._is_visible && (i += 1);
+                let s = i > 0;
+                s != this.get("has_visible_views") && (this.set("has_visible_views", s), this.save_changes())
+            }
+            _send_response() {
+                let e = this.last_frame,
+                    t = {
+                        index: e.index,
+                        timestamp: e.timestamp,
+                        localtime: Date.now() / 1e3
+                    };
+                this.set("frame_feedback", t), this.save_changes()
+            }
+            _request_animation_frame() {
+                if (!this._img_update_pending) {
+                    this._img_update_pending = !0;
+                    let e = this._animate.bind(this);
+                    window.setTimeout(window.requestAnimationFrame, 5, e)
+                }
+            }
+            _animate() {
+                if (this._img_update_pending = !1, !this.frames.length) return void this._request_animation_frame();
+                let e, t = this.frames.shift();
+                if (t.buffers.length > 0) {
+                    let i = new Blob([t.buffers[0].buffer], {
+                        type: t.mimetype
+                    });
+                    e = URL.createObjectURL(i)
+                } else e = t.data_b64;
+                let i = this.img_elements?.[0]?.src;
+                i.startsWith("blob:") && URL.revokeObjectURL(i);
+                for (let t of this.img_elements) t.src = e;
+                this.last_frame = t, this._send_response(), 0 === this.img_elements.length && this._request_animation_frame()
+            }
+            close() {
+                this.send({
+                    event_type: "close",
+                    time_stamp: h()
+                }), super.close.apply(this, arguments)
+            }
+        }
+        class i extends e.DOMWidgetView {
+            render() {
+                var e = this;
+
+                function t() {
+                    let t = e._wheel_state.e,
+                        i = e.img.getBoundingClientRect(),
+                        s = {
+                            event_type: "wheel",
+                            x: Number(t.clientX - i.left),
+                            y: Number(t.clientY - i.top),
+                            dx: e._wheel_state.dx,
+                            dy: e._wheel_state.dy,
+                            buttons: e._last_buttons,
+                            modifiers: l(t),
+                            time_stamp: h()
+                        };
+                    e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
+                }
+
+                function i(t) {
+                    if (null === e.el.offsetParent) return;
+                    let i = {
+                        event_type: "key_" + t.type.slice(3),
+                        key: s[t.key] || t.key,
+                        modifiers: l(t),
+                        time_stamp: h()
+                    };
+                    t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
+                }
+                this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
+                    if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
+                }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this.el.style.cursor = this.model.get("cursor"), this.model.on("change:cursor", (function() {
+                    this.el.style.cursor = this.model.get("cursor")
+                }), this), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
+                    this.el.style.width = this.model.get("css_width")
+                }), this), this.model.on("change:css_height", (function() {
+                    this.el.style.height = this.model.get("css_height")
+                }), this), this.model.on("change:resizable", (function() {
+                    this.el.style.resize = this.model.get("resizable") ? "both" : "none"
+                }), this), this._current_size = [0, 0, 1], this._resizeObserver = new ResizeObserver(this._check_resize.bind(e)), this._resizeObserver.observe(this.img), window.addEventListener("resize", this._check_resize.bind(this)), this._pointers = {}, this._last_buttons = [], this.img.addEventListener("pointerdown", (function(t) {
+                    e.focus_el.focus(), e.img.setPointerCapture(t.pointerId), e._pointers[t.pointerId] = t;
+                    let i = r(e.img, t, e._pointers, "pointer_down");
+                    e._last_buttons = i.buttons, e.send(i), t.altKey || t.preventDefault()
+                })), this.img.addEventListener("lostpointercapture", (function(t) {
+                    let i = r(e.img, t, e._pointers, "pointer_up");
+                    delete e._pointers[t.pointerId], e._last_buttons = i.buttons, e.send(i)
+                })), this.img.addEventListener("pointermove", (function(t) {
+                    if (void 0 === e._pointers[t.pointerId] && Object.keys(e._pointers).length > 0) return;
+                    let i = r(e.img, t, e._pointers, "pointer_move");
+                    e.send_throttled(i, 20)
+                })), this.img.addEventListener("dblclick", (function(t) {
+                    let i = r(e.img, t, {}, "double_click");
+                    delete i.touches, delete i.ntouches, e.send(i), t.altKey || t.preventDefault()
+                })), this._wheel_state = {
+                    dx: 0,
+                    dy: 0,
+                    e: null,
+                    pending: !1
+                }, this.img.addEventListener("wheel", (function(i) {
+                    if (window.document.activeElement !== e.focus_el) return;
+                    let s = [1 / window.devicePixelRatio, 16, 600][i.deltaMode];
+                    e._wheel_state.dx += i.deltaX * s, e._wheel_state.dy += i.deltaY * s, e._wheel_state.pending || (e._wheel_state.pending = !0, e._wheel_state.e = i, window.setTimeout(t, 20)), i.altKey || i.preventDefault()
+                })), this.focus_el.addEventListener("keydown", i, !0), this.focus_el.addEventListener("keyup", i, !0)
+            }
+            remove() {
+                super.remove.apply(this, arguments), window.setTimeout(this.model.collect_view_img_elements.bind(this.model), 10)
+            }
+            _check_resize() {
+                if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.maxWidth = Math.max(1024, window.innerWidth) + "px", void(this.el.style.maxHeight = Math.max(1024, window.innerHeight) + "px");
+                let e = this.img.clientWidth,
+                    t = this.img.clientHeight,
+                    i = window.devicePixelRatio;
+                0 === e && 0 === t || this._current_size[0] === e && this._current_size[1] === t && this._current_size[2] === i || (this._current_size = [e, t, i], this.send_throttled({
+                    event_type: "resize",
+                    width: e,
+                    height: t,
+                    pixel_ratio: i,
+                    time_stamp: h()
+                }, 200))
+            }
+            send_throttled(e, t) {
+                let i = e.event_type || "",
+                    s = this._throttlers[i];
+                void 0 === s && (s = function(e, t) {
+                    var i, s, n, o = null,
+                        l = 0,
+                        r = function() {
+                            l = Date.now(), o = null, n = e.apply(i, s), o || (i = s = null)
+                        };
+                    return function() {
+                        var h = Date.now(),
+                            a = t - (h - l);
+                        return i = this, s = arguments, a <= 0 || a > t ? (o && (clearTimeout(o), o = null), l = h, n = e.apply(i, s), o || (i = s = null)) : o || (o = setTimeout(r, a)), n
+                    }
+                }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
+            }
+        }
+        var s = {
+            Ctrl: "Control",
+            Del: "Delete",
+            Esc: "Escape"
+        };
+
+        function l(e) {
+            return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => s[e] || e))
+        }
+
+        function r(e, t, i, s) {
+            let n = e.getBoundingClientRect(),
+                o = [n.left, n.top],
+                r = Number(t.clientX - o[0]),
+                a = Number(t.clientY - o[1]),
+                _ = {},
+                d = 0;
+            for (let e in i) {
+                let t = i[e],
+                    s = {
+                        x: Number(t.clientX - o[0]),
+                        y: Number(t.clientY - o[1]),
+                        pressure: t.pressure
+                    };
+                _[t.pointerId] = s, d += 1
+            }
+            var m = {
+                    0: 1,
+                    1: 3,
+                    2: 2,
+                    3: 4,
+                    4: 5,
+                    5: 6
+                } [t.button] || 0,
+                u = [];
+            for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && u.push(e + 1);
+            return {
+                event_type: s,
+                x: r,
+                y: a,
+                button: m,
+                buttons: u,
+                modifiers: l(t),
+                ntouches: d,
+                touches: _,
+                time_stamp: h()
+            }
+        }
+
+        function h() {
+            return Date.now() / 1e3
+        }
+        const a = "0.1.0"
+    })(), o
 })()));
```

### Comparing `jupyter_rfb-0.4.3/js/lib/labplugin.js` & `jupyter_rfb-0.4.4/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/js/lib/widget.js` & `jupyter_rfb-0.4.4/js/lib/widget.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/js/package.json` & `jupyter_rfb-0.4.4/jupyter_rfb/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9471153846153846%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^3.6 || ^4'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.cf57a6d7f00412526ea4.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'version'": "'0.1.0'"}*

```diff
@@ -2,24 +2,28 @@
     "author": "Almar Klein",
     "dependencies": {
         "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^5 || ^6",
         "lodash": "^4.17.4"
     },
     "description": "Remote Frame Buffer for Jupyter",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.1.3",
+        "@jupyterlab/builder": "^3.6 || ^4",
         "rimraf": "^2.6.1",
         "webpack": "^5",
         "webpack-cli": "^5.1.4"
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js"
     ],
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.cf57a6d7f00412526ea4.js"
+        },
         "extension": "lib/labplugin",
         "outputDir": "../jupyter_rfb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -45,9 +49,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../jupyter_rfb/labextension/ && rimraf ../jupyter_rfb/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.4.3"
+    "version": "0.1.0"
 }
```

### Comparing `jupyter_rfb-0.4.3/js/webpack.config.js` & `jupyter_rfb-0.4.4/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/js/yarn.lock` & `jupyter_rfb-0.4.4/js/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     "@types/backbone" "^1.4.1"
     "@types/lodash" "^4.14.134"
     backbone "1.2.3"
     base64-js "^1.2.1"
     jquery "^3.1.1"
     lodash "^4.17.4"
 
-"@jupyterlab/builder@^4.1.3":
+"@jupyterlab/builder@^3.6 || ^4":
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-4.2.0.tgz#6847347e5c91c427fc09f66ca18c2d95c214fcf0"
   integrity sha512-hYcwTcA5Ipni9x5At1TNfxMmhx9kIBZXaN+YdcQBU734zlBhLDHZBqZ2gkoGSp0hmaSK7LtcX0V0Cikh4ZU0Yg==
   dependencies:
     "@lumino/algorithm" "^2.0.1"
     "@lumino/application" "^2.3.1"
     "@lumino/commands" "^2.3.0"
```

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/__init__.py` & `jupyter_rfb-0.4.4/jupyter_rfb/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/_jpg.py` & `jupyter_rfb-0.4.4/jupyter_rfb/_jpg.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/_png.py` & `jupyter_rfb-0.4.4/jupyter_rfb/_png.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/_utils.py` & `jupyter_rfb-0.4.4/jupyter_rfb/_utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/events.py` & `jupyter_rfb-0.4.4/jupyter_rfb/events.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/labextension/package.json` & `jupyter_rfb-0.4.4/js/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9471153846153846%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^3.6 || ^4'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.1.0'"}*

```diff
@@ -2,28 +2,24 @@
     "author": "Almar Klein",
     "dependencies": {
         "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^5 || ^6",
         "lodash": "^4.17.4"
     },
     "description": "Remote Frame Buffer for Jupyter",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.1.3",
+        "@jupyterlab/builder": "^3.6 || ^4",
         "rimraf": "^2.6.1",
         "webpack": "^5",
         "webpack-cli": "^5.1.4"
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js"
     ],
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.0d5a3b6ccc7e17c1ed27.js"
-        },
         "extension": "lib/labplugin",
         "outputDir": "../jupyter_rfb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -49,9 +45,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../jupyter_rfb/labextension/ && rimraf ../jupyter_rfb/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.4.3"
+    "version": "0.1.0"
 }
```

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/493.cb43b5d572b2f6b10c8e.js` & `jupyter_rfb-0.4.4/jupyter_rfb/labextension/static/493.102804eff6eca0571ecf.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunkjupyter_rfb = self.webpackChunkjupyter_rfb || []).push([
-    [493], {
-        678: (e, t, i) => {
+    [493, 420], {
+        420: (e, t, i) => {
             i.r(t), i.d(t, {
                 RemoteFrameBufferModel: () => n,
                 RemoteFrameBufferView: () => r,
-                version: () => a.rE
+                version: () => a
             });
             var s = i(4);
             class n extends s.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "RemoteFrameBufferModel",
@@ -239,24 +239,22 @@
                     time_stamp: _()
                 }
             }
 
             function _() {
                 return Date.now() / 1e3
             }
-            const a = {
-                rE: "0.4.3"
-            }
+            const a = "0.1.0"
         },
         493: (e, t, i) => {
             i.r(t), i.d(t, {
                 default: () => r,
                 remoteFrameBufferPlugin: () => n
             });
-            var s = i(678);
+            var s = i(420);
             const n = {
                     id: "jupyter_rfb:plugin",
                     requires: [i(4).IJupyterWidgetRegistry],
                     activate: function(e, t) {
                         t.registerWidget({
                             name: "jupyter_rfb",
                             version: s.version,
```

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/678.c748912b15ffb2656a49.js` & `jupyter_rfb-0.4.4/jupyter_rfb/labextension/static/420.d43f6d92aa7a9fb70aad.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunkjupyter_rfb = self.webpackChunkjupyter_rfb || []).push([
-    [678, 4], {
-        678: (e, t, i) => {
+    [420], {
+        420: (e, t, i) => {
             i.r(t), i.d(t, {
                 RemoteFrameBufferModel: () => n,
                 RemoteFrameBufferView: () => l,
-                version: () => a.rE
+                version: () => a
             });
             var s = i(4);
             class n extends s.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "RemoteFrameBufferModel",
@@ -239,13 +239,11 @@
                     time_stamp: _()
                 }
             }
 
             function _() {
                 return Date.now() / 1e3
             }
-            const a = {
-                rE: "0.4.3"
-            }
+            const a = "0.1.0"
         }
     }
 ]);
```

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/remoteEntry.0d5a3b6ccc7e17c1ed27.js` & `jupyter_rfb-0.4.4/jupyter_rfb/labextension/static/remoteEntry.cf57a6d7f00412526ea4.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, a, i, u, f, l, s, d, p, c, h, v, b, g = {
             784: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(678).then((() => () => t(678))),
+                        "./index": () => Promise.all([t.e(4), t.e(420)]).then((() => () => t(420))),
                         "./extension": () => Promise.all([t.e(4), t.e(493)]).then((() => () => t(493)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -42,20 +42,20 @@
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
         4: "8c0b9e46657bfc157d84",
-        493: "cb43b5d572b2f6b10c8e",
-        678: "c748912b15ffb2656a49"
+        420: "d43f6d92aa7a9fb70aad",
+        493: "102804eff6eca0571ecf"
     } [e] + ".js?v=" + {
         4: "8c0b9e46657bfc157d84",
-        493: "cb43b5d572b2f6b10c8e",
-        678: "c748912b15ffb2656a49"
+        420: "d43f6d92aa7a9fb70aad",
+        493: "102804eff6eca0571ecf"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -102,19 +102,19 @@
                 var a = y.S[t],
                     i = "jupyter_rfb",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => y.e(678).then((() => () => y(678))),
+                        get: () => Promise.all([y.e(4), y.e(420)]).then((() => () => y(420))),
                         from: i,
                         eager: !1
                     })
-                })("jupyter_rfb", "0.4.3"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyter_rfb", "0.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -216,16 +216,15 @@
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1, 1
         ])
     }, v = {
-        4: [4],
-        678: [4]
+        4: [4]
     }, b = {}, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             if (!b[e]) {
                 var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
```

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/nbextension/extension.js` & `jupyter_rfb-0.4.4/jupyter_rfb/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/nbextension/index.js` & `jupyter_rfb-0.4.4/jupyter_rfb/nbextension/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,261 +1,10 @@
 define(["module", "@jupyter-widgets/base"], ((e, t) => (() => {
     "use strict";
     var i = {
-            747: (e, t, i) => {
-                var s = i(325);
-                const n = new URL(s.uri, document.location);
-                n.pathname = n.pathname.slice(0, n.pathname.lastIndexOf("/") + 1), i.p = `${n.origin}${n.pathname}`
-            },
-            681: (e, t, i) => {
-                i.r(t), i.d(t, {
-                    RemoteFrameBufferModel: () => n,
-                    RemoteFrameBufferView: () => o,
-                    version: () => _.i8
-                });
-                var s = i(146);
-                class n extends s.DOMWidgetModel {
-                    defaults() {
-                        return {
-                            ...super.defaults(),
-                            _model_name: "RemoteFrameBufferModel",
-                            _view_name: "RemoteFrameBufferView",
-                            _model_module: "jupyter_rfb",
-                            _view_module: "jupyter_rfb",
-                            _model_module_version: "0.1.0",
-                            _view_module_version: "0.1.0",
-                            frame_feedback: {},
-                            css_width: "500px",
-                            css_height: "300px",
-                            resizable: !0,
-                            has_visible_views: !1,
-                            cursor: "default"
-                        }
-                    }
-                    initialize() {
-                        super.initialize.apply(this, arguments), this.img_elements = [], this._intersection_observer = new IntersectionObserver(this._intersection_callback.bind(this)), window.setInterval(this.collect_view_img_elements.bind(this), 5e3), this.frames = [], this.on("msg:custom", this.on_msg, this), this.last_frame = {
-                            src: "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAADElEQVR42mOor68HAAL+AX6E2KOJAAAAAElFTkSuQmCC",
-                            index: 0,
-                            timestamp: 0
-                        }, this._img_update_pending = !1, this._request_animation_frame()
-                    }
-                    async collect_view_img_elements() {
-                        this._intersection_observer.disconnect();
-                        for (let e of this.img_elements) e.onload = null;
-                        this.img_elements = [];
-                        for (let e in this.views) {
-                            let t = await this.views[e];
-                            this._intersection_observer.observe(t.img), this.img_elements.push(t.img), t.img.onload = this._request_animation_frame.bind(this)
-                        }
-                        this._request_animation_frame()
-                    }
-                    on_msg(e, t) {
-                        "framebufferdata" === e.type && this.frames.push({
-                            ...e,
-                            buffers: t
-                        })
-                    }
-                    _intersection_callback(e, t) {
-                        for (let t of e) t.target._is_visible = t.isIntersecting;
-                        let i = 0;
-                        for (let e of this.img_elements) e._is_visible && (i += 1);
-                        let s = i > 0;
-                        s != this.get("has_visible_views") && (this.set("has_visible_views", s), this.save_changes())
-                    }
-                    _send_response() {
-                        let e = this.last_frame,
-                            t = {
-                                index: e.index,
-                                timestamp: e.timestamp,
-                                localtime: Date.now() / 1e3
-                            };
-                        this.set("frame_feedback", t), this.save_changes()
-                    }
-                    _request_animation_frame() {
-                        if (!this._img_update_pending) {
-                            this._img_update_pending = !0;
-                            let e = this._animate.bind(this);
-                            window.setTimeout(window.requestAnimationFrame, 5, e)
-                        }
-                    }
-                    _animate() {
-                        if (this._img_update_pending = !1, !this.frames.length) return void this._request_animation_frame();
-                        let e, t = this.frames.shift();
-                        if (t.buffers.length > 0) {
-                            let i = new Blob([t.buffers[0].buffer], {
-                                type: t.mimetype
-                            });
-                            e = URL.createObjectURL(i)
-                        } else e = t.data_b64;
-                        let i = this.img_elements?.[0]?.src;
-                        i.startsWith("blob:") && URL.revokeObjectURL(i);
-                        for (let t of this.img_elements) t.src = e;
-                        this.last_frame = t, this._send_response(), 0 === this.img_elements.length && this._request_animation_frame()
-                    }
-                    close() {
-                        this.send({
-                            event_type: "close",
-                            time_stamp: a()
-                        }), super.close.apply(this, arguments)
-                    }
-                }
-                class o extends s.DOMWidgetView {
-                    render() {
-                        var e = this;
-
-                        function t() {
-                            let t = e._wheel_state.e,
-                                i = e.img.getBoundingClientRect(),
-                                s = {
-                                    event_type: "wheel",
-                                    x: Number(t.clientX - i.left),
-                                    y: Number(t.clientY - i.top),
-                                    dx: e._wheel_state.dx,
-                                    dy: e._wheel_state.dy,
-                                    buttons: e._last_buttons,
-                                    modifiers: r(t),
-                                    time_stamp: a()
-                                };
-                            e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
-                        }
-
-                        function i(t) {
-                            if (null === e.el.offsetParent) return;
-                            let i = {
-                                event_type: "key_" + t.type.slice(3),
-                                key: l[t.key] || t.key,
-                                modifiers: r(t),
-                                time_stamp: a()
-                            };
-                            t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
-                        }
-                        this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
-                            if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
-                        }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this.el.style.cursor = this.model.get("cursor"), this.model.on("change:cursor", (function() {
-                            this.el.style.cursor = this.model.get("cursor")
-                        }), this), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
-                            this.el.style.width = this.model.get("css_width")
-                        }), this), this.model.on("change:css_height", (function() {
-                            this.el.style.height = this.model.get("css_height")
-                        }), this), this.model.on("change:resizable", (function() {
-                            this.el.style.resize = this.model.get("resizable") ? "both" : "none"
-                        }), this), this._current_size = [0, 0, 1], this._resizeObserver = new ResizeObserver(this._check_resize.bind(e)), this._resizeObserver.observe(this.img), window.addEventListener("resize", this._check_resize.bind(this)), this._pointers = {}, this._last_buttons = [], this.img.addEventListener("pointerdown", (function(t) {
-                            e.focus_el.focus(), e.img.setPointerCapture(t.pointerId), e._pointers[t.pointerId] = t;
-                            let i = h(e.img, t, e._pointers, "pointer_down");
-                            e._last_buttons = i.buttons, e.send(i), t.altKey || t.preventDefault()
-                        })), this.img.addEventListener("lostpointercapture", (function(t) {
-                            let i = h(e.img, t, e._pointers, "pointer_up");
-                            delete e._pointers[t.pointerId], e._last_buttons = i.buttons, e.send(i)
-                        })), this.img.addEventListener("pointermove", (function(t) {
-                            if (void 0 === e._pointers[t.pointerId] && Object.keys(e._pointers).length > 0) return;
-                            let i = h(e.img, t, e._pointers, "pointer_move");
-                            e.send_throttled(i, 20)
-                        })), this.img.addEventListener("dblclick", (function(t) {
-                            let i = h(e.img, t, {}, "double_click");
-                            delete i.touches, delete i.ntouches, e.send(i), t.altKey || t.preventDefault()
-                        })), this._wheel_state = {
-                            dx: 0,
-                            dy: 0,
-                            e: null,
-                            pending: !1
-                        }, this.img.addEventListener("wheel", (function(i) {
-                            if (window.document.activeElement !== e.focus_el) return;
-                            let s = [1 / window.devicePixelRatio, 16, 600][i.deltaMode];
-                            e._wheel_state.dx += i.deltaX * s, e._wheel_state.dy += i.deltaY * s, e._wheel_state.pending || (e._wheel_state.pending = !0, e._wheel_state.e = i, window.setTimeout(t, 20)), i.altKey || i.preventDefault()
-                        })), this.focus_el.addEventListener("keydown", i, !0), this.focus_el.addEventListener("keyup", i, !0)
-                    }
-                    remove() {
-                        super.remove.apply(this, arguments), window.setTimeout(this.model.collect_view_img_elements.bind(this.model), 10)
-                    }
-                    _check_resize() {
-                        if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.maxWidth = Math.max(1024, window.innerWidth) + "px", void(this.el.style.maxHeight = Math.max(1024, window.innerHeight) + "px");
-                        let e = this.img.clientWidth,
-                            t = this.img.clientHeight,
-                            i = window.devicePixelRatio;
-                        0 === e && 0 === t || this._current_size[0] === e && this._current_size[1] === t && this._current_size[2] === i || (this._current_size = [e, t, i], this.send_throttled({
-                            event_type: "resize",
-                            width: e,
-                            height: t,
-                            pixel_ratio: i,
-                            time_stamp: a()
-                        }, 200))
-                    }
-                    send_throttled(e, t) {
-                        let i = e.event_type || "",
-                            s = this._throttlers[i];
-                        void 0 === s && (s = function(e, t) {
-                            var i, s, n, o = null,
-                                l = 0,
-                                r = function() {
-                                    l = Date.now(), o = null, n = e.apply(i, s), o || (i = s = null)
-                                };
-                            return function() {
-                                var h = Date.now(),
-                                    a = t - (h - l);
-                                return i = this, s = arguments, a <= 0 || a > t ? (o && (clearTimeout(o), o = null), l = h, n = e.apply(i, s), o || (i = s = null)) : o || (o = setTimeout(r, a)), n
-                            }
-                        }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
-                    }
-                }
-                var l = {
-                    Ctrl: "Control",
-                    Del: "Delete",
-                    Esc: "Escape"
-                };
-
-                function r(e) {
-                    return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => l[e] || e))
-                }
-
-                function h(e, t, i, s) {
-                    let n = e.getBoundingClientRect(),
-                        o = [n.left, n.top],
-                        l = Number(t.clientX - o[0]),
-                        h = Number(t.clientY - o[1]),
-                        _ = {},
-                        d = 0;
-                    for (let e in i) {
-                        let t = i[e],
-                            s = {
-                                x: Number(t.clientX - o[0]),
-                                y: Number(t.clientY - o[1]),
-                                pressure: t.pressure
-                            };
-                        _[t.pointerId] = s, d += 1
-                    }
-                    var m = {
-                            0: 1,
-                            1: 3,
-                            2: 2,
-                            3: 4,
-                            4: 5,
-                            5: 6
-                        } [t.button] || 0,
-                        u = [];
-                    for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && u.push(e + 1);
-                    return {
-                        event_type: s,
-                        x: l,
-                        y: h,
-                        button: m,
-                        buttons: u,
-                        modifiers: r(t),
-                        ntouches: d,
-                        touches: _,
-                        time_stamp: a()
-                    }
-                }
-
-                function a() {
-                    return Date.now() / 1e3
-                }
-                const _ = {
-                    i8: "0.4.3"
-                }
-            },
             146: e => {
                 e.exports = t
             },
             325: t => {
                 t.exports = e
             }
         },
@@ -265,15 +14,15 @@
         var t = s[e];
         if (void 0 !== t) return t.exports;
         var o = s[e] = {
             exports: {}
         };
         return i[e](o, o.exports, n), o.exports
     }
-    return n.n = e => {
+    n.n = e => {
         var t = e && e.__esModule ? () => e.default : () => e;
         return n.d(t, {
             a: t
         }), t
     }, n.d = (e, t) => {
         for (var i in t) n.o(t, i) && !n.o(e, i) && Object.defineProperty(e, i, {
             enumerable: !0,
@@ -281,9 +30,258 @@
         })
     }, n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, n.p = "", n(747), n(681)
+    }, n.p = "";
+    var o = {};
+    return (() => {
+        var e = n(325);
+        const t = new URL(e.uri, document.location);
+        t.pathname = t.pathname.slice(0, t.pathname.lastIndexOf("/") + 1), n.p = `${t.origin}${t.pathname}`
+    })(), (() => {
+        n.r(o), n.d(o, {
+            RemoteFrameBufferModel: () => t,
+            RemoteFrameBufferView: () => i,
+            version: () => a
+        });
+        var e = n(146);
+        class t extends e.DOMWidgetModel {
+            defaults() {
+                return {
+                    ...super.defaults(),
+                    _model_name: "RemoteFrameBufferModel",
+                    _view_name: "RemoteFrameBufferView",
+                    _model_module: "jupyter_rfb",
+                    _view_module: "jupyter_rfb",
+                    _model_module_version: "0.1.0",
+                    _view_module_version: "0.1.0",
+                    frame_feedback: {},
+                    css_width: "500px",
+                    css_height: "300px",
+                    resizable: !0,
+                    has_visible_views: !1,
+                    cursor: "default"
+                }
+            }
+            initialize() {
+                super.initialize.apply(this, arguments), this.img_elements = [], this._intersection_observer = new IntersectionObserver(this._intersection_callback.bind(this)), window.setInterval(this.collect_view_img_elements.bind(this), 5e3), this.frames = [], this.on("msg:custom", this.on_msg, this), this.last_frame = {
+                    src: "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAADElEQVR42mOor68HAAL+AX6E2KOJAAAAAElFTkSuQmCC",
+                    index: 0,
+                    timestamp: 0
+                }, this._img_update_pending = !1, this._request_animation_frame()
+            }
+            async collect_view_img_elements() {
+                this._intersection_observer.disconnect();
+                for (let e of this.img_elements) e.onload = null;
+                this.img_elements = [];
+                for (let e in this.views) {
+                    let t = await this.views[e];
+                    this._intersection_observer.observe(t.img), this.img_elements.push(t.img), t.img.onload = this._request_animation_frame.bind(this)
+                }
+                this._request_animation_frame()
+            }
+            on_msg(e, t) {
+                "framebufferdata" === e.type && this.frames.push({
+                    ...e,
+                    buffers: t
+                })
+            }
+            _intersection_callback(e, t) {
+                for (let t of e) t.target._is_visible = t.isIntersecting;
+                let i = 0;
+                for (let e of this.img_elements) e._is_visible && (i += 1);
+                let s = i > 0;
+                s != this.get("has_visible_views") && (this.set("has_visible_views", s), this.save_changes())
+            }
+            _send_response() {
+                let e = this.last_frame,
+                    t = {
+                        index: e.index,
+                        timestamp: e.timestamp,
+                        localtime: Date.now() / 1e3
+                    };
+                this.set("frame_feedback", t), this.save_changes()
+            }
+            _request_animation_frame() {
+                if (!this._img_update_pending) {
+                    this._img_update_pending = !0;
+                    let e = this._animate.bind(this);
+                    window.setTimeout(window.requestAnimationFrame, 5, e)
+                }
+            }
+            _animate() {
+                if (this._img_update_pending = !1, !this.frames.length) return void this._request_animation_frame();
+                let e, t = this.frames.shift();
+                if (t.buffers.length > 0) {
+                    let i = new Blob([t.buffers[0].buffer], {
+                        type: t.mimetype
+                    });
+                    e = URL.createObjectURL(i)
+                } else e = t.data_b64;
+                let i = this.img_elements?.[0]?.src;
+                i.startsWith("blob:") && URL.revokeObjectURL(i);
+                for (let t of this.img_elements) t.src = e;
+                this.last_frame = t, this._send_response(), 0 === this.img_elements.length && this._request_animation_frame()
+            }
+            close() {
+                this.send({
+                    event_type: "close",
+                    time_stamp: h()
+                }), super.close.apply(this, arguments)
+            }
+        }
+        class i extends e.DOMWidgetView {
+            render() {
+                var e = this;
+
+                function t() {
+                    let t = e._wheel_state.e,
+                        i = e.img.getBoundingClientRect(),
+                        s = {
+                            event_type: "wheel",
+                            x: Number(t.clientX - i.left),
+                            y: Number(t.clientY - i.top),
+                            dx: e._wheel_state.dx,
+                            dy: e._wheel_state.dy,
+                            buttons: e._last_buttons,
+                            modifiers: l(t),
+                            time_stamp: h()
+                        };
+                    e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
+                }
+
+                function i(t) {
+                    if (null === e.el.offsetParent) return;
+                    let i = {
+                        event_type: "key_" + t.type.slice(3),
+                        key: s[t.key] || t.key,
+                        modifiers: l(t),
+                        time_stamp: h()
+                    };
+                    t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
+                }
+                this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
+                    if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
+                }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this.el.style.cursor = this.model.get("cursor"), this.model.on("change:cursor", (function() {
+                    this.el.style.cursor = this.model.get("cursor")
+                }), this), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
+                    this.el.style.width = this.model.get("css_width")
+                }), this), this.model.on("change:css_height", (function() {
+                    this.el.style.height = this.model.get("css_height")
+                }), this), this.model.on("change:resizable", (function() {
+                    this.el.style.resize = this.model.get("resizable") ? "both" : "none"
+                }), this), this._current_size = [0, 0, 1], this._resizeObserver = new ResizeObserver(this._check_resize.bind(e)), this._resizeObserver.observe(this.img), window.addEventListener("resize", this._check_resize.bind(this)), this._pointers = {}, this._last_buttons = [], this.img.addEventListener("pointerdown", (function(t) {
+                    e.focus_el.focus(), e.img.setPointerCapture(t.pointerId), e._pointers[t.pointerId] = t;
+                    let i = r(e.img, t, e._pointers, "pointer_down");
+                    e._last_buttons = i.buttons, e.send(i), t.altKey || t.preventDefault()
+                })), this.img.addEventListener("lostpointercapture", (function(t) {
+                    let i = r(e.img, t, e._pointers, "pointer_up");
+                    delete e._pointers[t.pointerId], e._last_buttons = i.buttons, e.send(i)
+                })), this.img.addEventListener("pointermove", (function(t) {
+                    if (void 0 === e._pointers[t.pointerId] && Object.keys(e._pointers).length > 0) return;
+                    let i = r(e.img, t, e._pointers, "pointer_move");
+                    e.send_throttled(i, 20)
+                })), this.img.addEventListener("dblclick", (function(t) {
+                    let i = r(e.img, t, {}, "double_click");
+                    delete i.touches, delete i.ntouches, e.send(i), t.altKey || t.preventDefault()
+                })), this._wheel_state = {
+                    dx: 0,
+                    dy: 0,
+                    e: null,
+                    pending: !1
+                }, this.img.addEventListener("wheel", (function(i) {
+                    if (window.document.activeElement !== e.focus_el) return;
+                    let s = [1 / window.devicePixelRatio, 16, 600][i.deltaMode];
+                    e._wheel_state.dx += i.deltaX * s, e._wheel_state.dy += i.deltaY * s, e._wheel_state.pending || (e._wheel_state.pending = !0, e._wheel_state.e = i, window.setTimeout(t, 20)), i.altKey || i.preventDefault()
+                })), this.focus_el.addEventListener("keydown", i, !0), this.focus_el.addEventListener("keyup", i, !0)
+            }
+            remove() {
+                super.remove.apply(this, arguments), window.setTimeout(this.model.collect_view_img_elements.bind(this.model), 10)
+            }
+            _check_resize() {
+                if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.maxWidth = Math.max(1024, window.innerWidth) + "px", void(this.el.style.maxHeight = Math.max(1024, window.innerHeight) + "px");
+                let e = this.img.clientWidth,
+                    t = this.img.clientHeight,
+                    i = window.devicePixelRatio;
+                0 === e && 0 === t || this._current_size[0] === e && this._current_size[1] === t && this._current_size[2] === i || (this._current_size = [e, t, i], this.send_throttled({
+                    event_type: "resize",
+                    width: e,
+                    height: t,
+                    pixel_ratio: i,
+                    time_stamp: h()
+                }, 200))
+            }
+            send_throttled(e, t) {
+                let i = e.event_type || "",
+                    s = this._throttlers[i];
+                void 0 === s && (s = function(e, t) {
+                    var i, s, n, o = null,
+                        l = 0,
+                        r = function() {
+                            l = Date.now(), o = null, n = e.apply(i, s), o || (i = s = null)
+                        };
+                    return function() {
+                        var h = Date.now(),
+                            a = t - (h - l);
+                        return i = this, s = arguments, a <= 0 || a > t ? (o && (clearTimeout(o), o = null), l = h, n = e.apply(i, s), o || (i = s = null)) : o || (o = setTimeout(r, a)), n
+                    }
+                }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
+            }
+        }
+        var s = {
+            Ctrl: "Control",
+            Del: "Delete",
+            Esc: "Escape"
+        };
+
+        function l(e) {
+            return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => s[e] || e))
+        }
+
+        function r(e, t, i, s) {
+            let n = e.getBoundingClientRect(),
+                o = [n.left, n.top],
+                r = Number(t.clientX - o[0]),
+                a = Number(t.clientY - o[1]),
+                _ = {},
+                d = 0;
+            for (let e in i) {
+                let t = i[e],
+                    s = {
+                        x: Number(t.clientX - o[0]),
+                        y: Number(t.clientY - o[1]),
+                        pressure: t.pressure
+                    };
+                _[t.pointerId] = s, d += 1
+            }
+            var m = {
+                    0: 1,
+                    1: 3,
+                    2: 2,
+                    3: 4,
+                    4: 5,
+                    5: 6
+                } [t.button] || 0,
+                u = [];
+            for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && u.push(e + 1);
+            return {
+                event_type: s,
+                x: r,
+                y: a,
+                button: m,
+                buttons: u,
+                modifiers: l(t),
+                ntouches: d,
+                touches: _,
+                time_stamp: h()
+            }
+        }
+
+        function h() {
+            return Date.now() / 1e3
+        }
+        const a = "0.1.0"
+    })(), o
 })()));
```

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb/widget.py` & `jupyter_rfb-0.4.4/jupyter_rfb/widget.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb.egg-info/PKG-INFO` & `jupyter_rfb-0.4.4/jupyter_rfb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-rfb
-Version: 0.4.3
+Version: 0.4.4
 Summary: Remote Frame Buffer for Jupyter
 Home-page: https://github.com/vispy/jupyter_rfb
 Author: Almar Klein
 Author-email: almar@almarklein.org
 License: MIT
 Keywords: ipython,jupyter,widgets,visualization,remote frame buffer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jupyter_rfb-0.4.3/jupyter_rfb.egg-info/SOURCES.txt` & `jupyter_rfb-0.4.4/jupyter_rfb.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 jupyter_rfb.json
 pyproject.toml
 setup.cfg
 setup.py
 js/.eslintrc.json
 js/README.md
 js/amd-public-path.js
+js/package-lock.json
 js/package.json
 js/webpack.config.js
 js/yarn.lock
 js/dist/index.js
 js/lib/extension.js
 js/lib/index.js
 js/lib/labplugin.js
@@ -27,17 +28,17 @@
 jupyter_rfb.egg-info/PKG-INFO
 jupyter_rfb.egg-info/SOURCES.txt
 jupyter_rfb.egg-info/dependency_links.txt
 jupyter_rfb.egg-info/not-zip-safe
 jupyter_rfb.egg-info/requires.txt
 jupyter_rfb.egg-info/top_level.txt
 jupyter_rfb/labextension/package.json
-jupyter_rfb/labextension/static/493.cb43b5d572b2f6b10c8e.js
-jupyter_rfb/labextension/static/678.c748912b15ffb2656a49.js
-jupyter_rfb/labextension/static/remoteEntry.0d5a3b6ccc7e17c1ed27.js
+jupyter_rfb/labextension/static/420.d43f6d92aa7a9fb70aad.js
+jupyter_rfb/labextension/static/493.102804eff6eca0571ecf.js
+jupyter_rfb/labextension/static/remoteEntry.cf57a6d7f00412526ea4.js
 jupyter_rfb/labextension/static/style.js
 jupyter_rfb/labextension/static/third-party-licenses.json
 jupyter_rfb/nbextension/extension.js
 jupyter_rfb/nbextension/index.js
 tests/test_jpg.py
 tests/test_png.py
 tests/test_utils.py
```

### Comparing `jupyter_rfb-0.4.3/setup.py` & `jupyter_rfb-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/tests/test_jpg.py` & `jupyter_rfb-0.4.4/tests/test_jpg.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/tests/test_png.py` & `jupyter_rfb-0.4.4/tests/test_png.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/tests/test_utils.py` & `jupyter_rfb-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.3/tests/test_widget.py` & `jupyter_rfb-0.4.4/tests/test_widget.py`

 * *Files identical despite different names*

