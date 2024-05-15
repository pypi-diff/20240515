# Comparing `tmp/rofi-notion-2.0.4.tar.gz` & `tmp/rofi_notion-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rofi-notion-2.0.4.tar", last modified: Mon Sep 18 11:01:44 2023, max compression
+gzip compressed data, was "rofi_notion-2.1.0.tar", last modified: Wed May 15 14:04:51 2024, max compression
```

## Comparing `rofi-notion-2.0.4.tar` & `rofi_notion-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 11:01:44.854539 rofi-notion-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2023-09-18 11:01:44.850539 rofi-notion-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 11:01:44.850539 rofi-notion-2.0.4/rofi_notion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/rofi_notion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/rofi_notion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/rofi_notion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/rofi_notion/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/rofi_notion/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/rofi_notion/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2023-09-18 11:01:26.000000 rofi-notion-2.0.4/rofi_notion/transcoders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 11:01:44.850539 rofi-notion-2.0.4/rofi_notion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2023-09-18 11:01:44.000000 rofi-notion-2.0.4/rofi_notion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-09-18 11:01:44.000000 rofi-notion-2.0.4/rofi_notion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 11:01:44.000000 rofi-notion-2.0.4/rofi_notion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-09-18 11:01:44.000000 rofi-notion-2.0.4/rofi_notion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-09-18 11:01:44.000000 rofi-notion-2.0.4/rofi_notion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-18 11:01:44.000000 rofi-notion-2.0.4/rofi_notion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-18 11:01:44.854539 rofi-notion-2.0.4/setup.cfg
+drwxr-xr-x   0 mathix    (1000) mathix    (1000)        0 2024-05-15 14:04:51.282467 rofi_notion-2.1.0/
+-rw-r--r--   0 mathix    (1000) mathix    (1000)     1073 2023-03-15 13:17:56.000000 rofi_notion-2.1.0/LICENSE
+-rw-r--r--   0 mathix    (1000) mathix    (1000)     4396 2024-05-15 14:04:51.282467 rofi_notion-2.1.0/PKG-INFO
+-rw-r--r--   0 mathix    (1000) mathix    (1000)     2352 2024-05-15 13:55:15.000000 rofi_notion-2.1.0/README.md
+-rw-r--r--   0 mathix    (1000) mathix    (1000)      893 2024-05-15 13:54:01.000000 rofi_notion-2.1.0/pyproject.toml
+drwxr-xr-x   0 mathix    (1000) mathix    (1000)        0 2024-05-15 14:04:51.279134 rofi_notion-2.1.0/rofi_notion/
+-rw-r--r--   0 mathix    (1000) mathix    (1000)        0 2023-03-15 13:17:56.000000 rofi_notion-2.1.0/rofi_notion/__init__.py
+-rw-r--r--   0 mathix    (1000) mathix    (1000)     1326 2023-05-26 10:37:36.000000 rofi_notion-2.1.0/rofi_notion/__main__.py
+-rw-r--r--   0 mathix    (1000) mathix    (1000)     1159 2023-03-15 13:17:56.000000 rofi_notion-2.1.0/rofi_notion/config.py
+-rw-r--r--   0 mathix    (1000) mathix    (1000)     2786 2023-03-16 17:11:11.000000 rofi_notion-2.1.0/rofi_notion/main.py
+-rw-r--r--   0 mathix    (1000) mathix    (1000)     3020 2023-03-15 13:29:12.000000 rofi_notion-2.1.0/rofi_notion/manage.py
+-rw-r--r--   0 mathix    (1000) mathix    (1000)      191 2023-03-15 13:17:56.000000 rofi_notion-2.1.0/rofi_notion/settings.py
+-rw-r--r--   0 mathix    (1000) mathix    (1000)     3813 2024-05-15 13:45:50.000000 rofi_notion-2.1.0/rofi_notion/transcoders.py
+drwxr-xr-x   0 mathix    (1000) mathix    (1000)        0 2024-05-15 14:04:51.282467 rofi_notion-2.1.0/rofi_notion.egg-info/
+-rw-r--r--   0 mathix    (1000) mathix    (1000)     4396 2024-05-15 14:04:51.000000 rofi_notion-2.1.0/rofi_notion.egg-info/PKG-INFO
+-rw-r--r--   0 mathix    (1000) mathix    (1000)      407 2024-05-15 14:04:51.000000 rofi_notion-2.1.0/rofi_notion.egg-info/SOURCES.txt
+-rw-r--r--   0 mathix    (1000) mathix    (1000)        1 2024-05-15 14:04:51.000000 rofi_notion-2.1.0/rofi_notion.egg-info/dependency_links.txt
+-rw-r--r--   0 mathix    (1000) mathix    (1000)       58 2024-05-15 14:04:51.000000 rofi_notion-2.1.0/rofi_notion.egg-info/entry_points.txt
+-rw-r--r--   0 mathix    (1000) mathix    (1000)      104 2024-05-15 14:04:51.000000 rofi_notion-2.1.0/rofi_notion.egg-info/requires.txt
+-rw-r--r--   0 mathix    (1000) mathix    (1000)       12 2024-05-15 14:04:51.000000 rofi_notion-2.1.0/rofi_notion.egg-info/top_level.txt
+-rw-r--r--   0 mathix    (1000) mathix    (1000)       38 2024-05-15 14:04:51.282467 rofi_notion-2.1.0/setup.cfg
```

### Comparing `rofi-notion-2.0.4/LICENSE` & `rofi_notion-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rofi-notion-2.0.4/PKG-INFO` & `rofi_notion-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rofi-notion
-Version: 2.0.4
+Version: 2.1.0
 Summary: Quickly create new Notion pages for your databases with rofi as GUI
 Author-email: Arnaud Gissinger <agissing@student.42.fr>
 License: MIT License
         
         Copyright (c) 2022 Arnaud Gissinger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,25 +56,27 @@
 ## Requirements
 
 - Python >= 3.7
 - A Notion integration with read and write access to the desired databases.
 
 ## Installation
 
