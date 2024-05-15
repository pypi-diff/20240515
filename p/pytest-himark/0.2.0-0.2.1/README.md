# Comparing `tmp/pytest_himark-0.2.0.tar.gz` & `tmp/pytest_himark-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_himark-0.2.0.tar", last modified: Fri May 10 05:40:42 2024, max compression
+gzip compressed data, was "pytest_himark-0.2.1.tar", last modified: Wed May 15 14:19:41 2024, max compression
```

## Comparing `pytest_himark-0.2.0.tar` & `pytest_himark-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.034252 pytest_himark-0.2.0/
--rw-rw-rw-   0        0        0     1111 2024-04-07 10:46:35.000000 pytest_himark-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     8904 2024-05-10 05:40:42.033251 pytest_himark-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6370 2024-05-10 05:40:28.000000 pytest_himark-0.2.0/README.rst
--rw-rw-rw-   0        0        0     3417 2024-05-10 05:39:26.000000 pytest_himark-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 05:40:42.034252 pytest_himark-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.022357 pytest_himark-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.027504 pytest_himark-0.2.0/src/pytest_himark/
--rw-rw-rw-   0        0        0        0 2024-04-07 10:46:35.000000 pytest_himark-0.2.0/src/pytest_himark/__init__.py
--rw-rw-rw-   0        0        0     3032 2024-05-09 19:35:33.000000 pytest_himark-0.2.0/src/pytest_himark/plugin.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.033251 pytest_himark-0.2.0/src/pytest_himark.egg-info/
--rw-rw-rw-   0        0        0     8904 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.032251 pytest_himark-0.2.0/tests/
--rw-rw-rw-   0        0        0     6593 2024-05-09 19:35:33.000000 pytest_himark-0.2.0/tests/test_himark.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:19:41.155824 pytest_himark-0.2.1/
+-rw-rw-rw-   0        0        0     1111 2024-04-07 10:46:35.000000 pytest_himark-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     9027 2024-05-15 14:19:41.155824 pytest_himark-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6493 2024-05-15 14:18:26.000000 pytest_himark-0.2.1/README.rst
+-rw-rw-rw-   0        0        0     4651 2024-05-15 14:18:53.000000 pytest_himark-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:19:41.155824 pytest_himark-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 14:19:41.136049 pytest_himark-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 14:19:41.141050 pytest_himark-0.2.1/src/pytest_himark/
+-rw-rw-rw-   0        0        0        0 2024-04-07 10:46:35.000000 pytest_himark-0.2.1/src/pytest_himark/__init__.py
+-rw-rw-rw-   0        0        0     3354 2024-05-15 14:18:26.000000 pytest_himark-0.2.1/src/pytest_himark/plugin.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:19:41.154823 pytest_himark-0.2.1/src/pytest_himark.egg-info/
+-rw-rw-rw-   0        0        0     9027 2024-05-15 14:19:41.000000 pytest_himark-0.2.1/src/pytest_himark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-05-15 14:19:41.000000 pytest_himark-0.2.1/src/pytest_himark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:19:41.000000 pytest_himark-0.2.1/src/pytest_himark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-15 14:19:41.000000 pytest_himark-0.2.1/src/pytest_himark.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 14:19:41.000000 pytest_himark-0.2.1/src/pytest_himark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 14:19:41.000000 pytest_himark-0.2.1/src/pytest_himark.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 14:19:41.153628 pytest_himark-0.2.1/tests/
+-rw-rw-rw-   0        0        0     6593 2024-05-09 19:35:33.000000 pytest_himark-0.2.1/tests/test_himark.py
```

### Comparing `pytest_himark-0.2.0/LICENSE` & `pytest_himark-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_himark-0.2.0/PKG-INFO` & `pytest_himark-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-himark
-Version: 0.2.0
+Version: 0.2.1
 Summary: This plugin aims to create markers automatically based on a json configuration.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: 
         The MIT License (MIT)
         
         Copyright (c) 2024 Rodolphe Mete Soyding
