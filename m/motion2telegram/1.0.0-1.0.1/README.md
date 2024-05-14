# Comparing `tmp/motion2telegram-1.0.0.tar.gz` & `tmp/motion2telegram-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion2telegram-1.0.0.tar", last modified: Tue May 14 11:44:49 2024, max compression
+gzip compressed data, was "motion2telegram-1.0.1.tar", last modified: Tue May 14 22:40:08 2024, max compression
```

## Comparing `motion2telegram-1.0.0.tar` & `motion2telegram-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-14 11:44:49.408109 motion2telegram-1.0.0/
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     1062 2024-05-12 22:06:34.000000 motion2telegram-1.0.0/LICENSE
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      148 2024-05-14 10:52:39.000000 motion2telegram-1.0.0/MANIFEST.in
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     3734 2024-05-14 11:44:49.398109 motion2telegram-1.0.0/PKG-INFO
--rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     2604 2024-05-14 10:52:39.000000 motion2telegram-1.0.0/README.md
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     1865 2024-05-14 11:39:00.000000 motion2telegram-1.0.0/pyproject.toml
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)       38 2024-05-14 11:44:49.408109 motion2telegram-1.0.0/setup.cfg
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      529 2024-05-12 22:06:34.000000 motion2telegram-1.0.0/setup.py
-drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-14 11:44:49.218106 motion2telegram-1.0.0/src/
-drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-14 11:44:49.298107 motion2telegram-1.0.0/src/motion2telegram/
--rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)       84 2024-05-12 23:03:28.000000 motion2telegram-1.0.0/src/motion2telegram/__init__.py
--rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     1261 2024-05-14 10:52:39.000000 motion2telegram-1.0.0/src/motion2telegram/cli.py
--rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     1905 2024-05-14 10:52:39.000000 motion2telegram-1.0.0/src/motion2telegram/configure.py
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      293 2024-05-14 10:52:39.000000 motion2telegram-1.0.0/src/motion2telegram/send.py
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     5399 2024-05-14 10:52:39.000000 motion2telegram-1.0.0/src/motion2telegram/template.motion.conf
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)       37 2024-05-14 10:52:39.000000 motion2telegram-1.0.0/src/motion2telegram/template.motion.env
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      225 2024-05-14 10:52:39.000000 motion2telegram-1.0.0/src/motion2telegram/template.motion.service
-drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-14 11:44:49.348108 motion2telegram-1.0.0/src/motion2telegram.egg-info/
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     3734 2024-05-14 11:44:48.000000 motion2telegram-1.0.0/src/motion2telegram.egg-info/PKG-INFO
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      558 2024-05-14 11:44:49.000000 motion2telegram-1.0.0/src/motion2telegram.egg-info/SOURCES.txt
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)        1 2024-05-14 11:44:48.000000 motion2telegram-1.0.0/src/motion2telegram.egg-info/dependency_links.txt
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)       60 2024-05-14 11:44:48.000000 motion2telegram-1.0.0/src/motion2telegram.egg-info/entry_points.txt
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      172 2024-05-14 11:44:48.000000 motion2telegram-1.0.0/src/motion2telegram.egg-info/requires.txt
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)       16 2024-05-14 11:44:48.000000 motion2telegram-1.0.0/src/motion2telegram.egg-info/top_level.txt
+drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-14 22:40:08.820083 motion2telegram-1.0.1/
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     1062 2024-05-12 22:06:34.000000 motion2telegram-1.0.1/LICENSE
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      148 2024-05-14 10:52:39.000000 motion2telegram-1.0.1/MANIFEST.in
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     3614 2024-05-14 22:40:08.810083 motion2telegram-1.0.1/PKG-INFO
+-rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     2484 2024-05-14 22:31:49.000000 motion2telegram-1.0.1/README.md
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     1866 2024-05-14 22:33:58.000000 motion2telegram-1.0.1/pyproject.toml
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)       38 2024-05-14 22:40:08.830083 motion2telegram-1.0.1/setup.cfg
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      529 2024-05-12 22:06:34.000000 motion2telegram-1.0.1/setup.py
+drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-14 22:40:08.630083 motion2telegram-1.0.1/src/
+drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-14 22:40:08.720083 motion2telegram-1.0.1/src/motion2telegram/
+-rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)       84 2024-05-14 22:33:58.000000 motion2telegram-1.0.1/src/motion2telegram/__init__.py
+-rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     1261 2024-05-14 10:52:39.000000 motion2telegram-1.0.1/src/motion2telegram/cli.py
+-rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     2272 2024-05-14 22:31:49.000000 motion2telegram-1.0.1/src/motion2telegram/configure.py
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      293 2024-05-14 10:52:39.000000 motion2telegram-1.0.1/src/motion2telegram/send.py
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     5399 2024-05-14 10:52:39.000000 motion2telegram-1.0.1/src/motion2telegram/template.motion.conf
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)       37 2024-05-14 10:52:39.000000 motion2telegram-1.0.1/src/motion2telegram/template.motion.env
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      225 2024-05-14 10:52:39.000000 motion2telegram-1.0.1/src/motion2telegram/template.motion.service
+drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-14 22:40:08.760083 motion2telegram-1.0.1/src/motion2telegram.egg-info/
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     3614 2024-05-14 22:40:08.000000 motion2telegram-1.0.1/src/motion2telegram.egg-info/PKG-INFO
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      558 2024-05-14 22:40:08.000000 motion2telegram-1.0.1/src/motion2telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)        1 2024-05-14 22:40:08.000000 motion2telegram-1.0.1/src/motion2telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)       60 2024-05-14 22:40:08.000000 motion2telegram-1.0.1/src/motion2telegram.egg-info/entry_points.txt
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      172 2024-05-14 22:40:08.000000 motion2telegram-1.0.1/src/motion2telegram.egg-info/requires.txt
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)       16 2024-05-14 22:40:08.000000 motion2telegram-1.0.1/src/motion2telegram.egg-info/top_level.txt
```

### Comparing `motion2telegram-1.0.0/LICENSE` & `motion2telegram-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `motion2telegram-1.0.0/PKG-INFO` & `motion2telegram-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion2telegram
-Version: 1.0.0
+Version: 1.0.1
 Summary: Notify a Telegram user when the motion service detects motion
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/motion2telegram
 Project-URL: Bug Tracker, https://github.com/p4irin/motion2telegram/issues
 Keywords: motion,python,telegram,motion-detection,webcam,raspberry-pi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -65,18 +65,14 @@
 
 ## Configuration
 
 Create a motion.env file and change it's access permissions. This file is used by the motion service to retrieve the Telegram bot token and the recipient's chat id.
 
 ```bash
 (venv) $ motion2telegram --init
