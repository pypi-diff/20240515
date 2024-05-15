# Comparing `tmp/monkey_plugintoolbox-0.3.0.tar.gz` & `tmp/monkey_plugintoolbox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monkey_plugintoolbox-0.3.0.tar", max compression
+gzip compressed data, was "monkey_plugintoolbox-0.4.0.tar", max compression
```

## Comparing `monkey_plugintoolbox-0.3.0.tar` & `monkey_plugintoolbox-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      478 2024-03-19 13:09:32.734365 monkey_plugintoolbox-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    35255 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/LICENSE
--rw-r--r--   0        0        0      319 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/README.md
--rw-r--r--   0        0        0      901 2024-03-14 16:14:20.570890 monkey_plugintoolbox-0.3.0/plugintoolbox/__init__.py
--rw-r--r--   0        0        0     1788 2024-03-18 12:22:58.451029 monkey_plugintoolbox-0.3.0/plugintoolbox/agent_operations.py
--rw-r--r--   0        0        0     3830 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/plugintoolbox/brute_force_credentials_generator.py
--rw-r--r--   0        0        0     1071 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/plugintoolbox/brute_force_credentials_provider.py
--rw-r--r--   0        0        0     8019 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/plugintoolbox/brute_force_exploiter.py
--rw-r--r--   0        0        0      607 2024-03-18 12:22:58.451029 monkey_plugintoolbox-0.3.0/plugintoolbox/file_filters.py
--rw-r--r--   0        0        0     5494 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/plugintoolbox/http_bytes_server.py
--rw-r--r--   0        0        0     2960 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/plugintoolbox/i_remote_access_client.py
--rw-r--r--   0        0        0      222 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/plugintoolbox/i_remote_access_client_factory.py
--rw-r--r--   0        0        0        0 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/plugintoolbox/py.typed
--rw-r--r--   0        0        0      633 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.3.0/plugintoolbox/script_dropper.py
--rw-r--r--   0        0        0     1213 2024-03-18 12:22:58.451029 monkey_plugintoolbox-0.3.0/plugintoolbox/web_tools.py
--rw-r--r--   0        0        0     1889 2024-03-19 13:09:32.734365 monkey_plugintoolbox-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 monkey_plugintoolbox-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      581 2024-05-15 13:21:38.904802 monkey_plugintoolbox-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35255 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.4.0/LICENSE
+-rw-r--r--   0        0        0      319 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.4.0/README.md
+-rw-r--r--   0        0        0      934 2024-05-15 13:21:38.904802 monkey_plugintoolbox-0.4.0/plugintoolbox/__init__.py
+-rw-r--r--   0        0        0     1788 2024-03-18 12:22:58.451029 monkey_plugintoolbox-0.4.0/plugintoolbox/agent_operations.py
+-rw-r--r--   0        0        0     3830 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.4.0/plugintoolbox/brute_force_credentials_generator.py
+-rw-r--r--   0        0        0     1071 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.4.0/plugintoolbox/brute_force_credentials_provider.py
+-rw-r--r--   0        0        0     8019 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.4.0/plugintoolbox/brute_force_exploiter.py
+-rw-r--r--   0        0        0     1762 2024-05-15 13:21:38.904802 monkey_plugintoolbox-0.4.0/plugintoolbox/dropper_script_wrapper_template.py
+-rw-r--r--   0        0        0      607 2024-03-18 12:22:58.451029 monkey_plugintoolbox-0.4.0/plugintoolbox/file_filters.py
+-rw-r--r--   0        0        0     5494 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.4.0/plugintoolbox/http_bytes_server.py
+-rw-r--r--   0        0        0     2960 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.4.0/plugintoolbox/i_remote_access_client.py
+-rw-r--r--   0        0        0      222 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.4.0/plugintoolbox/i_remote_access_client_factory.py
+-rw-r--r--   0        0        0        0 2024-03-07 13:48:13.965295 monkey_plugintoolbox-0.4.0/plugintoolbox/py.typed
+-rw-r--r--   0        0        0     1213 2024-03-18 12:22:58.451029 monkey_plugintoolbox-0.4.0/plugintoolbox/web_tools.py
+-rw-r--r--   0        0        0     1889 2024-05-15 13:21:38.908802 monkey_plugintoolbox-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 monkey_plugintoolbox-0.4.0/PKG-INFO
```

### Comparing `monkey_plugintoolbox-0.3.0/LICENSE` & `monkey_plugintoolbox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monkey_plugintoolbox-0.3.0/plugintoolbox/__init__.py` & `monkey_plugintoolbox-0.4.0/plugintoolbox/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     IRemoteAccessClient,
     RemoteAccessClientError,
     RemoteAuthenticationError,
     RemoteCommandExecutionError,
     RemoteFileCopyError,
 )
 from .i_remote_access_client_factory import IRemoteAccessClientFactory