@@ -259,14 +259,16 @@
     @pytest.mark.marker2
     def test_mytest():
         assert True
 ..
 
 This test is marked with *marker1* which is defined in the configuration, but also with *marker2* which is not. Therefore, despite being initially collected by pytest, this plugin will remove it from the selection.
 
+Note that any empty string as marker will be ignored by the plugin, and any leading or trailing spaces will be removed.
+
 Contributing
 ------------
 Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
 License
 -------
```

### Comparing `pytest_himark-0.2.0/README.rst` & `pytest_himark-0.2.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -209,14 +209,16 @@
     @pytest.mark.marker2
     def test_mytest():
         assert True
 ..
 
 This test is marked with *marker1* which is defined in the configuration, but also with *marker2* which is not. Therefore, despite being initially collected by pytest, this plugin will remove it from the selection.
 
+Note that any empty string as marker will be ignored by the plugin, and any leading or trailing spaces will be removed.
+
 Contributing
 ------------
 Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
 License
 -------
```

### Comparing `pytest_himark-0.2.0/src/pytest_himark/plugin.py` & `pytest_himark-0.2.1/src/pytest_himark/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,32 +58,37 @@
             config = json.load(file)
             devices = config.get("devices", list())
             markers = config.get("markers", list())
 
         # lists the enabled devices and turn them into markers
         for device in devices:
             name = device.get("name", None)
-            if device.get("used") is True:
-                markers_enabled.add(name)
+            if device.get("used") is True and name.strip() != "":
+                markers_enabled.add(name.strip())
                 # if device is enabled, check its do/di/ai/ao lists existence
                 for x in device.get("do", list()):
-                    markers_enabled.add(x)
+                    if x.strip() != "":
+                        markers_enabled.add(x.strip())
                 for x in device.get("di", list()):
-                    markers_enabled.add(x)
+                    if x.strip() != "":
+                        markers_enabled.add(x.strip())
                 for x in device.get("ai", list()):
-                    markers_enabled.add(x)
+                    if x.strip() != "":
+                        markers_enabled.add(x.strip())
                 for x in device.get("ao", list()):
-                    markers_enabled.add(x)
+                    if x.strip() != "":
+                        markers_enabled.add(x.strip())
                 # make a marker for 'type' key if it exists
-                if device.get("type", None) is not None:
-                    markers_enabled.add(device.get("type"))
+                type = device.get("type", None)
+                if type is not None and type.strip() != "":
+                    markers_enabled.add(type.strip())
 
         # lists the enabled markers
         for marker in markers:
-            if markers.get(marker) is True:
-                markers_enabled.add(marker)
+            if marker.strip() != "" and markers.get(marker) is True:
+                markers_enabled.add(marker.strip())
 
     markers_enabled = set(filter(None, markers_enabled))
     markers_list = markers_enabled
     # make an OR of the previously listed enabled markers and pass it with the -m option to the command line
     if len(markers_enabled) > 0:
         args[:] = (["-m", f'({" or ".join(markers_enabled)})'] + args)
```

### Comparing `pytest_himark-0.2.0/src/pytest_himark.egg-info/PKG-INFO` & `pytest_himark-0.2.1/src/pytest_himark.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-himark
-Version: 0.2.0
+Version: 0.2.1
 Summary: This plugin aims to create markers automatically based on a json configuration.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: 
         The MIT License (MIT)
         
         Copyright (c) 2024 Rodolphe Mete Soyding
@@ -259,14 +259,16 @@
     @pytest.mark.marker2
     def test_mytest():
         assert True
 ..
 
 This test is marked with *marker1* which is defined in the configuration, but also with *marker2* which is not. Therefore, despite being initially collected by pytest, this plugin will remove it from the selection.
 
+Note that any empty string as marker will be ignored by the plugin, and any leading or trailing spaces will be removed.
+
 Contributing
 ------------
 Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
 License
 -------
```

### Comparing `pytest_himark-0.2.0/tests/test_himark.py` & `pytest_himark-0.2.1/tests/test_himark.py`

 * *Files identical despite different names*