-# Change permissions
-(venv) $ chmod u+rw-x motion.env
-(venv) $ chmod g+r-wx motion.env)
-(venv) $ chmod o-rwx motion.env
 ```
 Specify your Telegram chat id and bot token in the file motion.env
 
 ```bash
 # motion.env
 TELEGRAM_BOT_TOKEN=
 TELEGRAM_CHAT_ID=
```

### Comparing `motion2telegram-1.0.0/README.md` & `motion2telegram-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,18 +38,14 @@
 
 ## Configuration
 
 Create a motion.env file and change it's access permissions. This file is used by the motion service to retrieve the Telegram bot token and the recipient's chat id.
 
 ```bash
 (venv) $ motion2telegram --init
-# Change permissions
-(venv) $ chmod u+rw-x motion.env
-(venv) $ chmod g+r-wx motion.env)
-(venv) $ chmod o-rwx motion.env
 ```
 Specify your Telegram chat id and bot token in the file motion.env
 
 ```bash
 # motion.env
 TELEGRAM_BOT_TOKEN=
 TELEGRAM_CHAT_ID=
```

### Comparing `motion2telegram-1.0.0/pyproject.toml` & `motion2telegram-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motion2telegram"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="p4irin", email="p4irin.github.io@gmail.com" },
 ]
 description = "Notify a Telegram user when the motion service detects motion"
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -56,15 +56,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
 
@@ -82,7 +82,8 @@
 
 
 [tool.mypy]
 
 [[tool.mypy.overrides]]
 module = "telegram_notifier_bot"
 ignore_missing_imports = true
+
```

### Comparing `motion2telegram-1.0.0/setup.py` & `motion2telegram-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `motion2telegram-1.0.0/src/motion2telegram/cli.py` & `motion2telegram-1.0.1/src/motion2telegram/cli.py`

 * *Files identical despite different names*

### Comparing `motion2telegram-1.0.0/src/motion2telegram/template.motion.conf` & `motion2telegram-1.0.1/src/motion2telegram/template.motion.conf`

 * *Files identical despite different names*

### Comparing `motion2telegram-1.0.0/src/motion2telegram.egg-info/PKG-INFO` & `motion2telegram-1.0.1/src/motion2telegram.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion2telegram
-Version: 1.0.0
+Version: 1.0.1
 Summary: Notify a Telegram user when the motion service detects motion
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/motion2telegram
 Project-URL: Bug Tracker, https://github.com/p4irin/motion2telegram/issues
 Keywords: motion,python,telegram,motion-detection,webcam,raspberry-pi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -65,18 +65,14 @@
 
 ## Configuration
 
 Create a motion.env file and change it's access permissions. This file is used by the motion service to retrieve the Telegram bot token and the recipient's chat id.
 
 ```bash
 (venv) $ motion2telegram --init
-# Change permissions
-(venv) $ chmod u+rw-x motion.env
-(venv) $ chmod g+r-wx motion.env)
-(venv) $ chmod o-rwx motion.env
 ```
 Specify your Telegram chat id and bot token in the file motion.env
 
 ```bash
 # motion.env
 TELEGRAM_BOT_TOKEN=
 TELEGRAM_CHAT_ID=
```

### Comparing `motion2telegram-1.0.0/src/motion2telegram.egg-info/SOURCES.txt` & `motion2telegram-1.0.1/src/motion2telegram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