-### For archlinux users
+### For archlinux users (AUR package)
 
 ```bash
 yay -S rofi-notion-bin
 ```
+[AUR package details](https://aur.archlinux.org/packages/rofi-notion)
 
 ### For everyone else
 
 ```bash
 pip install rofi-notion
 ```
+[Pypi package details](https://pypi.org/project/rofi-notion/)
 
 ## Setup
 
 Check if the installation was successful
 ```bash
 rofi-notion -h
 ```
@@ -108,17 +110,24 @@
 bindsym $mod+Insert exec rofi-notion run $YOUR_DB_NAME
 ```
 
 ## Config
 
 Default config destination is `$XDG_CONFIG_HOME/rofi-notion` or `$HOME/.config/rofi-notion` if `$XDG_CONFIG_HOME` is not set.
 
-## Deployment
+## Development
 
-Do not forget to bump versions in `setup.py` and `PKGBUILD`.
+Use this command to run the CLI locally.
+```bash
+python3 stub.py
+```
+
+## Publish
+
+Do not forget to bump versions in `pyproject.toml` and `PKGBUILD`.
 
 ### PyPi
 
 ~~Run `make` to publish a new version.~~
 
 Git tag the new version and push it.
 Then publish the automatically created Draft release.
```

### Comparing `rofi-notion-2.0.4/README.md` & `rofi_notion-2.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 ## Requirements
 
 - Python >= 3.7
 - A Notion integration with read and write access to the desired databases.
 
 ## Installation
 
-### For archlinux users
+### For archlinux users (AUR package)
 
 ```bash
 yay -S rofi-notion-bin
 ```
+[AUR package details](https://aur.archlinux.org/packages/rofi-notion)
 
 ### For everyone else
 
 ```bash
 pip install rofi-notion
 ```
+[Pypi package details](https://pypi.org/project/rofi-notion/)
 
 ## Setup
 
 Check if the installation was successful
 ```bash
 rofi-notion -h
 ```
@@ -64,17 +66,24 @@
 bindsym $mod+Insert exec rofi-notion run $YOUR_DB_NAME
 ```
 
 ## Config
 
 Default config destination is `$XDG_CONFIG_HOME/rofi-notion` or `$HOME/.config/rofi-notion` if `$XDG_CONFIG_HOME` is not set.
 
-## Deployment
+## Development
 
-Do not forget to bump versions in `setup.py` and `PKGBUILD`.
+Use this command to run the CLI locally.
+```bash
+python3 stub.py
+```
+
+## Publish
+
+Do not forget to bump versions in `pyproject.toml` and `PKGBUILD`.
 
 ### PyPi
 
 ~~Run `make` to publish a new version.~~
 
 Git tag the new version and push it.
 Then publish the automatically created Draft release.
```

### Comparing `rofi-notion-2.0.4/pyproject.toml` & `rofi_notion-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 56"]
 
 [project]
 name = "rofi-notion"
-version = "2.0.4"
+version = "2.1.0"
 authors = [
     {name = "Arnaud Gissinger", email = "agissing@student.42.fr"},
 ]
 description = "Quickly create new Notion pages for your databases with rofi as GUI"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["notion.so", "notion", "rofi", "dmenu", "x11", "i3"]
```

### Comparing `rofi-notion-2.0.4/rofi_notion/__main__.py` & `rofi_notion-2.1.0/rofi_notion/__main__.py`

 * *Files identical despite different names*

### Comparing `rofi-notion-2.0.4/rofi_notion/config.py` & `rofi_notion-2.1.0/rofi_notion/config.py`

 * *Files identical despite different names*

### Comparing `rofi-notion-2.0.4/rofi_notion/main.py` & `rofi_notion-2.1.0/rofi_notion/main.py`

 * *Files identical despite different names*

### Comparing `rofi-notion-2.0.4/rofi_notion/manage.py` & `rofi_notion-2.1.0/rofi_notion/manage.py`

 * *Files identical despite different names*

### Comparing `rofi-notion-2.0.4/rofi_notion/transcoders.py` & `rofi_notion-2.1.0/rofi_notion/transcoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 from functools import partial
 from typing import Any
 from rofi import Rofi
+from sys import exit
 
 
 def required(transcoder: (...), *args):
     result = transcoder(*args)
     if not result:
         exit('This field is required.')
     return result
@@ -163,14 +164,15 @@
 
 transcoders = {
     'title': partial(required, text),
     'relation': relation,
     'rich_text': text,
     'number': number,
     'select': select,
+    'status': select,
     'multi_select': multi_select,
     'date': date,
     'people': people,
     'checkbox': checkbox,
     'url': url,
     'email': email,
     'phone_number': phone_number,
```

### Comparing `rofi-notion-2.0.4/rofi_notion.egg-info/PKG-INFO` & `rofi_notion-2.1.0/rofi_notion.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rofi-notion
-Version: 2.0.4
+Version: 2.1.0
 Summary: Quickly create new Notion pages for your databases with rofi as GUI
 Author-email: Arnaud Gissinger <agissing@student.42.fr>
 License: MIT License
         
         Copyright (c) 2022 Arnaud Gissinger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,25 +56,27 @@
 ## Requirements
 
 - Python >= 3.7
 - A Notion integration with read and write access to the desired databases.
 
 ## Installation
 
-### For archlinux users
+### For archlinux users (AUR package)
 
 ```bash
 yay -S rofi-notion-bin
 ```
+[AUR package details](https://aur.archlinux.org/packages/rofi-notion)
 
 ### For everyone else
 
 ```bash
 pip install rofi-notion
 ```
+[Pypi package details](https://pypi.org/project/rofi-notion/)
 
 ## Setup
 
 Check if the installation was successful
 ```bash
 rofi-notion -h
 ```
@@ -108,17 +110,24 @@
 bindsym $mod+Insert exec rofi-notion run $YOUR_DB_NAME
 ```
 
 ## Config
 
 Default config destination is `$XDG_CONFIG_HOME/rofi-notion` or `$HOME/.config/rofi-notion` if `$XDG_CONFIG_HOME` is not set.
 
-## Deployment
+## Development
 
-Do not forget to bump versions in `setup.py` and `PKGBUILD`.
+Use this command to run the CLI locally.
+```bash
+python3 stub.py
+```
+
+## Publish
+
+Do not forget to bump versions in `pyproject.toml` and `PKGBUILD`.
 
 ### PyPi
 
 ~~Run `make` to publish a new version.~~
 
 Git tag the new version and push it.
 Then publish the automatically created Draft release.
```