-from .script_dropper import build_bash_dropper
+from .dropper_script_wrapper_template import build_bash_dropper_script_template
 from .file_filters import (
     filter_files,
     file_extension_filter,
     is_not_symlink_filter,
     is_not_shortcut_filter,
 )
 from .agent_operations import (
```

### Comparing `monkey_plugintoolbox-0.3.0/plugintoolbox/agent_operations.py` & `monkey_plugintoolbox-0.4.0/plugintoolbox/agent_operations.py`

 * *Files identical despite different names*

### Comparing `monkey_plugintoolbox-0.3.0/plugintoolbox/brute_force_credentials_generator.py` & `monkey_plugintoolbox-0.4.0/plugintoolbox/brute_force_credentials_generator.py`

 * *Files identical despite different names*

### Comparing `monkey_plugintoolbox-0.3.0/plugintoolbox/brute_force_credentials_provider.py` & `monkey_plugintoolbox-0.4.0/plugintoolbox/brute_force_credentials_provider.py`

 * *Files identical despite different names*

### Comparing `monkey_plugintoolbox-0.3.0/plugintoolbox/brute_force_exploiter.py` & `monkey_plugintoolbox-0.4.0/plugintoolbox/brute_force_exploiter.py`

 * *Files identical despite different names*

### Comparing `monkey_plugintoolbox-0.3.0/plugintoolbox/file_filters.py` & `monkey_plugintoolbox-0.4.0/plugintoolbox/file_filters.py`

 * *Files identical despite different names*

### Comparing `monkey_plugintoolbox-0.3.0/plugintoolbox/http_bytes_server.py` & `monkey_plugintoolbox-0.4.0/plugintoolbox/http_bytes_server.py`

 * *Files identical despite different names*

### Comparing `monkey_plugintoolbox-0.3.0/plugintoolbox/i_remote_access_client.py` & `monkey_plugintoolbox-0.4.0/plugintoolbox/i_remote_access_client.py`

 * *Files identical despite different names*

### Comparing `monkey_plugintoolbox-0.3.0/plugintoolbox/web_tools.py` & `monkey_plugintoolbox-0.4.0/plugintoolbox/web_tools.py`

 * *Files identical despite different names*

### Comparing `monkey_plugintoolbox-0.3.0/pyproject.toml` & `monkey_plugintoolbox-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 [tool.vulture]
 exclude=[]
 paths = ["plugintoolbox", "vulture_allowlist.py"]
 
 [tool.poetry]
 name = "monkey-plugintoolbox"
-version = "v0.3.0"
+version = "v0.4.0"
 description = "Miscellaneous convenience utilities for Monkey Plugins code"
 authors = ["Ilija Lazoroski <ilija.lazoroski@gmail.com>"]
 license = "GPLv3"
 classifiers=[
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.11"
 ]
```

### Comparing `monkey_plugintoolbox-0.3.0/PKG-INFO` & `monkey_plugintoolbox-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkey-plugintoolbox
-Version: 0.3.0
+Version: 0.4.0
 Summary: Miscellaneous convenience utilities for Monkey Plugins code
 Home-page: https://github.com/guardicode/plugintoolbox
 License: GPLv3
 Author: Ilija Lazoroski
 Author-email: ilija.lazoroski@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

