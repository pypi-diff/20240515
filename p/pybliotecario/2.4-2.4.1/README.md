# Comparing `tmp/pybliotecario-2.4.tar.gz` & `tmp/pybliotecario-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybliotecario-2.4.tar", last modified: Wed Nov 15 12:51:41 2023, max compression
+gzip compressed data, was "pybliotecario-2.4.1.tar", last modified: Wed May 15 10:12:47 2024, max compression
```

## Comparing `pybliotecario-2.4.tar` & `pybliotecario-2.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 jumax9     (501) staff       (20)        0 2023-11-15 12:51:41.980767 pybliotecario-2.4/
--rw-r--r--   0 jumax9     (501) staff       (20)     1169 2023-11-15 12:51:41.980528 pybliotecario-2.4/PKG-INFO
--rw-r--r--   0 jumax9     (501) staff       (20)     1356 2023-11-15 12:51:27.000000 pybliotecario-2.4/pyproject.toml
--rw-r--r--   0 jumax9     (501) staff       (20)       38 2023-11-15 12:51:41.980808 pybliotecario-2.4/setup.cfg
-drwxr-xr-x   0 jumax9     (501) staff       (20)        0 2023-11-15 12:51:41.969373 pybliotecario-2.4/src/
-drwxr-xr-x   0 jumax9     (501) staff       (20)        0 2023-11-15 12:51:41.971487 pybliotecario-2.4/src/pybliotecario/
--rw-r--r--   0 jumax9     (501) staff       (20)       20 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/__init__.py
--rw-r--r--   0 jumax9     (501) staff       (20)    10658 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/argument_parser.py
-drwxr-xr-x   0 jumax9     (501) staff       (20)        0 2023-11-15 12:51:41.973756 pybliotecario-2.4/src/pybliotecario/backend/
--rw-r--r--   0 jumax9     (501) staff       (20)      115 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/backend/__init__.py
--rw-r--r--   0 jumax9     (501) staff       (20)     3847 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/backend/backend_test.py
--rw-r--r--   0 jumax9     (501) staff       (20)     6233 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/backend/basic_backend.py
--rw-r--r--   0 jumax9     (501) staff       (20)     6867 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/backend/facebook_util.py
--rw-r--r--   0 jumax9     (501) staff       (20)     9827 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/backend/telegram_util.py
-drwxr-xr-x   0 jumax9     (501) staff       (20)        0 2023-11-15 12:51:41.977804 pybliotecario-2.4/src/pybliotecario/components/
--rw-r--r--   0 jumax9     (501) staff       (20)       32 2020-09-29 20:39:09.000000 pybliotecario-2.4/src/pybliotecario/components/__init__.py
--rw-r--r--   0 jumax9     (501) staff       (20)     8480 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/arxiv_mod.py
--rw-r--r--   0 jumax9     (501) staff       (20)     6274 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/component_core.py
--rw-r--r--   0 jumax9     (501) staff       (20)     3298 2023-11-15 11:54:34.000000 pybliotecario-2.4/src/pybliotecario/components/dnd.py
--rw-r--r--   0 jumax9     (501) staff       (20)     3413 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/github_component.py
--rw-r--r--   0 jumax9     (501) staff       (20)     1406 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/ip_lookup.py
--rw-r--r--   0 jumax9     (501) staff       (20)     4374 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/photocol.py
--rw-r--r--   0 jumax9     (501) staff       (20)     3402 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/pid.py
--rw-r--r--   0 jumax9     (501) staff       (20)     3138 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/reactions.py
--rw-r--r--   0 jumax9     (501) staff       (20)     3283 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/repositories.py
--rw-r--r--   0 jumax9     (501) staff       (20)     6354 2023-11-15 11:54:34.000000 pybliotecario-2.4/src/pybliotecario/components/scripts.py
--rw-r--r--   0 jumax9     (501) staff       (20)     4229 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/stocks.py
--rw-r--r--   0 jumax9     (501) staff       (20)     1412 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/system.py
--rw-r--r--   0 jumax9     (501) staff       (20)     2879 2023-11-01 21:03:38.000000 pybliotecario-2.4/src/pybliotecario/components/todo_management.py
--rw-r--r--   0 jumax9     (501) staff       (20)     4293 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/twitter.py
--rw-r--r--   0 jumax9     (501) staff       (20)     4917 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/weather.py
--rw-r--r--   0 jumax9     (501) staff       (20)     4880 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/components/wiki.py
--rw-r--r--   0 jumax9     (501) staff       (20)     5278 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/core_loop.py
--rw-r--r--   0 jumax9     (501) staff       (20)     1729 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/customconf.py
--rw-r--r--   0 jumax9     (501) staff       (20)     3586 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/on_cmd_message.py
--rw-r--r--   0 jumax9     (501) staff       (20)     2609 2023-09-11 20:40:23.000000 pybliotecario-2.4/src/pybliotecario/on_cmdline.py
--rwxr-xr-x   0 jumax9     (501) staff       (20)     5145 2023-11-05 21:21:56.000000 pybliotecario-2.4/src/pybliotecario/pybliotecario.py
-drwxr-xr-x   0 jumax9     (501) staff       (20)        0 2023-11-15 12:51:41.972486 pybliotecario-2.4/src/pybliotecario.egg-info/
--rw-r--r--   0 jumax9     (501) staff       (20)     1169 2023-11-15 12:51:41.000000 pybliotecario-2.4/src/pybliotecario.egg-info/PKG-INFO
--rw-r--r--   0 jumax9     (501) staff       (20)     1547 2023-11-15 12:51:41.000000 pybliotecario-2.4/src/pybliotecario.egg-info/SOURCES.txt
--rw-r--r--   0 jumax9     (501) staff       (20)        1 2023-11-15 12:51:41.000000 pybliotecario-2.4/src/pybliotecario.egg-info/dependency_links.txt
--rw-r--r--   0 jumax9     (501) staff       (20)       67 2023-11-15 12:51:41.000000 pybliotecario-2.4/src/pybliotecario.egg-info/entry_points.txt
--rw-r--r--   0 jumax9     (501) staff       (20)      256 2023-11-15 12:51:41.000000 pybliotecario-2.4/src/pybliotecario.egg-info/requires.txt
--rw-r--r--   0 jumax9     (501) staff       (20)       14 2023-11-15 12:51:41.000000 pybliotecario-2.4/src/pybliotecario.egg-info/top_level.txt
-drwxr-xr-x   0 jumax9     (501) staff       (20)        0 2023-11-15 12:51:41.979591 pybliotecario-2.4/tests/
--rw-r--r--   0 jumax9     (501) staff       (20)     2155 2023-10-29 20:00:11.000000 pybliotecario-2.4/tests/test_backend_test.py
--rw-r--r--   0 jumax9     (501) staff       (20)     1118 2023-10-29 20:00:11.000000 pybliotecario-2.4/tests/test_component_ip_lookup.py
--rw-r--r--   0 jumax9     (501) staff       (20)     1307 2023-10-29 20:00:11.000000 pybliotecario-2.4/tests/test_dnd.py
--rw-r--r--   0 jumax9     (501) staff       (20)     2053 2023-10-29 20:00:11.000000 pybliotecario-2.4/tests/test_pid.py
--rw-r--r--   0 jumax9     (501) staff       (20)      944 2023-10-29 20:00:11.000000 pybliotecario-2.4/tests/test_stocks.py
--rw-r--r--   0 jumax9     (501) staff       (20)      782 2023-10-29 20:00:11.000000 pybliotecario-2.4/tests/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:12:47.589836 pybliotecario-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-05-15 10:12:47.589836 pybliotecario-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:12:47.589836 pybliotecario-2.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:12:47.581836 pybliotecario-2.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:12:47.581836 pybliotecario-2.4.1/src/pybliotecario/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/argument_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:12:47.585836 pybliotecario-2.4.1/src/pybliotecario/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/backend/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/backend/basic_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/backend/facebook_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/backend/telegram_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:12:47.585836 pybliotecario-2.4.1/src/pybliotecario/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/arxiv_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/component_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/dnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/github_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/ip_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/photocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/components/wiki.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/core_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/customconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/on_cmd_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/on_cmdline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5145 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/src/pybliotecario/pybliotecario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:12:47.589836 pybliotecario-2.4.1/src/pybliotecario.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-05-15 10:12:47.000000 pybliotecario-2.4.1/src/pybliotecario.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-15 10:12:47.000000 pybliotecario-2.4.1/src/pybliotecario.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:12:47.000000 pybliotecario-2.4.1/src/pybliotecario.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 10:12:47.000000 pybliotecario-2.4.1/src/pybliotecario.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-15 10:12:47.000000 pybliotecario-2.4.1/src/pybliotecario.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 10:12:47.000000 pybliotecario-2.4.1/src/pybliotecario.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:12:47.589836 pybliotecario-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/tests/test_backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/tests/test_component_ip_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/tests/test_dnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/tests/test_pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/tests/test_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-15 10:12:36.000000 pybliotecario-2.4.1/tests/test_system.py
```

### Comparing `pybliotecario-2.4/pyproject.toml` & `pybliotecario-2.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [project]
 name = "pybliotecario"
 dynamic = ["version"]
 authors = [
     { name = "juacrumar", email = "juacrumar@lairen.eu" }
 ]
 description = "Personal telegram bot to interact between your Telegram account and your computer"
