# Comparing `tmp/pysdbots-3.0.tar.gz` & `tmp/pysdbots-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdbots-3.0.tar", last modified: Wed May 15 12:22:13 2024, max compression
+gzip compressed data, was "pysdbots-3.1.tar", last modified: Wed May 15 17:44:11 2024, max compression
```

## Comparing `pysdbots-3.0.tar` & `pysdbots-3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:22:13.296184 pysdbots-3.0/
--rw-rw-rw-   0        0        0     1093 2024-05-10 17:21:31.000000 pysdbots-3.0/LICENSE
--rw-rw-rw-   0        0        0     2767 2024-05-15 12:22:13.293185 pysdbots-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1494 2024-05-10 17:21:31.000000 pysdbots-3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 12:22:13.190047 pysdbots-3.0/pysdbots/
--rw-rw-rw-   0        0        0      260 2024-05-11 17:35:47.000000 pysdbots-3.0/pysdbots/__init__.py
--rw-rw-rw-   0        0        0       19 2024-05-11 17:34:40.000000 pysdbots-3.0/pysdbots/__version__.py
--rw-rw-rw-   0        0        0     9022 2024-05-11 18:17:29.000000 pysdbots-3.0/pysdbots/pysdbots.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:22:13.291353 pysdbots-3.0/pysdbots.egg-info/
--rw-rw-rw-   0        0        0     2767 2024-05-15 12:22:12.000000 pysdbots-3.0/pysdbots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-15 12:22:13.000000 pysdbots-3.0/pysdbots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:22:12.000000 pysdbots-3.0/pysdbots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-15 12:22:12.000000 pysdbots-3.0/pysdbots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 12:22:12.000000 pysdbots-3.0/pysdbots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 12:22:13.296184 pysdbots-3.0/setup.cfg
--rw-rw-rw-   0        0        0     1882 2024-05-15 12:14:20.000000 pysdbots-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:44:11.881738 pysdbots-3.1/
+-rw-rw-rw-   0        0        0     1093 2024-05-10 17:21:31.000000 pysdbots-3.1/LICENSE
+-rw-rw-rw-   0        0        0     2767 2024-05-15 17:44:11.878739 pysdbots-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1494 2024-05-10 17:21:31.000000 pysdbots-3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 17:44:11.557738 pysdbots-3.1/pysdbots/
+-rw-rw-rw-   0        0        0      260 2024-05-11 17:35:47.000000 pysdbots-3.1/pysdbots/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-05-15 17:36:45.000000 pysdbots-3.1/pysdbots/__version__.py
+-rw-rw-rw-   0        0        0     9024 2024-05-15 17:36:28.000000 pysdbots-3.1/pysdbots/pysdbots.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:44:11.807738 pysdbots-3.1/pysdbots.egg-info/
+-rw-rw-rw-   0        0        0     2767 2024-05-15 17:44:09.000000 pysdbots-3.1/pysdbots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-15 17:44:09.000000 pysdbots-3.1/pysdbots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:44:09.000000 pysdbots-3.1/pysdbots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 17:44:09.000000 pysdbots-3.1/pysdbots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 17:44:09.000000 pysdbots-3.1/pysdbots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 17:44:11.881738 pysdbots-3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1882 2024-05-15 12:14:20.000000 pysdbots-3.1/setup.py
```

### Comparing `pysdbots-3.0/LICENSE` & `pysdbots-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysdbots-3.0/PKG-INFO` & `pysdbots-3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdbots
-Version: 3.0
+Version: 3.1
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/Damantha126/pysdbots
 Author: DamanthaJasinghe
 Author-email: damanthaja@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/Damantha126/pysdbots/issues
 Project-URL: Community, https://t.me/SDBOTs_inifinity
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pysdbots Version: 3.0 Summary: A Project Made To
+Metadata-Version: 2.1 Name: pysdbots Version: 3.1 Summary: A Project Made To
 Centralize Various APIs ð No Authorization Needed :) Home-page: https://
 github.com/Damantha126/pysdbots Author: DamanthaJasinghe Author-email:
 damanthaja@gmail.com License: MIT Project-URL: Tracker, https://github.com/
 Damantha126/pysdbots/issues Project-URL: Community, https://t.me/
 SDBOTs_inifinity Project-URL: Source, https://github.com/Damantha126/pysdbots
 Project-URL: Documentation, https://docs.sdbots.tech Keywords: sdbots,python-
 pakage,sd-api,api,damanthaja,mritzme,damantha126,pysdbots,jasinghe,damantha-
```

### Comparing `pysdbots-3.0/README.md` & `pysdbots-3.1/README.md`

 * *Files identical despite different names*

### Comparing `pysdbots-3.0/pysdbots/pysdbots.py` & `pysdbots-3.1/pysdbots/pysdbots.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests
 from datetime import date
 from .__version__ import __version__
 
 # HTTP request headers
 headers = {
     'Content-Type': 'application/json',
-    'User-Agent': 'pysdbots'
+    'Request-Type': 'pysdbots'
 }
 
 # URL for fetching configurations
 CONFIGS="https://gist.githubusercontent.com/Damantha126/b18e14d0d04f25327773e0ab54cc090a/raw/config.json"
 # Fetch configurations from the URL
 req = requests.get(CONFIGS).json()
```

### Comparing `pysdbots-3.0/pysdbots.egg-info/PKG-INFO` & `pysdbots-3.1/pysdbots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdbots
-Version: 3.0
+Version: 3.1
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/Damantha126/pysdbots
 Author: DamanthaJasinghe
 Author-email: damanthaja@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/Damantha126/pysdbots/issues
 Project-URL: Community, https://t.me/SDBOTs_inifinity
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pysdbots Version: 3.0 Summary: A Project Made To
+Metadata-Version: 2.1 Name: pysdbots Version: 3.1 Summary: A Project Made To
 Centralize Various APIs ð No Authorization Needed :) Home-page: https://
 github.com/Damantha126/pysdbots Author: DamanthaJasinghe Author-email:
 damanthaja@gmail.com License: MIT Project-URL: Tracker, https://github.com/
 Damantha126/pysdbots/issues Project-URL: Community, https://t.me/
 SDBOTs_inifinity Project-URL: Source, https://github.com/Damantha126/pysdbots
 Project-URL: Documentation, https://docs.sdbots.tech Keywords: sdbots,python-
 pakage,sd-api,api,damanthaja,mritzme,damantha126,pysdbots,jasinghe,damantha-
```

### Comparing `pysdbots-3.0/setup.py` & `pysdbots-3.1/setup.py`

 * *Files identical despite different names*