-readme = "README"
+readme = "readme.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 license = {text = "GPLv3"}
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `pybliotecario-2.4/src/pybliotecario/argument_parser.py` & `pybliotecario-2.4.1/src/pybliotecario/argument_parser.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/backend/backend_test.py` & `pybliotecario-2.4.1/src/pybliotecario/backend/backend_test.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/backend/basic_backend.py` & `pybliotecario-2.4.1/src/pybliotecario/backend/basic_backend.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/backend/facebook_util.py` & `pybliotecario-2.4.1/src/pybliotecario/backend/facebook_util.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/backend/telegram_util.py` & `pybliotecario-2.4.1/src/pybliotecario/backend/telegram_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             self.send_message(text, chat, **kwargs)
 
     def send_image(self, img_path, chat):
         """Send an image to a given chat"""
         data = {"chat_id": chat}
         with open(img_path, "rb") as img:
             files = {"photo": ("picture.jpg", img)}  # Here, the "rb" thing
-        blabla = requests.post(self.send_img, data=data, files=files)
+            blabla = requests.post(self.send_img, data=data, files=files)
         log_request(blabla.status_code, blabla.reason, blabla.content)
 
     def send_file(self, filepath, chat):
         data = {"chat_id": chat}
         files = {"document": (filepath.name, filepath.open("rb"))}
         blabla = requests.post(self.send_doc, data=data, files=files)
         log_request(blabla.status_code, blabla.reason, blabla.content)
```

### Comparing `pybliotecario-2.4/src/pybliotecario/components/arxiv_mod.py` & `pybliotecario-2.4.1/src/pybliotecario/components/arxiv_mod.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/component_core.py` & `pybliotecario-2.4.1/src/pybliotecario/components/component_core.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/dnd.py` & `pybliotecario-2.4.1/src/pybliotecario/components/dnd.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/github_component.py` & `pybliotecario-2.4.1/src/pybliotecario/components/github_component.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/ip_lookup.py` & `pybliotecario-2.4.1/src/pybliotecario/components/ip_lookup.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/photocol.py` & `pybliotecario-2.4.1/src/pybliotecario/components/photocol.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/pid.py` & `pybliotecario-2.4.1/src/pybliotecario/components/pid.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/reactions.py` & `pybliotecario-2.4.1/src/pybliotecario/components/reactions.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/repositories.py` & `pybliotecario-2.4.1/src/pybliotecario/components/repositories.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/scripts.py` & `pybliotecario-2.4.1/src/pybliotecario/components/scripts.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/stocks.py` & `pybliotecario-2.4.1/src/pybliotecario/components/stocks.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/system.py` & `pybliotecario-2.4.1/src/pybliotecario/components/system.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/twitter.py` & `pybliotecario-2.4.1/src/pybliotecario/components/twitter.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/weather.py` & `pybliotecario-2.4.1/src/pybliotecario/components/weather.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/components/wiki.py` & `pybliotecario-2.4.1/src/pybliotecario/components/wiki.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/core_loop.py` & `pybliotecario-2.4.1/src/pybliotecario/core_loop.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/customconf.py` & `pybliotecario-2.4.1/src/pybliotecario/customconf.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/on_cmd_message.py` & `pybliotecario-2.4.1/src/pybliotecario/on_cmd_message.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/on_cmdline.py` & `pybliotecario-2.4.1/src/pybliotecario/on_cmdline.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario/pybliotecario.py` & `pybliotecario-2.4.1/src/pybliotecario/pybliotecario.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/src/pybliotecario.egg-info/SOURCES.txt` & `pybliotecario-2.4.1/src/pybliotecario.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 pyproject.toml
+readme.md
 src/pybliotecario/__init__.py
 src/pybliotecario/argument_parser.py
 src/pybliotecario/core_loop.py
 src/pybliotecario/customconf.py
 src/pybliotecario/on_cmd_message.py
 src/pybliotecario/on_cmdline.py
 src/pybliotecario/pybliotecario.py
@@ -26,15 +27,14 @@
 src/pybliotecario/components/photocol.py
 src/pybliotecario/components/pid.py
 src/pybliotecario/components/reactions.py
 src/pybliotecario/components/repositories.py
 src/pybliotecario/components/scripts.py
 src/pybliotecario/components/stocks.py
 src/pybliotecario/components/system.py
-src/pybliotecario/components/todo_management.py
 src/pybliotecario/components/twitter.py
 src/pybliotecario/components/weather.py
 src/pybliotecario/components/wiki.py
 tests/test_backend_test.py
 tests/test_component_ip_lookup.py
 tests/test_dnd.py
 tests/test_pid.py
```

### Comparing `pybliotecario-2.4/tests/test_backend_test.py` & `pybliotecario-2.4.1/tests/test_backend_test.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/tests/test_component_ip_lookup.py` & `pybliotecario-2.4.1/tests/test_component_ip_lookup.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/tests/test_dnd.py` & `pybliotecario-2.4.1/tests/test_dnd.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/tests/test_pid.py` & `pybliotecario-2.4.1/tests/test_pid.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/tests/test_stocks.py` & `pybliotecario-2.4.1/tests/test_stocks.py`

 * *Files identical despite different names*

### Comparing `pybliotecario-2.4/tests/test_system.py` & `pybliotecario-2.4.1/tests/test_system.py`

 * *Files identical despite different names*

